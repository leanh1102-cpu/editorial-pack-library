# SLTD Notion Update Discipline

This rule defines how an AI reports Notion update needs.

It does not grant permission to update Notion.

## Core rule

Do not update Notion unless the user clearly asks for a write action.

When a task finds a change that should be recorded, produce a Notion update candidate.

## Notion update candidate

Use this format:

```text
NOTION UPDATE CANDIDATE
PAGE:
PROPERTY OR SECTION:
OLD:
NEW:
REASON:
CONFIDENCE:
SAFE TO UPDATE: YES / NEEDS CONFIRMATION
```

## When to propose an update

Propose an update when:

- a scene rewrite has passed a named review step;
- a chapter lock status should remain blocked;
- a packet is blocked by a chapter;
- a source conflict is resolved by current Notion;
- a node checkpoint identifies a clear next node;
- a previous pass label is invalidated;
- a readiness label changes.

## When not to update

Do not update when:

- the task was audit only;
- the source was not confirmed;
- the change is only a suggestion;
- the rewrite has not passed read-back or reviewer checks;
- the user asked for discussion, not write-back;
- the status depends on a human pass.

## C030 example rule

If C030 still has unpassed linked scenes, do not mark C030 locked.

If C030 is not locked, do not mark C001-C030 packet locked.

If SC-030-01 is rewritten but not merged, update candidate may mention the scene page only, not the chapter lock.
