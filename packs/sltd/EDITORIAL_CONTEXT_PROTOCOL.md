# SLTD Editorial Context Protocol

This file defines how an AI should work around limited context windows.

It does not store live manuscript text. It does not replace Notion.

## Core idea

The agent should not try to hold the whole novel in the chat window.

It should build a small working context for each task:

```text
BOOT RULES
CURRENT SOURCE
TASK SCOPE
LOCAL CHAPTER OR SCENE
RELEVANT CANON
ACTIVE SKILLS
NODE LEDGER
OPEN LOOPS
```

## Context layers

### 1. Long memory

GitHub rule pack and Notion project pages.

Use for rules, source, and live state.

### 2. Retrieval layer

The exact pages or files opened for the current task.

Do not claim a source is in context if it was not opened or provided.

### 3. Working brief

A compact task brief created before action.

It should fit in the current answer context and name what is not included.

### 4. Output ledger

The result report, node checkpoint, and update candidate created after action.

This helps the next session recover without rereading everything.

## Rule

If the task is too large for the active context, split by node:

- chapter;
- scene;
- packet;
- role;
- source layer.

Do not summarize away canon, lock status, or blockers.
