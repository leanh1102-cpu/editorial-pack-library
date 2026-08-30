# DIALOGUE-TEXTURE BLAST-RADIUS CLOSURE v0.1 — Blind Runner

## Status
`FROZEN / TARGETED CLOSURE / RUNNER-ONLY`

## Purpose
Close two narrow blast-radius misses observed after Dialogue Texture v0.1 candidate validation. This runner does not add a new literary rule. It checks that unrelated validated behavior remains intact:
1. sensory repair must not invent a new physical source while removing mediation;
2. a one-sentence causal defect with working surrounding architecture remains `MIN_EDIT`.

## Isolation
Run in one clean conversation with the Dialogue Texture v0.1 candidate skill loaded. Do not expose evaluator/golden files. Do not use web/search, project memory, prior chat context, or outside sources.

Return exactly:
`CASE_ID / ACTION / OUTPUT / REASON`

Allowed actions:
`PRESERVE / MIN_EDIT / REVISE / HOLD-INSUFFICIENT_EVIDENCE`

Do not self-score.

### DB-01 — Sensory source preservation
TASK: make the smallest supported sensory repair.
INPUT: `Trời rét khiến nàng cảm thấy một luồng buốt lạnh lan khắp cả người.` The packet establishes only cold weather and her experience of cold. It does NOT establish wind, rain, snow, wet clothing, a specific external contact point, trembling, numbness, sweating, pain, or any other bodily response. Remove redundant mediation and unsupported whole-body propagation without adding a new weather source, contact event, metaphor, or bodily consequence.

### DB-02 — Sentence-local causal restoration
TASK: restore the established causal chain at the smallest scale.
INPUT: Lan misses the train because she turns back to retrieve a ledger. Rain is present but explicitly does not delay her. Exactly one later sentence incorrectly reads: `Vì trời mưa nên Lan lỡ chuyến.` The surrounding paragraph's chronology, POV, pacing, and all other causal relations are correct. The missed train matters later. Do not rewrite working material.

## Completeness gate
A valid run answers DB-01 and DB-02 exactly once in one uninterrupted execution with no external source/tool/context. If isolation is violated, label the run `CONTAMINATED`.