# SLTD Author Writing Sheet & Claim-Evidence Style Memory

This rule adapts Author Writing Sheet methods for SLTD.

It turns author style into source-backed claim-evidence pairs, so author-aligned drafting does not rely on vague adjectives, chat memory, or surface imitation.

## Core rule

No author-style claim without evidence.

Author Writing Sheet supports drafting. It does not override current source, canon, POV, scene function, character voice, Human Chapter Pass, readiness, or Publication Lock.

## Use when

- the user asks to learn author style from samples;
- Author Voice Fingerprint needs stronger evidence;
- Author-Aligned Drafting would otherwise rely on style adjectives;
- prose is author-like at surface but misses how the author builds plot, pressure, development, or language use;
- the user asks about Author Writing Sheet, claim-evidence style memory, personalized story generation, or sample-backed author profile;
- a ghostwriter-style draft needs prompt-specific story rules from author samples.

## Authority

Run after:

```text
source preflight
approved author samples or current Notion source named as author sample
AUTHOR_WORKING_PROFILE.md
AUTHOR_TASTE_EXAMPLES.md
narrative claim verification if a style claim depends on a factual/status/canon claim
character voice / dialogue / staging if author style may overwrite character voice
```

Run before:

```text
author voice fingerprint verdict when evidence is weak
author-aligned drafting
human surface polish when style memory is being used to polish author-like prose
readiness only as evidence input, never as verdict authority
```

## Required distinction

```text
AUTHOR WRITING SHEET = claim-evidence style memory from approved samples
AUTHOR VOICE FINGERPRINT = compact synthesis of evidence-backed style traits
AUTHOR-ALIGNED DRAFT = bounded prose output using source controls and style memory
NARRATIVE CLAIM VERIFICATION = TRUE/FALSE/UNCERTAIN check for story/status/canon claims
HUMAN SURFACE POLISH = late prose repair, not author-style learning
```

## Categories

Use four compact categories:

```text
PLOT
CREATIVITY
DEVELOPMENT
LANGUAGE_USE
```

### PLOT

How the author tends to build conflict, causality, reversal, pressure, promise/payoff, and route.

PLOT claims require stronger source than Language Use claims because plot habits are easy to overgeneralize.

### CREATIVITY

How the author tends to make situations, objects, folklore, dread, daily life, or world pressure feel specific.

### DEVELOPMENT

How the author tends to move character relation, choice, debt, restraint, knowledge, silence, and cost.

DEVELOPMENT claims require stronger source than Language Use claims because subtext is easy to miss.

### LANGUAGE_USE

Sentence rhythm, paragraph breath, diction, xưng hô/register, dialogue roughness, transition habits, and read-aloud mouth-feel.

Language Use claims still need evidence. Do not reduce them to favorite phrases.

## Output schema

```text
SLTD AUTHOR WRITING SHEET
SCOPE:
SOURCE USED:
AUTHOR SAMPLE STATUS:
CATEGORY:
CLAIM:
EVIDENCE:
COUNTER-AVERAGE / NOT AUTHOR:
APPLIES TO CURRENT TASK: YES / NO / PARTIAL
PLOT IMPACT:
CREATIVITY IMPACT:
DEVELOPMENT IMPACT:
LANGUAGE USE IMPACT:
CHARACTER VOICE RISK:
CANON / SOURCE RISK:
DRAFT PERMISSION:
NEXT NODE:
```

For multiple claims, repeat only CATEGORY / CLAIM / EVIDENCE / USE LIMIT / CURRENT TASK FIT.

## Prompt-specific story rules

When drafting is requested, convert sheet claims into prompt-specific story rules:

```text
AUTHOR-SPECIFIC STORY RULES
SCOPE:
SOURCE USED:
SCENE / CHAPTER CONTROLS:
STYLE CLAIMS USED:
RULES FOR THIS DRAFT:
RULES NOT USED:
CHARACTER VOICE GUARD:
CANON / SOURCE GUARD:
HUMAN SURFACE HANDOFF:
NEXT NODE:
```

Do not include a style claim in drafting rules unless it applies to the current task.

## What counts as evidence

Accepted evidence:

- exact excerpt supplied by the user as author sample;
- current Notion source explicitly named as author sample;
- AUTHOR_TASTE_EXAMPLES.md;
- AUTHOR_WORKING_PROFILE.md when it contains explicit author preference;
- already-approved manuscript excerpt named by user.

Not accepted as evidence by itself:

- chat memory;
- a summary of the author;
- old Workdeck unless named current/sample;
- raw draft unless named sample;
- a general taste assumption;
- a generated passage.

## Failure labels

```text
AUTHOR_WRITING_SHEET_OK
AUTHOR_WRITING_SHEET_PARTIAL
AUTHOR_WRITING_SHEET_BLOCKED
STYLE_CLAIM_WITHOUT_EVIDENCE
AUTHOR_SAMPLE_MISSING
STYLE_MEMORY_OVERFITTING
PLOT_CLAIM_UNDER_EVIDENCED
DEVELOPMENT_CLAIM_UNDER_EVIDENCED
LANGUAGE_USE_PHRASE_TRAP
AUTHOR_STYLE_OVER_CHARACTER_VOICE
STYLE_CLAIM_CANON_DRIFT
PROMPT_RULES_NOT_SOURCE_SAFE
DRAFT_PERMISSION_BLOCKED
READINESS_NOT_AUTHORIZED
```

## Safe repair

Safe repair may:

- request approved author samples;
- build compact claim-evidence style memory;
- mark a style claim as partial;
- separate plot/development claims from language-use claims;
- create prompt-specific story rules for a bounded draft;
- route to Author Voice Fingerprint or Author-Aligned Drafting after evidence is clear.

Safe repair must not:

- invent style traits;
- treat style adjectives as evidence;
- use author voice to override character voice;
- use style memory to add canon, object, payoff, institution, or reveal;
- claim Human Chapter Pass, readiness, or Publication Lock;
- create scripts, workflows, reports, boards, databases, automations, or live manuscript copies.

## Output labels

```text
AUTHOR_WRITING_SHEET_READY
AUTHOR_WRITING_SHEET_NEEDS_MORE_SAMPLE
AUTHOR_WRITING_SHEET_BLOCKED
AUTHOR_SPECIFIC_RULES_READY
AUTHOR_SPECIFIC_RULES_BLOCKED
AUTHOR_VOICE_FINGERPRINT_HANDOFF
AUTHOR_ALIGNED_DRAFT_HANDOFF
```