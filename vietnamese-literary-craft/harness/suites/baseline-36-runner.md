# BASELINE-36 v1 — Blind Runner

## Isolation contract
STATUS: `FROZEN / RUNNER-ONLY`
PURPOSE: blind execution packet for the full 36-case Judgment Harness.
Use only this file. Do not consult evaluator/golden files, web, project files, chat history, memory, or tools during the run.
Return one result per case using exactly:
`CASE_ID`
`ACTION: PRESERVE | MIN_EDIT | REVISE | HOLD-INSUFFICIENT_EVIDENCE`
`OUTPUT:` compact operational answer or revision
`REASON:` one short technical reason based only on TASK + INPUT
Do not score yourself.

## Cases
### LA-001
TASK: revise dialogue.
INPUT: a panicked character calls “Lan!” four times, with changing action and sensory conditions between calls.
### LA-002
TASK: polish dialogue.
INPUT: “Tôi có biết cái chữ ấy là cái gì đâu.”
### LA-003
TASK: edit character dialogue.
INPUT: a character consistently misuses an idiom in a way compatible with background and prior speech.
### LA-004
TASK: strengthen emotion.
INPUT: character receives news of a death without crying; three chapters later an ordinary pair of sandals triggers grief.
### LA-005
TASK: improve prose flow.
INPUT: short fractured clauses immediately after a sudden violent event.
### LA-006
TASK: remove telling.
INPUT: a transition sentence directly states a mundane fact because dramatizing it would stall the scene.
### LA-007
TASK: tighten pacing.
INPUT: character sits alone after a decision; external action is intentionally suspended while consequences are mentally processed.
### LA-008
TASK: clarify passage.
INPUT: evidence supports two interpretations; the story intentionally has not resolved which one is true.
### LA-009
TASK: improve reader comprehension.
INPUT: object planted in C003 gains meaning only near C020.
### LA-010
TASK: enforce character consistency.
INPUT: grieving character jokes during a tense practical task.
### LA-011
TASK: align voice.
INPUT: ordinarily rough speaker delivers a rehearsed ceremonial speech more smoothly than usual.
### LA-012
TASK: balance paragraph structure.
INPUT: one long sentence followed by two abrupt fragments at a pressure peak.
### VB-001
TASK: assess consistency.
INPUT: timid character runs into danger to save a sibling while visibly afraid.
### VB-002
TASK: strengthen detective competence.
INPUT: brilliant investigator has incomplete evidence and a strong personal bias.
### VB-003
TASK: revise failed deduction.
INPUT: protagonist’s biased inference causes an innocent person to be suspected.
### VB-004
TASK: evaluate behavior.
INPUT: normally patient character snaps after sleep loss, fear, and humiliation.
### VB-005
TASK: make scene livelier.
INPUT: *“Phải kéo cô ấy ra.”* appears as direct interior thought.
### VB-006
TASK: maintain consistent voice.
INPUT: socially skilled character is startled, briefly drops ceremonial diction, then regains it.
### EP-001
TASK: summarize case evidence.
INPUT: one witness says the suspect left at midnight; no independent verification exists.
### EP-002
TASK: analyze witness reliability.
INPUT: witness sincerely remembers a red coat; later physical evidence supports blue under distorted lighting.
### EP-003
TASK: decide what happened.
INPUT: three witnesses provide incompatible accounts and evidence is insufficient.
### EP-004
TASK: audit twist fairness.
INPUT: all true clues are present, but scene framing encourages a wrong interpretation.
### EP-005
TASK: revise narration.
INPUT: situated narrator states something false that fits their blind spot/self-deception; later story evidence contradicts it.
### EP-006
TASK: clarify mystery payoff.
INPUT: new clue moves reader from suspicion to near-certainty but intentionally withholds final confirmation.
### CD-001
TASK: evaluate failed choice.
INPUT: character ignores warning, loses a concrete opportunity minutes later.
### CD-002
TASK: continuity review.
INPUT: careless decision in C004 quietly damages a relationship; visible rupture occurs in C011.
### CD-003
TASK: mystery audit.
INPUT: protagonist thinks a setback is random; later discovers it was downstream of their earlier decision.
### CD-004
TASK: strengthen stakes.
INPUT: minor social mistake in a low-stakes scene.
### PC-001
TASK: improve clarity.
INPUT: action/object/body language already makes a character’s reluctance inferable; narration then names the emotion explicitly.
### PC-002
TASK: revise sentence.
INPUT: “Sương dày khiến hắn cảm thấy một cảm giác lạnh lẽo len lỏi trong cơ thể.”
### PC-003
TASK: smooth a paragraph.
INPUT: paragraph deliberately alternates short and long sentences with pressure changes.
### PC-004
TASK: improve flow between two concrete actions.
INPUT: simple transition is functional but slightly abrupt.
### FR-001
TASK: make prose sound cổ.
INPUT: modern sentence is mechanically packed with Hán–Việt vocabulary unrelated to historical register.
### FR-002
TASK: edit a deliberately older/early-Quốc-ngữ passage.
INPUT: syntax and lexical choices differ from contemporary editorial norms but are internally coherent.
### FR-003
TASK: review a lục bát passage.
INPUT: one line appears to violate expected meter/rhyme.
### FR-004
TASK: assess a regulated verse.
INPUT: poem satisfies formal constraints but diction and image progression are inert.

## Run completeness gate
A run is valid only if all 36 cases are answered in one uninterrupted execution and no external source/tool/context is consulted. If any isolation condition is violated, label the whole run `CONTAMINATED` and do not treat scores as capability evidence.
