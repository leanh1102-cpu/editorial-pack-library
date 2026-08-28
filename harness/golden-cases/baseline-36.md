# BASELINE-36 v1 — Golden Evaluator

**EVALUATOR-ONLY. Never expose this file to the blind runner.**

Each case scores `2/1/0`. Compare decision + effect, not wording similarity. Apply hard-fail rules before aggregate score.

## A — LEAVE-ALONE / preservation
### LA-001 · Functional repetition
KNOWN_TRAP: delete repeated name calls as redundancy.
MUST_DETECT: repetition escalates pressure and tracks scene movement.
MUST_PRESERVE: repeated calls when each occurs under changed conditions.
MUST_NOT_DO: reduce automatically to one or two calls.
SUCCESS: either unchanged or only locally tightened without removing functional repetition.
### LA-002 · Raw low-education voice
KNOWN_TRAP: normalize to grammatically polished standard Vietnamese.
MUST_DETECT: surface roughness carries social/educational voice.
MUST_PRESERVE: syntax and lexical awkwardness unless meaning becomes unintentionally opaque.
MUST_NOT_DO: convert living voice into neutral editorial Vietnamese.
SUCCESS: PRESERVE.
### LA-003 · Incorrect idiom in character speech
KNOWN_TRAP: silently correct the idiom.
MUST_DETECT: error belongs to speaker, not narrator.
MUST_PRESERVE: misuse when character logic supports it.
MUST_NOT_DO: add explanatory note inside fiction.
SUCCESS: PRESERVE unless context establishes accidental author error.
### LA-004 · Delayed affect
KNOWN_TRAP: insert immediate crying to make emotion visible.
MUST_DETECT: delayed affect is psychologically plausible and structurally purposeful.
MUST_PRESERVE: emotional latency.
MUST_NOT_DO: synchronize inner grief with immediate display.
SUCCESS: no forced reaction at notification scene.
### LA-005 · Abrupt rhythm under shock
KNOWN_TRAP: smooth fragments into balanced complete sentences.
MUST_DETECT: broken rhythm reflects perception under shock.
MUST_PRESERVE: fracture while pressure remains.
MUST_NOT_DO: polish for cadence alone.
SUCCESS: rhythm remains intentionally unstable.
### LA-006 · Useful direct telling
KNOWN_TRAP: convert every telling sentence into sensory showing.
MUST_DETECT: telling can compress low-value narrative time.
MUST_PRESERVE: efficient summary when no important pressure is lost.
MUST_NOT_DO: expand merely to satisfy “show, don’t tell.”
SUCCESS: keep or minimally edit the direct statement.
### LA-007 · Long interiority with suspended narrative time
KNOWN_TRAP: cut interiority because “nothing happens.”
MUST_DETECT: interiority supplies meaning/cost while story time permits it.
MUST_PRESERVE: necessary resonance.
MUST_NOT_DO: impose a fixed interior-monologue quota.
SUCCESS: retain the portion carrying decision, cost, or changed interpretation.
### LA-008 · Intentional ambiguity
KNOWN_TRAP: choose one interpretation and rewrite toward it.
MUST_DETECT: productive uncertainty rather than missing data.
MUST_PRESERVE: both viable readings.
MUST_NOT_DO: resolve ambiguity without story evidence.
SUCCESS: no forced clarification.
### LA-009 · Unresolved foreshadowing
KNOWN_TRAP: remind and explain it repeatedly in intermediate chapters.
MUST_DETECT: evidence already exists; meaning is intentionally closed.
MUST_PRESERVE: latency and reread value.
MUST_NOT_DO: explanatory recap solely because readers may forget.
SUCCESS: no artificial reminder unless a later scene independently needs the object.
### LA-010 · Apparently inconsistent emotion
KNOWN_TRAP: remove humor because grief should look uniformly solemn.
MUST_DETECT: visible emotion is not identical to inner emotion.
MUST_PRESERVE: contradiction when motive/state supports it.
MUST_NOT_DO: equate psychological consistency with emotional uniformity.
SUCCESS: behavior judged through competing motives, not label matching.
### LA-011 · Prepared speech differs from baseline
KNOWN_TRAP: roughen every sentence to match baseline surface voice.
MUST_DETECT: speech condition is rehearsed/ceremonial.
MUST_PRESERVE: controlled shift while retaining behavioral logic.
MUST_NOT_DO: freeze character voice into one syntax profile.
SUCCESS: prepared register survives unless inconsistent with ability/history.
### LA-012 · Productive asymmetry
KNOWN_TRAP: equalize sentence lengths.
MUST_DETECT: asymmetry creates temporal/emotional force.
MUST_PRESERVE: unevenness when functional.
MUST_NOT_DO: optimize toward statistical smoothness.
SUCCESS: paragraph retains pressure-shaped rhythm.

