# SLTD Review Mode Pass

Use this prompt when the user prefixes a task with a review mode such as TRUEMODE, REDTEAM, PREMORTEM, SOCRATES, SOURCELOCK, CANONLOCK, TASTELOCK, UNDERREACH, DIFFMODE, READINESS, NODETRACE, or HANDOFF.

## Read first

1. `prompts/boot_task.md`
2. `rules/sltd_source_preflight.md`
3. `rules/sltd_review_modes.md`
4. `rules/sltd_decision_safety.md`
5. `rules/sltd_evidence_discipline.md`
6. user request

## Output

```text
REVIEW MODE PASS
MODE:
SCOPE:
SOURCE USED:
BASE ROUTE:
SOURCE RULE:
EVIDENCE RULE:
FINDINGS:
BLOCKERS:
NEXT NODE:
```

## Rules

- A review mode changes the lens, not the source priority.
- Do not skip source preflight.
- Do not make current-state claims without evidence.
- Do not rewrite unless the user asked for rewrite.
- If multiple modes are requested, state how they combine.
- If modes conflict, use the safer mode and say which mode was dropped.
