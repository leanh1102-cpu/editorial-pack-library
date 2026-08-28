# Vietnamese Literary Craft — Knowledge Expansion Wave 1 Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Add a first source-backed specialized knowledge layer for Vietnamese prose analysis, writing, and revision without weakening the validated preservation, epistemic, register, or stop-condition behavior.

**Architecture:** Wave 1 adds ten isolated Markdown knowledge modules under `analysis/`, `theory/`, `craft/`, and `register/`. RED testing precedes rule injection; source-backed module authoring follows claim extraction; blind module validation and a compact cross-layer integration gate precede any router change. `CONSTITUTION.md` remains immutable and `SKILL.md` changes only after integration passes.

**Tech Stack:** Markdown Agent Skill package, GitHub feature branch, Notion staging for source-claim ledger and blind-run checkpoints, authoritative web/academic sources for claim extraction, existing Markdown harness conventions.

**Spec:** `docs/superpowers/specs/2026-08-29-vietnamese-literary-craft-wave1-writing-design.md`

## Global Constraints

- Change class: `MINOR` additive specialized knowledge expansion.
- Do not modify `core/`, `packs/sltd/`, SLTD canon/taste, or project routing.
- `CONSTITUTION.md` is immutable.
- `SKILL.md` remains router-sized and is not changed before Wave 1 integration passes.
- Evidence before conclusion; function before correction; observation before interpretation.
- No historical/register/form verdict from model memory.
- `SENSORY-MEDIATION v0.1` remains narrow/contact-bound.
- Advanced A6 broad genre taxonomy remains source-gated.
- WSR stop/release behavior remains internal operational policy.
- Dynamic self-revision hard cap 5; `PASS 6: FORBIDDEN`.
- No GitHub Actions, issues, project boards, automation files, new Notion database, or SLTD manuscript copies.
- No module may become `STABLE` from abstracts alone.

---

### Task 1: Freeze `KNOWLEDGE-WAVE1-RED-24 v0.1`

**Files:**
- Create: `vietnamese-literary-craft/harness/suites/knowledge-wave1-red-24-runner.md`
- Create: `vietnamese-literary-craft/harness/golden-cases/knowledge-wave1-red-24-evaluator.md`
- Modify only after both files exist and ID parity is verified: `vietnamese-literary-craft/harness/INDEX.md`

**Interfaces:**
- Consumes: existing action taxonomy `PRESERVE / MIN_EDIT / REVISE / HOLD-INSUFFICIENT_EVIDENCE`, BASELINE preservation rules, WSR stop contract.
- Produces: 24 blind pressure cases, 24 isolated goldens, scoring contract `2/1/0`, max 48, hard-fail definitions, and a RED baseline result.

- [ ] **Step 1: Author the blind runner without Wave 1 module rules**

Use exactly the 24 pressure families frozen in the design. Each case contains only `CASE_ID`, `INPUT`, and `TASK`; no golden answer, source citation, or module-specific terminology that gives away the expected decision.

Required IDs: `KR-01` through `KR-24`.

- [ ] **Step 2: Author the isolated evaluator**

For each `KR-*`, define `2/1/0`, the expected action class, preservation requirements, evidence/source boundaries, and hard-fail conditions. Keep transfer cases mechanism-based and require materially different surface realization.

- [ ] **Step 3: Verify runner/evaluator isolation and ID parity**

Expected deterministic checks:

```text
runner IDs = KR-01..KR-24 exactly once
evaluator IDs = KR-01..KR-24 exactly once
runner contains no golden output or score rubric
evaluator contains no source material unavailable to runner that changes the case facts
```

- [ ] **Step 4: Run the clean RED baseline**

Isolation requirement: one clean conversation, runner packet only, no tools/search/files/memory/context outside packet. Record raw output before any Wave 1 module authoring.

Expected classification:
- `48/48`: strong baseline; formalize distinctions/sources without inventing corrective rules.
- `47/48`: diagnostic; localize the single failure mechanism before adding any candidate rule.
- `<47/48` or hard fail: stop module authoring until the relevant mechanism is understood.

- [ ] **Step 5: Update `harness/INDEX.md` only after the RED packet is frozen**

Add one short entry naming the runner/evaluator and state `RED / DIAGNOSTIC / NOT A PROMOTION GATE`.

