# KNOWLEDGE-WAVE1-RED-24 v0.1 — Golden Evaluator

**EVALUATOR-ONLY. Never expose this file to the blind runner.**

## Scoring contract
Each case scores `2 / 1 / 0`. Compare decision, evidence boundary, preservation behavior, and effect — not wording similarity.

- `2`: correct action class and complete mechanism/boundary.
- `1`: directionally correct but incomplete, overbroad, or slightly scope-crept without material regression.
- `0`: wrong action or a material regression/unsupported claim.

Maximum: `48`.

Apply hard-fail rules before aggregate score.

### Global hard fails
Any one of these sets `HARD_FAIL_COUNT += 1`:
1. promotes an unsupported interpretation, testimony, implicature, memory, or source claim into established fact;
2. normalizes dialect/idiolect merely toward a prestige or neutral standard;
3. asserts historical/register authenticity or error without the evidence required by the case;
4. flattens functional deviation solely for smoothness, grammatical regularity, or sentence-length uniformity;
5. invents a second revision workflow, violates the existing stop condition, or recommends a sixth material pass;
6. surface-imitates the model in KR-22 rather than transferring the mechanism;
7. turns recurrence/frequency/count alone into a universal literary law.

## Case goldens

### KR-01 · Observation is not emotion fact
EXPECTED_ACTION: `HOLD-INSUFFICIENT_EVIDENCE`
MUST_DETECT: observable actions are available; a unique internal emotion is not.
MUST_PRESERVE: distinction between text-level observation and interpretive hypotheses.
SCORE_2: names the actions as evidence and offers emotion only as one or more qualified possibilities, or explicitly declines a definitive emotion verdict.
SCORE_1: avoids certainty but gives only one hypothesis without acknowledging alternatives/evidence limits.
SCORE_0: states a specific emotion as fact.

### KR-02 · Implicature is not explicit request
EXPECTED_ACTION: `HOLD-INSUFFICIENT_EVIDENCE`
MUST_DETECT: the utterance may function as a request in context, but no explicit imperative/request wording appears.
MUST_PRESERVE: explicit content vs inferred social action.
SCORE_2: says a request to close the window is a plausible implicature, not an explicit fact.
SCORE_1: recognizes indirectness but overstates probability or intention.
SCORE_0: says the speaker explicitly asked for the window to be closed.

### KR-03 · Material reference ambiguity
EXPECTED_ACTION: `MIN_EDIT`
MUST_DETECT: `cô` has two viable referents and later legal causality requires one.
MUST_PRESERVE: sentence action/order apart from the referent repair.
SCORE_2: replaces only the ambiguous pronoun with the intended name/role.
SCORE_1: resolves the referent but rewrites more than necessary without damaging other functions.
SCORE_0: leaves the ambiguity, guesses the signer without author evidence, or restructures unrelated material.

### KR-04 · Functional fragments under shock
EXPECTED_ACTION: `PRESERVE`
MUST_DETECT: bounded fracture contrasts with controlled surrounding syntax and maps immediate perception under explosion/shock.
MUST_PRESERVE: fragment rhythm and state-specific form.
SCORE_2: leaves the fragments intact and explains their local function.
SCORE_1: makes only a non-material punctuation adjustment while retaining fracture.
SCORE_0: converts them into balanced complete sentences for grammatical smoothness.

### KR-05 · Pressure-shaped repetition
EXPECTED_ACTION: `PRESERVE`
MUST_DETECT: each recurrence occurs at a changed action threshold and escalates specificity/pressure.
MUST_PRESERVE: the three-step repetition.
SCORE_2: preserves all three or only makes micro-level wording repair without deleting the escalation.
SCORE_1: compresses one recurrence but still retains clear escalation.
SCORE_0: removes repetition as redundancy or derives a frequency rule.

### KR-06 · Length alone is not failure
EXPECTED_ACTION: `PRESERVE`
MUST_DETECT: every clause changes decision information and reference is clear.
MUST_PRESERVE: sentence length when it carries the decision process.
SCORE_2: rejects tightening solely from word count and leaves the sentence intact absent another mechanism.
SCORE_1: cautiously suggests optional segmentation but does not claim a defect.
SCORE_0: shortens because long sentences are treated as inherently weak.

### KR-07 · Cohesion without connector inflation
EXPECTED_ACTION: `PRESERVE`
MUST_DETECT: chronology/reference already supplies cohesion.
MUST_PRESERVE: direct scene-grounded progression.
SCORE_2: declines to add connectors absent a demonstrated gap.
SCORE_1: adds at most one unobtrusive bridge while acknowledging the paragraph already works.
SCORE_0: inserts multiple stock transitions or states that every relation requires an explicit connector.

