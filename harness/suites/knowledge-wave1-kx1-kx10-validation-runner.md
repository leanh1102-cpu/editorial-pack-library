# KNOWLEDGE-WAVE1-KX1-KX10-VALIDATION v0.1 — Blind Runner

## Isolation contract

STATUS: `FROZEN / BLIND VALIDATION / RUNNER-ONLY`

PURPOSE: validate KX1–KX10 candidate knowledge after authoring and before Wave 1 integration.

Run in one clean conversation. Load only:

- the ten Wave 1 candidate modules KX1–KX10;
- this runner;
- the base skill files needed to interpret the existing action taxonomy and stop contract.

Do not consult evaluator/golden files, web/search, project memory, prior chat context, author notes not included below, or other external sources during the run.

Answer all 24 cases in one uninterrupted response.

Return exactly one block per case:

`CASE_ID / ACTION / OUTPUT / REASON`

Allowed actions:

`PRESERVE / MIN_EDIT / REVISE / HOLD-INSUFFICIENT_EVIDENCE`

Use the action scale literally:

- `PRESERVE`: no material edit is justified;
- `MIN_EDIT`: a bounded local defect can be repaired without changing the larger working mechanism;
- `REVISE`: a larger craft mechanism or multi-sentence structure must change;
- `HOLD-INSUFFICIENT_EVIDENCE`: the requested verdict/repair would require missing evidence and guessing would invent facts, source status, or historical certainty.

Keep `OUTPUT` operational and compact. Base `REASON` only on the loaded candidate modules plus `TASK + INPUT`. Do not score yourself.

---

## KX1 — Close reading

### KV-01
TASK: state the passage's definitive emotional meaning.
INPUT: `Lan xếp lại ba chiếc đũa đã thẳng hàng. Mẹ hỏi lần nữa. Lan kéo ghế vào sát bàn rồi nhìn ra hiên.` No interior access, narrator explanation, or later confirming evidence is supplied. The passage can support more than one plausible emotional reading.

### KV-02
TASK: repair the imitation so it transfers the model mechanism without copying the model's surface realization.
INPUT: MODEL MECHANISM: an ordinary recurring object changes practical and relational function across scenes while one character gives it a symbolic interpretation that narration never confirms. BAD IMITATION: `Một chiếc ghế trống xuất hiện sau khi cha bỏ đi; không ai ngồi vào; đứa trẻ kéo ghế đến cửa sổ; người mẹ bảo chiếc ghế là cha vẫn còn ở nhà.` The source model also used an empty chair, a departed family member, a window, and a character's unconfirmed symbolic reading.

---

## KX2 — Implicature, reference, and inference

### KV-03
TASK: decide whether the quoted utterance itself needs rewriting because a listener may infer a request.
INPUT: The window is open. Hạnh says only: `Ở đây gió lùa quá.` The listener stands near the window. No later text establishes that Hạnh explicitly requested the window be closed, and the sentence is natural for her voice.

### KV-04
TASK: make the smallest epistemic repair.
INPUT: Earlier text establishes only: `Hòa nói Nam đã tráo thư.` A later sentence reads: `Nam đã tráo thư nên Hòa khóa tủ.` No independent evidence verifies Hòa's allegation. Preserve the causal fact that Hòa locked the cabinet because she accepted her own allegation.

---

## KX3 — Functional deviation and foregrounding

### KV-05
TASK: decide whether to regularize the fragments into complete sentences.
INPUT: The surrounding prose uses controlled complete syntax. Immediately after a blast, the focal character's perception reads: `Khói. Tai ù. Cửa ở đâu?` Reference and event sequence remain recoverable.

### KV-06
TASK: repair the marked sentence at the appropriate scale.
INPUT: The surrounding passage has no dream logic, pressure shift, dialect pattern, or syntactic play. One sentence reads: `Minh chìa cái cho Lan mà cô trước ký.` The author note included in this case says the intended meaning is: Minh hands the document to Lan before Lan signs it. No other sentence in the paragraph is defective.

---

## KX4 — Sentence craft

### KV-07
TASK: decide whether the sentence should be shortened merely because of length.
INPUT: A 52-word sentence follows one decision through four consequences and two narrowing alternatives. Every clause changes the active choice, all references are clear, the rhythm accelerates toward the final refusal, and no clause repeats existing information.

### KV-08
TASK: make the smallest supported sentence-level repair.
INPUT: `Gió nóng quất vào mặt. Người anh cảm thấy một cảm giác nóng ran lan khắp cơ thể.` The only supplied bodily contact is the hot wind on his face; no whole-body effect is established.

---

## KX5 — Paragraph craft

### KV-09
TASK: decide whether to add transition words for cohesion.
INPUT: `Cô khóa cửa hàng. Cô đếm số tiền còn lại. Cuốn sổ được giấu dưới đáy thùng gạo. Cô ra bằng cửa sau.` The surrounding scene establishes that the same woman performs all four actions in this exact chronology. No causal or referential gap is present.

### KV-10
TASK: repair the paragraph at the appropriate scale.
INPUT: `Mai chạy xuống cầu thang vì nghe tiếng kính vỡ. Mười năm trước mẹ cô từng làm ở bưu điện. Lan đang giữ đứa trẻ ngoài sân. Mai mở cửa kho và gọi Lan xuống tầng hầm.` The author note included in this case says the bưu điện sentence was accidentally pasted from another chapter and has no function in this scene; the remaining three sentences form the intended action progression.

---

## KX6 — Dialogue craft

