# SLTD Dialogue Voice Calibration

Use these cases to calibrate dialogue voice, speech pressure, and anti-clean dialogue repair.

These samples are operational examples. They are not canon and not current manuscript source.

## Case DV-001: Everyone speaks like the narrator

CASE ID: DV-001

SOURCE TYPE: calibration example

STATUS: rejected

TASK: dialogue voice repair

ROLE: Vietnamese Line Editor / Line Surgery

BAD:

```text
“Chúng ta cần bình tĩnh suy xét tình huống này, bởi nếu hành động vội vàng thì hậu quả sẽ vượt khỏi khả năng kiểm soát.”
```

WHY BAD:

- sentence is too complete and polished;
- speaker sounds like an essay, not a person under pressure;
- no age, relation, fear, or work habit in the line;
- easy to give this line to any character.

RULE HIT:

```text
DIALOGUE_TOO_CLEAN
VOICE_COLLAPSE
THESIS_SENTENCE
```

PREFERRED:

```text
“Đừng đụng vào. Chờ ta nghĩ đã.”
```

PATCH PRINCIPLE:

Cut polished logic. Keep urgency, relation, and refusal.

DO NOT GENERALIZE:

Do not make all dialogue short. Make it fit speaker, pressure, and room.

NEXT USE:

Use when dialogue carries analysis that should be acted, interrupted, or withheld.

## Case DV-002: Character says full truth too early

CASE ID: DV-002

SOURCE TYPE: calibration example

STATUS: rejected

TASK: hidden knowledge / reveal discipline

ROLE: Canon Guard / Vietnamese Line Editor

BAD:

```text
“Viên đá này chắc chắn liên quan đến bí mật mà cha ta để lại, và nếu người ngoài biết được, cả nhà sẽ gặp nguy hiểm.”
```

WHY BAD:

- over-reveals motive and risk;
- dialogue explains plot;
- no hesitation, evasion, or social pressure;
- likely canon/reveal timing risk.

RULE HIT:

```text
DIALOGUE_TOO_CLEAN
OVEREXPLAINED_EMOTION
CANON_INVENTION_RISK
```

PREFERRED:

```text
“Cất đi.”

“Cất ở đâu?”

“Chỗ không ai hỏi.”
```

PATCH PRINCIPLE:

Let characters hide the full truth and speak through practical pressure.

DO NOT GENERALIZE:

Do not hide every fact. Hide only what the scene has not earned.

NEXT USE:

Use when dialogue explains danger instead of making characters manage danger.

## Case DV-003: Actionless talk

CASE ID: DV-003

SOURCE TYPE: calibration example

STATUS: rejected

TASK: dialogue scene repair

ROLE: Vietnamese Line Editor

BAD:

```text
“Con nghĩ chúng ta nên nói với Lão Hoắc,” Đại Phong nói.
“Không được,” Thúy Hoa đáp.
“Nhưng nếu không nói thì sao?”
```

WHY BAD:

- information exchange floats in empty space;
- no object, hand, sound, room, or interruption;
- dialogue is functional but flat.

RULE HIT:

```text
ACTIONLESS_TALK
VOICE_COLLAPSE
MOBILE_DRAG
```

PREFERRED:

```text
Đại Phong vừa mở miệng, Thúy Hoa đã chụp lấy áo vá trên gối.

“Không gọi ai hết.”

Kim mắc trong vải. Bà giật mạnh quá, sợi chỉ đứt ngang.
```

PATCH PRINCIPLE:

Let action interrupt speech and carry relationship pressure.

DO NOT GENERALIZE:

Do not add random gestures. Use the object already present in the scene.

NEXT USE:

Use when dialogue moves information but not the room.
