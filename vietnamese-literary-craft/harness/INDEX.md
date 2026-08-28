# Harness Index

Keep runner and evaluator artifacts separate.

## Frozen evidence chain
- CLEAN-BASELINE-8: 15/16, hard fail 0.
- TARGETED-PROBE-ABSTRACT-BODY: 8/8, hard fail 0.
- BASELINE-36: 71/72, hard fail 0.
- OPERATIONAL-VALIDATION-BUNDLE v0: 48/50, hard fail 0; no preservation/epistemic/voice-register/routing regression; repeated sensory-mediation failure confirmed.
- SENSORY-MEDIATION-REPAIR-REGRESSION v0.1: 24/24, hard fail 0; narrow patch promoted.
- FOUNDATION-INTEGRATION v0.5: 32/32, hard fail 0.
- INTERMEDIATE-INTEGRATION v0.5: 32/32, hard fail 0.
- ADVANCED-INTEGRATION v0.3: 32/32, hard fail 0.
- WRITER_SELF_REVIEW-INTEGRATION v0.3: 31/32, hard fail 0; targeted closure v0.3.1: 12/12, hard fail 0.

## Knowledge Expansion Wave 1
- `suites/knowledge-wave1-red-24-runner.md` + `golden-cases/knowledge-wave1-red-24-evaluator.md`: `RED / DIAGNOSTIC / NOT A PROMOTION GATE`; 24 blind pressure cases, scoring `2/1/0`, max 48. Raw clean baseline must be frozen before KX1–KX10 rule authoring.

## Physical-load regression order
1. Load this physical skill candidate using the actual runtime directory/path order.
2. Run `suites/baseline-36-runner.md` blind; score against `golden-cases/baseline-36.md` only after raw output is frozen.
3. Run `regression/sensory-mediation-runner.md` blind; score with `regression/sensory-mediation-evaluator.md` only after raw output is frozen.
4. Run compact load sentinels across Foundation, Intermediate, Advanced, and Writer Self Review: observation-vs-inference; intentional fragment; historical/source HOLD; POV access; causal reset; prepared/stateful voice; fair reveal; reliability uncertainty; false-allusion HOLD; functional hybridity; edition/translation boundary; author-memory contamination; blocker priority; epistemic regression diff; no-pass-6 release.
5. Reject the physical candidate if any new preservation, epistemic, voice/register, routing, source-attribution, pass-cap, or curriculum-routing regression appears.

Stable case IDs from BASELINE-36 must not change during migration. Golden material never enters blind runner packets.
