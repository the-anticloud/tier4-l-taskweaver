# Deploy Guide — L_TASKWEAVER
**Tier:** TIER_4_INFERENCE_AGENTS | **Stack:** Python 3.11, taskweaver 0.x, PAX 27B, sandboxed Python executor, AIOSS_FORMAT
**Air-gap capable after initial setup.**

## Prerequisites
Python 3.11+, taskweaver 0.x (install from source), PAX 27B, RestrictedPython (sandbox).

## Environment
8GB RAM. GPU for PAX code generation. RestrictedPython sandbox: no file system access outside designated paths.

## AIOSS Integration
```bash
aioss init --module L_TASKWEAVER --output ./l_taskweaver.aioss
aioss append --chain ./l_taskweaver.aioss --payload ./output.bin --module L_TASKWEAVER
aioss verify --chain ./l_taskweaver.aioss
```

## Air-Gap Setup
```bash
pip download -r requirements.txt -d ./wheels/
pip install --no-index --find-links ./wheels/ -r requirements.txt
```

## PAX 27B Harness Wiring
```python
from anticloud_pax import PAXHarness
harness = PAXHarness(
    model_path="./pax-27b-q4.gguf",
    module="L_TASKWEAVER",
    aioss_chain="./L_TASKWEAVER.aioss",
    classification="L5_NARROW_L2_GENERAL"
)
result = harness.process(input_data)
```

## Verification
```bash
aioss verify --chain ./L_TASKWEAVER.aioss --verbose
python -m L_TASKWEAVER.tests.smoke
```
