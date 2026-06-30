# SLTD Node Checkpoint

Use this prompt after a focused editorial task, especially after a scene rewrite, audit pass, packet review, or readiness check.

## Required reading

1. `prompts/boot_task.md`
2. `EDITORIAL_MINDMAP.md`
3. `rules/sltd_node_traversal.md`
4. `rules/sltd_notion_update_discipline.md`
5. task output just produced

## Output

```text
NODE CHECKPOINT
SCOPE:
DONE:
- ...
PASSED:
- ...
NOT PASSED:
- ...
NOT READ:
- ...
BLOCKED BY:
- ...
OPEN LOOPS:
- ...
NEXT NODE:
- ...
NOTION UPDATE CANDIDATE:
PAGE:
PROPERTY OR SECTION:
OLD:
NEW:
REASON:
SAFE TO UPDATE: YES / NEEDS CONFIRMATION
```

## Rules

- If no Notion update is needed, write `NOTION UPDATE CANDIDATE: NO`.
- If the user did not ask for write-back, do not write back.
- If a scene is not merged, do not mark its chapter locked.
- If one chapter blocks a packet, name the blocker.
- If a role was not run, do not mark it passed.
