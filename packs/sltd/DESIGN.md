# SLTD Pack Design

This file is the architecture contract for the SLTD pack. `manifest.yml` is the machine-readable entry. `DESIGN.md` explains how the pack should be extended without turning GitHub into a workflow system.

## Purpose

The pack helps the agent:

- read the right source;
- preserve exact source surface before editing;
- run a first-pass editorial workflow before targeted gates;
- control chapter assembly and split risk after scene edits;
- judge the scene before using checklists;
- detect composite AI failure after many correct-looking passes;
- preserve character agency;
- preserve dynamic range and cadence;
- keep canon stable;
- route by chapter, scene, packet, role, and node;
- preserve handoff continuity;
- avoid extra project-management structure.

## Source of truth

```text
Notion = live manuscript state
GitHub = editorial rules, routing, evidence discipline, role entries, calibration, source fidelity, first-pass workflow, chapter assembly and split control, scene-first prose judgment, anti-AI composite checks, character agency, dynamic range, handoff continuity
User instruction = current task and final authority for writes
```

Legacy Google Docs or Workdecks are historical unless the user names them as current.

## Runtime loop

```text
boot_task
source_preflight
task_intake
task_router
source surface check when exact source may be missing
first-pass editorial workflow when beginning prose repair
chapter assembly split check when scene edits become a chapter or reader unit is overloaded
scene-first prose judgment when checklist-first risk appears
anti-AI composite check when synthetic/checklist risk appears
character agency check when OOC/OCC risk appears
dynamic range check when cadence risk appears
role entry card when a role is named
decision_safety
task-specific prompt
agentic iteration checkpoint when continuation is requested
calibration check when examples are relevant
role boundary check when multiple roles overlap
handoff continuity when context degrades or transfer is needed
node_checkpoint
result_report
```

Use the smallest route that answers the request.

## Context strategy

The agent must not try to hold the whole novel in the chat window. For each task, build a small working context:

```text
current source
source surface status
scope
local chapter or scene
scene list
length type and total length
reader unit
governing chapter pressure
natural breakpoints
scene function
first-pass edit layer
edit strategy
scene-first prose status
governing scene pressure
anti-AI composite risk
character agency state
cadence state
relevant canon
active role and boundary
active iteration node
handoff status when transferring
node ledger
open loops
```

## Source fidelity model

```text
SOURCE TEXT > DERIVED DIGEST > CHAT MEMORY
```

Line edit, line surgery, copyedit, proofread, rewrite, exact patch, readiness, and lock verdicts require the right source surface. Digest may guide navigation; it must not become prose surface or current-state evidence.

## First-pass editorial workflow model

Edit first as a human prose editor. Verify after.

```text
FIRST PASS = source surface + scene intake + diagnosis + one edit strategy + human-read prose pass
GATES = targeted later checks, not the first writing method
QUALITY = natural Vietnamese prose with scene pressure, character behavior, and rhythm working together
```

## Chapter assembly and split model

Scene is the edit unit. Chapter is the reader unit. Packet is the continuity and momentum unit.

Scene-level pass does not guarantee chapter-level pass.

Chapter assembly checks whether edited scenes still form one natural reader unit. It controls length risk, reader question, governing chapter pressure, major turns, payoff points, open/closed loops, natural breakpoints, and split recommendations.

Length warnings are not absolute law. Word-count bands apply only when the length type is words. If the count is characters, label it and do not apply word bands mechanically.

A live manuscript must not be split, renumbered, deleted, or updated without explicit user instruction.

## Scene-first prose judgment model

Scene first. Checklist after.

The agent must read the scene as lived Vietnamese prose and find the governing pressure before applying gates.

```text
SCENE JUDGMENT = read the scene as lived Vietnamese prose before applying gates
CHECKLIST = later verification, not the writing method
PROSE LIFE = pressure, relation, object, body, silence, and sentence rhythm working as one movement
```

## Anti-AI composite model

A scene can be correct and still feel AI-made. Composite AI failure happens when safe repairs stack into a scene that is cleaner and more functional but less lived.

Anti-AI composite check catches scene-card visibility, object-as-proof-item, explanation-duty dialogue, universal narrator voice, consequence vacuum, repair collage, false human texture, clean transition disease, negative explanation habit, and false readiness.

## Character agency model

Characters must not become tools for the outline, scene card, clue delivery, or explanation duty. A scene preserves agency when plot function is reached through character pressure:

```text
want
fear
knowledge limit
avoidance or misread
pressure
choice
visible cost
```

## Dynamic range model

Restraint is not flattening. The agent must preserve quiet pressure, controlled escalation, scene turn, and aftershock while matching intensity to scene function.

## Role boundaries

```text
source and canon before story
story before intensity
intensity before line surgery
line surgery before copyedit
copyedit before proofread
proofread before readiness
readiness before publication lock claim
```

Review modes are lenses, not roles. Learned taste, calibration, first-pass workflow, chapter assembly checks, scene-first judgment, anti-AI composite checks, character agency checks, and dynamic range checks guide safe edits; they do not override source, canon, evidence, human pass, or publication lock.

## Healthcheck discipline

Check manifest version, required files, allowed tasks, route coverage, source fidelity, first-pass workflow, chapter assembly/split control, scene-first judgment, anti-AI composite, character agency, dynamic range, role entry, role boundary, iteration, calibration, handoff continuity, evidence, orphan risk, and changelog.

## Extension policy

Add new files only when they improve editorial reading, rewriting, routing, source fidelity, first-pass workflow, chapter assembly/split control, scene-first judgment, anti-AI composite checks, character agency, dynamic range, role boundaries, controlled iteration, calibration, handoff continuity, evidence, context handling, or pack health.

Allowed file types: rule, prompt, sample, role entry, design note, manifest update, changelog entry.

Do not add scripts, workflows, boards, reports, project management files, automation files, or live manuscript copies.

## 1000+ chapter operating model

```text
1 scene = rewrite unit
1 excerpt = line surgery unit
1 chapter = reader/readiness unit
10 chapters = packet check
30 chapters = arc or part check
100+ chapters = map-level review
1000+ chapters = series-level navigation, not line edit
```

Prefer retrieval, exact source surface, context brief, first-pass editorial workflow, chapter assembly split check, scene-first prose judgment, anti-AI composite check, character agency check, dynamic range check, node checkpoint, role entry, role handoff, iteration checkpoint, calibration case, continuity handoff, and session handoff over trying to remember everything.

## Invariants

- Notion is the live manuscript state.
- GitHub is editorial memory and rules.
- User instruction outranks the pack.
- No canon invention.
- No source write without clear user request.
- No readiness claim without evidence.
- No prose edit from summary.
- Scene is the edit unit; chapter is the reader unit.
- No mechanical split by word count alone.
- No silent split or renumber of live manuscript.
- No checklist-first prose repair.
- First-pass editing starts from scene pressure and edit layer, not all gates.
- No hiding synthetic structure with more texture.
- No forcing character behavior only to satisfy scene function.
- No handoff-as-source truth.
- Split large work by node.
