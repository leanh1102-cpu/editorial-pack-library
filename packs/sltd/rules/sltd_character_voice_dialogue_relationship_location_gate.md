# SLTD Character Voice, Dialogue Weight, Relationship Memory & Location Staging Protocol

This gate prevents dialogue, relationship beats, and staged scenes from becoming generic, static, same-voice, or detached from place.

It adapts scenario-specific input discipline into SLTD prose.

## Core rule

No scene may proceed as prose if voice, relationship, and location are too vague to support it.

```text
CHARACTER_VOICE = how a character speaks: sentence length, word choice, address terms, omissions, work habit, fear, warmth, guardedness, power, age, and relationship pressure
DIALOGUE_WEIGHT = whether a line carries weight proportional to who says it and what they are carrying now
UNSAID_CONTENT = what a character chooses not to say, shown through silence, action, object handling, interruption, avoidance, or changed address
RELATIONSHIP_MEMORY = prior shared events showing up in how characters speak, stand, interrupt, help, avoid, or name each other
PRESENCE_TRACE = who is physically present in a multi-character scene and why each person speaks, stays silent, or reacts
LOCATION_STAGE = the concrete layout and material stage of the scene: doors, thresholds, stove, well, mud, road, shrine steps, forest edge, roots, light, sound, tools, bodies, animals
USABLE_OBJECTS = objects characters can touch, move, hide, use, pay with, lean on, or avoid
TASK_WHILE_SPEAKING = what hands, feet, breath, work, or watching are doing while dialogue happens
TONE_INTEGRITY = comedy, warmth, grief, dread, and tension must arise inside the scene tone, not break it
```

Dialogue is not information delivery. Silence is not absence. Location is not backdrop.

## Use when

- dialogue, multi-character conversation, relationship development, scene staging, location, comedy, grief, confession, realization, tense exchange, or physical struggle is in scope;
- a scene has same-voice dialogue, static talk, characters disappearing from a group scene, stiff exposition, or relationship changes that feel unearned;
- prose needs character voice distinction before line edit or rewrite;
- the scene input is too vague about who is present, what they carry, where they stand, what they touch, and what must remain unsaid.

## Authority

This gate does not invent voice profiles, relationships, backstory, location layout, ability, or canon.

If exact dialogue/prose is being judged or repaired, source surface is required.

If relationship history or location detail is missing, report source gap or Notion update candidate instead of inventing.

## SLTD sound and physical action adaptation

Do not import mandatory bold-caps comic sound effects into SLTD prose.

For SLTD, sound should be written in natural Vietnamese prose and matched to tone:

```text
rắc, bụp, phịch, xoạt, soạt, cạch, keng, rầm, lộp bộp, rào, ục, khục
```

Use sound, rhythm, body, breath, and environment to make impact felt. Do not label impact like a game/comic unless the source style explicitly allows it.

Physical struggle should use the actual place: mud, roots, wall, door, threshold, crowd, water, shrine step, smoke, darkness, slope, rope, tool, animal, or debris.

## Output schema

```text
CHARACTER VOICE / DIALOGUE / STAGING CHECK
SCOPE:
SOURCE USED:
SOURCE SURFACE:
SCENE / CHAPTER:
CHARACTERS PRESENT:
WHO SPEAKS:
WHO STAYS SILENT:
WHY SILENT:
VOICE DIFFERENCE:
RELATIONSHIP MEMORY:
DIALOGUE WEIGHT:
UNSAID CONTENT:
INTERRUPTION / COLLISION:
TASK WHILE SPEAKING:
LOCATION LAYOUT:
USABLE OBJECTS:
ENVIRONMENT PRESSURE:
WORLD RULES IN SCENE:
CHARACTER LIMITS:
POV / KNOWLEDGE LIMIT:
TONE INTEGRITY:
FAILURE LABELS:
SAFE REPAIR:
PROSE PERMISSION:
NEXT NODE:
```

## Scene input minimum

Before drafting or rewriting a dialogue-heavy or staged scene, identify who is present, who speaks, who stays silent and why, what each person carries now, how relationship history changes address and behavior, where bodies stand, what objects can be used, what should not be said directly, what POV can know, and what tone the scene allows.

## Failure labels

```text
SAME_VOICE_DIALOGUE
STATIC_TALK
CHARACTER_DROPS_OUT_OF_SCENE
SILENCE_WITHOUT_REASON
DIALOGUE_AS_FUNCTION_LABEL
RELATIONSHIP_MEMORY_MISSING
UNSAID_CONTENT_MISSING
INTERRUPTION_COLLISION_MISSING
TASK_WHILE_SPEAKING_MISSING
LOCATION_AS_BACKDROP
USABLE_OBJECTS_MISSING
ENVIRONMENT_NOT_USED
SCENE_INPUT_TOO_VAGUE
VOICE_LIMIT_UNDEFINED
AI_SPEAKS_FOR_CHARACTER
TONE_BREAK_FOR_JOKE
COMEDY_OUTSIDE_TONE
GRIEF_RUSHED_OR_OVEREXPLAINED
COMBAT_SOUND_STYLE_MISMATCH
PHYSICAL_SPACE_UNUSED
```

## Safe repair

Safe repair may identify who is present, mark why silence is unearned or needed, separate voice profiles, add task-while-speaking where source supports it, stage the location with existing source objects, reduce exposition through action or avoidance, and propose a Notion update candidate for missing voice/location notes.

Safe repair must not invent new habits, jokes, relationships, secrets, skills, or location objects; add comedy that breaks tone; force sound effects into SLTD style; make all characters speak only to prove presence; or rewrite from summary only.

## Output labels

```text
VOICE_STAGING_OK
VOICE_STAGING_PARTIAL
SCENE_INPUT_REQUIRED
SOURCE_SURFACE_REQUIRED
PROSE_PERMISSION_BLOCKED
```