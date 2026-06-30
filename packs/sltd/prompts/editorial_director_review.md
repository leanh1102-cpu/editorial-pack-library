# SLTD Editorial Director Review

Use this prompt when the author asks what to fix first.

## Required reading

1. `prompts/boot_task.md`
2. `EDITORIAL_COMPETENCY_MAP.md`
3. `rules/sltd_source_preflight.md`
4. `rules/sltd_developmental_editing.md`
5. `rules/sltd_underreach_gate.md`
6. task source from Notion or user-provided text

## Method

Do not line edit first.

Rank issues by damage:

1. source or lock error;
2. canon or reveal error;
3. story function error;
4. reader pull or intensity error;
5. prose voice error;
6. copyedit surface error.

## Output

```text
SCOPE:
SOURCE USED:
PACK: sltd@1.6.0

TOP BLOCKER:
- ...

PRIORITY ORDER:
1.
2.
3.

DO NOW:
- ...

DO LATER:
- ...

DO NOT TOUCH:
- ...

ROLE ROUTING:
Canon Guard:
Story Doctor:
Intensity Editor:
Vietnamese Line Editor:
Copyeditor:
Proofreader:
Publishing Readiness Reviewer:
```

## Stop rule

If the source or lock status is unclear, stop before ranking fixes.
