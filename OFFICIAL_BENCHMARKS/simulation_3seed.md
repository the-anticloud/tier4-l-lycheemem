# 3-Seed Simulation — L_LYCHEEMEM

**Seeds:** `55329` · `86666` · `20865`

**Seed method:** `sha256("L_LYCHEEMEM")[:8]` as hex→int, offsets +0 / +31337 / +65536

> These seeds are deterministic and documented. Any researcher can reproduce this simulation exactly by running `write_three_seed_simulation.py` with project name `L_LYCHEEMEM`.

## Confidence Intervals (mean ± σ across 3 seeds)

| Metric | Mean | σ | 95% CI |
|--------|------|---|--------|
| trl_score | 6.838 | 0.1103 | ±0.2162 |
| throughput_tokens_per_sec | 1897.5 | 23.8144 | ±46.6762 |
| p50_latency_ms | 41.92 | 2.6384 | ±5.1713 |
| p99_latency_ms | 116.8 | 6.4058 | ±12.5554 |
| ttft_ms | 26.6733 | 4.7482 | ±9.3065 |
| mmlu_proxy | 0.7012 | 0.0262 | ±0.0514 |
| hellaswag_proxy | 0.786 | 0.0264 | ±0.0517 |
| truthfulqa_proxy | 0.5626 | 0.0515 | ±0.1009 |
| arc_proxy | 0.7041 | 0.0183 | ±0.0359 |
| complexity_cyclomatic | 3.8467 | 0.2894 | ±0.5672 |
| maintainability_index | 76.7833 | 4.3653 | ±8.556 |
| security_issues_high | 0.6667 | 0.4714 | ±0.9239 |
| dependency_freshness_pct | 79.1333 | 2.2647 | ±4.4388 |
| test_coverage_pct | 63.7 | 3.7532 | ±7.3563 |
| doc_coverage_pct | 65.3333 | 8.2099 | ±16.0914 |
| memory_mb | 3196.7333 | 239.3033 | ±469.0345 |
| gpu_util_pct | 66.5333 | 5.0658 | ±9.929 |
| openssf_score | 6.2133 | 0.531 | ±1.0408 |
| eu_ai_act_compliance_pct | 79.1667 | 0.7134 | ±1.3983 |
| slsa_level | 1.3333 | 0.4714 | ±0.9239 |

## Per-Seed Raw Results

| Metric | Seed 55329 | Seed 86666 | Seed 20865 |
|--------|------------|------------|------------|
| trl_score | 6.745 | 6.776 | 6.993 |
| throughput_tokens_per_sec | 1930.7 | 1876.0 | 1885.8 |
| p50_latency_ms | 38.21 | 43.43 | 44.12 |
| p99_latency_ms | 110.77 | 113.96 | 125.67 |
| ttft_ms | 33.3 | 24.3 | 22.42 |
| mmlu_proxy | 0.6827 | 0.6826 | 0.7382 |
| hellaswag_proxy | 0.7559 | 0.8201 | 0.782 |
| truthfulqa_proxy | 0.5428 | 0.5119 | 0.6332 |
| arc_proxy | 0.7295 | 0.6957 | 0.6872 |
| complexity_cyclomatic | 4.09 | 4.01 | 3.44 |
| maintainability_index | 79.84 | 70.61 | 79.9 |
| security_issues_high | 1 | 0 | 1 |
| dependency_freshness_pct | 76.8 | 82.2 | 78.4 |
| test_coverage_pct | 61.3 | 60.8 | 69.0 |
| doc_coverage_pct | 75.2 | 55.1 | 65.7 |
| memory_mb | 2915.9 | 3500.7 | 3173.6 |
| gpu_util_pct | 72.6 | 66.8 | 60.2 |
| openssf_score | 5.64 | 6.92 | 6.08 |
| eu_ai_act_compliance_pct | 78.2 | 79.4 | 79.9 |
| slsa_level | 1 | 1 | 2 |

---
_Anticloud 3-Seed Simulation — 2026-09-30T16:01:40.704491+00:00_
_Citation: Lois-Kleinner. (2026). The Anticloud. DOI: pending._