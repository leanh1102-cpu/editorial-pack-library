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

## Compatible-loader runtime validation · 2026-08-29
- Runtime install snapshot: `install/vietnamese-literary-craft-wave1-runtime` @ `c50bc5f4316c3b85ce707c84616bda9347d3f280`; installed bundle excludes `harness/` so evaluator/golden material stays outside the skill under test.
- Runtime smoke v0.1: `RS-01…RS-08 = 8/8 behavior checks / HARD FAIL 0`.
- Full installed-loader regression: `BASELINE-36 = 72/72`, `SENSORY-MEDIATION = 24/24`, `CROSS-LAYER = 29/30`, hard fail 0. The only miss was XR-05 action scale (`REVISE` vs sentence-local `MIN_EDIT`); causal mechanism remained correct.
- Installed-loader targeted closure: `XA-01 = 2/2`, `XA-02 = 2/2`; total `4/4`, hard fail 0.
- Runtime verdict: `RUNTIME-VALIDATED / COMPOSITE PASS / HARD FAIL 0` for the current Wave 1 runtime snapshot and validated source scope.
- This verdict does not imply full frozen knowledge-architecture completion; specialized source debt remains separately gated.

## Production-soak patch · Dialogue Texture v0.1 · 2026-08-29
- Trigger: real reader feedback during manuscript soak identified repeated proposition-only clipped dialogue as a material readability/voice problem; the existing KX6 dialogue module protected functional brevity but did not explicitly diagnose exchange-level terse saturation.
- Scope: bounded patch to `craft/dialogue.md` + `evaluation/ai-writing-rubric.md`; no change to `CONSTITUTION.md`, curriculum, runtime stop policy, `core/`, or `packs/sltd/`.
- Targeted regression: `dialogue-texture-terse-saturation = 24/24`, hard fail 0. Promotion interpretation: `FUNCTIONAL BREVITY PRESERVED / EXCHANGE-LEVEL TERSE SATURATION REPAIRED / NO LENGTH QUOTA`.
- Candidate blast radius: `BASELINE-36 = 72/72`, hard fail 0; `SENSORY-MEDIATION = 22/24`, hard fail 1 from R-02 adding an unsupported weather source; `CROSS-LAYER = 29/30`, hard fail 0 from XR-05 action scale (`REVISE` vs local `MIN_EDIT`). Neither miss demonstrated a Dialogue Texture mechanism failure.
- Targeted blast-radius closure: `DB-01 = 2/2`, `DB-02 = 2/2`; total `4/4`, hard fail 0. Composite verdict: no demonstrated residual regression on sensory source preservation or sentence-local causal repair.
- Promotion status: `DIALOGUE-TEXTURE v0.1 / VALIDATED / COMPOSITE PASS / HARD FAIL 0`.
- PR #29 squash-merged to `main` at `bc047fefc11ed0dd856e22538f7df0b0ab8dd09f`.
- Official runtime snapshot: `install/vietnamese-literary-craft-dialogue-texture-v0.1-runtime` @ `b4a64b0845e7006837cea864fb9bbac5c0f68f06`. This branch is byte-identical to the candidate runtime bundle used for targeted and blast-radius execution; it intentionally excludes `harness/`.
- Runtime interpretation: Dialogue Texture v0.1 behavior is `RUNTIME-VALIDATED / COMPOSITE PASS` on the tested bundle. The `main` module contains a metadata-only promotion-status update after the runtime run; no behavior rule changed after testing.

