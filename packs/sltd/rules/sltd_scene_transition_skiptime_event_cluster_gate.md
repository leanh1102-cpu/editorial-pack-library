# SLTD Scene Transition, Skiptime & Event Cluster Continuity Gate

This gate controls scene seams, transitions, skiptime, sensory bridges, symbolic bridges, process traces, and event-cluster continuity.

It prevents scenes, objects, phenomena, and events from becoming isolated units that reset after serving one scene.

## Core rule

A transition must carry pressure, information, cost, time, POV access, material state, or aftershock.

```text
SCENE SEAM = the join between one scene/beat and the next
TRANSITION ANCHOR = sound, smell, image, object, action, dialogue, silence, weather, rumor, body state, symbol, or hard cut that carries continuity
SKIPTIME = elapsed time not dramatized on-page
PROCESS TRACE = residue showing what happened during skipped time without summary dump
EVENT CLUSTER = related event chain with start, development, result, and aftershock
```

Skiptime must leave process trace.

A sensory or symbolic bridge is valid only if it changes continuity, not just mood.

An event cluster must have start, development, result, and aftershock.

## Use when

- scene transitions feel abrupt, decorative, or emotionally reset;
- sound, smell, image, symbol, or object is used as a bridge but carries no pressure;
- skiptime summarizes instead of showing process trace;
- a short or long time cut loses consequence heat;
- objects, phenomena, or events reset between scenes;
- scenes are individually functional but do not form an event cluster;
- a cluster lacks start, development, result, or aftershock;
- transitions by sound, smell, image, symbol, weather, rumor, or body state need audit;
- the user asks about chuyển cảnh, nối cảnh, tiếp cảnh, skiptime, cụm sự kiện, process trace, dư chấn, or seam continuity.

## Authority

This gate sits below:

```text
current user instruction
current Notion source or user-provided source packet
source fidelity gate
canon guard
evidence discipline
role boundary contracts
```

It must not invent new scenes, events, chronology, canon, folklore, clue, or payoff.

If exact transition text or scene boundary is missing, run Source Surface Check before patching.

## Seam ledger

For each transition in scope, identify:

```text
FROM SCENE:
TO SCENE:
SEAM TYPE: sound / smell / image / object / action / dialogue / silence / weather / rumor / body / symbol / hard cut
TRANSITION ANCHOR:
WHAT CARRIES OVER:
TIME SKIPPED:
PROCESS TRACE:
WHAT CONTINUED OFF-PAGE:
WHAT COOLED:
WHAT HEATED:
POV ACCESS AFTER CUT:
EMOTIONAL CONTINUITY:
OBJECT / MATERIAL CONTINUITY:
SEAM STATUS:
```

A seam is healthy when the next scene inherits at least one trace of pressure, information, cost, time, POV access, material state, or aftershock.

## Sensory / symbolic bridge test

Ask:

```text
Where does this sound, smell, image, or symbol come from?
Who perceives it?
What does it tell us about time, distance, access, danger, witness, or consequence?
Does it carry an object state, body state, rumor state, weather state, or social state across the cut?
Would the transition lose pressure if the bridge were removed?
```

If the bridge only carries mood, mark sensory bridge as ornament or symbolic bridge without causality.

## Skiptime process trace test

Skiptime should be shown through residue, not list summary.

Useful process traces include:

```text
medicine cools
mud dries
smoke thins or stops
dog behavior changes
door remains open / shuts too early
clothing dries, stains, tears, or is mended halfway
child repeats a wrong phrase
rumor arrives before the person does
stool, bowl, paper, tool, lamp, ash, or footprint changes state
someone waits long enough to shift posture or change speech
```

Ask:

```text
What did time do to object, body, weather, rumor, work, access, or relation?
What happened off-page that the reader can infer from residue?
What consequence heat changed from hot to warm, cooled, or intensified?
```

If skiptime only says time passed, mark skiptime without process trace.

## Event cluster test

For any related event chain, identify:

```text
EVENT CLUSTER:
START:
DEVELOPMENT:
RESULT:
AFTERSHOCK:
LINKING MATERIAL:
LINKING WITNESS / RUMOR:
LINKING COST:
NEXT INHERITED PRESSURE:
```

