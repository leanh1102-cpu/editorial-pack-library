# SLTD Human Expert AI-Smell Explanation Calibration

These samples calibrate human-expert AI-smell explanation for SLTD.

They are not canon and are not proof of authorship.

## 1. Keyword-only detector verdict

```text
BAD PATTERN:
This passage uses words like however, furthermore, therefore, so it is AI.

WHY BAD:
Keyword spotting is not human reading and can create false positives.

EXPECTED OUTPUT:
KEYWORD_ONLY_VERDICT_BLOCKED
NO_AI_PROBABILITY_SCORING
REPAIR DIRECTION: explain exact span effect, not authorship
```

## 2. Outline label visible on page

```text
BAD PATTERN:
The prose names the theme, symbol, or lesson before the scene creates pressure through body, object, relation, witness, debt, or choice.

WHY BAD:
The reader sees the outline instead of living through the scene.

EXPECTED OUTPUT:
EXPLANATION DIMENSION: OUTLINE LABEL VISIBLE ON PAGE
STRUCTURAL ROOT CAUSE: YES
NEXT NODE: narrative_feature_audit or scene rewrite, not surface polish alone
```

## 3. Same-voice dialogue

```text
BAD PATTERN:
A child, elder, hunter, and narrator all speak in the same clean register with complete explanatory sentences.

WHY BAD:
Dialogue loses age, relation, status, fear, evasion, and interruption.

EXPECTED OUTPUT:
EXPLANATION DIMENSION: SAME-VOICE DIALOGUE
VOICE_SMELL_HANDOFF
NEXT NODE: character_voice_dialogue_staging_check
```

## 4. Correct but synthetic surface

```text
BAD PATTERN:
The source facts are preserved, but the prose is too smooth, transitions are too clean, and emotion is named before pressure exists.

WHY BAD:
Meaning is correct, but the reader cannot feel a body making a choice under pressure.

EXPECTED OUTPUT:
HUMAN_SURFACE_HANDOFF
SURFACE-ONLY REPAIR SAFE: YES if story/source/voice are clear
```

## 5. False positive: ritual formality

```text
RISK PATTERN:
A ritual speaker uses formal, repetitive language.

WHY RISKY:
Repetition and formality may be source-required or genre-required, not AI-smell.

EXPECTED OUTPUT:
FALSE POSITIVE RISK: HIGH
SURFACE-ONLY REPAIR SAFE: NO / UNCERTAIN
DO NOT DO: flatten ritual register into casual speech
```

## 6. Object density without consequence

```text
BAD PATTERN:
The scene adds many concrete objects, but none changes action, cost, witness, resource, relation, debt, or choice.

WHY BAD:
Concrete detail becomes decoration; the prose feels engineered.

EXPECTED OUTPUT:
EXPLANATION DIMENSION: OBJECT / BODY DETAIL WITHOUT CONSEQUENCE
STRUCTURAL ROOT CAUSE: YES
NEXT NODE: narrative_feature_audit or intensity editor
```

## 7. Vietnamese surface friction

```text
BAD PATTERN:
The Vietnamese sentence is grammatical but sounds translated, stiff, or over-formal for the character and scene pressure.

EXPECTED OUTPUT:
VIETNAMESE_SURFACE_HANDOFF
NEXT NODE: vietnamese_senior_editor_surface_check
```

## 8. Humanization misuse

```text
BAD PATTERN:
The user asks to make it less detectable as AI without source, span, or editorial reason.

WHY BAD:
This becomes detector bypass rather than editorial repair.

EXPECTED OUTPUT:
AUTHORSHIP_CLAIM_NOT_ALLOWED
AI_SMELL_EXPLANATION_NEEDS_SPAN
SAFE CLAIM: I can explain reader-facing synthetic effects after seeing the span.
```