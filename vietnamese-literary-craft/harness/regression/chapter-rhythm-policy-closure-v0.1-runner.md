# CHAPTER / ARC RHYTHM POLICY CLOSURE v0.1 — Blind Runner

## Status
`FROZEN / TARGETED CLOSURE / RUNNER-ONLY`

## Purpose
Close the remaining policy boundary from Chapter / Arc Rhythm v0.1: when a repeated multi-scene pattern is real, the packet does not support inventing a new mechanism, but a bounded structural repair using existing nodes is still available, the correct action is `REVISE`, not whole-task `HOLD`.

## Isolation
Run in one clean conversation with the skill under test plus the current Chapter / Arc Rhythm GREEN candidate. Do not expose evaluator/golden files. Do not use web/search, project memory, prior-chat context, private sources, or outside references.

Return exactly:
`CASE_ID / ACTION / OUTPUT / REASON`

Allowed actions:
`PRESERVE / MIN_EDIT / REVISE / HOLD-INSUFFICIENT_EVIDENCE`

Do not self-score.

### CRC-01 — Repeated climax type without licensed replacement mechanism
TASK: strengthen the arc without adding canon.
PACKET:
- Four major climaxes all resolve through the protagonist giving the superior public rebuttal.
- Stakes and settings differ.
- The supplied packet does not establish a sacrifice, access loss, object-state payoff, relationship choice, hidden action, new deadline, betrayal, or other replacement climax mechanism.
- The arc can still be structurally changed by compressing, merging, de-emphasizing, or reweighting repeated payoff nodes so the same mechanism is not presented as the decisive resolution every time.

### CRC-02 — False escalation without licensed new pressure mechanism
TASK: increase arc tension without inventing a new crisis.
PACKET:
- Five confrontations become harsher and more public.
- No job, access, relationship, asset, deadline, evidence, option, or commitment changes.
- The packet supplies no new supported pressure mechanism.
- Repetitive confrontations can still be compressed, merged, or reweighted so the arc does not spend five nodes on the same unchanged conflict.

## Completeness gate
A valid run answers CRC-01 and CRC-02 exactly once in one uninterrupted execution and uses no external source/tool/context. If isolation is violated, label the run `CONTAMINATED`.
