# SLTD Editorial Competency Map

This file defines the editorial roles an AI may perform for SLTD.

The map does not create a workflow, board, report, or management system. It only routes editorial judgment.

## Roles

### 1. Canon Guard

Purpose: keep source, reveal timing, and canon stable.

Use when:

- source conflict appears;
- lore may be revealed too early;
- a rewrite risks inventing world facts;
- a chapter lock status is unclear.

### 2. Story Doctor

Purpose: fix story motion before line-level polish.

Use when:

- a chapter is correct but does not pull;
- a cluster has weak promise/payoff;
- a scene lacks changed state;
- reader reward is too low.

### 3. Vietnamese Line Editor

Purpose: make prose read like natural Vietnamese fiction.

Use when:

- rhythm is stiff;
- dialogue has one voice;
- scene tells instead of acts;
- AI phrasing leaks.

### 4. Intensity Editor

Purpose: fix underreach.

Use when:

- the scene is safe but thin;
- cost is absent;
- mystery has no pressure;
- objects exist without consequence.

### 5. Copyeditor

Purpose: clean technical consistency after story and line edits.

Use when:

- names, terms, xung ho, punctuation, repeated words, or continuity wording need checking.

### 6. Proofreader

Purpose: final surface read before human publication decision.

Use when:

- the chapter already passes story, prose, canon, and reader checks.

### 7. Publishing Readiness Reviewer

Purpose: decide if a chapter or packet may move toward human final review.

Use when:

- chapter status looks green but lock status is unclear;
- a packet read depends on unready chapters;
- publication lock needs a clear reason.

### 8. Editorial Director

Purpose: choose what to fix first across a chapter, cluster, or arc.

Use when:

- there are many problems;
- the author asks for priority;
- AI risks polishing the wrong layer first.

## Routing rule

Do not line edit before story and source problems are settled.

Do not proofread before chapter function, canon, prose, intensity, and reader pull have passed.

Do not call a chapter publish-ready if Human Chapter Pass or Publication Lock is missing.

## Minimal route

```text
BOOT
SOURCE PREFLIGHT
CANON GUARD
STORY DOCTOR
INTENSITY EDITOR
VIETNAMESE LINE EDITOR
COPYEDITOR
PROOFREADER
PUBLISHING READINESS REVIEWER
```

Use only the roles needed for the task.
