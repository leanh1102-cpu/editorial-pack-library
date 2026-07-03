# SLTD Context Capsule & Lore Retrieval Discipline Protocol

This gate prevents long-form SLTD work from using memory, summaries, legacy drafts, or plausible lore as if they were current source.

It adapts memory/lorebook/context-retrieval discipline for SLTD without creating an autonomous lore system, database, workflow, script, report, project board, or live manuscript copy in GitHub.

## Core rule

Do not retrieve context to replace source.

Before drafting, rewriting, reviewing, readiness checking, or locking a scene/chapter, the agent must build only the smallest source-grounded capsule needed for the task.

```text
CONTEXT_CAPSULE = compact task-local context extracted from source nodes read in the current run
LORE_RETRIEVAL = finding relevant canon/status/thread/source nodes before judgment; not inventing or updating lore
ALLOWED_CONTEXT = facts, states, objects, relationships, locations, constraints, and hidden information explicitly present in the source read
BLOCKED_CONTEXT = chat memory, likely continuity, legacy workdeck material, raw drafts, old summaries, or external references that have not been named as current source
POV_KNOWLEDGE = what the active POV can know, infer, misread, hide, or not know at this point
HIDDEN_CANON_LOCK = canon or future information that may guide review but must not leak into prose or verdict unless the current source grants access
PROSE_PERMISSION = whether the capsule is sufficient to proceed to spine, tracking, voice/staging, rewrite, line edit, or readiness review
```

A capsule is a routing and source-discipline artifact. It is not a new canon source.

## Use when

- the user asks for current/latest status, Notion current source, lock, readiness, Publication Lock, Human Chapter Pass, packet verdict, canon conflict, or source status;
- the task spans more than one scene/chapter or depends on long-range continuity;
- rewrite, line edit, or review depends on who knows what, hidden information, object location, debt, injury, relationship state, route state, residue, folklore, clue, or thread status;
- a scene packet, chapter card, outline, chapter index, plot thread, comment, note, or current source node must be reconciled before prose;
- the agent is tempted to use memory, summary, raw draft, legacy workdeck, or plausible lore to bridge a gap;
- another gate needs a bounded context object before running.

## Authority

This gate does not authorize new canon, autonomous lore updates, source writes, database creation, workflow creation, report generation, project boards, scripts, automations, or live manuscript copies in GitHub.

This gate may identify relevant source nodes, compact what was read, mark missing source, and propose a NOTION UPDATE CANDIDATE for existing Notion nodes.

If current status is requested and current Notion source was not read or provided, stop with:

```text
SOURCE NOT READ / EVIDENCE MISSING
```

If the capsule cannot be grounded in source, stop with:

```text
CONTEXT_CAPSULE_BLOCKED
```

## Source priority

Use current source priority exactly:

```text
1. Current user instruction
2. Current Notion live source
3. User-provided current scene/chapter packet
4. GitHub SLTD editorial pack
5. Core job packet
6. Core Vietnamese prose rules
7. Legacy Google Docs / Workdecks only when explicitly named or clearly marked as current
```

Do not treat raw drafts, older Workdecks, summaries, or chat memory as live manuscript state unless the user explicitly names them as current source.

## Context Capsule schema

```text
CONTEXT CAPSULE PREFLIGHT
SCOPE:
REQUEST TYPE:
REVIEW MODE:
SOURCE READ:
SOURCE NOT READ:
SOURCE STATUS:
UNIT:
CURRENT STRUCTURAL SLOT:
ACTIVE CHARACTERS:
POV:
POV KNOWS:
POV DOES NOT KNOW:
READER KNOWS / SUSPECTS:
HIDDEN CANON LOCK:
LOCATION STATE:
OBJECTS IN PLAY:
BODY / INJURY STATE:
RESOURCE / DEBT STATE:
RELATIONSHIP STATE:
RESIDUE / FOLKLORE STATE:
THREADS ACTIVE:
THREADS HELD BACK:
THREADS PAID / RETIRED:
CANON IN:
CANON OUT:
ALLOWED CONTEXT:
BLOCKED CONTEXT:
DOWNSTREAM RISK:
MISSING SOURCE:
CAPSULE VERDICT:
PROSE PERMISSION:
NEXT NODE:
```