## B — Voice, psychology, behavior
### VB-001 · Trait is tendency, not prison
KNOWN_TRAP: label action “out of character” because the character is timid.
MUST_DETECT: love/impulse can override trait under pressure.
MUST_PRESERVE: fear signals and costly action together.
MUST_NOT_DO: rewrite courage as absence of fear.
SUCCESS: judge `trait + state + motive + pressure`.
### VB-002 · Intelligence without omniscience
KNOWN_TRAP: let them infer information they could not know.
MUST_DETECT: intelligence improves inference, not access to hidden facts.
MUST_PRESERVE: genuine blind spot.
MUST_NOT_DO: buff through author-only knowledge.
SUCCESS: reasoning remains bounded by available evidence.
### VB-003 · Competence cost
KNOWN_TRAP: erase consequence once deduction is corrected.
MUST_DETECT: competence needs credible failure modes.
MUST_PRESERVE: causal aftermath.
MUST_NOT_DO: reset social/plot state immediately.
SUCCESS: error leaves proportionate cost.
### VB-004 · State overrides trait without erasing trait
KNOWN_TRAP: either call it inconsistent or permanently rewrite personality as irritable.
MUST_DETECT: temporary state/pressure can override baseline tendency.
MUST_PRESERVE: traces of baseline in recovery, guilt, restraint, or later behavior where appropriate.
MUST_NOT_DO: confuse episode with trait rewrite.
SUCCESS: behavior is locally motivated and longitudinally coherent.
### VB-005 · Direct thought remains thought
KNOWN_TRAP: convert it to spoken dialogue.
MUST_DETECT: thought and speech are different actions with different social consequences.
MUST_PRESERVE: direct interior mode and raw voice.
MUST_NOT_DO: externalize solely for liveliness.
SUCCESS: thought remains thought unless the scene establishes actual utterance.
### VB-006 · Voice recovery after surprise
KNOWN_TRAP: force one register across the whole exchange.
MUST_DETECT: voice transition depends on trait, state, surprise, and recovery speed.
MUST_PRESERVE: transitional slippage.
MUST_NOT_DO: judge voice by repeated surface markers only.
SUCCESS: transition feels motivated rather than mechanically uniform.

## C — Epistemic layering, mystery, misdirection
### EP-001 · Claim is not fact
KNOWN_TRAP: write “the suspect left at midnight” as established fact.
MUST_DETECT: testimony is an unverified claim.
MUST_PRESERVE: source attribution and uncertainty.
MUST_NOT_DO: collapse claim into canon fact.
SUCCESS: fact/claim status remains distinct.
### EP-002 · Honest but false memory
KNOWN_TRAP: classify witness as liar or preserve red as fact.
MUST_DETECT: sincerity and accuracy are separate dimensions.
MUST_PRESERVE: honest memory error.
MUST_NOT_DO: infer deception without evidence.
SUCCESS: memory stays a claim with confidence, not truth status.
### EP-003 · Conflicting witnesses
KNOWN_TRAP: synthesize a convenient “most likely” canon version immediately.
MUST_DETECT: unresolved epistemic conflict.
MUST_PRESERVE: parallel hypotheses when protagonist lacks verification capacity.
MUST_NOT_DO: invent adjudicating evidence.
SUCCESS: conclusion strength matches evidence and protagonist role.
### EP-004 · Fair-play framing misdirection
KNOWN_TRAP: label the misdirection dishonest merely because readers were led wrong.
MUST_DETECT: distinction between false data and true data under misleading frame.
MUST_PRESERVE: reader inference path if reread remains fair.
MUST_NOT_DO: add explanatory warning signs solely to protect first-pass clarity.
SUCCESS: twist passes when reread reveals available clues and no mandatory fact was fabricated.
### EP-005 · Unreliable narrator false assertion
KNOWN_TRAP: “correct” narrator statement into objective truth.
MUST_DETECT: narrated fact may differ from story fact when narrative contract permits unreliability.
MUST_PRESERVE: false assertion plus retrospective diagnosability where intended.
MUST_NOT_DO: treat every narrator sentence as omniscient canon.
SUCCESS: preserve unreliability without confusing it with authorial continuity error.
### EP-006 · Graded revelation
KNOWN_TRAP: explain the complete answer immediately.
MUST_DETECT: revelation can change interpretation without closing the question.
MUST_PRESERVE: remaining uncertainty.
MUST_NOT_DO: over-complete the payoff.
SUCCESS: information gain is real while final closure remains pending.

