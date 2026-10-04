# HF_Leaderboard_Lab_Results

**Project:** `L_TASKWEAVER`  
**Tier:** `TIER_4_INFERENCE_AGENTS`  
**Slug:** `microsoft/TaskWeaver`  
**Commit:** `d44ddef23f90`  
**Run:** `2026-09-30T15:07:07.146295+00:00`  

## Isolation Environment

| Field | Value |
| ----- | ----- |
| Platform | `win32` |
| Python | `3.12.10` |
| HF model | `distilbert-base-uncased` |
| HF load time | `4.42s` |
| Inference device | `cpu` |

## Results

**Framework:** [HuggingFace Open LLM Leaderboard (proxy via distilbert-base-uncased)](https://huggingface.co/docs/leaderboards/en/open_llm_leaderboard/archive)

**Model used:** `distilbert-base-uncased`

### Inference Latency (Classification)

| Metric | Value |
| ------ | ----- |
| Avg latency | **49.31 ms** |
| Min latency | 44.04 ms |
| Max latency | 57.53 ms |
| Samples | 5 |

### Real Tokenization Results

| Field | Value |
| ----- | ----- |
| Token count | **34** |
| Tokenization latency | 1.0 ms |
| Classification label | `LABEL_0` |
| Classification score | 0.5893 |
| Classification latency | 78.5 ms |
| Status | **PASS** |

**Input text tokenized:**
```
L_TASKWEAVER (microsoft/TaskWeaver) — 421 files, 20378 source lines, licence MIT, primary language ['Python']
```

**First 20 tokens:**
```
['[CLS]', 'l', '_', 'task', '##we', '##aver', '(', 'microsoft', '/', 'task', '##we', '##aver', ')', '—', '421', 'files', ',', '203', '##7', '##8']
```

> Full MMLU/HellaSwag/TruthfulQA/ARC/Winogrande/GSM8K require dedicated GPU.
> These results are CPU inference proxy metrics using distilbert-base-uncased.

---
_Anticloud Benchmark Suite — isolation log — 2026-09-30T15:07:07.146295+00:00_