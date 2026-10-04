# L5 Narrow / L2 General Classification — L_LYCHEEMEM
**Platform:** Anticloud | **Tier:** TIER_4_INFERENCE_AGENTS | **PAX:** 27B
**IP:** USPTO pending 2026, Anticloud FZ LLE, 0-1.gg | **License:** Apache-2.0

## L5 Narrow
L_LYCHEEMEM manages PAX 27B's effective context window for long conversations and multi-session tasks. Narrow scope: Anticloud conversation and task memory. Selective compression retains high-salience content while compressing low-salience context.

## L2 General
L2 General: L_LYCHEEMEM enables long-context operation for any tier. TIER_7 clinical agents maintaining month-long patient interaction histories and TIER_9 mission planners tracking multi-day operations both use L_LYCHEEMEM.

## PAX 27B Integration
PAX 27B performs salience scoring and compression. L_LYCHEEMEM identifies which context segments to retain verbatim vs compress, calls PAX to generate compressed summaries, and reconstructs context for the next inference.

## AIOSS Audit Chain
Every memory operation (original context hash + salience scores hash + compressed context hash + compression ratio) is chained: H_n = SHA3-256(H_{n-1} || entry_hash_n || timestamp_n).
Offline-verifiable, tamper-evident, zero cloud dependency.

## Regulatory / Compliance
GDPR Art. 17 (right to erasure). ISO 27001 A.8.2 (classification of information).