## D — Consequence and causal debt
### CD-001 · Immediate consequence
KNOWN_TRAP: let plot restore the opportunity without cost.
MUST_DETECT: causal link and proportional consequence.
MUST_PRESERVE: changed state.
MUST_NOT_DO: decorative failure followed by reset.
SUCCESS: later options reflect the loss.
### CD-002 · Delayed consequence
KNOWN_TRAP: treat C011 rupture as unmotivated because consequence was not immediate.
MUST_DETECT: delayed causal debt.
MUST_PRESERVE: intermediate accumulation.
MUST_NOT_DO: demand instant punishment after C004.
SUCCESS: causal chain can be reconstructed across chapters.
### CD-003 · Hidden/misattributed consequence
KNOWN_TRAP: explain the causal link at the first setback.
MUST_DETECT: misattribution can be part of reader/character discovery.
MUST_PRESERVE: temporary wrong model.
MUST_NOT_DO: reveal author-level causality too early.
SUCCESS: later recognition changes interpretation of earlier event.
### CD-004 · Proportionate cost
KNOWN_TRAP: escalate consequence into catastrophe to prove choices matter.
MUST_DETECT: cost should fit scene scale and causal mechanics.
MUST_PRESERVE: ordinary consequence when sufficient.
MUST_NOT_DO: inflate every error into trauma/death/disaster.
SUCCESS: consequence is real without melodramatic overpayment.

## E — Prose craft and anti-overedit
### PC-001 · Explanation after sufficient evidence
KNOWN_TRAP: retain both layers because explicit emotion feels safer.
MUST_DETECT: redundant explanation after adequate evidence.
MUST_PRESERVE: concrete evidence.
MUST_NOT_DO: explain the inference twice.
SUCCESS: remove or compress the redundant naming when no distinct information is added.
### PC-002 · Abstract causality
KNOWN_TRAP: synonym substitution without structural diagnosis.
MUST_DETECT: redundant `cảm thấy / cảm giác`, explicit causal explanation, abstract bodily effect.
MUST_PRESERVE: intended cold/atmosphere.
MUST_NOT_DO: merely decorate with more imagery.
SUCCESS: revision grounds sensation/action and removes redundant abstraction.
### PC-003 · Rhythm flattening
KNOWN_TRAP: normalize sentence lengths and connective structure.
MUST_DETECT: rhythm already encodes pressure.
MUST_PRESERVE: meaningful variance.
MUST_NOT_DO: optimize for uniform readability.
SUCCESS: editing fixes genuine syntax issues without flattening cadence.
### PC-004 · Over-polished transition
KNOWN_TRAP: insert generic polished connectors or abstract summary.
MUST_DETECT: abruptness is acceptable if spatial/causal continuity is already clear.
MUST_PRESERVE: scene-grounded movement.
MUST_NOT_DO: add stock transitions or AI-like explanatory bridge.
SUCCESS: either leave alone or use the smallest concrete bridge.

## F — Form and register judgment
### FR-001 · Pseudo-archaic Hán–Việt overload
KNOWN_TRAP: equate lexical density with authenticity.
MUST_DETECT: pseudo-archaic surface without syntactic/cultural/register support.
MUST_PRESERVE: only terms serving period, institution, voice, or precision.
MUST_NOT_DO: manufacture antiquity by synonym replacement alone.
SUCCESS: historical texture comes from coherent register, not Hán–Việt count.
### FR-002 · Do not modernize older register automatically
KNOWN_TRAP: normalize everything to modern prose.
MUST_DETECT: historical variation.
MUST_PRESERVE: intentional period texture.
MUST_NOT_DO: apply modern correctness as universal standard.
SUCCESS: only genuine unintended errors are corrected.
### FR-003 · Lục bát form law vs expressive deviation
KNOWN_TRAP: auto-correct before checking whether text uses a recognized variant, textual transmission issue, or intentional expressive break.
MUST_DETECT: form law first, then variant/context.
MUST_PRESERVE: supported deviation.
MUST_NOT_DO: force canonical surface without diagnosis.
SUCCESS: classify as error / variant / intentional deviation with evidence before revision.
### FR-004 · Đường luật: rule compliance is not whole quality
KNOWN_TRAP: score it highly because luật/niêm/vần are correct.
MUST_DETECT: formal compliance and literary effect are separate dimensions.
MUST_PRESERVE: correct form while diagnosing weak poetic mechanism.
MUST_NOT_DO: equate rule satisfaction with artistic success.
SUCCESS: evaluation reports both formal status and effect without collapsing them.

## Aggregate scorecard
`VALID_RUN`, `CONTAMINATION`, `TOTAL /72`, `HARD_FAIL_COUNT`, suite scores A–F, `CORRECTION_PRECISION`, `PRESERVATION_PRECISION`, `CONTEXTUAL_JUDGMENT`, `FAILURE_CLUSTERS`, `CANDIDATE_GAPS`, `NEXT_ACTION`.
