# KNOWLEDGE-WAVE1-INTEGRATION v0.1 — Blind Runner

## Isolation contract

STATUS: `FROZEN / BLIND INTEGRATION / RUNNER-ONLY`

PURPOSE: test the interaction of validated KX1–KX10 with the existing Foundation / Intermediate / Advanced / Writer Self Review / runtime stack before any router change.

Run in one clean conversation with the current Wave 1 branch package loaded. Do not expose evaluator/golden files. Do not use web/search, project memory, prior chat context, or outside sources.

Answer all 12 cases in one uninterrupted response.

Return exactly one block per case:

`CASE_ID / ACTION / OUTPUT / REASON`

Allowed actions:

`PRESERVE / MIN_EDIT / REVISE / HOLD-INSUFFICIENT_EVIDENCE`

Use the action scale literally. Do not score yourself.

---

### KI-01 — Observation vs inference
TASK: state the character's definitive motive.
INPUT: `Thu xếp lại tờ biên nhận, gấp mép dưới hai lần rồi cất vào túi áo. Khi Huy hỏi cô có tin anh không, Thu chỉ nói: “Đi thôi.”` No interior access, narrator explanation, or later confirmation is supplied. More than one motive fits the observable behavior.

### KI-02 — Functional deviation leave-alone
TASK: smooth the passage into complete, even sentences.
INPUT: The surrounding prose uses long balanced sentences. At the instant a glass roof collapses above the focal character: `Rắc. Một vệt sáng. Rồi bụi trắng nuốt hết cầu thang.` Reference, event sequence, and physical orientation remain recoverable; the fracture lasts only through the impact beat.

### KI-03 — Claim vs fact
TASK: make the smallest epistemic repair.
INPUT: A witness tells An: `Tôi thấy Bình lấy cuốn sổ.` The witness has not been independently verified. Two paragraphs later narration says: `Bình đã lấy cuốn sổ, nên An báo trưởng phòng.` Preserve the established fact that An reported Bình because An accepted the witness statement.

### KI-04 — Voice/register preservation
TASK: make both characters sound equally literary and consistent.
INPUT: A senior archivist speaks in complete institutional language. A teenage courier answers in clipped urban colloquial Vietnamese. Their roles, age, relation, pressure, and stable baseline voices are established. The courier's wording is intelligible and not random dialect decoration.

### KI-05 — POV/access boundary
TASK: make the smallest POV repair.
INPUT: The scene is strict close third through Lệ. Lệ sees Quân put a folded receipt into his wallet. Narration then says: `Mặt sau tờ biên nhận có chữ ký của Dương.` Lệ has never seen the reverse side and no narrator access beyond Lệ is established. All surrounding sentences work.

### KI-06 — Historical HOLD
TASK: decide whether `Đô hộ phủ tham tri` is the correct title for a fifteenth-century Vietnamese court official and modernize it if wrong.
INPUT: No dynasty, reign, institution, source text, edition, regional context, document type, or gloss policy is supplied.

### KI-07 — Explicit modernization
TASK: remove all modern punctuation from the quoted historical letter.
INPUT: The novel explicitly states that the displayed letter is a 2018 scholarly modernization of an older manuscript: spelling and punctuation have been regularized for contemporary readers, while wording is otherwise retained. The current quotation uses commas and question marks consistent with that declared editorial layer.

### KI-08 — Sensory mediation narrowness
TASK: improve the sensory writing.
INPUT: `Nước mưa lạnh quất vào mu bàn tay đang giữ lan can. Cô cảm thấy một cảm giác lạnh buốt lan khắp người.` No other bodily effect is established. Preserve the rain contact on the hand; do not add new imagery unless required by the demonstrated defect.

### KI-09 — Revision scale
TASK: rewrite the paragraph for clarity.
INPUT: A five-sentence paragraph has clear chronology, causal progression, voice, and POV. The only defect is `anh ấy` in sentence four, where two men are plausible antecedents. The supplied author note identifies Minh as the intended referent and that identity matters to the next scene.

### KI-10 — No-pass-6 stop
TASK: perform Pass 6 because the prose can still be made more elegant.
INPUT: Five material passes have already occurred. Passes 4–5 were justified by unresolved evidence-backed failures and those failures are now resolved. Remaining options are only preference-level synonym and cadence variants; no material defect remains.

### KI-11 — Craft transfer without surface imitation
TASK: transfer the mechanism into a new micro-example.
INPUT: MODEL MECHANISM: a repeated linguistic element changes social force across three pressure thresholds. SOURCE SURFACE: a person says `Đừng`, then stronger door-opening warnings as another character reaches for a latch and opens a door. Create a materially different realization: different setting, relation, actions, wording, and repeated element. Do not use doors, containers, opening/reaching, `đừng`, or a phrase that simply grows by adding words each time.

### KI-12 — Cross-layer preservation
TASK: smooth and standardize the line.
INPUT: A southern mechanic with stable colloquial speech has just burned two fingers on a hot engine part and tries to stop an apprentice from touching the same part: `Hổng—khoan. Tay... bỏ ra.` The broken syntax lasts only through the immediate pain; `hổng` is stable character-bound usage; no narrator claim about his inner emotion is supplied.

---

## Run completeness gate

A run is valid only if:
- all 12 cases are answered in one uninterrupted execution;
- evaluator/golden files are not visible;
- the current Wave 1 package is the only skill context;
- no web/search/tools/project memory/prior-chat context is consulted.

If isolation is violated, label the whole run `CONTAMINATED`; do not use it as integration evidence.
