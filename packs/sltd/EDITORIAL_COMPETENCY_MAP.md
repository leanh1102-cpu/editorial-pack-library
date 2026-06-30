# SLTD Editorial Competency Map

This file defines the editorial roles an AI may perform for SLTD.

The map does not create a workflow, board, report, or management system. It only routes editorial judgment.

For exact start, stop, handoff, and must-not-do boundaries, use `rules/sltd_role_boundary_contracts.md`.

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

### 3. Intensity Editor

Purpose: fix underreach.

Use when:

- the scene is safe but thin;
- cost is absent;
- mystery has no pressure;
- objects exist without consequence.

### 4. Vietnamese Line Editor

Purpose: make prose read like natural Vietnamese fiction.

Use when:

- rhythm is stiff;
- dialogue has one voice;
- scene tells instead of acts;
- AI phrasing leaks.

### 5. Line Surgery

Purpose: repair stiff, translated, over-clean, or AI-like prose at sentence level.

Use when:

- an excerpt of 300-1500 words needs line-level diagnosis;
- the scene may be usable but the prose fails mouth-read;
- the user asks why the passage reads gượng, AI, or not natural Vietnamese.

### 6. Copyeditor

Purpose: clean technical consistency after story, intensity, and line edits.

Use when:

- names, terms, xung ho, punctuation, repeated words, or continuity wording need checking.

### 7. Proofreader

Purpose: final surface read before human publication decision.

Use when:

- the chapter already passes story, prose, canon, intensity, and reader checks.

### 8. Publishing Readiness Reviewer

Purpose: decide if a chapter or packet may move toward human final review.

Use when:

- chapter status looks green but lock status is unclear;
- a packet read depends on unready chapters;
- publication lock needs a clear reason.

### 9. Editorial Director

Purpose: choose what to fix first across a chapter, cluster, or arc.

Use when:

- there are many problems;
- the author asks for priority;
- AI risks polishing the wrong layer first.

## Routing rule

Do not line edit before story and source problems are settled.

Do not run line surgery when the problem is structural scene design.

Do not copyedit before story, canon, intensity, line prose, and reader pull are acceptable.

Do not proofread before chapter function, canon, prose, intensity, and reader pull have passed.

Do not call a chapter publish-ready if Human Chapter Pass or Publication Lock is missing.

If roles overlap, run `rules/sltd_role_boundary_contracts.md` and use the earlier-layer blocker.

## Minimal route

```text
BOOT
SOURCE PREFLIGHT
CANON GUARD
STORY DOCTOR
INTENSITY EDITOR
VIETNAMESE LINE EDITOR
LINE SURGERY if needed
COPYEDITOR
PROOFREADER
PUBLISHING READINESS REVIEWER
EDITORIAL DIRECTOR for priority when needed
```

Use only the roles needed for the task.