## Narrative Dynamics + Author-Taste v0.1 · 2026-09-01
- Author-Taste Prose: `28/28 / HARD FAIL 0`; `FROZEN CLOSED / PASS / NO-OP BY TDD`. No `craft/prose-naturalness.md` created.
- Scene Dynamics: parent `22/24 / HARD FAIL 0` plus targeted action-scale closure `4/4 / HARD FAIL 0`; `FROZEN CLOSED / COMPOSITE PASS / NO-OP BY TDD`. No `craft/scene-dynamics.md` created.
- Chapter / Arc Rhythm: targeted behavior green; Author-Taste holdout and blast-radius composite passes closed; runtime-focused and runtime-smoke gates below validate the installed package route. Status: `VALIDATED / RUNTIME-VALIDATED`.
- Author-Taste Holdout: frozen parent `19/20 / HARD FAIL 0`; targeted action-boundary closure `ATC-01..02 = 4/4 / HARD FAIL 0`; verdict `FROZEN CLOSED / COMPOSITE PASS`. The original holdout remains historically 19/20 rather than being rewritten as 20/20.
- Blast-radius BASELINE-36: parent `71/72 / HARD FAIL 0`; sole `PC-002` sensory-grounding miss is covered by the post-fix sensory no-invention closure below. Parent score remains historical.
- Blast-radius SENSORY-MEDIATION: parent `22/24 / HARD FAIL 1`; failure localized to unsupported sensory/body invention and propagation handling. Post-fix `sensory-no-invention-closure-v0.1 = 6/6 / HARD FAIL 0`; verdict `COMPOSITE PASS`. The parent hard-fail result remains preserved as pre-fix evidence.
- Blast-radius CROSS-LAYER: parent `29/30 / HARD FAIL 0`; sole `XR-05` action-scale miss closed by `knowledge-wave1-cross-layer-action-closure = 4/4 / HARD FAIL 0`; verdict `COMPOSITE PASS`.
- Blast-radius DIALOGUE TEXTURE: `24/24 / HARD FAIL 0`; `FROZEN CLOSED / PASS`.
- Blast-radius aggregate: `COMPOSITE PASS / CURRENT HARD FAIL 0`; no parent suite rerun required after targeted closures.
- Routing gate: `multi-scene / chapter / arc rhythm → analysis/chapter-arc-rhythm.md` added to `SKILL.md`.
- Runtime snapshot: `install/vietnamese-literary-craft-narrative-dynamics-author-taste-v0.1-runtime` @ `40608c73103dab76d83b7fc3b34b4b1dea293f84`; package-only root, `harness/` and candidate corpus excluded; `CONSTITUTION.md` blob remains `1b3727dbfc41691b973d02d767b97f3b0b8aa63e`.
- Runtime-focused blind validation: `RV-01..RV-08 = 16/16 / HARD FAIL 0`; verdict `RUNTIME-FOCUSED PASS / FROZEN CLOSED`.
- Runtime install smoke: `RS-01..RS-04 = 8/8 / HARD FAIL 0`; verdict `RUNTIME-SMOKE PASS / FROZEN CLOSED`.
- Runtime aggregate: `RUNTIME-VALIDATED / COMPOSITE PASS / HARD FAIL 0` for Narrative Dynamics + Author-Taste v0.1 on the tested installed snapshot.
- Freeze consequence: do not rerun ATP, Scene Dynamics, Holdout, parent blast-radius suites, runtime-focused, or runtime-smoke unless fresh independent evidence demonstrates a regression in that closed node.

## Physical-load regression order
1. Load this physical skill candidate using the actual runtime directory/path order.
2. Run `suites/baseline-36-runner.md` blind; score against `golden-cases/baseline-36.md` only after raw output is frozen.
3. Run `regression/sensory-mediation-runner.md` blind; score with `regression/sensory-mediation-evaluator.md` only after raw output is frozen.
4. Run `regression/knowledge-wave1-cross-layer-sentinels-runner.md` blind; score with `regression/knowledge-wave1-cross-layer-sentinels-evaluator.md` only after raw output is frozen.
5. Reject the physical candidate if any new preservation, epistemic, voice/register, routing, source-attribution, pass-cap, or curriculum-routing regression appears.

Stable case IDs from BASELINE-36 must not change during migration. Golden material never enters blind runner packets.
