# HF_Leaderboard_Lab_Results

**Project:** `L_LYCHEEMEM`  
**Tier:** `TIER_4_INFERENCE_AGENTS`  
**Slug:** `getzep/zep`  
**Commit:** `495bf72880d1`  
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
| Avg latency | **53.86 ms** |
| Min latency | 48.49 ms |
| Max latency | 57.04 ms |
| Samples | 5 |

### Real Tokenization Results

| Field | Value |
| ----- | ----- |
| Token count | **41** |
| Tokenization latency | 2.0 ms |
| Classification label | `LABEL_0` |
| Classification score | 0.5881 |
| Classification latency | 81.49 ms |
| Status | **PASS** |

**Input text tokenized:**
```
L_LYCHEEMEM (getzep/zep) — 947 files, 104173 source lines, licence Apache-2.0, primary language ['Python']
```

**First 20 tokens:**
```
['[CLS]', 'l', '_', 'l', '##ych', '##eem', '##em', '(', 'get', '##ze', '##p', '/', 'ze', '##p', ')', '—', '94', '##7', 'files', ',']
```

> Full MMLU/HellaSwag/TruthfulQA/ARC/Winogrande/GSM8K require dedicated GPU.
> These results are CPU inference proxy metrics using distilbert-base-uncased.

---
_Anticloud Benchmark Suite — isolation log — 2026-09-30T15:07:07.146295+00:00_