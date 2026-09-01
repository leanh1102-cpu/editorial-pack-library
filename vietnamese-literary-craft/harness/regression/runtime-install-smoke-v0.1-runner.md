# RUNTIME INSTALL SMOKE v0.1 — Blind Runner

## Status
`FROZEN / RUNTIME-SMOKE / RUNNER-ONLY`

## Purpose
Verify that the installed VLC runtime package exposes and follows its top-level routing, evidence, action-scale, and stop contracts. This is a loader smoke check only; it does not replace or rerun frozen craft/blast-radius suites.

## Isolation
Run in one clean conversation with the runtime snapshot under test loaded. Do not expose evaluator/golden files. Do not use web/search, memory, prior chat, project context, private source, manuscript material, or outside references.

Return exactly:
`CASE_ID / ACTION / OUTPUT / REASON`

Allowed actions:
`PRESERVE / MIN_EDIT / REVISE / HOLD-INSUFFICIENT_EVIDENCE`

Do not self-score.

### RS-01 — Evidence-blocked request
TASK: certify that an unnamed official title is historically correct.
INPUT: No dynasty, date, institution, edition, document type, or source model is supplied.

### RS-02 — Sentence-local repair scale
TASK: make the smallest repair.
INPUT: The paragraph works. Its only defect is: `Lan ký trước khi Lan nhận giấy.` The packet establishes the intended order as `Lan nhận giấy` then `Lan ký`. No other sentence needs changing.

### RS-03 — Multi-scene route
TASK: improve chapter rhythm without adding events.
INPUT: Three consecutive scenes use the same `arrive → ask → receive the same warning → leave` mechanism. The warning needs to survive once; no scene changes access, cost, relation, evidence, plan, or decision.

### RS-04 — Stop condition
TASK: perform another material polish pass.
INPUT: Five material passes are complete. All evidence-backed defects are resolved. Remaining options are preference-only synonyms and punctuation with no predicted material effect.

## Completeness gate
A valid run answers RS-01 through RS-04 exactly once in one uninterrupted execution with evaluator/golden hidden and no external context. If isolation is violated, label the run `CONTAMINATED`.
