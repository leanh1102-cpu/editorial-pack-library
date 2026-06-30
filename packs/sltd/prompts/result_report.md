# SLTD Result Report

Use this prompt at the end of an SLTD task.

## Purpose

Return a compact report that shows what was done, which sources and skills were used, what remains open, and whether a Notion update candidate exists.

## Output

```text
WHAT I DID:
SOURCE USED:
SKILLS RUN:
NODE LEDGER:
DECISION:
FINDINGS:
BLOCKERS:
NEXT NODE:
NOTION UPDATE CANDIDATE:
```

## Report rules

- Do not claim a source was read if it was not opened or provided.
- Do not claim a skill was run if no findings came from it.
- If the task stopped, put the reason in BLOCKERS.
- If a write-back is useful, give a candidate instead of writing unless the user asked for writing.
- Keep reports short unless the user asks for a full audit.
