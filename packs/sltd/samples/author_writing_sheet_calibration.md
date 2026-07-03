# SLTD Author Writing Sheet Calibration

These samples calibrate claim-evidence author style memory for SLTD.

They are not canon and are not prose to imitate.

## 1. Style adjective is not evidence

```text
BAD PATTERN:
The agent says the author's style is gritty, poetic, restrained, and atmospheric without quoting or citing samples.

WHY BAD:
- adjectives are not evidence
- drafting from adjectives produces generic imitation

PREFERRED CALIBRATION:
CATEGORY: LANGUAGE_USE
CLAIM: blocked
EVIDENCE: missing
VERDICT: AUTHOR_WRITING_SHEET_BLOCKED / AUTHOR_SAMPLE_MISSING
```

## 2. Plot claim needs stronger evidence

```text
BAD PATTERN:
From one scene, the agent claims the author always uses delayed causality and anti-clean plot turns.

WHY BAD:
- plot habits need wider sample coverage
- one scene may reflect local design, not author fingerprint

PREFERRED CALIBRATION:
CATEGORY: PLOT
CLAIM: partial
EVIDENCE: one sample only
RISK: PLOT_CLAIM_UNDER_EVIDENCED
NEXT NODE: ask for more approved samples or keep claim local
```

## 3. Development claim must track relation and cost

```text
BAD PATTERN:
The agent says the author likes emotional restraint, then writes everyone silent without consequence.

WHY BAD:
- restraint is not absence
- author development often appears through choice, debt, witness, relation, and withheld speech

PREFERRED CALIBRATION:
CATEGORY: DEVELOPMENT
CLAIM: characters hide part of what they know, but silence must create cost or misrecognition
EVIDENCE: approved sample lines / author taste example
USE LIMIT: do not make all characters equally quiet
```

## 4. Language use is not catchphrase mining

```text
BAD PATTERN:
The style sheet lists favorite phrases and repeats them in every draft.

WHY BAD:
- repeated phrases become formula
- author voice is rhythm, pressure, and omission, not stickers

PREFERRED CALIBRATION:
CATEGORY: LANGUAGE_USE
CLAIM: varied short/medium sentence rhythm under pressure
EVIDENCE: sample paragraphs
COUNTER-AVERAGE: avoids clean thesis transitions
```

## 5. Creativity must remain source-safe

```text
BAD PATTERN:
The agent learns the author likes eerie household objects and adds a new ritual object to a scene.

WHY BAD:
- author style cannot add canon or object

PREFERRED CALIBRATION:
CATEGORY: CREATIVITY
CLAIM: ordinary objects become pressure when they change work, speech, access, or witness
EVIDENCE: approved sample
DRAFT RULE: use only objects already allowed by Scene Packet
```

## 6. Prompt-specific rules must be selective

```text
BAD PATTERN:
The agent uses every style claim in every draft.

WHY BAD:
- style memory becomes overfitting
- scenes lose their own pressure

PREFERRED CALIBRATION:
STYLE CLAIMS USED: only those relevant to current Scene Question / Must Show / Reader Effect
RULES NOT USED: claims that would conflict with character voice or canon lock
```

## 7. C030-style calibration

```text
SCOPE:
SC-030-01 · Kệ Bếp Lạnh Tên

LIKELY AUTHOR-SHEET RULE:
- PLOT: let household pressure expose danger before explanation
- CREATIVITY: ordinary objects carry the uncanny only when they disturb work or care
- DEVELOPMENT: family speech hides fear through practical tasks
- LANGUAGE_USE: keep Vietnamese mouth-feel plain, broken by object pressure, not lyrical dread

SOURCE REQUIREMENT:
These rules need approved samples or AUTHOR_TASTE_EXAMPLES.md before drafting.

USE LIMIT:
Do not add new lore, new object, or high-law explanation.
```

## 8. Writing sheet is not readiness

```text
BAD PATTERN:
A scene matches author writing sheet and is called ready.

WHY BAD:
- style match is not Human Chapter Pass
- readiness requires current source, chapter assembly, surface pass, copy/proof, and lock evidence

PREFERRED CALIBRATION:
OUTPUT: AUTHOR_WRITING_SHEET_READY only for style-memory handoff
NEXT NODE: Author Voice Fingerprint / Author-Aligned Draft / Human Surface / Readiness as required
```