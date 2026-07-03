# SLTD Pack Design

This file is the architecture contract for the SLTD pack. `manifest.yml` is the machine-readable entry. `DESIGN.md` explains how the pack should be extended without turning GitHub into a workflow system.

## Purpose

The pack helps the agent:

- read the right source;
- preserve exact source surface before editing;
- keep Entry as a router, not a maze;
- choose one primary route and cap secondary gates;
- enforce structural spine, outline pre-prose, and borderbound before prose work;
- protect supernatural event residue and dread amplitude without early deep-lore reveal;
- control Dai Phong's inquiry, private reasoning, clue chain, and small tests as source-bound exploration;
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
- route by act, arc, hồi, chapter, scene, packet, role, and node.

## Source of truth

```text
Notion = live manuscript state
GitHub = editorial rules, routing, evidence discipline, role entries, calibration, source fidelity, entry route governance, structural spine/outline pre-prose/borderbound, supernatural event residue/dread amplitude, protagonist inquiry/clue-chain pressure, protagonist advancement/growth route calibration, first-pass workflow, scene transition/skiptime/event-cluster continuity, timeline/POV/foreshadowing/folklore thread management, prose craft/style/material calibration, scene composition and component balance, narrative beat escalation and aftershock, chapter assembly and split control, Vietnamese register and Viet Dao calibration, webnovel paragraphing and layout rhythm, character distinctiveness and iceberg profiles, living world and community motion, scene-first prose judgment, anti-AI composite checks, character agency, dynamic range, handoff continuity
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
structural spine outline pre-prose check when act, arc, hồi, chapter, scene, Story Outline, Chapter by Chapter Outline, Chapter Card, Scene Packet, Replacement Spine, borderbound, or prose permission is in scope
supernatural event residue check when supernatural residue, dread amplitude, folklore incident, beast residue, relic trace, old battlefield leak, Mê Thúy Lâm, Hồn sương, Trọc khí, or deep-lore residue is in scope
protagonist inquiry check when Dai Phong's private question, inner reasoning, small test, kept detail, clue chain, small secret, supernatural pressure, or inquiry route is in scope
protagonist advancement check when Dai Phong's development path, gain type, cost, knowledge limit, forbidden gain, or world-rule sensitivity is in scope
first-pass editorial workflow when beginning prose repair
timeline POV foreshadowing folklore check when timeline, POV boundary, reader knowledge, foreshadowing ledger, folklore mutation, material thread, or planting density is in scope
living world community motion check when setting, community, custom, offscreen motion, or environment pushback is in scope
prose craft style check when writing technique, editing technique, genre style, prose style, voice, material, or craft sample calibration is in scope
scene transition skiptime event cluster check when transitions, seams, skiptime, process trace, sensory/symbolic bridge, hard cut, object/material continuity, emotional continuity, or event cluster continuity is in scope
narrative beat escalation check when beat rhythm, anchor, aftershock, off-POV conflict, or promise/payoff is in scope
chapter assembly split check when scene edits become a chapter or reader unit is overloaded
scene-first prose judgment when checklist-first risk appears
anti-AI composite check when synthetic/checklist risk appears
node_checkpoint
result_report
```

Use the smallest route that answers the request.

## Source fidelity model

```text
SOURCE TEXT > STRUCTURAL SOURCE > DERIVED DIGEST > CHAT MEMORY
```

Line edit, line surgery, copyedit, proofread, rewrite, exact patch, readiness, current seam, skiptime, event-cluster, timeline, POV, thread ledger, structural spine, outline pre-prose, borderbound, supernatural event residue, protagonist inquiry, protagonist advancement, route selection when current status is at stake, and lock verdicts require the right source surface.

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

## Structural spine, outline pre-prose, and borderbound model

Do not use prose to solve missing structure.

```text
STRUCTURAL_SPINE = the source-backed hierarchy from story premise -> act/arc/hồi -> chapter function -> scene function -> prose permission
OUTLINE_PREFLIGHT = reading and checking Story Outline, Chapter by Chapter Outline, Chapter Index, and relevant Scene Bank / Chapter Card before prose work
BORDERBOUND = what the scene/chapter is allowed to cover and what it must not cross
CHAPTER_CARD_LOCK = chapter goal, engine, changed state, aftertaste, continuity, risk flags, and beat map are present enough to guide prose
SCENE_PACKET_LOCK = scene question, pressure, character want/fear, object anchor, canon in/out, must show, must not reveal, and reader effect are present enough to guide prose
PROSE_PERMISSION = allowed only when outline and border are adequate for the requested scope
OUTLINE_REPAIR_REQUIRED = prose must stop because outline/detail spine is missing, thin, contradictory, or not source-current
```

