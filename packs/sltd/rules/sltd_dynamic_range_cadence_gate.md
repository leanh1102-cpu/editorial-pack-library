# SLTD Dynamic Range & Cadence Gate

This gate prevents excessive restraint from flattening scene rhythm, conflict, payoff, and reader pull.

It protects dynamic range: quiet pressure, controlled escalation, scene turn, and aftershock.

## Core rule

Restraint is not flattening.

```text
RESTRAINT = hold back what should not be revealed yet
PRESSURE = make the room, body, relation, object, or choice tighten
ESCALATION = let the scene gain force when its function requires a turn
```

A scene may keep lore quiet while still increasing pressure through action, cost, silence, body, object, or relation.

## Use when

- AI edits make everything calmer, cleaner, and flatter;
- a discovery, turn, or choice loses force;
- dialogue becomes polite, complete, or defanged;
- a scene is correct but the turn is removed;
- every paragraph has the same safe cadence;
- line edit makes prose smoother but not sharper;
- the user says restraint, moderation, subtlety, or anti-melodrama has gone too far.

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

It must not add canon, change locked outcome, or turn every scene into a high-force scene.

## Intensity target by scene function

Use target intensity by scene function:

```text
1-2 = connective / decompression / aftermath scene
3 = regular pressure scene
4 = cluster turn / discovery-adjacent / irreversible social shift
5 = major turn / major reveal / irreversible choice / signature chapter beat
```

Do not force every scene to 2-3.

Do not force every scene to 4-5.

Match intensity to scene function.

## Cadence check

A scene may use some of these beats:

```text
quiet pressure
interruption
tightening
wrong relief
turn
peak emphasis
aftershock
```

Not every scene needs every beat.

A scene with a strong function must have at least one clear tightening or turn and at least one visible consequence or aftershock.

## Quiet material / stronger pressure

Always separate:

```text
WHAT MUST STAY QUIET:
- unrevealed lore
- hidden motive
- canon secret
- future payoff
- emotion the page has not earned

WHAT NEEDS STRONGER PRESSURE:
- object pressure
- relation pressure
- physical cost
- choice cost
- interruption
- silence after a turn
- practical consequence
```

A good SLTD scene can hide explanation while increasing pressure.

## Failure labels

Use these labels when auditing or patching:

```text
OVER_RESTRAINT
FLATTENED_CADENCE
TURN_REMOVED
CONFLICT_SOFTENED
DIALOGUE_DEFANGED
COST_MUTED
PAYOFF_UNDERCUT
CLEAN_BUT_NOT_SHARP
QUIET_BUT_NOT_PRESSURED
WRONG_SCENE_INTENSITY_TARGET
AFTERSHOCK_MISSING
```

## Safe escalation

Safe escalation may:

- sharpen cost already seeded;
- make an existing object interfere with action;
- make a character fail to answer or answer late;
- let dialogue snap, evade, interrupt, or mishear;
- add a small consequence with source basis;
- preserve mystery while making the room harder to manage;
- add aftershock through silence, delayed task, broken object, debt, illness, animal reaction, or changed body behavior.

Safe escalation must not:

- add new lore;
- add new power;
- add new named character;
- change locked outcome;
- reveal hidden canon early;
- turn every beat into melodrama;
- overwrite source surface.

## Dynamic range audit

Check:

```text
SCENE FUNCTION:
TARGET INTENSITY:
CURRENT INTENSITY:
CADENCE:
TURN / PEAK EMPHASIS:
AFTERSHOCK:
WHAT MUST STAY QUIET:
WHAT NEEDS STRONGER PRESSURE:
OVER-RESTRAINT RISK:
SAFE ESCALATION:
DO NOT ADD:
```

## Patch rule

For local patch:

```text
OLD:
PROBLEM LABEL:
WHY IT FLATTENS:
NEW:
WHAT STAYS QUIET:
WHAT GAINS PRESSURE:
RISK:
```

If exact source text is missing, do not patch. Run source surface check.

## Handoff

If dynamic range fails but source is not available, hand off to Source Surface Check.

If story function is unclear, hand off to Story Doctor.

If pressure exists but line rhythm is flat, hand off to Vietnamese Line Editor or Line Surgery.

If the scene is clean but not sharp, hand off to Intensity Editor.

## Output labels

```text
DYNAMIC_RANGE_OK
DYNAMIC_RANGE_PARTIAL
OVER_RESTRAINT_DETECTED
CADENCE_FLATTENED
SAFE_ESCALATION_CANDIDATE
SOURCE_SURFACE_REQUIRED
```
