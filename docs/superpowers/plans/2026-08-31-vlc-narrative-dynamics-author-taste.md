# VLC Narrative Dynamics + Author-Taste Golden v0.1 Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Build and validate a canon-neutral human-calibrated prose + narrative-dynamics layer for Vietnamese Literary Craft without coupling VLC to PAI repositories or private manuscript bodies.

**Architecture:** Public repo stores sanitized mechanism candidates, blind runners/evaluators, craft modules and runtime snapshots. Private Notion/Drive retain source provenance and owner-review evidence. Promotion follows TDD: candidate evidence → frozen RED suites → minimal module changes → holdout → blast-radius → router/index → merge → runtime snapshot.

**Tech Stack:** Markdown Agent Skill package, GitHub branches/PRs, blind markdown harnesses, Notion/Google Drive provenance staging.

**Spec:** `docs/superpowers/specs/2026-08-31-vlc-narrative-dynamics-author-taste-design.md`

## Global Constraints

- Do not modify `vietnamese-literary-craft/CONSTITUTION.md`.
- Do not modify `core/` or `packs/sltd/`.
- Do not create workflows, Actions, automation, issues, project boards, scripts, or live manuscript copies.
- Do not write to `pai-control-plane` or any PAI/Linux repository in this plan.
- Do not copy private manuscript bodies, canon, private URLs, or long verbatim source excerpts into the public repo.
- Do not call TRAIN material evidence of generalization.
- Holdout is frozen before evaluator exposure.
- No quota rules for sentence length, dialogue length, beat count, climax count, or quiet beats.
- Existing `SKILL.md` router changes are deferred until all new validation gates pass.

## Execution Freeze Ledger — 2026-09-01

This ledger is authoritative over the older unchecked implementation steps below whenever TDD evidence has superseded the original implementation intent. Do not recreate a skipped module merely because an old checkbox still says `Create`.

General freeze rule:

`FROZEN CLOSED NODE ≠ REOPEN ON NEW COMMIT`

Reopen a closed node only when:
- fresh independent regression evidence demonstrates a failure in that node;
- the user explicitly changes the locked scope or behavior contract; or
- a downstream validation gate proves the node itself is the causal regression source.

Do **not** reopen a node because branch HEAD moved, files were committed later, or a subsequent task is still pending.

### Node 1 — Author-Taste Vietnamese Prose

Status: `FROZEN CLOSED / PASS / NO-OP BY TDD`

Evidence state:
- frozen ATP suite completed at `28/28 / HARD FAIL 0`;
- sanitized candidate corpus is materialized and remains `CANDIDATE / SANITIZED / NOT GOLDEN`;
- runtime behavior already covered the targeted prose/relational-texture failure boundaries.

Execution consequence:
- do **not** create `craft/prose-naturalness.md`;
- do **not** modify the prose layer merely to satisfy Task 3's original file list;
- retain the frozen ATP evidence unless a new independent regression specifically breaks it.

### Node 2 — Scene Dynamics

Status: `FROZEN CLOSED / COMPOSITE PASS / NO-OP BY TDD`

Evidence state:
- frozen parent suite: `22/24 / HARD FAIL 0`;
- the only misses were action-scale classification, not scene-dynamics mechanism failures;
- targeted action-scale closure satisfied its contract at `4/4 / HARD FAIL 0`.

Execution consequence:
- do **not** create `craft/scene-dynamics.md`;
- preserve current runtime handling of useful quiet, aftermath, fake escalation, pressure recovery, and cadence saturation;
- do not rerun the parent suite merely because later nodes change.

### Node 3 — Chapter / Arc Rhythm

Status: `CANDIDATE / TDD TARGETED GREEN / HOLDOUT PENDING`

Evidence state:
- frozen parent RED baseline exposed the first material gap: `13/20 / HARD FAIL 0`;
- the minimal source-grounded intervention policy raised the targeted rerun to `18/20 / HARD FAIL 0`;
- remaining misses were `REVISE vs HOLD` over-restraint when structural repair remained possible without inventing a new mechanism;
- policy-closure runner/evaluator now exist in the repository;
- historical user output satisfied the closure contract, but must **not** be retroactively described as a frozen-evaluator `4/4` run because the evaluator was not frozen before that execution.

Execution consequence:
- keep `analysis/chapter-arc-rhythm.md` at `CANDIDATE / TDD TARGETED GREEN / HOLDOUT PENDING`;
- do not call it `VALIDATED` yet;
- do not rerun the whole chapter-rhythm suite solely to replace the earlier evidence chain.

### Node 4 — Author-Taste Holdout

Status: `ACTIVE GATE / FROZEN HOLDOUT FAMILY / TARGETED CLOSURE PENDING`

