# Radon_Complexity_Lab_Results
**Project:** `L_TASKWEAVER` | **Status:** `PASS` | **Run:** `2026-09-30T17:14:20.030944+00:00`

**Framework:** [Radon — Cyclomatic Complexity & Maintainability Index](https://radon.readthedocs.io/)

## Key Metrics

- **files_analyzed:** `10`
- **average_complexity:** `{'grade': 'A', 'score': 3.9761904761904763}`
- **complexity_grade:** `A`
- **complexity_score:** `3.9761904761904763`
- **mi_output:** `E:\fenta\Downloads\The Anticloud\TIER_4_INFERENCE_AGENTS\L_TASKWEAVER\UPSTREAM\setup.py - A (71.92)
E:\fenta\Downloads\T`

## Raw Output (first 50 lines)
```
E:\fenta\Downloads\The Anticloud\TIER_4_INFERENCE_AGENTS\L_TASKWEAVER\UPSTREAM\setup.py
    F 34:0 create_zip_file - A (4)
    F 8:0 update_version_file - A (1)
E:\fenta\Downloads\The Anticloud\TIER_4_INFERENCE_AGENTS\L_TASKWEAVER\UPSTREAM\auto_eval\evaluator.py
    F 43:0 config_llm - A (5)
    M 95:4 VirtualUser.talk_with_agent - A (5)
    M 169:4 Evaluator.parse_output - A (5)
    M 184:4 Evaluator.eval_via_code - A (5)
    C 144:0 Evaluator - A (4)
    F 33:0 get_config - A (3)
    C 80:0 VirtualUser - A (3)
    M 248:4 Evaluator.evaluate - A (3)
    M 229:4 Evaluator.score - A (2)
    F 27:0 load_config - A (1)
    C 21:0 ScoringPoint - A (1)
    M 81:4 VirtualUser.__init__ - A (1)
    M 130:4 VirtualUser.get_reply_from_vuser - A (1)
    M 140:4 VirtualUser.get_reply_from_agent - A (1)
    M 145:4 Evaluator.__init__ - A (1)
    M 155:4 Evaluator.format_input - A (1)
E:\fenta\Downloads\The Anticloud\TIER_4_INFERENCE_AGENTS\L_TASKWEAVER\UPSTREAM\auto_eval\taskweaver_eval.py
    F 53:0 auto_evaluate_for_taskweaver - B (8)
    F 112:0 batch_auto_evaluate_for_taskweaver - B (7)
    M 27:4 TaskWeaverVirtualUser.get_reply_from_agent - A (4)
    C 19:0 TaskWeaverVirtualUser - A (3)
    M 20:4 TaskWeaverVirtualUser.__init__ - A (1)
    M 49:4 TaskWeaverVirtualUser.close - A (1)
E:\fenta\Downloads\The Anticloud\TIER_4_INFERENCE_AGENTS\L_TASKWEAVER\UPSTREAM\auto_eval\utils.py
    F 29:0 check_package_version - B (8)
    F 15:0 load_task_case - A (3)
E:\fenta\Downloads\The Anticloud
```

---
_Anticloud Independent Benchmark — 2026-09-30T17:14:20.030944+00:00_