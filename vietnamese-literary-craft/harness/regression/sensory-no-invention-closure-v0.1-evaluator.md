# SENSORY NO-INVENTION CLOSURE v0.1 — Evaluator

## Status
`FROZEN / TARGETED CLOSURE / EVALUATOR-ONLY`

Runner: `harness/regression/sensory-no-invention-closure-v0.1-runner.md`

Score each case `2 / 1 / 0`. Maximum `6`.

Promotion closure gate:
`6/6 + HARD FAIL 0`.

This closure supplements the current BASELINE-36 and SENSORY-MEDIATION blast-radius evidence. It does not erase their parent scores.

## Hard fails
Any one of the following is a hard fail:
1. inventing a body site, garment, wetness, contact point, posture, movement, or sensory fact not supplied by SNC-01/SNC-02;
2. preserving unsupported whole-body propagation solely to avoid invention;
3. adding ornamental metaphor or a sensory stack where a direct bounded repair is sufficient;
4. broad paragraph/scene rewrite for this sentence-local defect.

### SNC-01
EXPECTED ACTION: `MIN_EDIT`.

Full credit requires:
- remove redundant mediation/nominalization such as `khiến ... cảm thấy một cảm giác`;
- remove generic unsupported propagation such as `len lỏi trong cơ thể`;
- preserve only the supplied dense-mist + cold-sensation facts;
- do not invent a body site, clothing, wetness, wind contact, or new action.

Accept any natural direct equivalent that stays within those facts, e.g. a bounded formulation equivalent in effect to `Sương dày. Hắn lạnh.` or another natural Vietnamese sentence that removes mediation without adding new sensory facts.

### SNC-02
EXPECTED ACTION: `MIN_EDIT`.

Full credit requires:
- remove redundant mediation/nominalization;
- remove unsupported whole-body propagation;
- preserve only harsh sun + hot/burning sensation;
- do not invent a body site, sweat, clothing, skin detail, movement, or contact point.

### SNC-03
EXPECTED ACTION: `MIN_EDIT`.

Full credit requires:
- remove redundant mediation;
- remove unsupported whole-body propagation;
- use only the supplied hot-wind contact on the face as grounding;
- do not spread the sensation to a new body location or add a new response/ornament.

A strong equivalent may keep the first sentence and localize the second to the already supplied face contact.

## Interpretation
`6/6 + HARD FAIL 0` closes the sensory source-boundary precision miss and can serve as the targeted closure for the overlapping BASELINE PC-002 grounding miss. It does not by itself validate the broader runtime.
