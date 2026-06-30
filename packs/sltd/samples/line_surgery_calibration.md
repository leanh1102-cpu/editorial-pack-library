# SLTD Line Surgery Calibration

Use these cases to calibrate line-level Vietnamese prose repair.

These samples are operational examples. They are not canon and not current manuscript source.

## Case LS-001: Abstract pressure disguised as prose

CASE ID: LS-001

SOURCE TYPE: calibration example

STATUS: rejected

TASK: line surgery / anti-AI prose

ROLE: Line Surgery

BAD:

```text
Cái lạnh ấy như nhắc nhở hắn rằng số phận chưa từng buông tha cho gia đình này.
```

WHY BAD:

- explains meaning instead of making pressure happen;
- uses abstract fate language;
- no body, object, or immediate action;
- sounds like polished assistant prose.

RULE HIT:

```text
ABSTRACT_PRESSURE
THESIS_SENTENCE
OVEREXPLAINED_EMOTION
```

PREFERRED:

```text
Hắn kéo áo xuống. Mép vải chạm lưng, lạnh đến mức hắn quên mất câu mẹ vừa dặn.
```

PATCH PRINCIPLE:

Replace abstract pressure with body, object contact, and a missed action.

DO NOT GENERALIZE:

Do not remove all interiority. Remove only explanation that the scene has not earned.

NEXT USE:

Use when a line tells the reader what pressure means instead of letting a physical detail carry it.

## Case LS-002: Symbol label instead of object force

CASE ID: LS-002

SOURCE TYPE: calibration example

STATUS: rejected

TASK: line surgery / object grounding

ROLE: Line Surgery

BAD:

```text
Viên đá nằm đó như một dấu hiệu của bí mật cổ xưa đang chờ được đánh thức.
```

WHY BAD:

- object becomes symbolic label;
- no one in the room has to act differently;
- mystery is announced too early;
- prose pushes lore before scene pressure.

RULE HIT:

```text
SYMBOL_LABEL
FALSE_LITERARY_IMAGE
ABSTRACT_PRESSURE
```

PREFERRED:

```text
Viên đá chèn dưới chân bếp. Thúy Hoa đẩy chén thuốc ra, rồi lại kéo về bằng hai ngón tay.
```

PATCH PRINCIPLE:

Make the object change hand movement, household action, or immediate risk.

DO NOT GENERALIZE:

Do not turn every object into a prop beat. Use the object only when it affects action.

NEXT USE:

Use when a prop looks meaningful but does not alter the scene.

## Case LS-003: Clean AI transition

CASE ID: LS-003

SOURCE TYPE: calibration example

STATUS: rejected

TASK: transition repair

ROLE: Vietnamese Line Editor / Line Surgery

BAD:

```text
Sau khoảnh khắc ấy, mọi thứ trong căn bếp dường như trở nên nặng nề hơn.
```

WHY BAD:

- vague transition;
- tells atmosphere instead of changing the room;
- could appear in many scenes;
- no scene-native interruption.

RULE HIT:

```text
CLEAN_AI_TRANSITION
ABSTRACT_PRESSURE
MOBILE_DRAG
```

PREFERRED:

```text
Con chó vàng thôi cào cửa. Tiếng móng ngừng lại làm Thúy Hoa ngẩng đầu.
```

PATCH PRINCIPLE:

Enter the next beat through sound, silence, hand, object, animal reaction, or unfinished speech.

DO NOT GENERALIZE:

Do not overuse animal reaction as a universal solution. Use the scene's actual pressure source.

NEXT USE:

Use when a paragraph bridge is smooth but dead.
