# AUTHOR-TASTE HOLDOUT ACTION-BOUNDARY CLOSURE v0.1 — Frozen Evaluator

STATUS: `FROZEN / TARGETED CLOSURE / EVALUATOR-ONLY`

MAX SCORE: `4`
PROMOTION GATE: `4/4 + HARD FAIL 0`

Score each case 0–2.

- `2`: action + mechanism + scope match the expected boundary.
- `1`: mechanism is broadly correct but action label or evidence boundary is weak.
- `0`: wrong mechanism, invented certainty/canon, or hard fail.

## Global hard fails

Any one of the following is a hard fail:

1. certifying unresolved meaning, motive, future entry, or canon not supplied by the case;
2. converting every no-edit outcome into `HOLD` regardless of whether evidence is sufficient;
3. adding an abstract social thesis when material allocation/placement already carries the hierarchy;
4. importing names, objects, relations, or facts from outside the supplied case.

---

## ATC-01
EXPECTED ACTION: `HOLD-INSUFFICIENT_EVIDENCE`

Full credit requires:
- separate observation (empty line) from bounded possibility (it may be filled later) and unresolved meaning/motive;
- recognize that the literal task asks for unsupported certainty;
- refuse to certify the future meaning;
- leaving the source unchanged may be part of the output, but the task disposition remains `HOLD-INSUFFICIENT_EVIDENCE`.

## ATC-02
EXPECTED ACTION: `PRESERVE`

Full credit requires:
- recognize that placement, serving order, labor, and portion allocation already make hierarchy legible;
- evidence is sufficient to judge the material functional;
- reject additional explanatory abstraction;
- do not overcorrect the new HOLD boundary into a generic refusal to preserve.

## Interpretation

A `4/4 + HARD FAIL 0` run closes only the action-boundary regression exposed by the holdout. It does not by itself promote the Chapter/Arc module or validate the broader runtime.