Use only fields that matter to the task. Do not inflate the capsule.

## Retrieval rules

1. Build the capsule after Source Preflight and before Spine Lock, Tracking / Logic Ledger, Voice / Dialogue / Staging, Rewrite, Line Edit, Feedback Matrix, or Readiness.
2. Read exact current source when the user asks for current/latest/Notion/lock/readiness/canon conflict.
3. Use summaries only to locate source, never to replace exact source.
4. Separate fact, inference, and recommendation when source is partial.
5. Mark hidden canon as held-back context. Do not leak it into POV prose.
6. Mark legacy source as legacy unless the user says it is current.
7. Do not merge conflicting source states. Report the conflict and next source needed.
8. Do not use the capsule to solve missing structure. Hand off to Structural Spine / Borderbound when spine or scene function is unclear.
9. Do not use the capsule to solve missing logic. Hand off to Tracking / Logic Ledger when state, knowledge, object, thread, or downstream risk is affected.
10. Do not use the capsule to solve missing voice or staging. Hand off to Voice / Dialogue / Staging when characters, silence, relationship, or location stage is vague.

## Prose permission

Prose is blocked when:

```text
current source is required but not read
source status is unclear
POV knowledge is unclear
hidden canon may leak
object/location/body/debt state is unclear
relationship state is invented or assumed
thread status is inferred from memory
legacy source conflicts with current source
scene packet or chapter card is required but missing
canon conflict lacks current decision
```

Prose may proceed only when the capsule identifies the allowed context and the next relevant gate grants permission.

## Failure labels

```text
CONTEXT_CAPSULE_OK
CONTEXT_CAPSULE_PARTIAL
CONTEXT_CAPSULE_BLOCKED
SOURCE_NOT_READ_EVIDENCE_MISSING
CURRENT_NOTION_REQUIRED
LEGACY_SOURCE_RISK
CHAT_MEMORY_CONTEXT_RISK
SUMMARY_REPLACES_SOURCE
HIDDEN_CANON_LEAK_RISK
POV_KNOWLEDGE_UNCLEAR
OBJECT_STATE_UNCLEAR
LOCATION_STATE_UNCLEAR
RELATIONSHIP_STATE_UNCLEAR
THREAD_STATUS_UNCLEAR
CANON_CONFLICT_UNRESOLVED
SCENE_PACKET_REQUIRED
CHAPTER_CARD_REQUIRED
PROSE_PERMISSION_BLOCKED
```

## Safe repair

Safe repair may:

- reduce the scope to one scene, one chapter, one packet, one source node, or one thread;
- list the exact source nodes that must be read next;
- build a partial capsule from provided source and mark missing fields;
- return NOTION UPDATE CANDIDATE for an existing Chapter Card, Scene Bank, Chapter Index, Plot Thread, Notes, or comment;
- route to Tracking / Logic Ledger, Structural Spine, Voice / Dialogue / Staging, Vietnamese Senior Editor Surface, or Readiness.

Safe repair must not:

- invent source state, canon, hidden knowledge, object placement, relationship history, location layout, thread payoff, or pass status;
- create a new project-management layer;
- write to Notion, GitHub, Google Docs, or any source file without explicit user write instruction;
- mark readiness from capsule alone;
- rewrite prose from capsule alone when exact source surface is required.

## Output labels

```text
CAPSULE_READY
CAPSULE_PARTIAL
CAPSULE_BLOCKED
SOURCE_REQUIRED
NOTION_UPDATE_CANDIDATE
NEXT_NODE_REQUIRED
PROSE_PERMISSION_GRANTED
PROSE_PERMISSION_BLOCKED
```
