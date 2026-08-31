# SCENE DYNAMICS ACTION-SCALE CLOSURE v0.1 — Blind Runner

## Status
`FROZEN / TARGETED CLOSURE / RUNNER-ONLY`

## Purpose
Close two action-scale misses from Scene Dynamics v0.1. This closure does not add a new narrative rule. It distinguishes a local sentence/phrase repair (`MIN_EDIT`) from a bounded multi-turn or multi-paragraph restructuring (`REVISE`).

## Isolation
Run in one clean conversation with the same skill under test loaded. Do not expose evaluator/golden files. Do not use web/search, project memory, prior-chat context, private sources, or outside references.

Return exactly:
`CASE_ID / ACTION / OUTPUT / REASON`

Allowed actions:
`PRESERVE / MIN_EDIT / REVISE / HOLD-INSUFFICIENT_EVIDENCE`

Do not self-score.

### SDC-01 — Post-danger exchange recovery
TASK: choose the smallest correct action scale and repair scope.
INPUT: Six emergency turns while smoke enters a room are appropriately compressed. Everyone reaches the courtyard safely. The following ten turns discuss a forgotten coat and whether a child should sit down, but all ten remain one-to-three-word exchanges with no address terms, reassurance, explanation, hesitation, or syntactic recovery. The first six turns work and must remain untouched. Restoring natural post-danger speech requires changing several of the ten later turns, not merely deleting or replacing one sentence.

### SDC-02 — Paragraph-ending cadence saturation
TASK: choose the smallest correct action scale and repair scope.
INPUT: In a 700-word confrontation, thirteen of fifteen paragraphs end with isolated short declaratives. Two mark genuine turns and should remain. Eleven others restate prior meaning. Repair requires removing, merging, or redistributing endings across multiple paragraphs while preserving the scene's existing causal movement and voices. No new event or chapter rewrite is needed.

## Completeness gate
A valid run answers SDC-01 and SDC-02 exactly once in one uninterrupted execution with no external source/tool/context. If isolation is violated, label the run `CONTAMINATED`.
