# SLTD Session Handoff

Use this prompt when ending a long task or when the next chat may need to continue.

## Purpose

Create a compact handoff that survives context-window loss.

## Output

```text
SLTD SESSION HANDOFF
DATE:
SCOPE:
TASK:
SOURCE READ:
RULES USED:
NODE LEDGER:
DECISION:
DONE:
NOT DONE:
OPEN LOOPS:
BLOCKERS:
NEXT NODE:
NOTION UPDATE CANDIDATE:
DO NOT FORGET:
```

## Rules

- Keep handoff compact.
- Name exact nodes, not vague summaries.
- Do not store live manuscript text unless the user asks.
- Do not mark a chapter locked unless current Notion supports it.
- If source was not read, mark it NOT READ.
