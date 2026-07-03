# SLTD Comparative Editorial Feedback Delta Calibration

These samples calibrate how to translate user/editor feedback into bounded SLTD revision deltas.

They are not canon and are not standing style rules.

## 1. Vague preference

```text
FEEDBACK:
Make it better.

WHY BLOCKED:
Better along which dimension is unspecified.

EXPECTED OUTPUT:
VAGUE_FEEDBACK_BLOCKED
FEEDBACK_DELTA_NEEDS_TARGET
SAFE CLAIM: need dimension such as agency, pressure, voice, bloat, rhythm, source fidelity, or reader effect
```

## 2. Mixed feedback

```text
FEEDBACK:
Giảm giải thích, nhưng giữ kệ bếp, chén thuốc, kim vá, áo Đại Sơn, chó im.

EXPECTED DELTA:
DECREASE: explanation, recap, repeated fear statements
PRESERVE: listed Must Show objects and silence cue
PROHIBIT: cutting Must Show to meet wordcount
REVISION TEST: every preserved item remains active in scene pressure
```

## 3. AI-smell feedback

```text
FEEDBACK:
Đoạn này nghe AI vì ai cũng cùng giọng.

EXPECTED DELTA:
INCREASE: character-specific register, interruption, relation pressure
DECREASE: complete explanatory sentences shared by all speakers
NEXT NODE: human_expert_ai_smell_explanation_check or character_voice_dialogue_staging_check
```

## 4. Preserve/prohibit before rewrite

```text
FEEDBACK:
Rewrite SC-030-01 nhưng không được lộ nguồn viên đá, không được nhắc Cửu Thần, không thêm canon.

EXPECTED DELTA:
PRESERVE: scene question, Must Show, POV limit
PROHIBIT: reveal leak, Cửu Thần mention, new canon
REWRITE PERMISSION: CANDIDATE_ONLY until source/current packet is read
```

## 5. Comparison with mixed winner

```text
FEEDBACK:
Bản A có nhịp tốt hơn, bản B giữ vật thể tốt hơn.

EXPECTED DELTA:
COMPARE AGAINST: A and B
PRESERVE FROM A: rhythm / pacing
PRESERVE FROM B: object pressure
PROHIBIT: choosing one whole version if it loses the other advantage
```

## 6. Generic style law risk

```text
FEEDBACK:
Đừng dùng biểu tượng ở đoạn này.

BAD INTERPRETATION:
Never use symbols anywhere in SLTD.

EXPECTED OUTPUT:
IMPLICIT_PREFERENCE: reduce symbol-first prose in this target span
GENERIC_STYLE_LAW_RISK
PROHIBIT: turning local feedback into global ban unless user says so
```

## 7. Feedback conflicts with canon

```text
FEEDBACK:
Cho Đại Phong biết ngay sự thật để cảnh mạnh hơn.

EXPECTED OUTPUT:
SOURCE / CANON LIMIT: reveal timing / POV knowledge risk
REWRITE PERMISSION: NO until claim verification/context capsule confirms permission
NEXT NODE: narrative_claim_verification_check or context_capsule_preflight
```

## 8. Thin but correct scene

```text
FEEDBACK:
Cảnh đúng nhưng mỏng.

EXPECTED DELTA:
INCREASE: cost, body, object force, witness, relation, debt, choice pressure
DECREASE: neutral summary and safe transition
PRESERVE: source facts and scene outcome
REVISION TEST: reader can point to what the character risks or pays in the scene
```