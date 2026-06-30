# SLTD Underreach Calibration

Use these cases to calibrate scenes that are correct in outline but weak in cost, pressure, object consequence, or reader pull.

These samples are operational examples. They are not canon and not current manuscript source.

## Case UR-001: Object present but not acting

CASE ID: UR-001

SOURCE TYPE: calibration example

STATUS: rejected

TASK: underreach audit

ROLE: Intensity Editor

BAD:

```text
Viên đá được đặt trên bàn. Mọi người nhìn nó với cảm giác bất an.
```

WHY BAD:

- object is present but does not force a choice;
- emotion is named vaguely;
- no cost, action, or consequence;
- scene can be removed without changing behavior.

RULE HIT:

```text
SYMBOL_LABEL
ABSTRACT_PRESSURE
MISSING_OBJECT_PRESSURE
```

PREFERRED:

```text
Viên đá chặn đúng chỗ đặt chén thuốc. Thúy Hoa đổi tay hai lần vẫn không đặt xuống được.
```

PATCH PRINCIPLE:

Make the object interfere with an existing necessity.

DO NOT GENERALIZE:

Do not invent a new necessity. Use what the scene already requires.

NEXT USE:

Use when a prop exists only to be looked at.

## Case UR-002: Correct decision without visible cost

CASE ID: UR-002

SOURCE TYPE: calibration example

STATUS: rejected

TASK: consequence pass

ROLE: Intensity Editor / Story Doctor

BAD:

```text
Đại Phong quyết định giấu chuyện này cho đến khi rõ ràng hơn.
```

WHY BAD:

- decision is summarized;
- no immediate cost;
- no one is put under pressure;
- reader does not feel the consequence.

RULE HIT:

```text
MISSING_COST
THESIS_SENTENCE
UNDERREACH
```

PREFERRED:

```text
Đại Phong nhét viên đá vào đáy sọt tro. Lúc rút tay ra, móng tay hắn đen sì. Thúy Hoa nhìn thấy, nhưng không hỏi.
```

PATCH PRINCIPLE:

Turn decision into a physical act that leaves a mark or relationship pressure.

DO NOT GENERALIZE:

Do not make every cost dramatic. Small visible cost is enough when it changes behavior.

NEXT USE:

Use when the scene states a decision without making anyone pay for it.

## Case UR-003: Mystery without pressure

CASE ID: UR-003

SOURCE TYPE: calibration example

STATUS: rejected

TASK: mystery loop repair

ROLE: Story Doctor / Intensity Editor

BAD:

```text
Câu hỏi về nguồn gốc viên đá vẫn còn đó, khiến mọi chuyện trở nên khó lường hơn.
```

WHY BAD:

- mystery is declared, not felt;
- no immediate danger or practical problem;
- line could be moved to any chapter;
- reader receives label instead of hook.

RULE HIT:

```text
THESIS_SENTENCE
ABSTRACT_PRESSURE
WEAK_MYSTERY_LOOP
```

PREFERRED:

```text
Đến trưa, bếp vẫn không bén lửa ở chân kệ ấy.
```

PATCH PRINCIPLE:

Tie mystery to a practical failure that must be handled soon.

DO NOT GENERALIZE:

Do not explain the cause. Let pressure carry the question.

NEXT USE:

Use when mystery exists only as narration.
