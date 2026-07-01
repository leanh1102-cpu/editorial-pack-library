# SLTD Pack Design

This file is the architecture contract for the SLTD pack. `manifest.yml` is the machine-readable entry. `DESIGN.md` explains how the pack should be extended without turning GitHub into a workflow system.

## Purpose

The pack helps the agent:

- read the right source;
- preserve exact source surface before editing;
- keep Entry as a router, not a maze;
- choose one primary route and cap secondary gates;
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
- route by chapter, scene, packet, role, and node.

## Source of truth

```text
Notion = live manuscript state
GitHub = editorial rules, routing, evidence discipline, role entries, calibration, source fidelity, entry route governance, protagonist inquiry/clue-chain pressure, protagonist advancement/growth route calibration, first-pass workflow, scene transition/skiptime/event-cluster continuity, timeline/POV/foreshadowing/folklore thread management, prose craft/style/material calibration, scene composition and component balance, narrative beat escalation and aftershock, chapter assembly and split control, Vietnamese register and Viet Dao calibration, webnovel paragraphing and layout rhythm, character distinctiveness and iceberg profiles, living world and community motion, scene-first prose judgment, anti-AI composite checks, character agency, dynamic range, handoff continuity
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
protagonist inquiry check when Dai Phong's private question, inner reasoning, small test, kept detail, clue chain, small secret, supernatural pressure, or inquiry route is in scope
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

## Source fidelity model

```text
SOURCE TEXT > DERIVED DIGEST > CHAT MEMORY
```

Line edit, line surgery, copyedit, proofread, rewrite, exact patch, readiness, current seam, skiptime, event-cluster, timeline, POV, thread ledger, protagonist inquiry, protagonist advancement, route selection when current status is at stake, and lock verdicts require the right source surface.

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

A strange sign must create private question, small test, kept detail, partial read/misread, or next return. Inner reasoning should place concrete signs beside each other, not explain the world. Do not add source-unsupported clues or future answers. Do not let Dai Phong form adult system theory too early.

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

## Other core models

```text
TRANSITION: carries pressure, information, cost, time, POV access, material state, or aftershock.
TIMELINE / POV / THREAD: threads must be planted, held, paid, or retired with evidence.
PROSE CRAFT: craft samples are calibration, not voice to imitate.
COMPOSITION: follows scene function; ratios are diagnostic, not formula.
BEAT: must change pressure, information, position, cost, or promise.
LIVING WORLD: the world must not wait for protagonist POV.
FIRST PASS: source surface + scene intake + diagnosis + one edit strategy + human-read prose pass.
```

## Healthcheck discipline

Check manifest version, required files, allowed tasks, route coverage, source fidelity, entry route governance/gate budget, protagonist inquiry/clue-chain pressure, protagonist advancement/growth route calibration, first-pass workflow, transition/thread/prose/composition/beat/world/character/register/layout gates, role boundary, evidence, orphan risk, and changelog.

## Extension policy

Add new files only when they improve editorial reading, rewriting, routing, source fidelity, entry route governance/gate budget, protagonist inquiry/clue-chain pressure, protagonist advancement/growth route calibration, first-pass workflow, transition/thread/prose/composition/beat/world/character/register/layout gates, role boundaries, controlled iteration, calibration, handoff continuity, evidence, context handling, or pack health.

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

Prefer retrieval, exact source surface, context brief, entry route governance check, protagonist inquiry check, protagonist advancement check, first-pass editorial workflow, scene transition skiptime event cluster check, timeline POV foreshadowing folklore check, prose craft style check, scene composition balance check, narrative beat escalation check, chapter assembly split check, living world community motion check, Vietnamese register check, webnovel paragraphing layout check, character distinctiveness check, scene-first prose judgment, anti-AI composite check, character agency check, dynamic range check, node checkpoint, and handoff over trying to remember everything.

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
- Dai Phong must not only receive events; inquiry must show private question, small test, kept detail, partial read/misread, or next return.
- Inner reasoning places concrete signs beside each other; it does not explain the world.
- Supernatural pressure must not remain mood only.
- A protagonist gain must be shown through object, body, relation, witness/social trace, cost, knowledge limit, and aftershock.
- Do not use Notion labels as prose.
- Gain type is not a prose label.
- C030 low-layer lore is valid when it becomes world-rule sensitivity, not system knowledge.
- Do not upgrade intelligence, power, or Dao insight without source evidence and visible cost.
- No gate cascade.
- No checklist-first prose repair.
- Threads must be planted, held, paid, or retired with evidence.
- POV boundary must not leak unearned knowledge.
- Folklore must alter behavior before explanation.
- Material threads must carry pressure, not decorative motif repetition.
- Craft samples are calibration, not voice to imitate.
- A beat must change pressure, information, position, cost, or promise.
- The world does not wait for protagonist POV.
- Scene is the edit unit; chapter is the reader unit.
- Paragraph is reader breath, not decoration.
- Line break is structural, not artificial emphasis.
- Hán Việt is controlled, not purged and not allowed to sprawl.
- Viet Dao prose must stay anchored in Vietnamese life.
- Characters are not replaceable scene functions.
- Split large work by node.