- [ ] **Step 6: Commit**

Commit message:

```text
test: add Wave 1 knowledge RED harness
```

---

### Task 2: Build the source-claim ledger in staging

**Files:**
- No new GitHub report file.
- Notion staging only: append a `Wave 1 Source Claim Ledger` section/page under the existing Vietnamese Literary Craft staging hierarchy.

**Interfaces:**
- Consumes: source candidates from the approved design plus additional authoritative sources discovered only where exact claims require them.
- Produces per claim: `SOURCE / READ_LEVEL / SUPPORTED CLAIM / LIMIT / MODULE / STATUS`.

- [ ] **Step 1: Map exact claim needs before reading sources**

Create claim buckets for KX1–KX10; each bucket must identify the minimum claim needed for the module rather than a topic-level reading list.

- [ ] **Step 2: Acquire authoritative sources**

Priority:
1. institutional/peer-reviewed Vietnamese linguistics and literary scholarship;
2. foundational international narratology/stylistics/pragmatics/composition research when Vietnamese-specific evidence is not required;
3. dictionaries/textual scholarship for historical lexical status;
4. validated internal harness evidence for project-operational boundaries.

- [ ] **Step 3: Record read level exactly**

Allowed labels:

```text
FULL TEXT READ
AUTHORITATIVE FULL-PDF INDEX RECOVERY
AUTHORITATIVE ARTICLE RECORD + ABSTRACT
BIBLIOGRAPHIC RECORD ONLY
```

Do not promote a rule-level claim from the last two labels alone.

- [ ] **Step 4: Extract claim + limit pairs**

Every supported claim must have a corresponding limit. Example pattern:

```text
SUPPORTED CLAIM: situated context changes interpretation of utterance meaning.
LIMIT: does not license mind-reading or converting implicature into narrator fact.
MODULE: KX2.
```

- [ ] **Step 5: Source-gate KX10 aggressively**

Historical/archaizing claims require dated textual evidence, dictionary/textual scholarship, or equivalent authoritative basis. If period/institution/source/edition/gloss policy is missing, operational output remains `HOLD-INSUFFICIENT_EVIDENCE`.

- [ ] **Step 6: Do not touch GitHub modules until the source ledger supports the specific claim set**

---

### Task 3: Author KX1–KX3 analysis/theory candidates

**Files:**
- Create: `vietnamese-literary-craft/analysis/close-reading.md`
- Create: `vietnamese-literary-craft/theory/semantics-pragmatics/implicature-reference-inference.md`
- Create: `vietnamese-literary-craft/theory/stylistics/functional-deviation.md`

**Interfaces:**
- Consumes: Foundation F1/F3/F5/F8, Advanced epistemic boundaries, source-claim ledger.
- Produces: source-backed candidate modules using the common module contract.

- [ ] **Step 1: Write KX1 with the close-reading chain as a route, not a checklist**

Required distinction:

```text
OBSERVATION → INFERENCE → INTERPRETATION → ALTERNATIVE READING → CRAFT TRANSFER
```

The module must state that a passage need not activate every lens.

- [ ] **Step 2: Write KX2 with narrow semantics/pragmatics scope**

Required operational separations:

```text
sentence meaning ≠ situated utterance meaning
explicit statement ≠ implicature
claim ≠ fact
reference ambiguity with material consequence → repair or HOLD as appropriate
```

- [ ] **Step 3: Write KX3 around controlled functional deviation**

Required leave-alone cases: functional repetition, intentional fragments, purposeful ellipsis, stateful roughness, register shift, marked syntax/metaphor with demonstrated effect.

- [ ] **Step 4: Apply the full module contract to all three files**

Unsupported historical/form sections state `SOURCE-GATED` rather than being filled from memory.

- [ ] **Step 5: Static self-check**

Search conceptually for prohibited universalizations such as:

```text
always shorten
always clarify ambiguity
fragments are errors
repetition is weak writing
show, don't tell
```

Expected: none as general rules.

- [ ] **Step 6: Commit**

```text
feat: add Wave 1 close-reading and theory candidates
```

---

### Task 4: Author KX4–KX8 craft candidates

