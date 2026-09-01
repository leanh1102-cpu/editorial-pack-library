# SCENE DYNAMICS ACTION-SCALE CLOSURE v0.1 — Frozen Evaluator

STATUS: `FROZEN / EVALUATOR-ONLY`

MAX SCORE: `4`
PROMOTION GATE: `4/4 + HARD FAIL 0`

Score each case 0–2.

- `2`: action + mechanism + scope match.
- `1`: mechanism is correct but action scale remains too small or too broad.
- `0`: mechanism is wrong or a hard fail occurs.

## Global hard fails

1. changing the functional emergency turns in SDC-01;
2. lengthening every later turn mechanically;
3. banning short paragraph endings in SDC-02;
4. deleting the two functional turn endings;
5. inventing a new event, emotion certainty, relationship, or canon fact;
6. broad chapter rewrite.

## SDC-01
EXPECTED ACTION: `REVISE`

Full credit requires:
- preserve the first six emergency turns;
- revise several of the ten post-danger turns so speech selectively recovers relation/syntax/reassurance or hesitation;
- recognize that a multi-turn exchange repair exceeds sentence-local `MIN_EDIT` even though the scene-level scope remains bounded;
- do not lengthen every turn.

## SDC-02
EXPECTED ACTION: `REVISE`

Full credit requires:
- preserve the two functional short endings;
- remove/merge/redistribute the eleven redundant endings across multiple paragraphs;
- recognize that a multi-paragraph cadence repair exceeds sentence-local `MIN_EDIT` while remaining far smaller than a chapter rewrite;
- do not create a quota or ban on short paragraph endings.

## Interpretation

A 4/4 closure resolves action-scale classification only. It does not add scene-dynamics mechanism evidence beyond the parent 22/24 run.