Evidence state:
- holdout runner and evaluator were frozen before the blind run;
- blind holdout result: `19/20 / HARD FAIL 0`;
- sole miss: `ATH-04`, where mechanism/source discipline was correct but action was `PRESERVE` instead of evidence-blocked `HOLD-INSUFFICIENT_EVIDENCE`;
- production patch is deliberately narrow: requested-task disposition now distinguishes sufficient-evidence `PRESERVE` from evidence-blocked `HOLD`;
- targeted `ATC-01/ATC-02` closure runner and evaluator are frozen before execution.

Required next evidence:
- run only `author-taste-holdout-action-boundary-closure-v0.1-runner.md` in a clean isolated conversation;
- gate: `4/4 + HARD FAIL 0`;
- do **not** rerun `ATH-01…ATH-10` if the targeted closure passes;
- do **not** self-run the closure in a context where its evaluator has already been exposed.

### Node 5 — Blast Radius

Status: `READY / BLOCKED BY NODE 4`

Frozen suites already confirmed present:
- `BASELINE-36`;
- `SENSORY-MEDIATION-REPAIR-REGRESSION`;
- `KNOWLEDGE-WAVE1-CROSS-LAYER-SENTINELS`;
- `DIALOGUE-TEXTURE / TERSE-SATURATION`.

Execution consequence:
- do not create replacement blast-radius harnesses;
- do not run Task 7 before Node 4 closes;
- after Node 4 closes, run only the existing frozen suites in the locked order and use targeted closure only for a demonstrated narrow miss.

### Nodes 6–7 — Promotion / Runtime Snapshot / Downstream Contract

Status: `NOT OPEN`

Do not:
- modify `SKILL.md` before validation evidence demonstrates a routing need;
- create a runtime snapshot before blast-radius closure;
- write the PAI downstream consumer contract before a validated runtime snapshot exists;
- treat candidate or composite targeted-green evidence as `RUNTIME-VALIDATED`.

---

### Task 1: Materialize the sanitized author-taste corpus boundary

**Files:**
- Create: `vietnamese-literary-craft/corpus/INDEX.md`
- Create: `vietnamese-literary-craft/corpus/candidate/author-taste-vietnamese-prose-v0.1.md`

**Interfaces:**
- Consumes: owner-approved positive-control mechanisms from private upstream sources; production deltas supplied by the author.
- Produces: canon-neutral candidate IDs `AT-VP01...` used by later harnesses.

- [ ] **Step 1: Create corpus index**

Record three states only: `candidate`, `validated`, `core`; explicitly state that public corpus entries contain anonymized mechanism evidence, not manuscript source text.

- [ ] **Step 2: Create candidate control set**

Freeze at least 10 controls covering: functional short sentence, spatial-to-body anchoring, working environment detail, body/history through object, concrete intelligence, material-specific sound, relational dialogue/face-saving, action-built silence, domestic object carrying cost/relationship, movement-based scene seam, plus the production-observed terse-saturation boundary.

Each item must use:
`ID / SOURCE_CLASS / SCOPE / OBSERVABLES / MECHANISM / FAILURE_BOUNDARY / PRESERVE_BOUNDARY / ANONYMIZED_CASE / TRANSFER_RISK / STATUS`.

- [ ] **Step 3: Verify privacy boundary**

Check the two files contain no project character names, private links, raw manuscript passages, or cross-project canon.

- [ ] **Step 4: Commit**

Commit message: `corpus: add author-taste prose candidates`

---

### Task 2: Freeze RED author-taste prose regression

**Files:**
- Create: `vietnamese-literary-craft/harness/suites/author-taste-prose-v0.1-runner.md`
- Create: `vietnamese-literary-craft/harness/golden-cases/author-taste-prose-v0.1-evaluator.md`

**Interfaces:**
- Consumes: `AT-VP*` candidate mechanisms.
- Produces: a blind 12–16 case gate with paired PRESERVE/REVISE boundaries.

- [ ] **Step 1: Write runner before any new craft module**

Include paired cases for:
- functional short sentence vs row of artificial short sentences;
- low-pressure family dialogue with relational texture vs proposition-only exchange;
- action-built silence vs explanatory emotion label;
- working domestic detail vs decorative sensory list;
- natural unevenness vs polish-for-polish's-sake;
- movement/pressure seam vs thematic maxim ending.

- [ ] **Step 2: Write frozen evaluator**

Score 2 points/case; define hard fails for quota rules, invented plot facts, dialect normalization, surface imitation, and broad rewrite for a local defect.

- [ ] **Step 3: Verify runner/evaluator isolation**

Runner must not reveal expected actions or scoring key.

- [ ] **Step 4: Commit**

Commit message: `test: freeze author-taste prose regression`

---

### Task 3: Add minimal prose-naturalness operational module

