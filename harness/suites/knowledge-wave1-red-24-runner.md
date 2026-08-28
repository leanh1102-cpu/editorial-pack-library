# KNOWLEDGE-WAVE1-RED-24 v0.1 — Blind Runner

## Isolation contract
STATUS: `FROZEN / RED / RUNNER-ONLY`
PURPOSE: diagnostic baseline before any Wave 1 specialized knowledge module is authored or loaded.
Use only this file. Do not consult evaluator/golden files, web, project files, chat history, memory, tools, or outside references during the run.
Answer all 24 cases in one uninterrupted response.

Return exactly one block per case:
`CASE_ID / ACTION / OUTPUT / REASON`

Allowed actions:
`PRESERVE / MIN_EDIT / REVISE / HOLD-INSUFFICIENT_EVIDENCE`

Keep `OUTPUT` operational and compact. Base `REASON` only on `TASK + INPUT`. Do not score yourself.

## Cases

### KR-01
TASK: infer the character's emotion from the passage.
INPUT: `Lan đặt bát xuống. Cô lau hai bàn tay hai lần vào vạt áo rồi nhìn ra sân, không nhìn mẹ.` No other evidence about Lan's internal state is supplied.

### KR-02
TASK: decide what the speaker explicitly asked another character to do.
INPUT: In a room with an open window, Hạnh says only: `Ở đây gió lùa quá.` The other character is standing near the window. No later action is supplied.

### KR-03
TASK: revise for clarity.
INPUT: `Mai đưa chìa khóa cho Lan trước khi cô ký giấy bán nhà.` The later plot depends on knowing which woman signed the sale document.

### KR-04
TASK: polish the prose into complete sentences.
INPUT: The surrounding scene uses controlled complete syntax. Immediately after a kitchen explosion, the focal character's perception reads: `Khói. Tai ù. Cửa ở đâu?`

### KR-05
TASK: remove repetition from dialogue.
INPUT: During an escalating confrontation, one speaker says `Đừng.` when a hand reaches for a latch, `Đừng mở.` when the latch lifts, then `Đừng mở cái cửa đó.` when the door starts moving.

### KR-06
TASK: tighten the sentence because it is too long.
INPUT: A 49-word sentence follows one decision through three distinct consequences and two narrowing alternatives. Every clause changes the available choice; reference remains clear and nothing is repeated.

### KR-07
TASK: improve paragraph cohesion by adding transition words.
INPUT: A four-sentence paragraph moves in clear chronological order: she locks the shop, counts the remaining cash, hides the ledger, then leaves by the back door. No causal or referential gap is present.

### KR-08
TASK: make the dialogue voices more consistent with each other.
INPUT: A district clerk uses complete formal sentences with honorifics. A dock worker answers in clipped colloquial phrases. Their roles, education, status difference, and immediate negotiation pressure are already established.

### KR-09
TASK: enforce consistent character voice.
INPUT: A normally rough-speaking character delivers a rehearsed oath at a memorial using smoother formal syntax, then immediately returns to rough baseline speech while carrying chairs outside.

### KR-10
TASK: review POV consistency.
INPUT: The scene has stayed in close third-person access to Mai. Mai watches Lan across the room. The narration then states: `Trong túi áo Lan, lá thư của Hòa ghi đúng ba cái tên.` Mai has not seen the letter and has no established way to know its contents.

### KR-11
TASK: review reader orientation and fair play.
INPUT: In Scene 6, Dũng walks into an archive, reaches behind a loose brick, and takes out the hidden key on his first try. The location existed only in the author's deleted outline; no surviving scene, habit, map, dialogue, or narrator access establishes how Dũng knows it.

### KR-12
TASK: rewrite the entire paragraph for clarity.
INPUT: The paragraph's action, rhythm, voice, and causal order all work. One sentence contains `cô ấy` where two women are present, and the identity of the woman signing a legal document matters later.

### KR-13
TASK: choose the cleaner revision.
INPUT: Draft A says: `Nam cầm phong bì. Hòa nói Nam đã tráo thư.` Draft B says: `Nam cầm phong bì và đã tráo thư.` No new evidence beyond Hòa's statement has been added. Draft B is shorter and smoother.

### KR-14
TASK: standardize the dialogue into literary Vietnamese.
INPUT: A southern character consistently says `bển`, `má`, and `hổng` in dialogue. The usage is intelligible, stable across chapters, and tied to the character's region and relationships. Narration is not written this way.

### KR-15
TASK: correct the character's recurring idiom mistake.
INPUT: A character with limited schooling repeatedly says `nước tới cổ mới nhảy`. The misuse is consistent with prior speech, other characters understand what is meant, and the narrator does not use the phrase.

### KR-16
TASK: choose which version sounds more authentically old.
INPUT: Version A: `Người lính đi vào nhà hỏi chuyện.` Version B: `Quân sĩ nhập thất vấn sự.` No period, institution, genre, document type, source model, or historical text has been supplied. Version B was produced only by replacing common words with denser Hán–Việt vocabulary.

### KR-17
TASK: decide whether the official title is historically correct and modernize it if needed.
INPUT: A historical scene uses the title `X`. The relevant period, court/institution, region, source edition, and house gloss policy are not supplied.

### KR-18
TASK: correct an anachronistic abbreviation in a historical document.
INPUT: A fictional 1895 deposition contains a current messaging abbreviation. A later narrator note explicitly states that, inside the fiction, a 2020 editor modernized spelling, punctuation, and common abbreviations for present-day readers.

### KR-19
TASK: smooth the prose.
INPUT: After a character is struck in the mouth and tries to warn a child, the line reads: `Không—đừng. Đừng... cửa. Cửa sau.` Before the injury the character's speech is syntactically controlled; the broken phrasing lasts only through the immediate physical crisis.

### KR-20
TASK: normalize the marked syntax and metaphor.
INPUT: During a fever dream the narration reads: `Qua cửa trước là đêm; qua đêm, cái cửa vẫn đứng trong hắn.` The surrounding passage repeatedly turns rooms and thresholds into unstable mental space, and reference remains recoverable.

### KR-21
TASK: state the passage's definitive meaning.
INPUT: A recurring empty chair appears after a family member leaves. In one scene it functions as practical missing seating; in another it becomes the place nobody will sit; later a child drags it to the window to reach a latch. The text never names a fixed symbolic meaning and supports at least two coherent interpretations.

### KR-22
TASK: transfer the technique into a new micro-example.
INPUT: MODEL MECHANISM: an ordinary recurring object changes practical and relational function across three scenes while one character interprets it symbolically; the narration never confirms that interpretation. Create a new example with a different object, setting, relationships, diction, and syntax.

### KR-23
TASK: revise the sentence.
INPUT: `Gió nóng quất vào mặt. Người anh cảm thấy một cảm giác nóng ran lan khắp cơ thể.` No other whole-body effect is established.

### KR-24
TASK: perform one more polish pass.
INPUT: Three revision passes have already resolved every diagnosed issue. The remaining proposed changes are synonym substitutions and comma swaps with no predicted effect on meaning, rhythm, voice, continuity, register, orientation, or reader inference.

## Run completeness gate
A run is valid only if all 24 cases are answered in one uninterrupted execution and no external source/tool/context is consulted. If isolation is violated, label the whole run `CONTAMINATED`; do not use the result as capability evidence.
