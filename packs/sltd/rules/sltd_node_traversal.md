# SLTD Node Traversal

Use this rule whenever an SLTD task touches more than one source, chapter, scene, or editorial role.

## Purpose

The agent must leave a visible trail of what it read, what it ran, what it skipped, and what blocks the next conclusion.

## Required node ledger

Use this compact ledger for audits, packet reads, scene rewrites, and readiness checks:

```text
NODE LEDGER
SCOPE:
SOURCE NODE READ:
- ...
ROLE NODE RUN:
- ...
NOT READ:
- ...
BLOCKED BY:
- ...
OPEN LOOPS:
- ...
NEXT NODE:
- ...
NOTION UPDATE NEEDED: YES / NO
DO NOT UPDATE WITHOUT USER CONFIRMATION: YES
```

## Rules

- Do not claim a node was read if it was not opened or provided.
- Do not claim a role was run if no findings came from that role.
- If a source is legacy, mark it legacy.
- If a packet depends on an unready chapter, put that chapter in BLOCKED BY.
- If a scene is rewritten but not merged, put merge in OPEN LOOPS.
- If the task changes a status candidate, record a Notion update candidate instead of silently updating.

## Common blockers

```text
SOURCE_MISSING
SOURCE_CONFLICT
CURRENT_LEGACY_CONFUSION
SCENE_BANK_NOT_READ
CHAPTER_LOCK_NOT_READY
HUMAN_PASS_MISSING
PUBLICATION_LOCK_NOT_READY
PACKET_BLOCKED_BY_CHAPTER
CANON_CONFLICT
UNDERREACHED
```

## Minimal use

For short answers, include only:

```text
NODE LEDGER: source / role / blocker / next node
```

For major editorial work, include the full ledger.
