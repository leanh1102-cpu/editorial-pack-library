# SLTD Pack Design

This file is the architecture contract for the SLTD pack.

## Purpose

The pack helps the agent read the right source, preserve exact source surface, keep Entry as a router, enforce structural spine, tracking, character voice/dialogue/location staging, Vietnamese surface/pass integrity, and produce matrix-style multi-chapter feedback without losing evidence discipline.

## Source of truth

```text
Notion = live manuscript state
GitHub = editorial rules and routing memory
User instruction = current task and final authority for writes
```

## Runtime loop

```text
boot_task
source_preflight
task_intake
task_router
source surface check when exact source may be missing
structural spine outline pre-prose check when outline/card/packet/border is in scope
tracking logic ledger check when state, knowledge, object, residue, thread, pass trace, downstream risk, or verify target is in scope
character voice dialogue staging check when dialogue, relationship memory, multi-character presence, location staging, or tone integrity is in scope
vietnamese senior editor surface check when exact Vietnamese surface, semantic load, pass metadata, or readiness trust is in scope
general chapter feedback matrix check when packet/arc review needs both global feedback and chapter-specific actions
node_checkpoint
result_report
```

Use the smallest route that answers the request.

## Voice / dialogue / staging model

```text
CHARACTER_VOICE = how a character speaks: sentence length, word choice, address terms, omissions, work habit, fear, warmth, guardedness, power, age, and relationship pressure
DIALOGUE_WEIGHT = whether a line carries weight proportional to who says it and what they carry now
RELATIONSHIP_MEMORY = prior shared events showing up in speech, silence, help, avoidance, address, or interruption
PRESENCE_TRACE = who is present in a multi-character scene and why each person speaks, stays silent, or reacts
LOCATION_STAGE = concrete layout and material stage of the scene
USABLE_OBJECTS = objects characters can touch, move, hide, use, pay with, lean on, or avoid
```

Dialogue is not information delivery. Silence is not absence. Location is not backdrop. For SLTD, sound and physical detail should use natural Vietnamese prose, not forced comic-style effects.

## Feedback matrix model

```text
GENERAL_FEEDBACK = packet/story-level critique: spine, tracking, protagonist route, supernatural residue, Vietnamese surface, pass integrity, readiness risk
CHAPTER_FEEDBACK = chapter-specific feedback tied to chapter number, current status, core function, blockers, and next action
SOURCE_STATUS = whether current source was read, partial, missing, or blocked
REVIEW_VERDICT = ready / partial / blocked / source missing / tracking blocked / surface blocked
```

The matrix is an output protocol, not a substitute for evidence. General feedback must frame chapter feedback. Chapter feedback must not ignore global blockers.

## Source fidelity model

```text
SOURCE TEXT > TRACKING SURFACE > STRUCTURAL SOURCE > DERIVED DIGEST > CHAT MEMORY
```

Exact prose, readiness, lock verdict, structural spine, tracking logic, character voice/staging, Vietnamese surface, pass integrity, feedback matrix source status, supernatural residue, and protagonist route require the right source surface.

## Invariants

- Notion is live manuscript state.
- GitHub is editorial memory and rules.
- User instruction outranks the pack.
- No canon invention.
- No source write without clear user request.
- No readiness claim without evidence.
- Stop at the first real blocker.
- Matrix output must show source used, source status, evidence check, and next node.
- Do not use formal pass labels as readiness proof.
- Logic continuity verdict requires current tracking surface.
- Character voice and relationship verdicts require current source surface or character/source notes.
- Exact Vietnamese surface verdict requires exact prose.
- Scene is the edit unit; chapter is the reader unit.
