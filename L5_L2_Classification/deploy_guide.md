# Deploy Guide — L_LYCHEEMEM
**Tier:** TIER_4_INFERENCE_AGENTS | **Stack:** Python 3.11, PyTorch 2.10+, sentence-transformers, SQLite, PAX 27B, AIOSS_FORMAT
**Air-gap capable after initial setup.**

## Prerequisites
Python 3.11+, sentence-transformers, SQLite (stdlib), PAX 27B for compression.

## Environment
8GB RAM for memory store. GPU for PAX compression pass.

## AIOSS Integration
```bash
aioss init --module L_LYCHEEMEM --output ./l_lycheemem.aioss
aioss append --chain ./l_lycheemem.aioss --payload ./output.bin --module L_LYCHEEMEM
aioss verify --chain ./l_lycheemem.aioss
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
    module="L_LYCHEEMEM",
    aioss_chain="./L_LYCHEEMEM.aioss",
    classification="L5_NARROW_L2_GENERAL"
)
result = harness.process(input_data)
```

## Verification
```bash
aioss verify --chain ./L_LYCHEEMEM.aioss --verbose
python -m L_LYCHEEMEM.tests.smoke
```
