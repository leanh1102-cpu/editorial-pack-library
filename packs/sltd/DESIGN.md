# SLTD Pack Design

This file is the architecture contract for the SLTD pack. `manifest.yml` is the machine-readable entry. `DESIGN.md` explains how the pack should be extended without turning GitHub into a workflow system.

## Purpose

The pack helps the agent:

- read the right source;
- preserve exact source surface before editing;
- run a first-pass editorial workflow before targeted gates;
- control chapter assembly and split risk after scene edits;
- calibrate Vietnamese register and Viet Dao prose;
- control webnovel paragraphing, layout rhythm, and mobile readability;
- preserve character distinctiveness and iceberg profiles;
- keep the living world and community motion active beyond POV;
- judge the scene before using checklists;
- detect composite AI failure after many correct-looking passes;
- preserve character agency;
- preserve dynamic range and cadence;
- keep canon stable;
- route by chapter, scene, packet, role, and node.

## Source of truth

```text
Notion = live manuscript state
GitHub = editorial rules, routing, evidence discipline, role entries, calibration, source fidelity, first-pass workflow, chapter assembly and split control, Vietnamese register and Viet Dao calibration, webnovel paragraphing and layout rhythm, character distinctiveness and iceberg profiles, living world and community motion, scene-first prose judgment, anti-AI composite checks, character agency, dynamic range, handoff continuity
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
Vietnamese register check when Hán Việt, translated-Chinese syntax, or Viet Dao balance is in scope
webnovel paragraphing layout check when line breaks, paragraph rhythm, or mobile readability is in scope
character distinctiveness check when cast voice, body, habit, relation, or iceberg profile is in scope
living world community motion check when setting, community, custom, offscreen motion, or environment pushback is in scope
scene-first prose judgment when checklist-first risk appears
anti-AI composite check when synthetic/checklist risk appears
character agency check when OOC/OCC risk appears
dynamic range check when cadence risk appears
node_checkpoint
result_report
```

Use the smallest route that answers the request.

## Context strategy

For each task, build a small working context:

```text
current source
source surface status
scope
local chapter or scene
location
world layer
community activity
custom / habit / taboo
offscreen motion
butterfly trace
environment pushback
social consequence
world iceberg trace
characters in scope
character function
voice signature
body / gesture signature
object / clothing signature
private want / private fear
concealment strategy
iceberg trace
interchangeability risk
scene list
length type and total length
paragraph length map
short-line density
layout rhythm risk
reader unit
governing chapter pressure
natural breakpoints
scene function
first-pass edit layer
edit strategy
Vietnamese register target
Hán Việt load
Viet Dao balance
governing scene pressure
anti-AI composite risk
character agency state
cadence state
relevant canon
node ledger
open loops
```

## Source fidelity model

```text
SOURCE TEXT > DERIVED DIGEST > CHAT MEMORY
```

Line edit, line surgery, copyedit, proofread, rewrite, exact patch, readiness, and lock verdicts require the right source surface.

## Living world and community motion model

The world must not wait for the protagonist to enter.

```text
LIVING WORLD = place + work + custom + rumor + witness + weather + object + social habit moving beyond POV
COMMUNITY MOTION = what people keep doing, avoiding, mishearing, trading, hiding, or repeating when the scene is not looking
WORLD ICEBERG = social rules, old fears, habits, and taboos carried by behavior before explanation
ENVIRONMENT PUSHBACK = space, weather, animal, object, crowd, road, door, stove, market, field, or forest changing action or cost
```

A location is not ready because it is described. A custom is not ready because it is named. A community is not ready because people appear as witnesses.

Living-world repair must not invent major lore, custom, institution, ritual, faction, village history, canon geography, or social system. Missing evidence becomes a world-motion gap, not new canon.

## First-pass editorial workflow model

```text
FIRST PASS = source surface + scene intake + diagnosis + one edit strategy + human-read prose pass
GATES = targeted later checks, not the first writing method
QUALITY = natural Vietnamese prose with scene pressure, character behavior, living world motion, rhythm, readable layout, and distinct cast life working together
```

## Chapter assembly and split model

Scene is the edit unit. Chapter is the reader unit. Packet is the continuity and momentum unit.

Scene-level pass does not guarantee chapter-level pass.

## Vietnamese register and Viet Dao model

Vietnamese life carries the scene. Sino-Vietnamese carries law, rite, rank, taboo, old object, canon term, and Dao pressure when earned.

## Webnovel paragraphing and layout rhythm model

Paragraph is reader breath, not decoration. Line break is a structural signal, not artificial emphasis.

## Character distinctiveness and iceberg model

Agency is not the same as distinctiveness. A character must not exist only as the one who asks, blocks, explains, witnesses, discovers, or moves the scene to the next beat.

## Scene-first prose judgment model

Scene first. Checklist after.

## Anti-AI composite model

A scene can be correct and still feel AI-made.

## Character agency model

Characters must not become tools for the outline, scene card, clue delivery, or explanation duty.

## Dynamic range model

Restraint is not flattening.

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

Review modes are lenses, not roles. Learned taste, calibration, first-pass workflow, chapter assembly checks, Vietnamese register checks, webnovel layout checks, character distinctiveness checks, living world checks, scene-first judgment, anti-AI composite checks, character agency checks, and dynamic range checks guide safe edits; they do not override source, canon, evidence, human pass, or publication lock.

## Healthcheck discipline

Check manifest version, required files, allowed tasks, route coverage, source fidelity, first-pass workflow, chapter assembly/split control, Vietnamese register/Viet Dao calibration, webnovel paragraphing/layout rhythm, character distinctiveness/iceberg profiles, living world/community motion, scene-first judgment, anti-AI composite, character agency, dynamic range, role boundary, iteration, calibration, handoff continuity, evidence, orphan risk, and changelog.

## Extension policy

Add new files only when they improve editorial reading, rewriting, routing, source fidelity, first-pass workflow, chapter assembly/split control, Vietnamese register/Viet Dao calibration, webnovel paragraphing/layout rhythm, character distinctiveness/iceberg profiles, living world/community motion, scene-first judgment, anti-AI composite checks, character agency, dynamic range, role boundaries, controlled iteration, calibration, handoff continuity, evidence, context handling, or pack health.

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

Prefer retrieval, exact source surface, context brief, first-pass editorial workflow, chapter assembly split check, living world community motion check, Vietnamese register check, webnovel paragraphing layout check, character distinctiveness check, scene-first prose judgment, anti-AI composite check, character agency check, dynamic range check, node checkpoint, and handoff over trying to remember everything.

## Invariants

- Notion is the live manuscript state.
- GitHub is editorial memory and rules.
- User instruction outranks the pack.
- No canon invention.
- No source write without clear user request.
- No readiness claim without evidence.
- No prose edit from summary.
- The world does not wait for protagonist POV.
- Missing world depth is marked as world-motion gap, not invented.
- Scene is the edit unit; chapter is the reader unit.
- Paragraph is reader breath, not decoration.
- Line break is structural, not artificial emphasis.
- Hán Việt is controlled, not purged and not allowed to sprawl.
- Viet Dao prose must stay anchored in Vietnamese life.
- Characters are not replaceable scene functions.
- No checklist-first prose repair.
- Split large work by node.
