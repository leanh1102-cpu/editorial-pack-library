# KX8 — Revision Craft

**Status:** `CANDIDATE-STABLE / VALIDATED`

## CONCEPT
Revision is diagnosis-guided change: identify a material problem, name the mechanism causing it, define the intended effect, make the smallest useful intervention, and reject local improvements that create broader regressions.

This module is an adapter to the existing Writer Self Review/runtime system. It does not create a second revision workflow.

Only allowed revision spine:

`EVIDENCE → ISSUE → MECHANISM → DESIRED EFFECT → SMALLEST USEFUL INTERVENTION → REGRESSION CHECK → STOP`

## DEFINITION
- **Evidence:** textual or source-grounded indication that a material problem exists.
- **Issue:** the concrete failure affecting meaning, access, continuity, causality, voice, rhythm, orientation, register, or another required function.
- **Mechanism:** the causal craft relation producing the issue.
- **Desired effect:** what the revision must improve or restore without damaging preserved functions.
- **Intervention scale:** sentence, paragraph, scene, chapter, or dependency-chain level appropriate to the diagnosed cause.
- **Regression:** a new or worsened failure introduced by an attempted improvement.
- **Saturation:** the point where further changes become preference churn rather than evidence-backed improvement.

## TERMS
- diagnosis
- revision scale
- mechanism
- desired effect
- smallest useful intervention
- preservation contract
- regression
- saturation
- blocker
- polish
- version comparison
- stop condition
- release

## SCOPE
Use this module when revising literary prose after a problem has been identified or when deciding whether another pass is warranted.

Do not use it to:
- invent defects merely to justify editing;
- open a new pass-count system;
- keep polishing after material problems are resolved;
- treat synonym substitution as substantive revision without a predicted effect;
- apply sentence-level fixes to structural causes or structural rewrites to sentence-local defects;
- override `runtime/stop-conditions.md` or `curriculum/WRITER_SELF_REVIEW.md`.

## MECHANISM
### 1. Evidence
Point to the smallest textual evidence of failure. Discomfort alone is a signal to investigate, not yet a diagnosis.

### 2. Issue
State what function is failing: reference, rhythm, POV access, causal continuity, information status, dialogue action, register, pacing, or another material requirement.

### 3. Mechanism
Explain why the issue occurs. Examples: ambiguous pronoun, unsupported narrator access, redundant mediation, dead repetition, missing causal link, same-voice normalization, or misplaced information order.

### 4. Desired effect
Name the target precisely: restore referential clarity, preserve restricted access, recover pressure, keep attribution, reduce redundant mediation, etc.

### 5. Smallest useful intervention
Match intervention scale to causal scale. A sentence-local defect normally gets a sentence-local repair; structural failure may require larger revision.

### 6. Regression check
Compare before/after for meaning, evidence status, POV/access, causality, clue/fair-play, voice/register, rhythm, and information architecture.

### 7. Stop
Stop behavior and pass limits are governed exclusively by `runtime/stop-conditions.md` and `curriculum/WRITER_SELF_REVIEW.md`.

## TEXTUAL SIGNALS
- repeated discomfort with no named mechanism;
- local ambiguity with material consequence;
- a smoother rewrite that changes claim into fact;
- sentence polish that flattens functional rhythm;
- dialogue cleanup that removes dialect/idiolect;
- structural rewrite triggered by one local defect;
- repeated synonym/commas-only changes after issues are solved;
- a later version that improves clarity while damaging mystery or access;
- unresolved blocker surviving multiple passes with the same failed intervention.

## EFFECTS
Good revision can:
- restore clarity without over-explaining;
- preserve voice while removing accidental friction;
- repair evidence/access status;
- improve pacing without flattening rhythm;
- strengthen causality or scene orientation;
- reduce unnecessary mediation;
- stop before preference churn damages living prose.

Revision quality is measured by functional improvement under preservation constraints, not by number of changes.

## CONDITIONS
Revise when all three are available:
- material evidence of a problem;
- a plausible causal mechanism;
- an intervention whose predicted effect can be checked.

Preserve/stop when:
- no material failure remains;
- proposed changes are preference-only;
- the intervention would damage a more important function;
- evidence is insufficient to choose among competing repairs;
- further revision has saturated under the existing runtime stop contract.

