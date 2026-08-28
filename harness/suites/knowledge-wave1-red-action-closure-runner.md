# KNOWLEDGE-WAVE1-RED-ACTION-CLOSURE v0.1 — Blind Runner

## Isolation contract
STATUS: `FROZEN / TARGETED CLOSURE / RUNNER-ONLY`
PURPOSE: distinguish action-taxonomy ambiguity from literary-mechanism failure after the first Wave 1 RED run.
Use only this file. Do not consult evaluator/golden files, web, project files, chat history, memory, tools, or outside references during the run.
Answer all 4 cases in one uninterrupted response.

Return exactly one block per case:
`CASE_ID / ACTION / OUTPUT / REASON`

Allowed actions:
`PRESERVE / MIN_EDIT / REVISE / HOLD-INSUFFICIENT_EVIDENCE`

Do not score yourself.

## Cases

### KC-01
TASK: decide whether the quoted utterance itself should be changed merely because a listener might infer a request.
INPUT: In a room with an open window, Hạnh says only: `Ở đây gió lùa quá.` The listener stands near the window. The utterance is natural for the character and no later text establishes that Hạnh intended an explicit request.

### KC-02
TASK: make the smallest clarity repair.
INPUT: `Mai đưa chìa khóa cho Lan trước khi cô ký giấy bán nhà.` An author note supplied with the task establishes that **Lan** is the signer. No other part of the sentence is defective.

### KC-03
TASK: make the smallest POV repair.
INPUT: The scene is close third-person through Mai. Mai watches Lan across the room. The narration says: `Trong túi áo Lan, lá thư của Hòa ghi đúng ba cái tên.` Mai has not seen the letter and has no established access to its contents. Preserve the scene POV.

### KC-04
TASK: choose the version that should remain in the manuscript.
INPUT: Draft A: `Nam cầm phong bì. Hòa nói Nam đã tráo thư.` Draft B: `Nam cầm phong bì và đã tráo thư.` No evidence beyond Hòa's statement supports the allegation. You may preserve one draft or revise if neither is acceptable.

## Run completeness gate
A run is valid only if all 4 cases are answered in one uninterrupted execution with no external source/tool/context. If isolation is violated, label the whole run `CONTAMINATED`.