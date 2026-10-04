# 3-Seed Simulation — L_TASKWEAVER

**Seeds:** `64876` · `96213` · `30412`

**Seed method:** `sha256("L_TASKWEAVER")[:8]` as hex→int, offsets +0 / +31337 / +65536

> These seeds are deterministic and documented. Any researcher can reproduce this simulation exactly by running `write_three_seed_simulation.py` with project name `L_TASKWEAVER`.

## Confidence Intervals (mean ± σ across 3 seeds)

| Metric | Mean | σ | 95% CI |
|--------|------|---|--------|
| trl_score | 7.104 | 0.1737 | ±0.3405 |
| throughput_tokens_per_sec | 585.4333 | 33.3619 | ±65.3893 |
| p50_latency_ms | 41.45 | 4.4566 | ±8.7349 |
| p99_latency_ms | 108.75 | 6.4058 | ±12.5554 |
| ttft_ms | 27.3733 | 1.2378 | ±2.4261 |
| mmlu_proxy | 0.7242 | 0.0262 | ±0.0514 |
| hellaswag_proxy | 0.7679 | 0.0264 | ±0.0517 |
| truthfulqa_proxy | 0.5823 | 0.0476 | ±0.0933 |
| arc_proxy | 0.6594 | 0.0183 | ±0.0359 |
| complexity_cyclomatic | 3.6167 | 0.2894 | ±0.5672 |
| maintainability_index | 76.1933 | 4.3653 | ±8.556 |
| security_issues_high | 1.0 | 0.8165 | ±1.6003 |
| dependency_freshness_pct | 77.5333 | 2.2647 | ±4.4388 |
| test_coverage_pct | 63.9667 | 10.3722 | ±20.3295 |
| doc_coverage_pct | 65.7333 | 8.2099 | ±16.0914 |
| memory_mb | 55.3 | 3.9421 | ±7.7265 |
| gpu_util_pct | 67.4667 | 5.4908 | ±10.762 |
| openssf_score | 6.71 | 0.5266 | ±1.0321 |
| eu_ai_act_compliance_pct | 77.8667 | 0.7134 | ±1.3983 |
| slsa_level | 2.0 | 0.0 | ±0.0 |

## Per-Seed Raw Results

| Metric | Seed 64876 | Seed 96213 | Seed 30412 |
|--------|------------|------------|------------|
| trl_score | 7.211 | 7.242 | 6.859 |
| throughput_tokens_per_sec | 538.6 | 603.9 | 613.8 |
| p50_latency_ms | 47.74 | 37.96 | 38.65 |
| p99_latency_ms | 102.72 | 105.91 | 117.62 |
| ttft_ms | 26.0 | 29.0 | 27.12 |
| mmlu_proxy | 0.7057 | 0.7057 | 0.7612 |
| hellaswag_proxy | 0.7377 | 0.802 | 0.7639 |
| truthfulqa_proxy | 0.5158 | 0.6249 | 0.6062 |
| arc_proxy | 0.6848 | 0.651 | 0.6425 |
| complexity_cyclomatic | 3.86 | 3.78 | 3.21 |
| maintainability_index | 79.25 | 70.02 | 79.31 |
| security_issues_high | 2 | 1 | 0 |
| dependency_freshness_pct | 75.2 | 80.6 | 76.8 |
| test_coverage_pct | 71.5 | 71.1 | 49.3 |
| doc_coverage_pct | 75.6 | 55.5 | 66.1 |
| memory_mb | 59.8 | 55.9 | 50.2 |
| gpu_util_pct | 66.8 | 61.1 | 74.5 |
| openssf_score | 6.14 | 7.41 | 6.58 |
| eu_ai_act_compliance_pct | 76.9 | 78.1 | 78.6 |
| slsa_level | 2 | 2 | 2 |

---
_Anticloud 3-Seed Simulation — 2026-09-30T16:01:40.704491+00:00_
_Citation: Lois-Kleinner. (2026). The Anticloud. DOI: pending._