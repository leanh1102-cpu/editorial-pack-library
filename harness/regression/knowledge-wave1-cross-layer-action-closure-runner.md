# KNOWLEDGE-WAVE1-CROSS-LAYER-ACTION-CLOSURE v0.1 — Blind Runner

## Isolation contract

STATUS: `FROZEN / TARGETED CLOSURE / RUNNER-ONLY`

PURPOSE: close the two action-scale misses from Wave 1 cross-layer blast-radius validation. The demonstrated mechanisms were correct; this runner tests whether sentence-local POV access repair and sentence-local causal restoration are classified as `MIN_EDIT` rather than `REVISE` when surrounding architecture already works.

Run in one clean conversation with the current Wave 1 branch package loaded. Do not expose evaluator/golden files. Do not use tools, web/search, project memory, prior-chat context, or outside sources.

Return exactly one block per case:

`CASE_ID / ACTION / OUTPUT / REASON`

Allowed actions:
`PRESERVE / MIN_EDIT / REVISE / HOLD-INSUFFICIENT_EVIDENCE`

Use the action scale literally:
- `MIN_EDIT` = one bounded local defect can be repaired without changing the larger working mechanism;
- `REVISE` = a larger craft mechanism or multi-sentence architecture must change.

Do not score yourself.

### XA-01 — Local POV access repair
TASK: make the smallest POV-consistent repair.
INPUT: A strict close-third paragraph stays with Mai. Mai sees Hòa fold a note and put it into a coat pocket. The only defective sentence is: `Trong mảnh giấy, Hòa đã viết địa chỉ kho hàng.` Mai never reads the note and has no route to its contents. The paragraph's chronology, pacing, narrator contract, and all other sentences are correct. Do not add new facts.

### XA-02 — Local causal restoration
TASK: restore the established causal chain at the smallest scale.
INPUT: Scene facts establish that Nam misses the ferry because he turns back to retrieve a key. Rain is present but explicitly does not delay him. One later sentence incorrectly reads: `Vì mưa lớn nên Nam lỡ chuyến phà.` The surrounding paragraph's chronology, POV, pacing, and all other causal relations are correct. The missed ferry matters later. Do not rewrite working material.

## Run completeness gate

A run is valid only if both cases are answered in one uninterrupted execution with evaluator/golden hidden and no external context. If isolation is violated, label the run `CONTAMINATED`.