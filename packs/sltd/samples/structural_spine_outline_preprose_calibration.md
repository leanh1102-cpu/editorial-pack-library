# SLTD Structural Spine / Outline Pre-Prose Calibration

These samples calibrate outline preflight, chapter card lock, scene packet lock, and borderbound decisions.

They are not canon, not current manuscript, and not prose to imitate.

## 1. Prose cannot fix missing chapter function

```text
BAD PATTERN:
The scene has strong objects, body pressure, and good dialogue, but the chapter question is unknown.

WHY BAD:
- prose becomes a polished guess
- later gates may pass surface quality while the chapter spine is wrong

PREFERRED CALIBRATION:
Before prose, identify the chapter question, chapter changed state, and how each scene moves that state.
If the chapter question cannot be sourced, mark OUTLINE_REPAIR_REQUIRED.
```

## 2. Chapter Card must become permission, not decoration

```text
BAD PATTERN:
Chapter Card exists but goal, engine, changed state, aftertaste, and object anchor are blank.
The agent proceeds because the prose source is available.

WHY BAD:
- source surface exists but structural permission does not
- line edit will make the text smoother without locking what the chapter must do

PREFERRED CALIBRATION:
CHAPTER_CARD_STATUS: incomplete
PROSE_PERMISSION: blocked
SAFE NEXT ACTION: fill card from current outline and source, or ask user to confirm missing fields
```

## 3. Scene Packet prevents border drift

```text
BAD PATTERN:
A scene introduces stronger supernatural residue because the atmosphere feels thin, but the detailed outline only needs social pressure.

WHY BAD:
- good genre texture crosses the scene border
- lore residue floats outside the chapter function

PREFERRED CALIBRATION:
Map SUPERNATURAL / LORE RESIDUE SLOT before prose.
If no slot exists, do not add residue. Return BORDERBOUND_MISSING or LORE_SLOT_OUT_OF_SPINE.
```

## 4. Outline repair must happen before line edit

```text
BAD PATTERN:
The detailed outline has a contradiction: scene A requires Dai Phong to know a clue; scene B treats the clue as first discovery.
The agent line-edits both scenes for smoother prose.

WHY BAD:
- prose hides continuity conflict
- later readiness creates false pass

PREFERRED CALIBRATION:
OUTLINE_GAPS: clue discovery order conflict
PROSE_PERMISSION: blocked
SAFE NEXT ACTION: patch outline/scene packet first, then line edit exact source
```

## 5. Borderbound protects protagonist growth

```text
BAD PATTERN:
Dai Phong gets a clever deduction because the scene needs momentum.

WHY BAD:
- growth is not sourced by arc/chapter spine
- protagonist becomes too adult or too convenient

PREFERRED CALIBRATION:
PROTAGONIST GAIN PER SCENE must be sourced from Chapter by Chapter Outline / Scene Packet.
If no gain slot exists, keep him observing or mark PROTAGONIST_GAIN_OUT_OF_SPINE.
```