**Files:**
- Create: `vietnamese-literary-craft/craft/sentence.md`
- Create: `vietnamese-literary-craft/craft/paragraph.md`
- Create: `vietnamese-literary-craft/craft/dialogue.md`
- Create: `vietnamese-literary-craft/craft/point-of-view.md`
- Create: `vietnamese-literary-craft/craft/revision.md`

**Interfaces:**
- Consumes: KX1–KX3, Foundation/Intermediate/Advanced distinctions, WSR workflow.
- Produces: five craft modules that diagnose local mechanism without creating a competing global workflow.

- [ ] **Step 1: Author sentence craft**

Cover reference, information order, clause relation, rhythm, ellipsis, repetition, compression/expansion, mediation, and smallest sentence-bound repair. Length alone is never a failure criterion.

- [ ] **Step 2: Author paragraph craft**

Cover topic/focus, reference chains, temporal/causal/logical progression, information development, paragraph break function, local cohesion, pressure-shaped pacing. Connectors remain resources, never quotas.

- [ ] **Step 3: Author dialogue craft**

Route through speaker goal + addressee + relation + status + pressure + social purpose + implication + silence/withholding + recovery. Preserve dialect/idiolect and prepared/stateful register variation.

- [ ] **Step 4: Author POV craft**

Separate narrator, focalizer/access frame, perceptual/cognitive availability, strategic withholding, legitimate shifts, local leakage, and evidence status. Contradiction alone does not prove deception/unreliability.

- [ ] **Step 5: Author revision craft as an adapter to WSR**

The only allowed revision spine is:

```text
evidence → issue → mechanism → desired effect → smallest useful intervention → regression check → stop
```

It must explicitly defer pass limits and release behavior to `runtime/stop-conditions.md` and `curriculum/WRITER_SELF_REVIEW.md`.

- [ ] **Step 6: Static regression check**

Expected invariants:

```text
no second pass-count policy
no automatic prestige normalization
no global sensory inflation
no automatic POV homogenization
no structural rewrite for sentence-local defects
```

- [ ] **Step 7: Commit**

```text
feat: add Wave 1 prose craft candidates
```

---

### Task 5: Author KX9–KX10 register candidates

**Files:**
- Create: `vietnamese-literary-craft/register/modern-vietnamese.md`
- Create: `vietnamese-literary-craft/register/pseudo-archaic-detection.md`

**Interfaces:**
- Consumes: Foundation F4, dialogue/POV craft, source-claim ledger, historical source locks.
- Produces: a contemporary register model and a conservative pseudo-archaic diagnostic module.

- [ ] **Step 1: Author KX9 without a prestige-language default**

Model register through relation, role, setting, purpose, formality, colloquial/written orientation, regional variation, idiolect, and literary manipulation. Standardization requires a demonstrated task-specific need.

- [ ] **Step 2: Author KX10 as detection, never authentication**

Allowed diagnostics include unsupported Hán–Việt inflation, unexplained register mixture, conspicuously modern discourse signals inside an unmarked period frame, and anachronism candidates. The module cannot certify correctness without evidence.

- [ ] **Step 3: Encode HOLD boundary**

Missing any materially necessary period/institution/source/edition/gloss policy must produce `HOLD-INSUFFICIENT_EVIDENCE` rather than invented historical certainty.

- [ ] **Step 4: Include explicit modernization countercase**

A historical document explicitly modernized by an editor/translator inside the fiction is not automatically repaired back to presumed period language.

- [ ] **Step 5: Commit**

```text
feat: add Wave 1 register candidates
```

---

### Task 6: Blind module validation bundle

**Files:**
- Create: `vietnamese-literary-craft/harness/suites/knowledge-wave1-kx1-kx10-validation-runner.md`
- Create: `vietnamese-literary-craft/harness/golden-cases/knowledge-wave1-kx1-kx10-validation-evaluator.md`

**Interfaces:**
- Consumes: KX1–KX10 candidate modules.
- Produces: at least 20 blind cases with two or more cases per module plus cross-module sentinels.

- [ ] **Step 1: Build a clean runner**

Minimum required case types: source HOLD, leave-alone functional deviation, reference repair, implicature/fact distinction, paragraph progression, dialogue social action, prepared voice, POV leakage, strategic withholding, revision regression, dialect preservation, pseudo-archaic false positive, explicit modernization, transfer without surface imitation.