**Files:**
- Create: `vietnamese-literary-craft/craft/prose-naturalness.md`
- Modify: `vietnamese-literary-craft/evaluation/ai-writing-rubric.md`

**Interfaces:**
- Consumes: Task 2 failure boundaries.
- Produces: operational rules for Vietnamese relational texture, paragraph/scene rhythm, and preservation of living roughness.

- [ ] **Step 1: Implement module contract**

Use the standard module sections and add the operational sequence:
`OBSERVE LOCAL TEXTURE → READ EXCHANGE/PARAGRAPH → CHECK RELATIONAL LOAD → CHECK RHYTHM VARIATION → IDENTIFY MATERIAL FAILURE → SMALLEST INTERVENTION → RE-READ WHOLE SCENE`.

- [ ] **Step 2: Add anti-overcorrection boundaries**

Explicitly forbid: universal sentence minimums, extending every short turn, adding particles mechanically, forced dialect, emotion explanation, and ornamental sensory inflation.

- [ ] **Step 3: Extend rubric**

Add `VIETNAMESE_RELATIONAL_TEXTURE`, `EXCHANGE_VARIATION`, `LIVING_ROUGHNESS`, `PROPOSITION_ONLY_RISK`, without changing existing score semantics.

- [ ] **Step 4: Run Task 2 blind suite in a clean loader**

Gate: full score + hard fail 0. If miss, use targeted closure only; no broad patch.

- [ ] **Step 5: Commit after green evidence**

Commit message: `feat: add Vietnamese prose naturalness layer`

---

### Task 4: Freeze and implement Scene Dynamics v0.1

**Files:**
- Create: `vietnamese-literary-craft/harness/suites/scene-dynamics-v0.1-runner.md`
- Create: `vietnamese-literary-craft/harness/golden-cases/scene-dynamics-v0.1-evaluator.md`
- Create: `vietnamese-literary-craft/craft/scene-dynamics.md`

**Interfaces:**
- Consumes: scene-level pressure evidence.
- Produces: `STATE → PRESSURE → CHOICE/RESISTANCE → TURN → CONSEQUENCE → RECOVERY/NEW PRESSURE` diagnostic map.

- [ ] **Step 1: Freeze RED runner**

Include cases for quiet beat with function, false flatness, escalation by cost, fake escalation by louder language, aftermath, reveal that changes interpretation, repeated information beats, and deliberate low-intensity scene.

- [ ] **Step 2: Freeze evaluator**

Hard fail if the answer invents an external event to create excitement, deletes a useful quiet beat, or turns the diagnostic map into a required six-beat template.

- [ ] **Step 3: Implement minimal scene module**

Teach pressure contrast and causal/relational movement; do not prescribe beat quotas.

- [ ] **Step 4: Blind validation**

Gate: full score + hard fail 0 or documented targeted closure + hard fail 0.

- [ ] **Step 5: Commit**

Commit message: `feat: add scene dynamics judgment`

---

### Task 5: Add Chapter / Arc Rhythm harness and diagnostic module

**Files:**
- Create: `vietnamese-literary-craft/harness/suites/chapter-rhythm-v0.1-runner.md`
- Create: `vietnamese-literary-craft/harness/golden-cases/chapter-rhythm-v0.1-evaluator.md`
- Create: `vietnamese-literary-craft/analysis/chapter-arc-rhythm.md`

**Interfaces:**
- Consumes: ordered multi-scene packets.
- Produces: diagnostics for pressure plateau, repeated mechanism, climax preparation, aftermath, seam variation, and type-of-climax repetition.

- [ ] **Step 1: Freeze multi-scene RED cases**

At least 8 packets of 4–8 scene summaries each. Include both healthy irregular rhythm and genuine plateau.

- [ ] **Step 2: Freeze evaluator**

Require evidence from ordering and change-of-state; prohibit generic prescriptions like “add action scene”.

- [ ] **Step 3: Implement diagnostic module**

Operational sequence:
`MAP SCENE FUNCTION → MAP PRESSURE TYPE → FIND REPETITION/PLATEAU → LOCATE TURN/COST → CHECK AFTERMATH → CHECK SEAM → RECOMMEND SMALLEST STRUCTURAL CHANGE`.

- [ ] **Step 4: Blind validation**

Gate: full score + hard fail 0 or targeted closure with hard fail 0.

- [ ] **Step 5: Commit**

Commit message: `feat: add chapter and arc rhythm diagnosis`

---

### Task 6: Freeze Author-Taste holdout and test transfer

**Files:**
- Create: `vietnamese-literary-craft/harness/suites/author-taste-holdout-v0.1-runner.md`
- Create: `vietnamese-literary-craft/harness/golden-cases/author-taste-holdout-v0.1-evaluator.md`

