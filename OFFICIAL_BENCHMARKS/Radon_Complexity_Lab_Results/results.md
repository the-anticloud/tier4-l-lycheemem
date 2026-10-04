# Radon_Complexity_Lab_Results
**Project:** `L_LYCHEEMEM` | **Status:** `PASS` | **Run:** `2026-09-30T17:14:20.030944+00:00`

**Framework:** [Radon — Cyclomatic Complexity & Maintainability Index](https://radon.readthedocs.io/)

## Key Metrics

- **files_analyzed:** `10`
- **average_complexity:** `{'grade': 'B', 'score': 5.568181818181818}`
- **complexity_grade:** `B`
- **complexity_score:** `5.568181818181818`
- **mi_output:** `E:\fenta\Downloads\The Anticloud\TIER_4_INFERENCE_AGENTS\L_LYCHEEMEM\UPSTREAM\ontology\default_ontology.py - A (80.86)
E`

## Raw Output (first 50 lines)
```
E:\fenta\Downloads\The Anticloud\TIER_4_INFERENCE_AGENTS\L_LYCHEEMEM\UPSTREAM\ontology\default_ontology.py
    C 4:0 User - A (1)
    C 17:0 Assistant - A (1)
    C 23:0 Preference - A (1)
    C 35:0 Location - A (1)
    C 47:0 Event - A (1)
    C 56:0 Object - A (1)
    C 68:0 Topic - A (1)
    C 80:0 Organization - A (1)
    C 89:0 Document - A (1)
    C 103:0 LocatedAt - A (1)
    C 111:0 OccurredAt - A (1)
E:\fenta\Downloads\The Anticloud\TIER_4_INFERENCE_AGENTS\L_LYCHEEMEM\UPSTREAM\zep-eval-harness\checkpoint.py
    F 20:0 delete_checkpoint - A (2)
    F 5:0 save_checkpoint - A (1)
    F 14:0 load_checkpoint - A (1)
E:\fenta\Downloads\The Anticloud\TIER_4_INFERENCE_AGENTS\L_LYCHEEMEM\UPSTREAM\zep-eval-harness\retry.py
    F 5:0 retry_with_backoff - A (4)
E:\fenta\Downloads\The Anticloud\TIER_4_INFERENCE_AGENTS\L_LYCHEEMEM\UPSTREAM\zep-eval-harness\zep_chunk_documents.py
    F 255:0 run_chunking - C (17)
    F 45:0 load_documents - B (8)
    F 465:0 main - B (8)
    F 111:0 extract_document_title - B (7)
    F 224:0 read_completed_chunks - B (7)
    F 192:0 get_next_chunk_set_number - A (5)
    F 79:0 create_document_chunker - A (2)
    F 136:0 summarize_document - A (1)
    F 157:0 contextualize_chunk - A (1)
    F 210:0 write_meta - A (1)
    F 218:0 append_chunk_line - A (1)
    F 427:0 parse_args - A (1)
E:\fenta\Downloads\The Anticloud\TIER_4_INFERENCE_AGENTS\L_LYCHEEMEM\UPSTREAM\zep-eval-harness\zep_evaluate.py
    F 673:0 calculate_aggregate_statistics - F (41)
   
```

---
_Anticloud Independent Benchmark — 2026-09-30T17:14:20.030944+00:00_