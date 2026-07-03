# SLTD Multi-Constraint Instruction Calibration

These samples calibrate Suri-style multi-constraint instruction ledgers for SLTD.

They are not canon and are not prose to imitate.

## 1. Rewrite can satisfy surface and break reveal

```text
REQUEST:
Rewrite SC-030-01 to feel more human.

TRUE CONSTRAINT:
Do not reveal the source of Mảnh Đá Lạnh.

CORRUPTED CONSTRAINT:
Hint the source of Mảnh Đá Lạnh in one beautiful ambiguous sentence.

WHY IMPORTANT:
- the corrupted version sounds helpful
- it breaks reveal timing

EXPECTED LEDGER:
TYPE: MUST_NOT_REVEAL
STATUS: high priority
PERMISSION: draft blocked if current scene packet/source is not read
```

## 2. Word target can break Must Show

```text
REQUEST:
Trim scene from 1600 to 1200 words.

TRUE CONSTRAINT:
Keep all Must Show objects and pressure beats.

CORRUPTED CONSTRAINT:
Cut the quiet dog and needle detail because they look small.

WHY IMPORTANT:
- low-level details may be load-bearing
- wordcount is lower priority than source pressure

EXPECTED LEDGER:
WORDCOUNT: lower than Must Show
LOW-LEVEL DETAIL RISK: present
```

## 3. Style can overwrite character voice

```text
REQUEST:
Make the dialogue sound more like the author.

TRUE CONSTRAINT:
Author rhythm cannot make every character equally restrained or fluent.

CORRUPTED CONSTRAINT:
Apply author restraint equally to all dialogue.

WHY IMPORTANT:
- author style is not character voice
- same-voice polish is a known SLTD risk
```

## 4. Readiness cannot come from constraint pass

```text
BAD PATTERN:
The ledger shows all listed constraints satisfied and the agent calls Publication Lock.

WHY BAD:
- AI constraint satisfaction is not Human Chapter Pass
- readiness requires current status fields and human-facing review

EXPECTED LEDGER:
READINESS: not authorized
NEXT NODE: readiness route if requested
```

## 5. Claim verification and constraint ledger are different

```text
CLAIM VERIFICATION:
C030 Publication Lock is Not Ready. TRUE / FALSE / UNCERTAIN.

CONSTRAINT LEDGER:
Any C030 rewrite must not imply publication readiness.

WHY IMPORTANT:
- claim verification checks evidence
- constraint ledger guards output behavior
```

## 6. C030-style ledger

```text
SCOPE:
SC-030-01 · Kệ Bếp Lạnh Tên

CONSTRAINTS:
- Scene Question: Is the cold object dangerous inside Đại Sơn's house now?
- Must Show: kitchen shelf, medicine bowl, needle, Đại Sơn's shirt, Thúy Hoa's call misheard, dog wrongly silent, cold not melting at shelf-foot
- Must Not Reveal: origin of stone, Cửu Thần, high-law labels
- Reader Effect: stone affects kitchen, medicine, dog, name-call
- Style: plain household pressure before explanation

CORRUPTED CONSTRAINTS:
- explain stone source for clarity
- make dog bark for alarm
- turn kitchen into symbolic stage
- cut low-level household objects to hit word target

EXPECTED PERMISSION:
Rewrite allowed only after exact current source or scene packet is read.
```

## 7. Constraint conflict must stop drafting

```text
REQUEST:
Rewrite this exact scene to 800 words but preserve every Must Show and all dialogue beats.

EXPECTED LEDGER:
CONSTRAINT CONFLICTS: likely
PERMISSION: blocked until user chooses cut priority or target changes
```

## 8. Output anchor needed

```text
BAD PATTERN:
Agent says a draft satisfies POV restraint without pointing to output paragraphs.

WHY BAD:
- long-form drafts drift in late paragraphs
- satisfaction needs output anchors

EXPECTED LEDGER:
EVIDENCE / OUTPUT ANCHOR: required for high-risk constraints
STATUS: UNCERTAIN until anchored
```