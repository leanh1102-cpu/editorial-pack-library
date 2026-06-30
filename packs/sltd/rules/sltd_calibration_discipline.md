# SLTD Calibration Discipline

Calibration cases turn rejected or approved AI output into reusable operational examples.

They are not canon, not current manuscript, and not publication evidence.

## Purpose

Use calibration to improve future execution of existing roles and gates.

Calibration helps the AI recognize:

- repeated prose smell;
- dialogue voice collapse;
- underreach;
- false readiness;
- over-polished AI repair;
- wrong role routing;
- unsafe canon invention.

## Authority

Calibration sits below:

```text
user current instruction
current Notion source
user-provided current packet
canon guard
evidence discipline
role boundary contracts
```

Calibration may guide choice among safe edits. It must not override current source, canon, scene function, human pass, or publication lock.

## Case format

Each calibration case should use:

```text
CASE ID:
SOURCE TYPE: user excerpt / AI output / Notion current / legacy reference
STATUS: accepted / rejected / mixed
TASK:
ROLE:
BAD:
WHY BAD:
RULE HIT:
PREFERRED:
PATCH PRINCIPLE:
DO NOT GENERALIZE:
NEXT USE:
```

## Quality over quantity

More cases help only when they are clear, labeled, non-duplicative, and tied to a role or rule.

Do not collect vague dislikes such as:

```text
not good
still AI
make it deeper
needs more emotion
```

Convert them into a labeled failure:

```text
DIALOGUE_TOO_CLEAN
VOICE_COLLAPSE
STIFF_TRANSLATED_SYNTAX
ABSTRACT_PRESSURE
SYMBOL_LABEL
FALSE_READINESS
CANON_INVENTION_RISK
```

## Collection rule

When the user rejects an output, do not silently add it to the pack.

Return:

```text
CALIBRATION CANDIDATE
TARGET FILE:
CASE TYPE:
BAD:
WHY BAD:
PREFERRED:
RULE HIT:
SAFE TO ADD: YES / NEEDS CONFIRMATION
```

Only update GitHub when the user asks for a write action.

## Anti-bloat rule

Do not create a new sample file for every small failure.

Append to one of the existing calibration files unless a distinct new category is needed.

Default target files:

```text
samples/line_surgery_calibration.md
samples/dialogue_voice_calibration.md
samples/underreach_calibration.md
samples/readiness_false_positive.md
```

## Use rule

Before line surgery, dialogue repair, underreach audit, or readiness verdict, read the relevant calibration file when the user asks for TASTELOCK, calibration, anti-AI prose, voice repair, underreach, or false readiness checks.

## Stop rule

Do not use calibration when:

- current source was not read but current status is requested;
- calibration conflicts with current user instruction;
- calibration would add canon;
- calibration would change scene outcome;
- calibration is being used to justify publication readiness.