A scene may be vivid and still fail if it answers the wrong chapter question. A chapter may read smoothly and still fail if it does not advance the act/arc/hồi spine. Protagonist gain, supernatural residue, lore, and clue chain must be slotted into the current scene/chapter spine before prose work.

## Supernatural event residue and dread amplitude model

Supernatural pressure must not become safe mood.

```text
SUPERNATURAL_EVENT_RESIDUE = a visible present trace of something that happened, leaks, repeats, or was socially remembered
DREAD_AMPLITUDE = how strongly the sign disturbs daily life, body, animals, route, price, witness, taboo, or community behavior without explaining deep lore
EVENT_ROOT = the actual or rumored event behind the sign: beast attack, missing traveler, old war scar, shrine incident, fog sickness, erased name, relic contact, battlefield leak
RESIDUE_TYPE = ecological / beast / folklore / relic / shrine-taboo / old-battlefield / record-name / social-memory / animal-community
SOCIAL_RESIDUE = how people changed habit, rule, route, price, speech, ritual, witness behavior, or silence because of the sign
ANIMAL_RESIDUE = how dogs, livestock, birds, insects, fish, beasts, or forest creatures changed behavior
MATERIAL_RESIDUE = what remains in object, water, mud, ash, bone, paper, bronze, stone, wound, smell, route, or sound
REVEAL_BOUNDARY = what the scene may show as residue, and what it must not explain yet
```

A supernatural sign must be residue of event, ecology, wound, taboo, beast conflict, relic trace, battlefield trace, or community memory. Canon discipline must not overclamp dread into mood-only fog, cold, silence, or vague omen. Deep lore may appear early only as residue, not explanation.

## Protagonist inquiry, inner reasoning, and clue chain model

Dai Phong must not only receive events. He must form child-scale private questions, test small clues, keep details, misread safely, and return to clues later.

```text
INQUIRY_CHAIN = pressure sign -> private question -> child-scale hypothesis -> small test -> partial read or misread -> kept detail -> small secret -> next return
PRIVATE_QUESTION = what Dai Phong silently asks because a daily pattern broke
CHILD_SCALE_HYPOTHESIS = a concrete guess based on body, object, person, animal, work, price, name, or route
SMALL_TEST = a low-power action: touch again, move object, ask sideways, wait, compare animal behavior, repeat a name, check heat/cold, look for a witness
PARTIAL_READ = what he can reasonably infer now
MISREAD = the wrong or incomplete conclusion that keeps future growth possible
KEPT_DETAIL = a clue he does not say aloud because saying it may create cost
SMALL_SECRET = a tiny discovery that changes his method, not a major lore reveal
NEXT_RETURN = where the clue or method must return later
```

Inner reasoning should place concrete signs beside each other, not explain the world. Do not add source-unsupported clues or future answers. Do not let Dai Phong form adult system theory too early.

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

A protagonist gain must be shown through object, body, relation, witness/social trace, cost, knowledge limit, and aftershock. Do not use Notion labels as prose. Do not upgrade intelligence, power, or Dao insight without source evidence and visible cost.

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
- Do not use prose to solve missing structure.
- Story Outline, Chapter by Chapter Outline, Chapter Card, and Scene Packet are structural sources when prose permission is at stake.
- Prose is blocked when borderbound is missing.
- Protagonist gain, supernatural residue, lore, and clue chain must sit inside the current scene/chapter spine.
- Supernatural pressure must not remain mood only.
- Canon discipline must not overclamp dread amplitude.
- Deep lore appears early as residue, not explanation.
- Beasts are not generic combat/loot threats.
- Folklore must have incident, consequence, or community residue.
- Dai Phong must not only receive events; inquiry must show private question, small test, kept detail, partial read/misread, or next return.
- Inner reasoning places concrete signs beside each other; it does not explain the world.
- A protagonist gain must be shown through object, body, relation, witness/social trace, cost, knowledge limit, and aftershock.
- Do not use Notion labels as prose.
- No gate cascade.
- No checklist-first prose repair.
- Threads must be planted, held, paid, or retired with evidence.
- POV boundary must not leak unearned knowledge.
- The world does not wait for protagonist POV.
- Scene is the edit unit; chapter is the reader unit.
- Split large work by node.
