# Environment Lab Results — L_LYCHEEMEM
**Benchmark type:** Local static analysis (Bandit + Radon)
**Date:** 2026-10-01
**Note:** GPU inference metrics (tok/s, latency, KV cache) available only for T4-scanned projects.

## Static Analysis

| Tool | Metric | Value |
|------|--------|-------|
| Bandit | HIGH findings | 0 |
| Bandit | MEDIUM findings | 2 |
| Bandit | Status | ✅ PASS |
| Radon CC | Avg complexity grade | 3.2986301369863016 |
| Radon MI | Avg maintainability | None |

## Code Metrics

| Metric | Value |
|--------|-------|
| Python files | 319 |
| Python LOC (est.) | 48,652 |
| Total files | 1283 |

## Anticloud Integration

This project's AIOSS integration layer (`aioss_integration.py`) uses SHA3-256
chain hashing for tamper-evident audit. See `SECURITY_PATCHES.md` for any upstream
Bandit findings documented and mitigated in the Anticloud wrapper.

---
*Anticloud FZ LLE | Apache-2.0 OR LicenseRef-Anticommons-Enterprise-1.0*
