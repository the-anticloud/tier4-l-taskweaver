# Developer Cookbook — L_TASKWEAVER
**Stack:** Python 3.11, taskweaver 0.x, PAX 27B, sandboxed Python executor, AIOSS_FORMAT
**Domain:** TaskWeaver: code-centric agentic task execution with PAX 27B for Anticloud automation

## TaskWeaver session
```python
from l_taskweaver import TaskWeaverAnticloud

tw = TaskWeaverAnticloud(
    pax_model="./pax-27b-q4.gguf",
    workspace="./taskweaver_workspace/",
    allowed_paths=["E:/fenta/Downloads/The Anticloud/"],
    aioss_chain="./taskweaver.aioss"
)

result = tw.run(
    "Load all EDF biosignal files from TIER_7, compute power spectral density for each, "
    "and generate a summary CSV with per-channel band powers"
)
print(result.output)
print(f"Code generated: {len(result.code_snippets)} snippets")
print(f"Chain: {result.chain_hash}")
```

## View generated code
```python
for snippet in result.code_snippets:
    print(f"--- Step {snippet.step} ---")
    print(snippet.code)
    print(f"Result: {snippet.execution_result[:80]}")
```

## Safe execution check
```python
tw.set_sandbox_policy(
    allow_imports=["numpy", "pandas", "scipy", "mne"],
    deny_imports=["subprocess", "socket", "requests"],
    max_execution_seconds=30
)
```

## AIOSS Chain Append
```python
import hashlib, time

def aioss_append(chain_path, payload: bytes, module_id: str):
    entry_hash = hashlib.sha3_256(payload).digest()
    ts = int(time.time_ns()).to_bytes(8, 'big')
    with open(chain_path, 'rb') as f:
        f.seek(-32, 2); prev_hash = f.read(32)
    new_hash = hashlib.sha3_256(prev_hash + entry_hash + ts).digest()
    with open(chain_path, 'ab') as f:
        f.write(ts + entry_hash + new_hash)
    return new_hash.hex()
```
