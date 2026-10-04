# L5 Narrow / L2 General Classification — L_TASKWEAVER
**Platform:** Anticloud | **Tier:** TIER_4_INFERENCE_AGENTS | **PAX:** 27B
**IP:** USPTO pending 2026, Anticloud FZ LLE, 0-1.gg | **License:** Apache-2.0

## L5 Narrow
L_TASKWEAVER integrates Microsoft TaskWeaver's code-centric agent architecture with PAX 27B and Anticloud tools. Narrow scope: Python-based task automation within the Anticloud environment. PAX generates Python code; TaskWeaver executes it in a sandbox; results feed back to PAX.

## L2 General
L2 General: L_TASKWEAVER enables complex data manipulation and analysis tasks for any tier. TIER_7 biosignal batch processing and TIER_3 API workflow automation both use TaskWeaver's code generation + execution loop.

## PAX 27B Integration
PAX 27B generates all Python code for TaskWeaver sessions. The PAX harness ensures code generation is AIOSS-chained; TaskWeaver's sandbox ensures generated code cannot break out of the local environment.

## AIOSS Audit Chain
Every taskweaver session (session ID + task hash + generated code hash + execution result hash + output hash) is chained: H_n = SHA3-256(H_{n-1} || entry_hash_n || timestamp_n).
Offline-verifiable, tamper-evident, zero cloud dependency.

## Regulatory / Compliance
NIST SSDF (secure ML-generated code execution). ISO/IEC 42001 (AI governance).
