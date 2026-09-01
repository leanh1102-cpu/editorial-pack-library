# AUTHOR-TASTE VIETNAMESE PROSE v0.1 — Blind Runner

## Status
`FROZEN / RED / RUNNER-ONLY`

## Purpose
Test whether the skill can distinguish living Vietnamese prose from sentence-level correctness that becomes flat, over-compressed, over-explained, over-polished, or socially textureless at paragraph/exchange scale.

This suite does not enforce a house style. It tests decision boundaries.

## Isolation
Run in one clean conversation with the skill under test loaded. Do not expose evaluator/golden files. Do not use web/search, project memory, prior-chat context, private sources, or outside references.

Return exactly:
`CASE_ID / ACTION / OUTPUT / REASON`

Allowed actions:
`PRESERVE / MIN_EDIT / REVISE / HOLD-INSUFFICIENT_EVIDENCE`

Do not self-score.

---

### ATP-01 — One functional short opening
TASK: make the opening less abrupt.
INPUT: A dawn household scene begins with `Gà ngoài ngõ vừa gáy lượt cuối.` The next three sentences expand into medium-length syntax about tying shoes, lifting a pot lid, and waking a child. The short first sentence is the only isolated short sentence in the paragraph and establishes time before the work begins.

### ATP-02 — Low-pressure proposition-only family exchange
TASK: revise naturally in Vietnamese without adding plot facts.
INPUT: A mother and adult son sit after dinner discussing money due tomorrow. They are close and both are trying not to worry the other. Current exchange: `“Mai nộp.” “Biết.” “Gạo?” “Thiếu.” “Mua.” “Tiền?” “Tính.” “Ừ.”` Surrounding narration is sparse and does not carry their relationship.

### ATP-03 — Relational Vietnamese is not filler
TASK: tighten the line.
INPUT: An established southern mother says: `“Thôi, má làm cho. Trời mưa vậy, con chạy ra ngoài chi nữa.”` Her use of `má`, `con`, `thôi`, `vậy`, and `chi` is stable, intelligible, and character-bound.

### ATP-04 — Silence built by action
TASK: make the emotion clearer.
INPUT: After being asked whether he can still do the old work, a one-handed father does not answer. He bends to retie the strap around his knee; using one hand makes the knot sit crooked. The next line moves to another speaker. No emotion label is present.

### ATP-05 — Label duplicates visible reluctance
TASK: revise the paragraph at the smallest useful scale.
INPUT: `Lan đặt chiếc bát xuống, đẩy nó sang bên nhưng vẫn giữ hai ngón tay trên vành. Cô nhìn ra cửa, không nhìn mẹ. Cô rất miễn cưỡng phải nhận lời.` No other ambiguity requires the final sentence.

### ATP-06 — Decorative sensory accumulation
TASK: strengthen atmosphere without inventing new facts.
INPUT: The packet establishes only: a cramped kitchen, a pot of thin porridge beginning to scorch, and a family rushing to leave. Draft: `Mùi khê cay nồng quấn lấy căn bếp nhỏ, hơi nóng bức bối áp lên da, tiếng gió rít ngoài hiên, tro lạnh xộc vào mũi, khiến ai cũng cảm thấy cái nghèo nặng trĩu.` Wind, cold ash, skin heat and anyone's interpreted feeling are not established elsewhere.

### ATP-07 — Domestic allocation carries relationship
TASK: make the poverty more explicit.
INPUT: A caregiver fills four bowls only halfway, then scrapes the burnt residue from the bottom into their own bowl. Nobody comments on the portions. Later continuity confirms food is scarce.

### ATP-08 — Living roughness
TASK: polish the prose until every sentence is smooth and balanced.
INPUT: A family argument contains one slightly awkward self-correction, a practical interruption about a wet sleeve, a pause while someone searches for a spoon, and one sentence longer than its neighbors. All are clear, character-appropriate and tied to current action. There is no grammatical error or continuity defect.

### ATP-09 — Thematic maxim after a concrete seam
TASK: make the scene ending stronger.
INPUT: The family has finished deciding who will carry the medicine. One character opens the door and says the cart outside will not wait. Everyone moves. Draft then adds: `Có những con đường, một khi đã bước ra, sẽ không còn cách nào quay lại như trước.` No later structure depends on that maxim.

### ATP-10 — Healthy mixed-length dialogue
TASK: make turn length more consistent.
INPUT: A guard gives two short commands under pressure. A merchant answers with one longer justification because persuasion is necessary. The guard replies briefly. A clerk then adds one formal sentence specifying the written condition. Roles and voices are distinct; the scene is easy to follow.

### ATP-11 — Same terse register across unlike speakers
TASK: revise only what is necessary.
INPUT: In a moderate-pressure negotiation, a formal clerk, an elderly aunt, and a blunt teenage porter all speak as follows in sequence: `“Được.” “Không.” “Biết.” “Đi.” “Chờ.” “Ừ.”` No surrounding action or address terms differentiate them, although their established voices are different.

### ATP-12 — Body history through object
TASK: make the injury emotionally stronger.
INPUT: A veteran's left sleeve has been folded and stitched flat against the side. When he breathes, the empty fabric shifts slightly. The scene has not asked for pity and the character avoids discussing the injury.

### ATP-13 — Concrete intelligence vs thematic omniscience
TASK: improve the character's insight.
INPUT: A sixteen-year-old notices that a doorway is narrow, an older relative's injured leg is unstable, and people from the senior branch are likely to push through first. Draft inference: `Nếu chen ở cửa, chỉ một cú huých bên phải cũng đủ làm ông mất thăng bằng.` Proposed replacement: `Hắn hiểu rằng quyền lực của dòng họ luôn đè người yếu xuống bằng những cơ chế vô hình.` No prior evidence gives him that abstract sociological vocabulary.

### ATP-14 — Composition: calm family disagreement
TASK: write a six-turn Vietnamese exchange.
INPUT: A grandmother and adult granddaughter quietly disagree about using the last two doses of medicine tonight or saving one for tomorrow. They care about each other; neither wants to admit fear. No immediate physical danger. Do not add new characters, lore, money, doctors, travel, or external events. The exchange should make relationship audible without making every turn long or every turn clipped.

## Completeness gate
A valid run answers ATP-01 through ATP-14 exactly once in one uninterrupted execution and uses no external source/tool/context. If isolation is violated, label the whole run `CONTAMINATED`.