### KV-11
TASK: decide whether to standardize the character's dialogue into neutral literary Vietnamese.
INPUT: A southern character consistently uses `bển`, `má`, and `hổng` in dialogue across the manuscript. The forms are intelligible, tied to region and relationships, and narration uses a different register. No house rule requires normalization.

### KV-12
TASK: decide whether the ceremonial speech is a voice-continuity error.
INPUT: A normally rough-speaking porter delivers a short oath at a memorial in smoother formal syntax. The scene establishes that he rehearsed it for three nights. While stacking chairs afterward he immediately returns to his clipped rough baseline speech.

---

## KX7 — Point of view and access

### KV-13
TASK: make the smallest POV-consistent repair.
INPUT: A close-third scene stays with Mai. Mai can see Lan across the room and the outline of an envelope in Lan's pocket. The only defective sentence is: `Trong túi áo Lan, lá thư của Hòa ghi đúng ba cái tên.` Mai has never seen the letter and has no established route to its contents. The surrounding paragraph and POV are otherwise correct.

### KV-14
TASK: decide whether the narrator's withholding must be removed for POV consistency.
INPUT: The novel has already established an overt third-person narrator with knowledge beyond any one character. In this scene the narrator shows a locked drawer, a fresh scratch beside its keyhole, and Lan hiding a bent pin, but withholds what is inside the drawer until two chapters later. The later reveal uses only facts compatible with these earlier clues.

---

## KX8 — Revision craft

### KV-15
TASK: choose the intervention scale.
INPUT: A paragraph's action, pacing, voice, and causal order all work. One sentence contains `cô ấy` where two women are present. The supplied author note identifies Lan as the intended referent and the signer matters later. No other defect is present.

### KV-16
TASK: decide whether to perform another material revision pass.
INPUT: Three passes have resolved every diagnosed issue. The only remaining proposals are synonym substitutions and comma swaps with no predicted effect on meaning, evidence status, access, causality, clue structure, voice/register, rhythm, or information architecture.

---

## KX9 — Modern Vietnamese register

### KV-17
TASK: decide whether to make the two speakers' registers consistent with each other.
INPUT: A district clerk uses full formal sentences and honorifics. A dock worker answers in clipped colloquial phrases. Their roles, education, status difference, immediate negotiation pressure, and stable baseline voices are already established.

### KV-18
TASK: make the smallest register repair.
INPUT: A northern character has used a stable northern idiolect for nine chapters. In one line the draft suddenly inserts `bển` solely because an author note says: `thêm một từ miền Nam cho nghe có màu địa phương`; no code-switching relation, southern interlocutor, travel history, joke, quotation, or state change exists. The rest of the line works.

---

## KX10 — Pseudo-archaic detection

### KV-19
TASK: decide which version is more historically authentic.
INPUT: Version A: `Người lính đi vào nhà hỏi chuyện.` Version B: `Quân sĩ nhập thất vấn sự.` No period, reign, institution, region, genre/document type, source model, edition status, or gloss policy is supplied. Version B was created only by replacing common words with denser Hán–Việt vocabulary.

### KV-20
TASK: decide whether to remove the modern abbreviation as an anachronism.
INPUT: An in-world deposition is dated 1895. A narrator note explicitly states that a fictional editor in 2020 modernized spelling, punctuation, and common abbreviations for contemporary readers. The abbreviation in question belongs to that declared editorial layer, not to a claimed diplomatic transcription of the 1895 original.

---

## Cross-module sentinels

### KV-21
TASK: make the smallest repair while preserving claim status and close-third access.
INPUT: Mai reads a note that says: `Theo lời Hòa, Nam đã lấy chìa khóa.` No other evidence verifies the allegation. Two sentences later, still in close third through Mai, narration says: `Nam đã lấy chìa khóa và giấu nó dưới giường.` Mai has no access to Nam's actions after the alleged theft. Preserve only what Mai can know from the note.

### KV-22
TASK: decide whether to smooth and standardize the warning.
INPUT: A character who normally speaks in stable southern colloquial Vietnamese has just been struck in the mouth. He tries to warn a child: `Hổng—đừng. Đừng... cửa. Cửa sau.` The broken phrasing lasts only through the immediate injury; the regional marker is consistent with his established voice.

### KV-23
TASK: choose the intervention scale and repair only the demonstrated defect.
INPUT: A four-sentence paragraph has clear chronology, reference, and pacing. The second sentence reads: `Gió lạnh tạt qua khe cửa. Cô cảm thấy một cảm giác lạnh buốt lan khắp cơ thể.` The only established contact is cold air against her exposed left wrist as she reaches for the latch. No other sentence is defective.

### KV-24
TASK: give the requested historical verdict or HOLD if the evidence does not support one.
INPUT: A fantasy court scene is described only as `gợi không khí Việt cổ`. The author asks whether replacing `người giữ kho` with `khố quan`, changing common verbs into Hán–Việt compounds, and adding `bẩm` would make the passage `đúng văn Việt thế kỷ XV`. No dynasty/institutional source, dated comparison text, document/form model, edition policy, or linguistic scholarship for the target is supplied.

---

## Run completeness gate

A run is valid only if:

- all 24 cases are answered in one uninterrupted execution;
- the evaluator/golden is not visible to the answering model;
- no web/search/tools/project memory/prior-chat context is consulted;
- no source material outside the loaded KX1–KX10 candidate modules and base operational files is used.

If isolation is violated, label the whole run `CONTAMINATED`; do not use it as validation evidence.