A cluster is not a theme. It is a causal or pressure chain.

If events share topic but not consequence, mark event cluster fragmented.

## Continuity heat test

Across a transition, ask:

```text
What is still hot?
What has cooled?
What has become harder because of the cut?
What has become easier or more dangerous because time passed?
Which object, rumor, wound, debt, witness, or relationship cannot reset?
```

Do not let objects, emotions, danger, or social pressure reset cleanly between scenes.

## Failure labels

Use these labels:

```text
TRANSITION_AS_DECORATION
SENSORY_BRIDGE_AS_ORNAMENT
SYMBOLIC_BRIDGE_WITHOUT_CAUSALITY
SKIPTIME_SUMMARY_DUMP
SKIPTIME_WITHOUT_PROCESS_TRACE
SCENE_SEAM_BREAK
EVENT_CLUSTER_FRAGMENTED
EVENT_WITHOUT_START
DEVELOPMENT_SKIPPED
RESULT_MISSING
AFTERSHOCK_MISSING
OBJECT_RESETS_BETWEEN_SCENES
EMOTION_RESET_AFTER_CUT
TIME_CUT_WITHOUT_HEAT_CHANGE
CAUSALITY_DROPPED
HARD_CUT_WITHOUT_INHERITED_PRESSURE
```

## Safe repair

Safe repair may:

- identify what carries over between two existing scenes;
- turn a sensory bridge into a continuity bridge when source supports it;
- replace summary skiptime with one process trace from existing material;
- clarify what cooled, heated, continued off-page, or changed state;
- connect existing events into start, development, result, and aftershock;
- preserve hard cuts when the inherited pressure is clear;
- reduce decorative bridges that carry only mood.

Safe repair must not:

- invent new scenes, events, witnesses, clues, folklore, or payoff;
- add symbolic bridges that override scene material;
- make every transition lyrical;
- explain all skipped time;
- turn every object into a continuity marker;
- change POV access or timeline to smooth a seam;
- update Notion, GitHub, or manuscript source without explicit permission.

## Transition audit

Use:

```text
SCENE TRANSITION / SKIPTIME / EVENT CLUSTER CHECK
SCOPE:
SOURCE USED:
SOURCE SURFACE:
FROM SCENE:
TO SCENE:
SEAM TYPE:
TRANSITION ANCHOR:
WHAT CARRIES OVER:
TIME SKIPPED:
PROCESS TRACE:
WHAT CONTINUED OFF-PAGE:
WHAT COOLED:
WHAT HEATED:
POV ACCESS AFTER CUT:
EMOTIONAL CONTINUITY:
OBJECT / MATERIAL CONTINUITY:
EVENT CLUSTER:
- START:
- DEVELOPMENT:
- RESULT:
- AFTERSHOCK:
SEAM BREAK RISK:
FAILURE LABELS:
SAFE REPAIR:
ROLE HANDOFF:
NEXT NODE:
```

## Patch rule

If exact source text is available:

```text
OLD:
SEAM FAILURE:
WHY THE TRANSITION / SKIPTIME / CLUSTER MISREADS:
NEW:
WHAT NOW CARRIES OVER:
PROCESS TRACE:
EVENT CLUSTER STATUS:
RISK:
```

If exact source text is missing, do not patch. Run Source Surface Check.

## Handoff

If the issue is event order or POV access, hand off to Timeline / POV / Foreshadowing / Folklore Check.

If the issue is promise/payoff or aftershock at beat level, hand off to Narrative Beat Escalation & Aftershock Check.

If the issue is material or sensory craft, hand off to Prose Craft / Style / Material Check.

If the issue is living-world residue or offscreen motion, hand off to Living World & Community Motion Check.

If the issue is chapter-level flow, hand off to Chapter Assembly & Split Check.

## Output labels

```text
SCENE_SEAM_OK
SCENE_SEAM_PARTIAL
TRANSITION_DECORATIVE_DETECTED
SKIPTIME_PROCESS_TRACE_MISSING
EVENT_CLUSTER_FRAGMENTED_DETECTED
OBJECT_RESET_DETECTED
SOURCE_SURFACE_REQUIRED
CANON_GAP_BLOCKED
```