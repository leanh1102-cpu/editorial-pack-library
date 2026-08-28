# Harness Index

Keep runner and evaluator artifacts separate.

## Frozen evidence chain
- CLEAN-BASELINE-8: 15/16, hard fail 0.
- TARGETED-PROBE-ABSTRACT-BODY: 8/8, hard fail 0.
- BASELINE-36 initial baseline: 71/72, hard fail 0.
- OPERATIONAL-VALIDATION-BUNDLE v0: 48/50, hard fail 0; no preservation/epistemic/voice-register/routing regression; repeated sensory-mediation failure confirmed.
- SENSORY-MEDIATION-REPAIR-REGRESSION v0.1: 24/24, hard fail 0; narrow patch promoted.
- FOUNDATION-INTEGRATION v0.5: 32/32, hard fail 0.
- INTERMEDIATE-INTEGRATION v0.5: 32/32, hard fail 0.
- ADVANCED-INTEGRATION v0.3: 32/32, hard fail 0.
- WRITER_SELF_REVIEW-INTEGRATION v0.3: 31/32, hard fail 0; targeted closure v0.3.1: 12/12, hard fail 0.

## Knowledge Expansion Wave 1
- `suites/knowledge-wave1-red-24-runner.md` + `golden-cases/knowledge-wave1-red-24-evaluator.md`: `RED / DIAGNOSTIC / NOT A PROMOTION GATE`.
- `suites/knowledge-wave1-red-action-closure-runner.md` + `golden-cases/knowledge-wave1-red-action-closure-evaluator.md`: 7/8, hard fail 0.
- `suites/knowledge-wave1-red-minedit-closure-runner.md` + `golden-cases/knowledge-wave1-red-minedit-closure-evaluator.md`: 2/2, hard fail 0.
- Task 1: `MECHANISM BASELINE STRONG / ACTION TAXONOMY CALIBRATED / CLOSED`.
- KX1–KX10 validation: original 47/48, hard fail 0; `knowledge-wave1-transfer-closure` 4/4, hard fail 0. Result: `KX1–KX10 CANDIDATE-STABLE / VALIDATED`; KX9–KX10 retain narrow source scope and KX10 remains diagnostic-only.
- Wave 1 integration blind: original 23/24, hard fail 0; `knowledge-wave1-integration-sensory-closure` 4/4, hard fail 0.
- Blast-radius rerun: `BASELINE-36 = 72/72`, hard fail 0; `SENSORY-MEDIATION-REPAIR-REGRESSION = 24/24`, hard fail 0.
- Cross-layer blast radius: original 28/30, hard fail 0; `knowledge-wave1-cross-layer-action-closure` 4/4, hard fail 0.
- Task 7: `KNOWLEDGE-WAVE1-INTEGRATED v0.1 / BLAST-RADIUS COMPOSITE PASS / HARD FAIL 0`.

## Physical-load regression order
1. Load this physical skill candidate using the actual runtime directory/path order.
2. Run `suites/baseline-36-runner.md` blind; score against `golden-cases/baseline-36.md` only after raw output is frozen.
3. Run `regression/sensory-mediation-runner.md` blind; score with `regression/sensory-mediation-evaluator.md` only after raw output is frozen.
4. Run `regression/knowledge-wave1-cross-layer-sentinels-runner.md` blind; score with `regression/knowledge-wave1-cross-layer-sentinels-evaluator.md` only after raw output is frozen.
5. Reject the physical candidate if any new preservation, epistemic, voice/register, routing, source-attribution, pass-cap, or curriculum-routing regression appears.

Stable case IDs from BASELINE-36 must not change during migration. Golden material never enters blind runner packets.
