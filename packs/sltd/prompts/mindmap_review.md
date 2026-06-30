# SLTD Mindmap Review

Use this prompt when the author asks which nodes have been read, which nodes remain open, or where an editorial route is blocked.

## Required reading

1. `prompts/boot_task.md`
2. `EDITORIAL_MINDMAP.md`
3. `EDITORIAL_COMPETENCY_MAP.md`
4. `rules/sltd_source_preflight.md`
5. `rules/sltd_node_traversal.md`
6. `rules/sltd_notion_update_discipline.md`
7. current Notion source or user-provided source

## Method

Map the requested scope through three layers:

1. source nodes;
2. role nodes;
3. output or blocker nodes.

Do not invent node status. If a node has not been read, mark it NOT READ.

## Output

```text
SCOPE:
SOURCE USED:
PACK: sltd@1.7.0

MINDMAP STATUS:
SOURCE NODES:
- READ:
- NOT READ:

ROLE NODES:
- RUN:
- NOT RUN:

BLOCKER NODES:
- ...

OPEN LOOPS:
- ...

NEXT NODE:
- ...

NOTION UPDATE CANDIDATE:
- YES / NO
```

## Rule

Mindmap review is not a rewrite.

Do not update Notion or GitHub unless the user asks for a write action.
