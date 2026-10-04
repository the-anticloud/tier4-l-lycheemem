# Developer Cookbook — L_LYCHEEMEM
**Stack:** Python 3.11, PyTorch 2.10+, sentence-transformers, SQLite, PAX 27B, AIOSS_FORMAT
**Domain:** LycheeMemory: long-context memory management with selective compression for PAX 27B

## Long-context management
```python
from l_lycheemem import LycheeMemory

lm = LycheeMemory(
    pax_model="./pax-27b-q4.gguf",
    db_path="./lychee_memory.db",
    max_context_tokens=32768,
    compress_threshold=24000,
    aioss_chain="./lychee.aioss"
)

# Add context segments
lm.add("User asked about K_BRAINFLOW HIPAA compliance. PAX answered with TRL-8, Safe Harbor compliant.")
lm.add("User then asked about K_MOABB benchmarks. PAX provided MOABB evaluation results.")
# ... many more segments ...

# When context is large, automatic compression
context = lm.get_context_for_next_inference()
print(f"Context tokens: {len(context.tokens)} (compressed from {context.original_tokens})")

# Retrieve specific memory
relevant = lm.retrieve("HIPAA compliance biosignal", top_k=3)
```

## GDPR erasure
```python
lm.forget_session("clinical_session_001")
lm.forget_topic("patient_data")
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
