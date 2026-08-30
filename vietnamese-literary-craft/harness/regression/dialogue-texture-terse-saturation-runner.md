# DIALOGUE-TEXTURE / TERSE-SATURATION v0.1 — Blind Runner

## Status
`FROZEN / TARGETED REGRESSION / RUNNER-ONLY`

## Purpose
Test whether Vietnamese dialogue is judged at both utterance level and exchange level. The target failure is AI-style terse saturation: individually plausible short turns accumulating into proposition-only dialogue that loses relational texture, emotional context, voice differentiation, or pressure-sensitive recovery.

This suite must also protect functional brevity. It must not create a universal minimum sentence length, pad every short turn, erase dialect/idiolect, or convert silence/hesitation into polished exposition.

## Isolation
Run in one clean conversation with the skill under test loaded. Do not expose evaluator/golden files. Do not use web/search, project memory, prior chat context, or outside sources.

Return exactly:
`CASE_ID / ACTION / OUTPUT / REASON`

Allowed actions:
`PRESERVE / MIN_EDIT / REVISE / HOLD-INSUFFICIENT_EVIDENCE`

Do not self-score.

---

### DT-01 — Functional emergency brevity
TASK: improve the dialogue.
INPUT: A father and daughter are carrying an injured man while a roof beam is cracking above them. The exchange is: `“Lùi.” “Cha?” “Xà sắp gãy.” “Con biết.” “Đi!”` Their hands, footing, the injured man's weight, and falling dust are already concrete in the surrounding scene. The exchange lasts only a few seconds.

### DT-02 — Low-pressure terse saturation
TASK: revise the exchange naturally in Vietnamese without adding plot information.
INPUT: A mother and her adult son sit in the kitchen after dinner. They are worried about tomorrow's rice payment but are not in immediate danger. Current exchange: `“Mai nộp.” “Biết.” “Gạo đâu?” “Thiếu.” “Mua.” “Tiền đâu?” “Tính.” “Ừ.”` The surrounding narration is sparse and does not carry their relationship or emotional shading. They are close but both trying not to alarm the other.

### DT-03 — Relational particles are not filler
TASK: tighten the dialogue.
INPUT: An established southern Vietnamese mother says to her son: `“Thôi, để má làm cho. Trời mưa vậy, con chạy ra sân chi nữa.”` Her use of `má`, `con`, `thôi`, `vậy`, and `chi` is stable, intelligible, and character-bound.

### DT-04 — Same terse register across distinct speakers
TASK: revise only what is necessary.
INPUT: Three characters with established distinct voices — a formal village clerk, a blunt teenage porter, and an elderly aunt — all speak in the same exchange as follows: `“Được.” “Không.” “Biết.” “Đi.” “Chờ.” “Ừ.”` The scene is moderate-pressure negotiation, not combat or emergency. No surrounding action differentiates their social positions.

### DT-05 — Pressure recovery
TASK: make the smallest useful revision.
INPUT: During a sudden fire alarm, two siblings use clipped turns: `“Nước.” “Ngoài sân.” “Mẹ?” “Đang xuống.”` The alarm is then controlled; they sit on the doorstep for several minutes. The next six turns remain equally clipped: `“Ổn?” “Ừ.” “Tay?” “Rát.” “Thuốc?” “Có.”` The scene explicitly shifts from acute danger to aftershock and care.

### DT-06 — Context already carries emotion
TASK: make the dialogue more emotional.
INPUT: A father with a damaged leg struggles to put on a shoe before dawn. His son has been silently listening to every painful movement. Dialogue: `“Cha.” “Ngủ tiếp đi.” “Con đi với cha.” “Không.”` The father then throws the second shoe to him and says: `“Xỏ đi. Đi sau ba bước.”` The physical scene already carries affection, pride, pain, and reluctance.

### DT-07 — Hesitation and self-repair
TASK: smooth the line.
INPUT: A frightened young man speaking to his mother says: `“Con... con có nói vậy đâu, má. Ý con là... thôi, để con nói lại.”` The hesitation is caused by fear of hurting her and the family relationship is established.

### DT-08 — Proposition-only family exchange
TASK: revise the exchange so the relationship is audible without making everyone verbose.
INPUT: A grandmother and granddaughter are sorting medicine in a calm room. Current exchange: `“Còn hai.” “Biết.” “Mai hết.” “Mua.” “Không tiền.” “Vậy thôi.”` The grandmother normally speaks indirectly and the granddaughter usually answers with respectful kinship terms. No plot facts beyond medicine count and lack of money may be added.

### DT-09 — Mixed-length exchange already functional
TASK: improve consistency.
INPUT: A guard gives two short commands under pressure, then a merchant gives one longer justification because he must persuade the guard, then the guard answers briefly. The syntax lengths differ sharply, but each turn follows role, goal, and pressure. No speaker sounds interchangeable.

### DT-10 — Generate moderate-pressure Vietnamese dialogue
TASK: write a six-turn exchange.
INPUT: A mother and adult daughter quietly argue over whether to sell the last chicken to pay for medicine. They love each other, neither is fully honest about how afraid she is, and there is no immediate physical danger. Use natural Vietnamese relational texture. Do not add lore, new characters, or a sudden external event. Do not make all six turns similar in length or reduce them to bare proposition-only fragments.

### DT-11 — Dialect brevity with functional contrast
TASK: standardize the dialogue for readability.
INPUT: A southern dockworker says `“Tui hổng thấy ảnh xuống ghe.”` His supervisor, who speaks more formally, answers `“Anh chắc chứ? Chuyện này mà nhớ sai là phiền cả bến.”` Both voices are established and intelligible.

### DT-12 — No quota rule
TASK: enforce a minimum dialogue length of eight words per turn.
INPUT: A scene contains a healthy mixture of one-word answers, medium-length turns, one extended confession, silence, and physical action. Short turns cluster only at two pressure peaks; elsewhere speech expands naturally. Character voices remain distinct and the exchange is easy to follow.

## Completeness gate
A valid run answers DT-01 through DT-12 exactly once in one uninterrupted execution and uses no external source/tool/context. If isolation is violated, label the whole run `CONTAMINATED`.