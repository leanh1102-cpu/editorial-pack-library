# SLTD Agent-Native Context Memory Lifecycle & ByteRover Discipline

This rule adapts ByteRover-style agent-native hierarchical memory lessons for SLTD editorial work.

It governs how context briefs, handoff items, node ledgers, source-status notes, feedback deltas, author-style notes, risk notes, and route decisions may be retained, reused, updated, or deprecated.

## Core rule

No context entry without provenance.

No stale handoff as current source.

No GitHub live manuscript memory.

This is a context-memory lifecycle discipline. It is not source authority, not canon authority, not a rewrite role, not readiness, and not Publication Lock.

## Use when

- the task depends on prior handoff, session memory, context brief, node ledger, route decision, author-style note, feedback delta, topic map, readiness note, or risk note;
- the user asks for handoff, current context, source status, what the AI remembers, or whether prior claims still apply;
- a context item may be stale, legacy, inferred, compressed, or superseded by current Notion source;
- the agent needs to decide whether to keep, update, deprecate, or block a memory-like item;
- a prior rule/result should guide routing but must not become source truth.

## Authority

Run after:

```text
source preflight when current source or source-status claim is in scope
multilingual long-context retrieval when the memory item depends on found/not-found/aggregation evidence
context capsule when hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, reveal timing, or long-range continuity is in scope
narrative claim verification when a memory item contains a factual/status/canon/continuity claim
comparative editorial feedback delta when user feedback has been converted into a reusable delta
```

Run before:

```text
using a prior handoff as active context
using a context brief to route current work
claiming current status, Human Chapter Pass, Publication Lock, canon state, packet readiness, or source absence from memory
creating a new session handoff
turning a prior decision into current instruction
```

## Required distinction

```text
LIVE SOURCE = current Notion source or current user-provided packet
CONTEXT ENTRY = compressed memory-like item used for routing or handoff
PROVENANCE = where the entry came from and when/why it was created
MATURITY = RAW / CHECKED / STABLE / DEPRECATED / BLOCKED
RECENCY = whether the entry is current enough for the requested task
SOURCE-TRUTH LIMIT = what the entry may not prove without re-reading source
RELATION = linked source node, rule node, feedback delta, claim, risk, route, or handoff item
```

A context entry may guide routing. It may not replace current source.

## Entry types

```text
CLAIM
DECISION
HANDOFF
ROUTE
STYLE
CANON
STATUS
FEEDBACK
RISK
TOPIC / THREAD
QUALITY
READINESS
SOURCE MAP
```

## Output schema

```text
SLTD CONTEXT MEMORY LIFECYCLE CHECK
SCOPE:
CONTEXT ENTRY:
SOURCE USED:
SOURCE STATUS:
PROVENANCE:
ENTRY TYPE: CLAIM / DECISION / HANDOFF / ROUTE / STYLE / CANON / STATUS / FEEDBACK / RISK / TOPIC / QUALITY / READINESS / SOURCE MAP
MATURITY: RAW / CHECKED / STABLE / DEPRECATED / BLOCKED
RECENCY:
RELATIONS:
RETRIEVAL USE:
MUST RE-READ BEFORE:
SOURCE-TRUTH LIMIT:
STALE MEMORY RISK:
SEMANTIC DRIFT RISK:
DECISION: KEEP / UPDATE / DEPRECATE / BLOCK
BLOCKERS:
NEXT NODE:
```

## Maturity rules

```text
RAW = captured from chat, handoff, draft, or partial source; not safe as source truth
CHECKED = anchored to source at the time of checking, but may become stale
STABLE = rule-level, author-taste, or project policy item that remains valid unless superseded
DEPRECATED = contradicted, superseded, invalidated, legacy, or no longer current
BLOCKED = cannot be used because provenance, source, scope, or status is missing
```

Only current source or explicitly current user packet can support current manuscript status.

## Recency rules

Mark stale risk when:

- the entry came from chat memory;
- the entry came from an old handoff;
- the source has likely changed;
- Notion current was not read for current-status work;
- Workdeck or legacy Google Docs are being treated as current;
- an AI verdict was later invalidated by human read;
- the entry contains readiness, lock, pass, canon, or source absence claims.

## Hierarchy rule

A safe context memory may be organized as:

```text
DOMAIN -> TOPIC -> SUBTOPIC -> ENTRY
```

For SLTD this is only a conceptual organization inside reports, handoffs, or rule memory. Do not create a new database, graph, vector index, project board, workflow, or manuscript copy.

## Source-truth limits

Context entries cannot prove:

```text
current Notion status
Human Chapter Pass
Publication Lock
canon conflict absence
packet readiness
exact prose quality
object state in current manuscript
scene source fidelity
```

unless current source or user-provided packet is read and cited in the current task.

## Blockers

```text
provenance missing
source missing when current/source claim is in scope
context entry treated as source truth
legacy source treated as current without instruction
stale handoff used as current status
maturity label unsupported
recency risk hidden
semantic drift risk unexamined
memory would copy live manuscript into GitHub
memory would create database/workflow/report artifact
```

## Failure labels

```text
CONTEXT_MEMORY_READY
CONTEXT_MEMORY_PARTIAL
CONTEXT_MEMORY_BLOCKED
PROVENANCE_REQUIRED
STALE_HANDOFF_RISK
CHAT_MEMORY_SOURCE_TRUTH_RISK
LEGACY_SOURCE_AS_CURRENT_RISK
MATURITY_UNSUPPORTED
SEMANTIC_DRIFT_RISK
SOURCE_RECHECK_REQUIRED
NO_GITHUB_LIVE_MANUSCRIPT_MEMORY
```

## Safe repair

Safe repair may:

- mark provenance;
- mark maturity and recency;
- separate current source, old source, inference, and recommendation;
- deprecate stale handoff items;
- create a bounded handoff summary;
- recommend source re-read, claim verification, retrieval check, context capsule, or readiness route.

Safe repair must not:

- store live manuscript text in GitHub;
- create vector database, graph database, workflow, project board, automation, report file, or new Notion database;
- treat chat memory as current source;
- hide stale risk;
- update Notion, GitHub, Google Docs, or manuscript source unless explicitly asked.

## Output labels

```text
CONTEXT_MEMORY_READY
CONTEXT_MEMORY_NEEDS_PROVENANCE
CONTEXT_MEMORY_NEEDS_SOURCE
CONTEXT_MEMORY_BLOCKED
KEEP_CONTEXT_ENTRY
UPDATE_CONTEXT_ENTRY
DEPRECATE_CONTEXT_ENTRY
SOURCE_RECHECK_HANDOFF
CLAIM_VERIFICATION_HANDOFF
RETRIEVAL_HANDOFF
```