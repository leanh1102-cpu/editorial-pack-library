# SLTD Tracking, Logic Ledger & Traceability Protocol

This gate prevents scene/chapter edits from breaking accumulated logic across SLTD.

It is a traceability gate. It does not create project-management systems. It records and checks only the logic needed to keep act, arc, chapter, scene, object, residue, knowledge, thread, pass, and change-state continuity coherent.

## Core rule

No prose change without tracking impact.

Before drafting, rewriting, line editing, readiness checking, or locking a scene/chapter, the agent must know what logic state the task touches and where that logic is tracked.

```text
TRACKING_SURFACE = the current source node(s) that hold traceable logic: Story Outline, Chapter by Chapter Outline, Chapter Index, Scene Bank, Chapter Card, Plot Threads, canon index, Notes, comments, or source excerpt
LOGIC_LEDGER = a compact record of state before/after, who knows what, what object/residue/thread is open, held, paid, retired, or changed
STATE_TRACE = before state -> after state for body, family, house, debt, name, paper, route, object, witness, rumor, power, and relation
KNOWLEDGE_TRACE = what Dai Phong knows, what adults know, what village/community knows or misreads, what reader suspects, and what must remain hidden
OBJECT_TRACE = when a material object appears, changes function, is hidden, witnessed, paid off, retired, or remains open
THREAD_TRACE = plant / hold / pay / retire status for foreshadowing, folklore, residue, clue, social pressure, and protagonist method
CHANGE_TRACE = what an edit changes and what downstream source nodes must be checked afterward
VERIFY_TARGET = exact source node, text, property, or note that must be checked after a write or patch
```

Do not rely on chat memory for tracking.

Do not let a later prose improvement erase earlier logic.

Do not treat a green pass as logic continuity.

## Use when

- the user asks for tracking, logic, ledger, continuity, traceability, status trace, state trace, knowledge trace, object trace, thread trace, payoff, open loop, or downstream risk;
- a rewrite, line edit, or repair touches an object, residue, clue, name, debt, paper, route, witness, rumor, family state, body state, or pass status;
- a chapter/packet/arc review needs readiness, lock, or publication verdict;
- a source note, property, comment, or user instruction conflicts with another status source;
- a chapter has many correct gates but continuity across chapters may be broken;
- a scene card is correct but the edit may change who knows what, what is paid off, or what remains open;
- the task involves long-range SLTD continuity over more than one scene.

## Authority

This gate does not authorize new databases, project boards, workflows, scripts, reports, automation files, or live manuscript copies in GitHub.

This gate does not invent logic, canon, object function, thread payoff, or downstream dependency.

If tracking surface is missing and current logic status is required, stop with TRACKING_SURFACE_MISSING.

If an exact write is requested, source surface and verify target are required.

## Tracking / Logic Ledger schema

```text
TRACKING / LOGIC LEDGER CHECK
SCOPE:
SOURCE USED:
TRACKING SURFACE:
UNIT:
CURRENT STRUCTURAL SLOT:
BEFORE STATE:
AFTER STATE:
KNOWLEDGE STATE:
OBJECTS TRACKED:
RESIDUES TRACKED:
THREADS PLANTED:
THREADS HELD:
THREADS PAID:
THREADS RETIRED:
OPEN DEBTS:
CLOSED DEBTS:
CANON IN:
CANON OUT:
STATUS / PASS TRACE:
CHANGE IMPACT:
DOWNSTREAM RISK:
VERIFY TARGET:
TRACKING VERDICT:
PROSE PERMISSION:
NEXT NODE:
```

## Required ledger layers

Use only layers relevant to the task. Do not inflate the ledger.

```text
STRUCTURAL_LEDGER = act / arc / hồi / chapter / scene function and current slot
STATE_LEDGER = before -> after state for body, family, house, debt, name, route, resource, witness, paper, relation
KNOWLEDGE_LEDGER = who knows / hides / misreads / suspects / must not know
OBJECT_RESIDUE_LEDGER = material object or supernatural residue appearance, state, handler, witness, open payoff
THREAD_PAYOFF_LEDGER = plant / hold / pay / retire status and next return
STATUS_PASS_LEDGER = Anti-AI Pass, Vietnamese Reader Pass, Human Chapter Pass, Publication Lock, notes, comments, user instruction conflicts
CHANGE_TRACE_LEDGER = exact patch/change impact and verify target
```

## Logic check rules

A prose task is blocked when:

```text
tracking surface is missing for the requested logic claim
before/after state is unclear
knowledge state is unclear
object/residue/thread status is unclear
open debt/payoff is untracked
status/pass trace conflicts and readiness is requested
downstream dependency may be affected but not identified
verify target is missing for write/patch
```

## Workdeck inheritance rule

Older Workdeck rules already required reading rules, locating the right tab, reading the right scope, running a pass, writing only into the right region, and verifying exact text after writing. This protocol imports that discipline into Entry as logic traceability, not as a new workflow system.

The agent must be able to say:

```text
what was read
what was changed or not changed
what logic state moved
where the change should be verified
what remains open
```

If it cannot, it must report NOT VERIFIED or TRACKING_SURFACE_MISSING.

## Failure labels

```text
TRACKING_SURFACE_MISSING
LOGIC_LEDGER_MISSING
STATE_CHANGE_UNTRACKED
KNOWLEDGE_STATE_UNCLEAR
OBJECT_LEDGER_MISSING
RESIDUE_LEDGER_MISSING
THREAD_STATUS_UNCLEAR
PAYOFF_DEBT_UNTRACKED
DOWNSTREAM_DEPENDENCY_MISSED
PASS_TRACE_CONFLICT
CHANGE_TRACE_MISSING
VERIFY_TARGET_MISSING
LOGIC_LEDGER_FALSE_CONFIDENCE
CHAT_MEMORY_TRACKING_RISK
GREEN_PASS_WITHOUT_LOGIC_TRACE
EDIT_BREAKS_PRIOR_STATE
EDIT_BREAKS_DOWNSTREAM_STATE
```

## Safe repair

Safe repair may:

- create a compact ledger from existing current source;
- identify missing tracking surfaces;
- list open logic debts before prose;
- mark which object/thread/residue/status needs verification;
- propose a Notion update candidate for existing Story Outline, Chapter by Chapter Outline, Chapter Index, Scene Bank, Chapter Card, Plot Threads, or Notes;
- block prose until state/knowledge/thread tracking is clear.

Safe repair must not:

- create new tracking databases or management systems;
- invent missing logic states, canon, payoffs, clues, witnesses, or source status;
- rewrite prose from ledger only;
- hide unresolved conflict by marking tracking OK;
- add tracking notes to live sources without explicit user write instruction.

## Output labels

```text
TRACKING_LEDGER_OK
TRACKING_LEDGER_PARTIAL
TRACKING_SURFACE_MISSING
LOGIC_TRACE_BLOCKED
PROSE_PERMISSION_GRANTED
PROSE_PERMISSION_BLOCKED
VERIFY_TARGET_REQUIRED
NOT_VERIFIED
```