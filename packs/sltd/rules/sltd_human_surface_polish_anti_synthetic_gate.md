# SLTD Human Surface Polish & Anti-Synthetic Prose Gate

This rule adapts polish/humanization ideas for SLTD without using detector-bypass goals.

It exists to catch prose that is correct in meaning but still reads synthetic, over-smoothed, same-voiced, outline-shaped, or emotionally generic.

## Core rule

Do not humanize by smoothing.

A human-surface polish may make Vietnamese prose more lived-in, voiced, and read-aloud natural only after source, canon, structure, tracking, voice/staging, and Vietnamese senior surface constraints are clear enough for prose work.

This gate does not authorize:

- bypassing AI detectors;
- changing scene function;
- adding canon;
- adding metaphor to hide stiffness;
- making all speakers fluent;
- leaking hidden canon;
- rewriting from summary;
- marking Human Chapter Pass or Publication Lock.

## Use when

- the scene content is correct but reads like polished AI prose;
- transitions are too clean, generic, or essay-like;
- dialogue has no household, age, class, pressure, or relationship difference;
- body/object pressure was preserved in outline but flattened in prose;
- narration names emotion before pressure exists;
- props act as symbols instead of forces in the scene;
- a line edit made the scene smoother but less alive;
- the task asks for human-surface polish, anti-synthetic prose pass, read-aloud naturalness, hoặc văn nghe người hơn.

## Authority

Run this gate after:

```text
source surface when exact prose is required
context capsule when current source, hidden canon, POV knowledge, source-status separation, or long-range continuity is in scope
structural / tracking / voice / Vietnamese senior editor gates when their blockers are in scope
```

Run it before:

```text
copyedit
proofread
readiness
publication lock claim
```

If source, canon, structure, state, POV, relationship, or voice is still blocked, do not polish. Hand back to the earlier gate.

## Human surface principles

Prefer:

- concrete body, breath, hand, mouth, skin, silence, work, tool, room, weather;
- one pressure per sentence cluster;
- Vietnamese sentence rhythm that can be read aloud;
- character-specific roughness, hesitation, class, age, and household pressure;
- objects that cause action or risk;
- small unevenness when the scene needs fear, poverty, embarrassment, fatigue, or concealment.

Avoid:

- detector-bypass framing;
- elegant smoothing that removes survival roughness;
- generic emotional polish;
- symbolic upgrading;
- clean thesis endings;
- same-voice dialogue;
- abstract transitions;
- Westernized passive phrasing;
- replacing Vietnamese mouth-feel with literary gloss.

## Required distinction

```text
LINE EDIT = improves sentence rhythm and clarity
LINE SURGERY = repairs broken or AI-smelling line sets
HUMAN SURFACE POLISH = restores lived human pressure after the scene is already source-safe and prose-permitted
COPYEDIT = technical consistency after prose is already alive
PROOFREAD = final surface error catch
```

Human Surface Polish must not become a second rewrite. If more than 30 percent of the excerpt needs replacement, return to Line Surgery or Rewrite Scene.

## Output schema

```text
HUMAN SURFACE POLISH PASS
SCOPE:
SOURCE USED:
SOURCE STATUS:
CONTEXT CAPSULE STATUS:
SCENE QUESTION:
MUST SHOW:
MUST NOT REVEAL:
READER EFFECT:
AUTHOR VOICE SAMPLE USED:
AI-SYNTHETIC SMELL:
FALSE SMOOTHING RISK:
VOICE FLATTENING RISK:
OBJECT / BODY LOSS:
RELATIONSHIP LOSS:
REVEAL LEAK RISK:
OLD:
NEW:
WHY THIS FIX:
READ-ALOUD RESULT:
PROSE PERMISSION:
NEXT NODE:
```

Use only fields needed by the task. Keep OLD/NEW patches minimal.

## Prose permission blockers

```text
current source required but not read
context capsule blocked
scene function unclear
canon conflict unresolved
POV knowledge unclear
hidden canon leak risk
voice profile / relationship memory unclear
object, body, debt, or location state unclear
exact prose surface not read
repair load exceeds 30 percent
```

## Failure labels

```text
HUMAN_SURFACE_OK
HUMAN_SURFACE_PARTIAL
HUMAN_SURFACE_BLOCKED
FALSE_SMOOTHING_RISK
SAME_VOICE_POLISH_RISK
OBJECT_BODY_LOSS
RELATIONSHIP_FLATTENING
SYMBOLIC_POLISH_DRIFT
DETECTOR_BYPASS_FRAMING
PROSE_PERMISSION_BLOCKED
NEEDS_LINE_SURGERY
NEEDS_SCENE_REWRITE
```

## Safe repair

Safe repair may:

- return a small OLD/NEW patch;
- mark where the prose got too smooth;
- restore object/body/action already present in source;
- separate speaker voices using existing relationship and scene pressure;
- cut abstract transitions;
- route back to Line Surgery, Voice/Staging, Tracking, Structural Spine, or Context Capsule.

Safe repair must not:

- add new beat, lore, object, relationship, secret, or payoff;
- alter scene outcome;
- overwrite author taste with generic polish;
- use hidden canon in POV prose;
- call readiness or publication lock.

## Output labels

```text
HUMAN_SURFACE_READY
HUMAN_SURFACE_NEEDS_PATCH
HUMAN_SURFACE_BLOCKED
NEXT_NODE_REQUIRED
COPYEDIT_READY
READINESS_NOT_AUTHORIZED
```