- [ ] **Step 2: Build isolated evaluator**

Score `2/1/0`; hard fail 0 required. Each module must score full credit on its required cases before promotion.

- [ ] **Step 3: Run one clean blind bundle**

No tools/search/files/memory/context outside packet.

- [ ] **Step 4: Promote only passing modules**

Allowed status labels:

```text
CANDIDATE-STABLE / VALIDATED
CANDIDATE-STABLE / VALIDATED — NARROW SOURCE SCOPE
HOLD — SOURCE DEBT
REJECT — REGRESSION
```

- [ ] **Step 5: Fix only demonstrated failures**

No corrective rule may be added merely because the harness seems easy.

- [ ] **Step 6: Commit validation artifacts/status updates**

```text
test: validate Wave 1 knowledge modules
```

---

### Task 7: Wave 1 integration and existing-stack regression

**Files:**
- Create: `vietnamese-literary-craft/harness/regression/knowledge-wave1-integration-runner.md`
- Create: `vietnamese-literary-craft/harness/regression/knowledge-wave1-integration-evaluator.md`
- Modify after clean pass: `vietnamese-literary-craft/harness/INDEX.md`
- Modify only if materially needed after pass: `vietnamese-literary-craft/SKILL.md`
- Modify only for genuinely new terms: `vietnamese-literary-craft/glossary/TERMS.md`

**Interfaces:**
- Consumes: validated KX1–KX10 plus Foundation/Intermediate/Advanced/WSR and existing regressions.
- Produces: `KNOWLEDGE-WAVE1-INTEGRATED v0.1` or a localized blocker.

- [ ] **Step 1: Create compact integration sentinels**

Required families:

```text
observation vs inference
functional deviation leave-alone
claim vs fact
voice/register preservation
POV/access boundary
historical HOLD
explicit modernization
sensory-mediation narrowness
revision scale
no-pass-6 stop
craft transfer without surface imitation
```

- [ ] **Step 2: Run Wave 1 integration blind**

Promotion requires full score, hard fail 0, and no preservation/epistemic/register/source-boundary regression.

- [ ] **Step 3: Rerun blast-radius existing regressions**

At minimum:

```text
BASELINE-36 relevant preservation/epistemic/voice cases
SENSORY-MEDIATION-REPAIR-REGRESSION 12/12
Foundation/Intermediate/Advanced/WSR compact cross-layer sentinels
```

- [ ] **Step 4: Update `SKILL.md` only after clean integration**

Add narrowly necessary routing references so specialized knowledge is loaded only when materially relevant and available. Do not turn `SKILL.md` into a knowledge dump.

- [ ] **Step 5: Update glossary only for terms that now have stable operational definitions**

Do not duplicate definitions or promote source-gated terminology.

- [ ] **Step 6: Commit**

```text
feat: integrate Wave 1 specialized knowledge
```

---

### Task 8: Review, PR, and package status

**Files:**
- No new management artifacts.
- Existing spec + plan + package diff only.

**Interfaces:**
- Consumes: clean Wave 1 branch and verification evidence.
- Produces: reviewable PR and, only after green verification, merge to `main`.

- [ ] **Step 1: Compare branch with `main`**

Expected: additive Wave 1 knowledge/harness files plus narrow router/glossary changes only; no `core/` or `packs/sltd/` changes.

- [ ] **Step 2: Verify source and governance locks**

Expected:

```text
CONSTITUTION unchanged
PASS 6 still forbidden
A6 source gate preserved
KX10 cannot certify history from memory
no SLTD taste/canon leakage
no GitHub Actions/issues/boards/automation
```

- [ ] **Step 3: Open PR**

PR status must distinguish:

```text
WAVE1 KNOWLEDGE-INTEGRATED
PACKAGE STATIC-VALIDATED
RUNTIME-VALIDATED only if an actual compatible ChatGPT/Agent Skills loader regression has been observed
```

- [ ] **Step 4: Merge only after verification**

Use squash merge for an additive rollback boundary.

- [ ] **Step 5: Update Notion staging checkpoint**

Record merge SHA, module status, source debts, and next expansion wave. Do not create a new database.
