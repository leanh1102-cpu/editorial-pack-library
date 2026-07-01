# SLTD Pack Design

This file is the architecture contract for the SLTD pack. `manifest.yml` is the machine-readable entry. `DESIGN.md` explains how the pack should be extended without turning GitHub into a workflow system.

## Purpose

The pack helps the agent:

- read the right source;
- preserve exact source surface before editing;
- keep Entry as a router, not a maze;
- choose one primary route and cap secondary gates;
- control Dai Phong's protagonist advancement as source-bound growth, not Notion labels or AI fantasy;
- run a first-pass editorial workflow before targeted gates;
- preserve scene transitions, skiptime process traces, and event-cluster continuity;
- manage timeline, POV boundary, foreshadowing, folklore, and material threads;
- calibrate prose craft, genre style, voice, and material choices without imitation;
- control scene composition and component balance without formulaic writing;
- control narrative beat escalation, aftershock, off-POV conflict, and promise/payoff;
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
GitHub = editorial rules, routing, evidence discipline, role entries, calibration, source fidelity, entry route governance, protagonist advancement/growth route calibration, first-pass workflow, scene transition/skiptime/event-cluster continuity, timeline/POV/foreshadowing/folklore thread management, prose craft/style/material calibration, scene composition and component balance, narrative beat escalation and aftershock, chapter assembly and split control, Vietnamese register and Viet Dao calibration, webnovel paragraphing and layout rhythm, character distinctiveness and iceberg profiles, living world and community motion, scene-first prose judgment, anti-AI composite checks, character agency, dynamic range, handoff continuity
User instruction = current task and final authority for writes
```

Legacy Google Docs or Workdecks are historical unless the user names them as current.

## Runtime loop

```text
boot_task
source_preflight
task_intake
task_router
entry route governance check when primary route, gate budget, or stop condition is unclear
source surface check when exact source may be missing
protagonist advancement check when Dai Phong's development path, gain type, cost, knowledge limit, forbidden gain, or world-rule sensitivity is in scope
first-pass editorial workflow when beginning prose repair
scene transition skiptime event cluster check when transitions, seams, skiptime, process trace, sensory/symbolic bridge, hard cut, object/material continuity, emotional continuity, or event cluster continuity is in scope
timeline POV foreshadowing folklore check when timeline, POV boundary, reader knowledge, foreshadowing ledger, folklore mutation, material thread, or planting density is in scope
prose craft style check when writing technique, editing technique, genre style, prose style, voice, material, or craft sample calibration is in scope
scene composition balance check when dialogue/action/thought/setting/object/body/silence/summary/aftershock mix is in scope
narrative beat escalation check when beat rhythm, anchor, aftershock, off-POV conflict, or promise/payoff is in scope
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
request type
source requirement
primary blocker
primary route
secondary gates allowed
secondary gates used
gate budget
stop condition
protagonist current state
gain target
gain type
visible object
body trace
relation trace
witness / social trace
cost
knowledge limit
what he can learn
what he must not know
what he misreads
what he does not say
forbidden gain
aftershock
next return
local chapter or scene
from scene / to scene
seam type
transition anchor
what carries over
time skipped
process trace
time position
event order
POV holder
foreshadowing ledger
folklore mutation
material layer
scene function
craft move needed
composition profile
beat map
anchor point
pressure ladder
promise / payoff
living world layer
characters in scope
reader unit
node ledger
open loops
```

## Source fidelity model

```text
SOURCE TEXT > DERIVED DIGEST > CHAT MEMORY
```

Line edit, line surgery, copyedit, proofread, rewrite, exact patch, readiness, current seam, skiptime, event-cluster, timeline, POV, thread ledger, protagonist advancement, route selection when current status is at stake, and lock verdicts require the right source surface.

## Entry route governance and gate budget model

Entry is a router, not a maze.

```text
PRIMARY ROUTE = the smallest route that directly answers the user's request
SECONDARY GATE = a dependent check added only when the primary route exposes a real blocker
GATE BUDGET = the maximum number of gates allowed before the task must stop, report, or ask for source/scope
STOP CONDITION = the point where enough evidence, verdict, or rewrite output has been produced
GATE CASCADE = running every related gate because it is available rather than required
CHECKLIST-FIRST REPAIR = editing to satisfy gates before reading the scene as lived prose
```

The agent must choose one primary route, add secondary gates only when evidence requires them, and stop when the answer, patch, or blocker is complete. If three or more gates seem necessary, create a context brief or prioritized node ledger instead of running a cascade.

## Protagonist advancement and growth route model

Dai Phong's growth must be source-bound.

```text
PROTAGONIST_ADVANCEMENT_NODE = one scene/chapter unit where the protagonist gains a specific capacity, limit, debt, sensitivity, or method
GAIN_TARGET = what the protagonist can now notice, endure, choose, hide, read, trade, refuse, or survive
GAIN_TYPE = body / perception / social reading / language-record / resource logic / concealment-silence / moral-Dao pressure / world-rule sensitivity
COST = what the gain takes from body, family, relation, safety, time, food, money, trust, witness, name, or future route
KNOWLEDGE_LIMIT = what the protagonist can know, infer, misread, hide, or must not know yet
FORBIDDEN_GAIN = growth the source does not allow yet: adult reasoning, clean power-up, system knowledge, hidden lore, moral lecture, sudden competence
```

A protagonist gain must be shown through object, body, relation, witness/social trace, cost, knowledge limit, and aftershock. Do not use Notion labels as prose. Do not upgrade intelligence, power, or Dao insight without source evidence and visible cost. C030 low-layer lore is valid when it becomes world-rule sensitivity for Dai Phong, not system knowledge.

## Scene transition, skiptime, and event cluster continuity model

A transition must carry pressure, information, cost, time, POV access, material state, or aftershock.

```text
SCENE SEAM = the join between one scene/beat and the next
TRANSITION ANCHOR = sound, smell, image, object, action, dialogue, silence, weather, rumor, body state, symbol, or hard cut that carries continuity
SKIPTIME = elapsed time not dramatized on-page
PROCESS TRACE = residue showing what happened during skipped time without summary dump
EVENT CLUSTER = related event chain with start, development, result, and aftershock
```

Skiptime must leave process trace. A sensory or symbolic bridge is valid only if it changes continuity, not just mood. An event cluster must have start, development, result, and aftershock. Missing seam evidence becomes a seam gap, not invented continuity.

## Timeline, POV, foreshadowing, and folklore model

Threads must be planted, held, paid, or retired with evidence.

```text
TIMELINE = where the scene sits in event order, elapsed time, and consequence heat
POV BOUNDARY = what the viewpoint holder can know, infer, misread, hide, or miss
READER KNOWLEDGE = what the reader knows beyond the POV and why that gap creates pressure
FORESHADOWING LEDGER = planted / paid / held / forgotten-risk items tracked by source evidence
FOLKLORE THREAD = rumor, taboo, proverb, song, custom, misheard phrase, ritual trace, or community behavior that mutates through social motion
MATERIAL THREAD = recurring object, place, animal, weather, work, food, medicine, debt, road, paper, clothing, tool, or sound that carries pressure across scenes
PLANTING DENSITY = how many thread signals a scene/chapter carries before it becomes overloaded or decorative
```

The agent must not plant without a route to payoff or pressure, pay off what was not planted or earned, or let narration know what POV cannot know unless source intentionally shifts access. Missing thread evidence becomes a thread gap, not invented canon.

## Prose craft, style, and material calibration model

Craft samples are calibration, not voice to imitate.

```text
CRAFT MOVE = a conditional editing / writing technique used for a scene function
STYLE CALIBRATION = a way to choose register, rhythm, material, and degree without copying a sample
MATERIAL LAYER = concrete life-substance that carries pressure: body, work, object, place, weather, debt, animal, tool, food, medicine, road, rumor, taboo
GENRE FUNCTION = what the move serves: mystery, dread, survival, cost, pursuit, reveal, concealment, consequence, promise/payoff
```

The agent must select one main craft move before patching and must not stack moves to make prose look rich. A craft move is valid only if it changes pressure, relation, information, cost, movement, reader breath, or genre promise.

## Scene composition and component balance model

Composition follows scene function. Percentages are diagnostic bands, not writing formulas.

## Narrative beat escalation and aftershock model

A beat is not an event. A beat must change pressure, information, position, cost, or promise.

## Living world and community motion model

The world must not wait for the protagonist to enter. Living-world repair must not invent major lore, custom, institution, ritual, faction, village history, canon geography, or social system. Missing evidence becomes a world-motion gap, not new canon.

## First-pass editorial workflow model

```text
FIRST PASS = source surface + scene intake + diagnosis + one edit strategy + human-read prose pass
GATES = targeted later checks, not the first writing method
QUALITY = natural Vietnamese prose with route discipline, source-safe protagonist advancement, seam and thread management, scene pressure, craft move discipline, component balance, beat escalation, character behavior, living world motion, rhythm, readable layout, and distinct cast life working together
```

## Chapter assembly and split model

Scene is the edit unit. Chapter is the reader unit. Packet is the continuity and momentum unit.

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

Review modes are lenses, not roles. Learned taste, calibration, route governance, protagonist advancement checks, first-pass workflow, transition/thread/prose/composition/beat/world/character/register/layout gates, scene-first judgment, anti-AI composite checks, character agency checks, and dynamic range checks guide safe edits; they do not override source, canon, evidence, human pass, or publication lock.

## Healthcheck discipline

Check manifest version, required files, allowed tasks, route coverage, source fidelity, entry route governance/gate budget, protagonist advancement/growth route calibration, first-pass workflow, scene transition/skiptime/event-cluster continuity, timeline/POV/foreshadowing/folklore thread management, prose craft/style/material calibration, scene composition/component balance, narrative beat escalation/aftershock, chapter assembly/split control, Vietnamese register/Viet Dao calibration, webnovel paragraphing/layout rhythm, character distinctiveness/iceberg profiles, living world/community motion, scene-first judgment, anti-AI composite, character agency, dynamic range, role boundary, iteration, calibration, handoff continuity, evidence, orphan risk, and changelog.

## Extension policy

Add new files only when they improve editorial reading, rewriting, routing, source fidelity, entry route governance/gate budget, protagonist advancement/growth route calibration, first-pass workflow, scene transition/skiptime/event-cluster continuity, timeline/POV/foreshadowing/folklore thread management, prose craft/style/material calibration, scene composition/component balance, narrative beat escalation/aftershock, chapter assembly/split control, Vietnamese register/Viet Dao calibration, webnovel paragraphing/layout rhythm, character distinctiveness/iceberg profiles, living world/community motion, scene-first judgment, anti-AI composite checks, character agency, dynamic range, role boundaries, controlled iteration, calibration, handoff continuity, evidence, context handling, or pack health.

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

Prefer retrieval, exact source surface, context brief, entry route governance check, protagonist advancement check, first-pass editorial workflow, scene transition skiptime event cluster check, timeline POV foreshadowing folklore check, prose craft style check, scene composition balance check, narrative beat escalation check, chapter assembly split check, living world community motion check, Vietnamese register check, webnovel paragraphing layout check, character distinctiveness check, scene-first prose judgment, anti-AI composite check, character agency check, dynamic range check, node checkpoint, and handoff over trying to remember everything.

## Invariants

- Notion is the live manuscript state.
- GitHub is editorial memory and rules.
- User instruction outranks the pack.
- No canon invention.
- No source write without clear user request.
- No readiness claim without evidence.
- No prose edit from summary.
- Entry is a router, not a maze.
- Choose one primary route before adding secondary gates.
- Secondary gates require evidence, not adjacency.
- Stop when the answer, blocker, patch, or budget is complete.
- A protagonist gain must be shown through object, body, relation, witness/social trace, cost, knowledge limit, and aftershock.
- Do not use Notion labels as prose.
- Gain type is not a prose label.
- C030 low-layer lore is valid when it becomes world-rule sensitivity, not system knowledge.
- Do not upgrade intelligence, power, or Dao insight without source evidence and visible cost.
- No gate cascade.
- No checklist-first prose repair.
- A transition must carry pressure, information, cost, time, POV access, material state, or aftershock.
- Skiptime must leave process trace.
- Sensory or symbolic bridge must change continuity, not just mood.
- Event clusters must have start, development, result, and aftershock.
- Threads must be planted, held, paid, or retired with evidence.
- POV boundary must not leak unearned knowledge.
- Folklore must alter behavior before explanation.
- Material threads must carry pressure, not decorative motif repetition.
- Craft samples are calibration, not voice to imitate.
- A craft move must change pressure, relation, information, cost, movement, reader breath, or genre promise.
- Do not stack craft moves to make prose look rich.
- Composition follows scene function.
- Percentages are diagnostic bands, not writing formulas.
- A beat must change pressure, information, position, cost, or promise.
- The world does not wait for protagonist POV.
- Scene is the edit unit; chapter is the reader unit.
- Paragraph is reader breath, not decoration.
- Line break is structural, not artificial emphasis.
- Hán Việt is controlled, not purged and not allowed to sprawl.
- Viet Dao prose must stay anchored in Vietnamese life.
- Characters are not replaceable scene functions.
- Split large work by node.
