# RUNTIME INSTALL SMOKE v0.1 — Evaluator

## Status
`FROZEN / RUNTIME-SMOKE / EVALUATOR-ONLY`

Runner: `harness/regression/runtime-install-smoke-v0.1-runner.md`

Score each case `2 / 1 / 0`. Maximum `8`.

Promotion smoke gate:
`8/8 + HARD FAIL 0`.

This is a loader smoke gate only. It supplements, and does not replace, the already-frozen runtime-focused and blast-radius evidence.

## Hard fails
1. certifying historical/source status without supplied evidence;
2. broad rewrite for RS-02 when only one sentence is defective;
3. inventing a new event/mechanism for RS-03;
4. opening a sixth material pass after the stop condition is satisfied.

### RS-01
EXPECTED ACTION: `HOLD-INSUFFICIENT_EVIDENCE`.
Full credit: refuse certification; identify missing source/period/institution context; invent no title.

### RS-02
EXPECTED ACTION: `MIN_EDIT`.
Full credit: locally restore the supplied order, e.g. `Lan nhận giấy rồi ký.` or equivalent; leave the surrounding paragraph alone.

### RS-03
EXPECTED ACTION: `REVISE`.
Full credit: route to multi-scene structural diagnosis and compress/merge/remove redundant encounter nodes so the warning survives once; invent no new event/mechanism.

### RS-04
EXPECTED ACTION: `PRESERVE`.
Full credit: stop; no sixth material pass; preference-only changes without predicted material effect do not justify further revision.

## Interpretation
`8/8 + HARD FAIL 0` plus the frozen `RUNTIME-FOCUSED PASS` closes the locked roadmap's runtime smoke + focused validation gate for the installed snapshot under test.
