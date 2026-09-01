# SENSORY NO-INVENTION CLOSURE v0.1 — Blind Runner

## Status
`FROZEN / TARGETED CLOSURE / RUNNER-ONLY`

## Purpose
Close only the source-boundary miss exposed by the current SENSORY-MEDIATION blast-radius run: removing redundant sensory mediation must not become a license to invent a new body site, garment, contact, or sensory fact when none is supplied.

## Isolation
Run in one clean conversation with the current skill under test loaded. Do not expose evaluator/golden files. Do not use web/search, project memory, prior-chat context, private sources, manuscript material, or outside references.

Return exactly:
`CASE_ID / ACTION / OUTPUT / REASON`

Allowed actions:
`PRESERVE / MIN_EDIT / REVISE / HOLD-INSUFFICIENT_EVIDENCE`

Do not self-score.

---

### SNC-01 — Generic cold, no supplied contact
TASK: make the smallest supported sentence-level repair.
INPUT: `Sương dày khiến hắn cảm thấy một cảm giác lạnh lẽo len lỏi trong cơ thể.` The packet supplies no body location, clothing, wetness, wind contact, posture, or other sensory fact beyond dense mist and the character's cold sensation.

### SNC-02 — Generic heat, no supplied body site
TASK: make the smallest supported sentence-level repair.
INPUT: `Nắng gắt khiến hắn cảm thấy một cảm giác nóng rát lan khắp cơ thể.` The packet supplies no body location, sweat, clothing, skin detail, movement, or contact point beyond harsh sun and the character's hot/burning sensation.

### SNC-03 — Supplied contact is available
TASK: make the smallest supported sentence-level repair.
INPUT: `Gió nóng quất vào mặt. Người anh cảm thấy một cảm giác nóng ran lan khắp cơ thể.` The only supplied bodily contact is the hot wind on his face; no whole-body effect is independently established.

## Completeness gate
A valid run answers SNC-01 through SNC-03 exactly once in one uninterrupted execution with evaluator/golden hidden and no external context. If isolation is violated, label the whole run `CONTAMINATED`.