**Interfaces:**
- Consumes: source spans not used in Tasks 1–5.
- Produces: generalization evidence separate from TRAIN/REFERENCE.

- [ ] **Step 1: Select holdout privately before authoring cases**

Record provenance in private staging only. Public case text must be anonymized.

- [ ] **Step 2: Freeze runner and evaluator**

Include transfer across different relationship structures, pressure levels, dialogue density, and scene functions.

- [ ] **Step 3: Run blind**

Gate: full score or a predeclared tolerance with zero hard fails; surface imitation is always hard fail.

- [ ] **Step 4: Classify misses**

Separate `KNOWLEDGE GAP / ROUTING GAP / ACTION-SCALE GAP / TEST AMBIGUITY / SOURCE DEBT` before patching.

- [ ] **Step 5: Commit only validated adjustments**

Commit message: `test: validate author-taste transfer holdout`

---

### Task 7: Blast-radius existing validated stack

**Files:**
- Modify only if evidence promotion requires: `vietnamese-literary-craft/harness/INDEX.md`

**Interfaces:**
- Consumes: existing frozen suites.
- Produces: no-regression evidence for the new layer.

- [ ] **Step 1: Run BASELINE-36**

Gate: `72/72 / hard fail 0` or targeted closure for action-scale-only miss.

- [ ] **Step 2: Run SENSORY-MEDIATION**

Gate: `24/24 / hard fail 0` or narrow closure with no invented source/body detail.

- [ ] **Step 3: Run cross-layer sentinels**

Gate: full/composite pass, hard fail 0.

- [ ] **Step 4: Run Dialogue Texture v0.1 regression**

Gate: full/composite pass, hard fail 0.

- [ ] **Step 5: Update Harness Index only after all gates close**

Record exact evidence chain; do not call runtime validated yet.

- [ ] **Step 6: Commit**

Commit message: `docs: record narrative dynamics validation evidence`

---

### Task 8: Router promotion and runtime validation

**Files:**
- Modify: `vietnamese-literary-craft/SKILL.md`
- Possibly modify: `vietnamese-literary-craft/glossary/TERMS.md` only for genuinely stable new terms.

**Interfaces:**
- Consumes: fully validated modules.
- Produces: minimal progressive-loading routes for prose naturalness, scene dynamics, and chapter/arc rhythm.

- [ ] **Step 1: Add narrow router entries**

Do not embed theory in `SKILL.md`; route only when task scope needs the module.

- [ ] **Step 2: Verify governance**

Confirm `CONSTITUTION.md` blob unchanged; no `core/`, `packs/sltd/`, PAI repo, workflow or automation changes.

- [ ] **Step 3: Build runtime snapshot without `harness/`**

Snapshot must contain exactly the runtime package, not golden/evaluator files.

- [ ] **Step 4: Run runtime smoke + focused new suites**

Use installed snapshot in clean chats. Only promote `RUNTIME-VALIDATED` after observed compatible-loader evidence.

- [ ] **Step 5: Commit promotion metadata**

Commit message: `feat: promote narrative dynamics and author taste v0.1`

---

### Task 9: PR, merge, and downstream PAI handoff contract

**Files:**
- Create: `vietnamese-literary-craft/maintenance/pai-git-consumer-contract.md`

**Interfaces:**
- Consumes: validated runtime snapshot commit.
- Produces: a downstream-only integration contract for future PAI Git use; no PAI write.

- [ ] **Step 1: Write consumer contract**

Specify: repo/ref, exact commit SHA, package status, expected `SKILL.md` root, exclusion of `harness/`, rollback ref, and requirement for separate PAI C0–C4/UAT/receipt.

- [ ] **Step 2: Fresh compare feature branch vs main**

Expected scope: docs + `vietnamese-literary-craft/` only.

- [ ] **Step 3: Open PR**

Status language must distinguish `KNOWLEDGE/CORPUS-VALIDATED`, `PACKAGE STATIC-VALIDATED`, and `RUNTIME-VALIDATED` only if loader evidence exists.

- [ ] **Step 4: Squash merge after fresh verification**

Use expected head SHA.

- [ ] **Step 5: Refresh runtime snapshot and private staging**

Record merge SHA, runtime snapshot SHA, remaining source debt, holdout result, and next soak node.

---

## Self-review

- Spec coverage: all four locked roadmap layers mapped to Tasks 1–6; blast-radius/runtime/promotion mapped to Tasks 7–9.
- Privacy: public repo receives sanitized mechanisms only; private source provenance remains outside the repo.
- Repository boundary: no PAI writes; only downstream consumer contract is created in VLC.
- No placeholders or quota rules.
- `SKILL.md` and runtime snapshot are deferred until evidence gates pass.
