# SLTD Editorial Harm Anticipation Calibration

These samples calibrate AHA-style harm vignettes for SLTD.

They are not canon and are not prose to imitate.

## 1. False readiness harm

```text
TARGET: HUMAN_CHAPTER_PASS / PUBLICATION_LOCK
FAILURE BEHAVIOR: FALSE_READINESS
VIGNETTE:
A chapter has several green technical pass labels, and the agent calls it ready without reading current Human Chapter Pass or Publication Lock fields.
LIKELY HARM:
A not-ready chapter moves forward; later repair has to undo false confidence and old pass labels.
REPAIR:
Narrative Claim Verification + current readiness route.
```

## 2. Reveal leak harm

```text
TARGET: CANON_REVEAL / READER_EFFECT
FAILURE BEHAVIOR: REVEAL_LEAK
VIGNETTE:
A polish pass adds one beautiful ambiguous line that hints the origin of an object the Scene Packet says must not reveal.
LIKELY HARM:
Mystery pressure turns into lore tease; reader gets the wrong contract; later reveal loses force.
REPAIR:
Source Surface + Multi-Constraint Ledger + Canon Guard.
```

## 3. Over-polish harm

```text
TARGET: VIETNAMESE_SURFACE / SCENE_FUNCTION
FAILURE BEHAVIOR: OVER_POLISH
VIGNETTE:
The agent smooths rough household speech until all family members speak in clean editorial Vietnamese.
LIKELY HARM:
The scene reads fluent but false; relationship pressure and class/household texture flatten.
REPAIR:
Character Voice / Dialogue / Staging before Human Surface Polish.
```

## 4. Wordcount harm

```text
TARGET: SCENE_FUNCTION / OBJECT_STATE
FAILURE BEHAVIOR: WORDCOUNT_CUTS_MUST_SHOW
VIGNETTE:
A trim pass removes the small object or animal behavior that looks minor but carries the scene's pressure.
LIKELY HARM:
The shorter scene becomes cleaner but no longer proves the object is affecting daily life.
REPAIR:
Multi-Constraint Ledger with Must Show priority above word target.
```

## 5. Author style over character voice

```text
TARGET: CHARACTER_VOICE / AUTHOR_STYLE
FAILURE BEHAVIOR: STYLE_OVER_CHARACTER_VOICE
VIGNETTE:
The agent applies author restraint to every character line, making elders, children, and protagonist share the same silence.
LIKELY HARM:
Author-like prose hides same-voice dialogue.
REPAIR:
Author Writing Sheet + Character Voice / Dialogue / Staging.
```

## 6. Compressed source harm

```text
TARGET: CANON_REVEAL / SOURCE_STATUS
FAILURE BEHAVIOR: COMPRESSED_SOURCE_REPLACES_CURRENT
VIGNETTE:
The agent trusts a chapter summary and misses a current Notion field that invalidates an old pass label.
LIKELY HARM:
A legacy or compressed source becomes false source truth.
REPAIR:
Context Capsule + Narrative Claim Verification.
```

## 7. C030-style calibration

```text
SCOPE: SC-030-01
TARGET: READER_EFFECT
FAILURE BEHAVIOR: AI_SMOOTHING_HOUSEHOLD_PRESSURE
VIGNETTE:
A surface polish makes the kitchen scene more lyrical and less awkward, but reduces the medicine bowl, needle, shirt, dog silence, and misheard call to atmospheric props.
LIKELY HARM:
The reader no longer feels the object disturbing household care and speech; the scene becomes symbol-first.
REPAIR:
Multi-Constraint Ledger + Human Surface Polish only after constraints are anchored.
```

## 8. Matrix overload

```text
BAD PATTERN:
The agent generates thirty harms for a small line edit.

WHY BAD:
- review cost exceeds usefulness
- highest blocker is hidden

PREFERRED CALIBRATION:
Return top 3 harms by severity and one next route.
```