# SLTD Context Capsule Calibration

These samples calibrate source-grounded context capsules, lore retrieval discipline, POV knowledge limits, hidden canon control, and safe routing.

They are not canon, not current manuscript, and not prose to imitate.

## 1. Chat memory cannot become current source

```text
BAD PATTERN:
The agent remembers that C030 was repaired last session and marks it ready.

WHY BAD:
- chat memory is not current source
- readiness needs current Notion source and pass trace
- a later edit may have changed the chapter

PREFERRED CALIBRATION:
SOURCE READ: current Notion C030, Chapter Card, relevant pass/status node
SOURCE NOT READ: none if verdict requested
SOURCE STATUS: current source verified
BLOCKED CONTEXT: chat memory summary
CAPSULE VERDICT: CONTEXT_CAPSULE_OK only after source read
PROSE PERMISSION: route to Readiness / Lock, not capsule verdict alone
```

## 2. Summary helps locate source but cannot replace it

```text
BAD PATTERN:
A chapter summary says Dai Phong kept a cold object, so the agent rewrites the next scene with the object in his sleeve.

WHY BAD:
- summary does not prove object handler, location, witness, or hidden status
- the next scene may depend on who saw it or whether it was left behind

PREFERRED CALIBRATION:
OBJECTS IN PLAY: cold object unknown until exact source read
MISSING SOURCE: previous chapter ending + next chapter opening
BLOCKED CONTEXT: summary claim treated as source
CAPSULE VERDICT: CONTEXT_CAPSULE_PARTIAL
NEXT NODE: Tracking / Logic Ledger after exact source read
```

## 3. Hidden canon must stay out of POV prose

```text
BAD PATTERN:
The agent knows from later outline that a relic is dangerous and writes the early-scene POV as if Dai Phong senses its true role.

WHY BAD:
- hidden canon leaks into character knowledge
- mystery turns into explanation
- future payoff loses pressure

PREFERRED CALIBRATION:
POV KNOWS: touch, cold, weight, witness behavior, local rumor if present
POV DOES NOT KNOW: relic identity, future function, later owner, payoff route
HIDDEN CANON LOCK: relic danger held back
ALLOWED CONTEXT: sensory pressure only
PROSE PERMISSION: do not name future function
```

## 4. Legacy Workdeck is not live manuscript unless named current

```text
BAD PATTERN:
The agent uses an older Workdeck chapter draft to decide the current Notion chapter status.

WHY BAD:
- legacy text may be stale
- current Notion is live manuscript state
- old draft can create false canon conflict

PREFERRED CALIBRATION:
SOURCE STATUS: Workdeck = legacy reference unless user names it current
SOURCE NOT READ: current Notion chapter
CAPSULE VERDICT: SOURCE_NOT_READ_EVIDENCE_MISSING for current verdict
SAFE CLAIM NOW: legacy draft contains X; current status unknown
NEXT NODE: read current Notion chapter
```

## 5. Capsule must stay compact

```text
BAD PATTERN:
The agent builds a full encyclopedia of the arc before editing one 700-word scene.

WHY BAD:
- context bloat hides the scene pressure
- irrelevant lore increases hallucination risk
- later gates lose the smallest safe route

PREFERRED CALIBRATION:
SCOPE: one scene
ACTIVE CHARACTERS: only characters physically present or directly constraining the scene
OBJECTS IN PLAY: only objects touched, hidden, paid, watched, or moved in the scene
THREADS ACTIVE: only threads that affect this scene's choice, cost, or reveal limit
CAPSULE VERDICT: compact and task-local
```

## 6. Capsule is not a readiness verdict

```text
BAD PATTERN:
The capsule has no missing source, so the agent marks the chapter Publication Lock.

WHY BAD:
- capsule only bounds context
- readiness needs exact prose surface, pass trace, blockers, and publication criteria

PREFERRED CALIBRATION:
CAPSULE VERDICT: CONTEXT_CAPSULE_OK
PROSE PERMISSION: route allowed
NEXT NODE: Vietnamese Senior Editor Surface + Tracking / Logic Ledger + Readiness / Lock
```

## 7. Source conflict must not be merged silently

```text
BAD PATTERN:
Scene Packet says A Quý is absent, current prose has him present, and the agent averages the two by leaving him silent in the room.

WHY BAD:
- presence affects dialogue, witness, relationship memory, and downstream knowledge
- silence may become false staging

PREFERRED CALIBRATION:
SOURCE STATUS: current prose conflicts with Scene Packet
ACTIVE CHARACTERS: unresolved
MISSING SOURCE: current decision source or user confirmation
CAPSULE VERDICT: CONTEXT_CAPSULE_BLOCKED
NEXT NODE: Source Preflight / Structural Spine before Voice Gate
```
