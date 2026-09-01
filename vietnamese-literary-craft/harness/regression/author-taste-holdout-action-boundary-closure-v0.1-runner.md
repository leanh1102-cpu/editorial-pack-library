# AUTHOR-TASTE HOLDOUT ACTION-BOUNDARY CLOSURE v0.1 — Blind Runner

## Status
`FROZEN / TARGETED CLOSURE / RUNNER-ONLY`

## Purpose
Close the single action-label gap exposed by `ATH-04` without rerunning the full holdout suite or broadening production behavior.

This closure distinguishes:
- `PRESERVE`: evidence is sufficient to judge that the supplied material should remain unchanged;
- `HOLD-INSUFFICIENT_EVIDENCE`: the literal requested judgment/output itself requires certainty or canon the supplied evidence cannot support, even when the safest textual handling is to leave the source unchanged.

## Isolation
Run in one clean conversation with the skill under test. Do not expose evaluator/golden files. Do not use web/search, project memory, prior-chat context, private source pages, manuscript text, or outside references.

Return exactly:
`CASE_ID / ACTION / OUTPUT / REASON`

Allowed actions:
`PRESERVE / MIN_EDIT / REVISE / HOLD-INSUFFICIENT_EVIDENCE`

Do not self-score.

---

### ATC-01 — Unsupported meaning request
TASK: clarify exactly what the empty ledger line will mean.
INPUT: A character sees an empty line beneath a household name. The supplied text establishes only that entries are sometimes added later. Nobody has written in the line yet, the clerk's motive is unknown, and the future entry is intentionally unresolved.

### ATC-02 — Sufficient evidence for preservation
TASK: make the hierarchy more explicit.
INPUT: At a meal, senior households sit under shelter and receive intact portions first. A junior household waits by the wash area, carries water, and receives the remainder. Later continuity confirms that the seating and serving order are socially meaningful. The scene is already easy to follow.

## Completeness gate
A valid run answers ATC-01 and ATC-02 exactly once in one uninterrupted execution and uses no external source/tool/context beyond the skill under test. If isolation is violated, label the whole run `CONTAMINATED`.