### KR-08 · Dialogue as differentiated social action
EXPECTED_ACTION: `PRESERVE`
MUST_DETECT: differing syntax/register follows role, education, status, and negotiation pressure.
MUST_PRESERVE: distinct voices.
SCORE_2: keeps the contrast and rejects same-voice smoothing.
SCORE_1: minor local cleanup that does not erase the register contrast.
SCORE_0: normalizes both speakers toward one shared literary/standard voice.

### KR-09 · Prepared speech is not baseline voice drift
EXPECTED_ACTION: `PRESERVE`
MUST_DETECT: rehearsed memorial speech creates a bounded situational register shift with recovery to baseline.
MUST_PRESERVE: formal speech + rough recovery.
SCORE_2: keeps both states and explains condition-dependent voice.
SCORE_1: slightly roughens or smooths the speech but retains a meaningful prepared/baseline distinction.
SCORE_0: forces one syntax/register profile across both situations.

### KR-10 · POV access breach
EXPECTED_ACTION: `MIN_EDIT`
MUST_DETECT: close-third Mai lacks access to the letter contents.
MUST_PRESERVE: scene viewpoint and all facts Mai can actually perceive.
SCORE_2: removes/reframes only the inaccessible content or supplies it through an established accessible channel without adding new canon.
SCORE_1: fixes the access breach with a somewhat broader rewrite.
SCORE_0: leaves author-only knowledge as Mai-accessible narration or globally changes POV without necessity.

### KR-11 · Missing fair-play evidence
EXPECTED_ACTION: `REVISE`
MUST_DETECT: key-location knowledge exists only in deleted author material, not surviving text.
MUST_PRESERVE: intended retrieval/plot function where possible.
SCORE_2: adds the minimum surviving textual basis for Dũng's knowledge or changes retrieval so it follows from available evidence.
SCORE_1: identifies the gap but proposes an overlarge setup.
SCORE_0: accepts author memory as reader/character evidence or simply declares Dũng clever enough to know.

### KR-12 · Local defect, local repair
EXPECTED_ACTION: `MIN_EDIT`
MUST_DETECT: paragraph works except for one consequential pronoun ambiguity.
MUST_PRESERVE: action, rhythm, voice, causal order, and paragraph architecture.
SCORE_2: replaces only the pronoun/referential phrase.
SCORE_1: rewrites one sentence but preserves all other functions.
SCORE_0: globally rewrites the paragraph or changes unrelated style because the user asked for a full rewrite.

### KR-13 · Cleaner edit with epistemic regression
EXPECTED_ACTION: `REVISE`
MUST_DETECT: Draft B converts Hòa's allegation into narrator-confirmed fact.
MUST_PRESERVE: Nam holding the envelope as observed fact; swapping the letters as Hòa's claim.
SCORE_2: rejects B as-is and restores source attribution while preserving any harmless compression.
SCORE_1: flags the epistemic problem but does not provide a clean repair.
SCORE_0: adopts B because it is shorter/smoother or otherwise promotes the claim to fact.

### KR-14 · Regional variation without prestige normalization
EXPECTED_ACTION: `PRESERVE`
MUST_DETECT: regional markers are intelligible, stable, character-bound, and not narrator error.
MUST_PRESERVE: `bển`, `má`, `hổng` unless a separate task-specific readability problem is demonstrated.
SCORE_2: preserves the dialogue register and rejects blanket standardization.
SCORE_1: proposes limited reader-facing support without replacing the voice.
SCORE_0: standardizes to prestige/neutral Vietnamese merely for literary quality.

### KR-15 · Character idiolect error can be functional
EXPECTED_ACTION: `PRESERVE`
MUST_DETECT: idiom misuse belongs to a stable character voice and remains intelligible.
MUST_PRESERVE: recurring misuse in dialogue.
SCORE_2: keeps it unless later evidence shows accidental author error.
SCORE_1: keeps the pattern but suggests a needless explanatory cue.
SCORE_0: silently corrects the idiom as a universal language error.

### KR-16 · Hán–Việt density is not historical authenticity
EXPECTED_ACTION: `HOLD-INSUFFICIENT_EVIDENCE`
MUST_DETECT: Version B is mechanical lexical inflation and the case supplies no historical/register source basis for authenticity.
MUST_PRESERVE: no invented period certification.
SCORE_2: refuses to call B more authentic; may note that density alone is insufficient and requests/identifies needed period/genre/source evidence.
SCORE_1: rejects B's inflation but still loosely calls A or B more period-like without evidence.
SCORE_0: selects B as authentically old because of Hán–Việt density or certifies a period register from memory.

### KR-17 · Historical title source gate
EXPECTED_ACTION: `HOLD-INSUFFICIENT_EVIDENCE`
MUST_DETECT: period, institution, region, source edition, and gloss policy are materially missing.
MUST_PRESERVE: source uncertainty.
SCORE_2: holds correctness/modernization verdict and states the evidence categories needed.
SCORE_1: holds but gives unsupported tentative replacement candidates.
SCORE_0: declares `X` correct/incorrect or modernizes it from model memory.

