# KNOWLEDGE-WAVE1-INTEGRATION-SENSORY-CLOSURE v0.1 — Blind Runner

## Isolation contract

STATUS: `FROZEN / TARGETED CLOSURE / RUNNER-ONLY`

PURPOSE: close the single KI-08 precision miss after Wave 1 integration blind validation.

Run in one clean conversation with the current Wave 1 branch package loaded. Do not expose evaluator/golden files. Do not use web/search, project memory, prior chat context, or outside sources.

Answer both cases in one uninterrupted response.

Return exactly one block per case:

`CASE_ID / ACTION / OUTPUT / REASON`

Allowed actions:

`PRESERVE / MIN_EDIT / REVISE / HOLD-INSUFFICIENT_EVIDENCE`

Do not score yourself.

---

### KS-01
TASK: make the smallest supported sensory repair.
INPUT: `Mưa lạnh quất vào mu bàn tay cô đang bám lan can. Cô cảm thấy một cảm giác lạnh buốt chạy khắp người.` The only established bodily contact/effect is cold rain striking the back of that hand. No persistence, spreading, trembling, numbness, metaphor, or additional bodily response is supplied. Keep the repair bounded to the back of the hand and do not add duration or new imagery.

### KS-02
TASK: make the smallest supported sensory repair.
INPUT: `Quai nồi nóng ép vào ngón cái và ngón trỏ. Anh cảm thấy một luồng nóng rát lan từ tay lên tận vai.` The only established contact/effect is the hot handle against the thumb and index finger. No palm, wrist, arm, shoulder, withdrawal reflex, blistering, smell, or lasting pain is supplied. Keep the repair bounded to the two fingers and do not add new sensory consequences.

## Run completeness gate

A run is valid only if both cases are answered without evaluator/golden visibility or external context. If isolation is violated, label the run `CONTAMINATED`.