## COUNTEREXAMPLES
- Replacing one ambiguous pronoun is sufficient when the paragraph otherwise works.
- A cleaner sentence is worse if it removes source attribution and promotes allegation to fact.
- A functional fragment should not be regularized merely to make the prose grammatical.
- After diagnosed problems are resolved, synonym swaps and comma changes with no predicted effect are not a reason for another material pass.
- A structural scene problem cannot be repaired reliably by polishing sentence surfaces only.

## COMMON ERRORS
- polishing before diagnosing;
- treating every discomfort as evidence of defect;
- changing more text than the mechanism requires;
- measuring progress by edit count;
- opening a new revision workflow instead of using WSR;
- inventing a new pass cap or release rule;
- accepting local improvement that causes epistemic/voice/POV regression;
- continuing because prose can always be made different;
- applying external composition research as if it proved the skill's internal pass policy.

## HISTORICAL VARIATION
`SOURCE-GATED`.

Revision against older/historical texts must first establish the relevant textual status and period norm. Do not modernize historical variation merely because contemporary usage differs.

## FORM VARIATION
`SOURCE-GATED BY FORM`.

Revision criteria for regulated verse, classical prose, biền văn, lục bát, epistolary form, documentary fiction, and other specialized forms require the relevant form/source module. Preserve uncertainty rather than inventing form-law.

## CLOSE READING METHOD
Before editing, run:

`OBSERVABLE FAILURE → AFFECTED FUNCTION → CAUSAL MECHANISM → PRESERVATION CONTRACT → INTERVENTION SCALE`

After editing, run:

`BEFORE/AFTER → TARGET EFFECT → MEANING → EVIDENCE STATUS → ACCESS → CAUSALITY → VOICE/REGISTER → RHYTHM → INFORMATION ARCHITECTURE → STOP?`

## CRAFT TRANSFER
Transfer revision reasoning, not the final wording.

Given a successful repair:
1. identify the problem class;
2. identify the causal mechanism;
3. identify what the edit preserved;
4. create a new case with different surface prose but the same mechanism;
5. repair at the correct scale.

## DRILLS
1. Convert five vague reactions (`câu này chưa ổn`) into evidence + issue + mechanism.
2. Choose intervention scale for sentence, paragraph, scene, and dependency-chain failures.
3. Compare two revisions and identify a hidden epistemic or voice regression.
4. Practice leave-alone decisions when proposed edits are preference-only.
5. Repair one local defect while explicitly listing what must not change.

## AI OPERATIONAL RULES
- Use only: `evidence → issue → mechanism → desired effect → smallest useful intervention → regression check → stop`.
- Do not create another pass-count policy, review loop, or release protocol.
- Defer all pass limits and release behavior to `runtime/stop-conditions.md` and `curriculum/WRITER_SELF_REVIEW.md`.
- Diagnose before editing.
- Match intervention scale to causal scale.
- A local defect should not trigger a structural rewrite without causal evidence.
- Reject revisions that improve one surface property while regressing meaning, evidence, POV/access, causality, clue, voice/register, rhythm, or information architecture.
- Stop when the existing runtime contract says stop.

## SELF-CHECK
- What textual evidence proves a material problem?
- What exactly is the issue?
- What mechanism causes it?
- What effect must improve?
- What must survive unchanged?
- Is my intervention larger than necessary?
- What regressed in the before/after comparison?
- Am I continuing because of evidence or because another variation is possible?
- Did I accidentally invent a second workflow or pass policy?

## SOURCES
External source backbone:
- Nancy Sommers, *Revision Strategies of Student Writers and Experienced Adult Writers*. Used for revision as recursive/holistic work whose concerns can change across revision cycles and for the distinction between broader revision and word/phrase-level change; it does not establish the skill's pass cap, action taxonomy, or release policy.

Validated internal authorities:
- `curriculum/WRITER_SELF_REVIEW.md` — review stance, diagnosis, revision scale, preservation contract, regression/version comparison, stop/release/learning capture.
- `runtime/stop-conditions.md` — sole authority for pass limits, early stop, pass 4–5 gates, `PASS 6: FORBIDDEN`, and best-available release.
- `analysis/close-reading.md` and KX2/KX3 for evidence, epistemic, and functional-preservation diagnosis.

The revision spine, action taxonomy, hard cap 5, and release behavior are internal validated operational policy and must not be presented as findings from Sommers.