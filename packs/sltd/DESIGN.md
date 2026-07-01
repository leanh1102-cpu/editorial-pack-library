# SLTD Pack Design

This file is the architecture contract for the SLTD pack. `manifest.yml` is the machine-readable entry. `DESIGN.md` explains how the pack should be extended without turning GitHub into a workflow system.

## Purpose

The pack helps the agent:

- read the right source;
- preserve exact source surface before editing;
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
GitHub = editorial rules, routing, evidence discipline, role entries, calibration, source fidelity, first-pass workflow, scene transition/skiptime/event-cluster continuity, timeline/POV/foreshadowing/folklore thread management, prose craft/style/material calibration, scene composition and component balance, narrative beat escalation and aftershock, chapter assembly and split control, Vietnamese register and Viet Dao calibration, webnovel paragraphing and layout rhythm, character distinctiveness and iceberg profiles, living world and community motion, scene-first prose judgment, anti-AI composite checks, character agency, dynamic range, handoff continuity
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
local chapter or scene
from scene / to scene
seam type
transition anchor
what carries over
time skipped
process trace
what continued off-page
what cooled / what heated
POV access after cut
emotional continuity
object / material continuity
event cluster start / development / result / aftershock
seam break risk
time position
event order
elapsed time
consequence heat
POV holder
POV knowledge boundary
reader knowledge
off-POV access
foreshadowing ledger
planted / paid / held / risk of forgetting
folklore form / source / believer / doubter / wrong repeater / behavior change / mutation step
material layer
scene-level planting density
chapter-level thread status
packet-level continuity risk
scene function
craft move needed
genre function
style register
voice target
bad pattern
preferred move
overuse risk
related gate
composition profile
dialogue ratio
action / blocking ratio
inner thought ratio
setting / living world ratio
object / clue ratio
sensory / body ratio
silence / pause ratio
summary / transition ratio
aftershock ratio
dominant component
missing component
overused component
fake balance risk
beat map
anchor point
pressure ladder
off-POV / parallel conflict
interruption point
aftershock
peak / turn
result
cost ledger
promise / payoff
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

Line edit, line surgery, copyedit, proofread, rewrite, exact patch, readiness, current seam, skiptime, event-cluster, timeline, POV, thread ledger, and lock verdicts require the right source surface.

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

Composition follows scene function.

Percentages are diagnostic bands, not writing formulas.

```text
SCENE COMPOSITION = how the scene distributes reader attention across dialogue, action, thought, place, object, body, silence, summary, and aftershock
COMPONENT BALANCE = whether each component serves pressure, relation, information, cost, movement, or reader breath
FAKE BALANCE = all components are present but none of them truly move the scene
```

A component is valid only if it changes pressure, relation, information, cost, movement, or reader breath. The agent must not add dialogue, action, inner thought, setting, object, sensory/body texture, silence, summary, or aftershock just to fill a ratio.

## Narrative beat escalation and aftershock model

A beat is not an event. A beat must change pressure, information, position, cost, or promise.

```text
BEAT = action / information / choice / conflict unit that changes reading pressure
ANCHOR = concrete point that holds the beat: object, debt, witness, deadline, taboo, path, resource, clue, relation, wound
ESCALATION = the next beat makes the situation harder, stranger, more costly, more public, or less reversible
AFTERSHOCK = trace left after interruption, turn, peak, or chapter end
```

Off-POV or parallel conflict must return as pressure, cost, rumor, resource shift, changed access, changed witness, delayed danger, misunderstanding, deadline, or proof. Benchmark works are mechanical checks only and must not be copied.

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
QUALITY = natural Vietnamese prose with source-safe seam and thread management, scene pressure, craft move discipline, component balance, beat escalation, character behavior, living world motion, rhythm, readable layout, and distinct cast life working together
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

Review modes are lenses, not roles. Learned taste, calibration, first-pass workflow, scene transition/skiptime/event-cluster checks, timeline/POV/thread checks, prose craft checks, scene composition checks, narrative beat checks, chapter assembly checks, Vietnamese register checks, webnovel layout checks, character distinctiveness checks, living world checks, scene-first judgment, anti-AI composite checks, character agency checks, and dynamic range checks guide safe edits; they do not override source, canon, evidence, human pass, or publication lock.

## Healthcheck discipline

Check manifest version, required files, allowed tasks, route coverage, source fidelity, first-pass workflow, scene transition/skiptime/event-cluster continuity, timeline/POV/foreshadowing/folklore thread management, prose craft/style/material calibration, scene composition/component balance, narrative beat escalation/aftershock, chapter assembly/split control, Vietnamese register/Viet Dao calibration, webnovel paragraphing/layout rhythm, character distinctiveness/iceberg profiles, living world/community motion, scene-first judgment, anti-AI composite, character agency, dynamic range, role boundary, iteration, calibration, handoff continuity, evidence, orphan risk, and changelog.

## Extension policy

Add new files only when they improve editorial reading, rewriting, routing, source fidelity, first-pass workflow, scene transition/skiptime/event-cluster continuity, timeline/POV/foreshadowing/folklore thread management, prose craft/style/material calibration, scene composition/component balance, narrative beat escalation/aftershock, chapter assembly/split control, Vietnamese register/Viet Dao calibration, webnovel paragraphing/layout rhythm, character distinctiveness/iceberg profiles, living world/community motion, scene-first judgment, anti-AI composite checks, character agency, dynamic range, role boundaries, controlled iteration, calibration, handoff continuity, evidence, context handling, or pack health.

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

Prefer retrieval, exact source surface, context brief, first-pass editorial workflow, scene transition skiptime event cluster check, timeline POV foreshadowing folklore check, prose craft style check, scene composition balance check, narrative beat escalation check, chapter assembly split check, living world community motion check, Vietnamese register check, webnovel paragraphing layout check, character distinctiveness check, scene-first prose judgment, anti-AI composite check, character agency check, dynamic range check, node checkpoint, and handoff over trying to remember everything.

## Invariants

- Notion is the live manuscript state.
- GitHub is editorial memory and rules.
- User instruction outranks the pack.
- No canon invention.
- No source write without clear user request.
- No readiness claim without evidence.
- No prose edit from summary.
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
- A component must change pressure, relation, information, cost, movement, or reader breath.
- A beat must change pressure, information, position, cost, or promise.
- Interruption must leave inherited pressure.
- Peak must leave result, cost, changed state, or promise/payoff movement.
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