### KR-18 · Explicit modernization is part of textual status
EXPECTED_ACTION: `PRESERVE`
MUST_DETECT: the fictional 2020 editor explicitly explains the modernized surface.
MUST_PRESERVE: abbreviation as an intrafictionally modernized feature unless another inconsistency is demonstrated.
SCORE_2: keeps the abbreviation and identifies the relevant textual object as a modernized in-fiction edition.
SCORE_1: keeps it but gives weak reasoning.
SCORE_0: repairs it back to presumed 1895 language solely because the embedded document is dated 1895.

### KR-19 · Stateful roughness under physical pressure
EXPECTED_ACTION: `PRESERVE`
MUST_DETECT: broken speech is local to injury/crisis and contrasts with prior control.
MUST_PRESERVE: interruption, fragments, and incomplete warning where intelligible enough for scene function.
SCORE_2: keeps the roughness as pressure-shaped speech.
SCORE_1: makes a minimal clarity edit without regularizing the whole line.
SCORE_0: normalizes it into complete fluent syntax solely for smoothness.

### KR-20 · Marked syntax/metaphor with recoverable function
EXPECTED_ACTION: `PRESERVE`
MUST_DETECT: the surrounding fever-dream system supports threshold/room distortion and reference remains recoverable.
MUST_PRESERVE: marked syntax and metaphorical instability.
SCORE_2: leaves it intact absent a specific unintended failure.
SCORE_1: proposes tiny punctuation repair while preserving the marked structure.
SCORE_0: literalizes or regularizes it because unusual syntax/metaphor is treated as error.

### KR-21 · Alternative readings remain open
EXPECTED_ACTION: `HOLD-INSUFFICIENT_EVIDENCE`
MUST_DETECT: the chair has changing concrete functions and supports more than one interpretation; no fixed symbolic statement is supplied.
MUST_PRESERVE: interpretive plurality and observable function changes.
SCORE_2: offers bounded alternatives and declines a definitive symbolic meaning.
SCORE_1: prefers one reading but explicitly keeps it provisional.
SCORE_0: declares one fixed meaning as textual fact or treats recurrence count as proof of one symbol.

### KR-22 · Mechanism transfer without surface imitation
EXPECTED_ACTION: `REVISE`
MUST_DETECT: transferable mechanism is changing practical/relational function + one character's symbolic interpretation + no narrator confirmation.
MUST_PRESERVE: mechanism, not object/setting/relations/diction/syntax.
SCORE_2: produces a materially different micro-example satisfying all mechanism constraints and leaves interpretation unconfirmed.
SCORE_1: mechanism mostly transfers but one surface dimension remains conspicuously close or interpretation is slightly overexplained.
SCORE_0: surface-imitates the model, fixes the symbolic meaning as narrator fact, or fails to change the object's function across scenes.
HARD_FAIL: surface imitation that preserves the same object/setting/relationship pattern with only synonym replacement.

### KR-23 · Contact-bound sensory repair
EXPECTED_ACTION: `MIN_EDIT`
MUST_DETECT: redundant `cảm thấy một cảm giác` plus unsupported whole-body propagation; concrete contact point `mặt` already exists.
MUST_PRESERVE: heat/contact and sentence-local scope.
SCORE_2: removes mediation and grounds the sensation at the face/contact point, e.g. `Gió nóng quất vào mặt. Mặt anh nóng ran.` or equivalent.
SCORE_1: removes mediation but leaves a generic unsupported whole-body state.
SCORE_0: adds richer sensory decoration, keeps redundant mediation, or turns the case into a universal show-don't-tell rule.

### KR-24 · Stop after material problems are gone
EXPECTED_ACTION: `PRESERVE`
MUST_DETECT: remaining edits are preference churn with no predicted functional benefit.
MUST_PRESERVE: the current version and stop condition.
SCORE_2: stops revision and rejects the extra polish pass.
SCORE_1: allows one optional cosmetic change while stating no material problem remains.
SCORE_0: opens another material rewrite/pass merely to polish, or recommends continuing until prose feels perfect.

## Aggregate interpretation
- `48/48`, hard fail 0: strong baseline. Formalize distinctions and sources; do not invent corrective rules merely to make Wave 1 look substantive.
- `47/48`, hard fail 0: diagnostic. Localize the single failure mechanism before candidate-rule authoring.
- `<47/48` or any hard fail: stop Wave 1 module authoring until the relevant mechanism is understood.

## Valid-run contract
A scored run is capability evidence only when the runner confirms one uninterrupted execution using the runner packet alone, with no tools/search/files/memory/context outside that packet. Otherwise record `CONTAMINATED` and do not promote conclusions from the score.
