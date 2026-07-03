# SLTD Multilingual Long-Context Source Retrieval & OneRuler Discipline

This rule adapts OneRuler-style multilingual long-context retrieval lessons for SLTD editorial work.

It checks whether the agent has actually retrieved the relevant Vietnamese source evidence before making found, not-found, absence, aggregation, canon, status, topic, quality, or readiness-adjacent claims across long manuscript context.

## Core rule

No absence claim without source check.

No not-found verdict from compressed source alone.

This is a retrieval and absence discipline. It is not canon authority, not readiness, not Publication Lock, not a detector, and not a rewrite role.

## Use when

- the user asks whether a motif, object state, thread, phrase, canon item, status field, Human Chapter Pass, Publication Lock, clue, event, voice pattern, or AI-smell pattern exists in a long source;
- the scope spans multiple scenes, chapters, packets, arcs, parts, or current Notion source nodes;
- the task requires a negative claim such as no conflict, not found, absent, missing, never appears, not mentioned, or no evidence;
- the task requires aggregation across long Vietnamese source;
- topic/thread discovery, claim verification, POLARIS quality check, readiness, canon lock, packet review, or source-status review depends on retrieval over long context;
- English rule memory or English prompt instructions are being applied to Vietnamese manuscript source.

## Authority

Run after:

```text
source preflight
source surface when exact text or status field is required
context capsule when current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, reveal timing, or long-range continuity is in scope
```

Run before:

```text
narrative claim verification when the claim depends on source retrieval
corpus topic / thread discovery when source assignment or motif/thread map depends on long-context search
reference-anchored longform story quality when quality depends on Must Show/source preservation
readiness or lock route when current status fields or absence of blockers are in scope
canon conflict verdict
packet/arc aggregation verdict
```

## Required distinction

```text
FOUND = target located with source segment and evidence anchor
NOT FOUND = target not found only after declared source segments were checked with adequate coverage
UNCERTAIN = source coverage, target definition, language, context length, or aggregation method is insufficient
BLOCKED = required current source, source surface, or scope is missing
ABSENCE CLAIM = claim that something does not appear, does not exist, is not present, or has no evidence
AGGREGATION CLAIM = claim that summarizes repeated or distributed evidence across many source segments
```

Do not collapse `UNCERTAIN` into `NOT FOUND`.

## Source and language requirements

Track:

```text
SOURCE LANGUAGE
INSTRUCTION LANGUAGE
CONTEXT LENGTH TIER
SOURCE SEGMENTS CHECKED
RETRIEVAL TARGET
TARGET TYPE
EVIDENCE ANCHORS
```

For SLTD, Vietnamese source may contain xưng hô, implicit relation, elliptical dialogue, object-state cues, folklore fragments, and status fields. English summaries do not replace Vietnamese source.

## Target types

```text
EXACT PHRASE
CANON CLAIM
STATUS FIELD
OBJECT STATE
POV KNOWLEDGE
RELATIONSHIP MEMORY
THREAD
MOTIF
REVEAL / FORESHADOWING
VOICE / DIALOGUE PATTERN
AI-SMELL PATTERN
ABSENCE CLAIM
AGGREGATION
```

## Output schema

```text
SLTD MULTILINGUAL LONG-CONTEXT SOURCE RETRIEVAL CHECK
SCOPE:
SOURCE USED:
SOURCE STATUS:
SOURCE LANGUAGE:
INSTRUCTION LANGUAGE:
CONTEXT LENGTH TIER:
RETRIEVAL TARGET:
TARGET TYPE:
SOURCE SEGMENTS CHECKED:
EVIDENCE ANCHORS:
FOUND:
NOT FOUND:
UNCERTAIN:
ABSENCE CLAIM STATUS: ALLOWED / NOT ALLOWED / UNCERTAIN
AGGREGATION REQUIRED: YES / NO
AGGREGATION METHOD:
CROSS-LINGUAL RISK:
TOKENIZATION / LENGTH RISK:
VERDICT: FOUND / NOT FOUND / UNCERTAIN / BLOCKED
BLOCKERS:
NEXT NODE:
```

## Absence claim rules

An absence claim is allowed only when:

- scope is explicit;
- current source or user-provided source packet was read as required;
- source segments checked are listed;
- target definition is clear enough to search or inspect;
- compressed source is not the only evidence;
- long-context risk is acknowledged;
- aggregation risk is handled when the target may be distributed.

Write `ABSENCE CLAIM STATUS: NOT ALLOWED` when the agent has only summary, chat memory, old Workdeck, partial excerpt, compressed source, or unspecified source coverage.

## Aggregation rules

Aggregation claims require packeted or segmented checking.

For large scope, split by:

```text
scene
chapter
packet
arc
part
source node
```

Do not claim a global pattern from a few salient examples. Do not claim no pattern because only one segment was checked.

## Cross-lingual risk rules

Mark cross-lingual risk when:

- instruction language differs from source language;
- evidence is translated before checking;
- a Vietnamese term, xưng hô, idiom, dialogue particle, status label, or folklore phrase may not match English query terms;
- long-context evidence is found through English summary rather than Vietnamese source.

Safe repair may include bilingual target expansion, Vietnamese keyword variants, source-node split, and anchor-first reporting.

## Blockers

```text
source missing
current source required but unread
scope missing
target undefined
source segments not listed
exact text/status needed but source surface not read
compressed source only
chat-memory-only retrieval
legacy Workdeck used as current without instruction
aggregation required but not segmented
absence claim requested but coverage insufficient
language mismatch risk unhandled
```

## Failure labels

```text
LONG_CONTEXT_RETRIEVAL_READY
LONG_CONTEXT_RETRIEVAL_PARTIAL
LONG_CONTEXT_RETRIEVAL_BLOCKED
FOUND_WITH_ANCHOR
NOT_FOUND_ALLOWED
NOT_FOUND_NOT_ALLOWED
ABSENCE_CLAIM_BLOCKED
COMPRESSED_SOURCE_ONLY_RISK
CHAT_MEMORY_RETRIEVAL_RISK
LEGACY_SOURCE_AS_CURRENT_RISK
AGGREGATION_WITHOUT_SEGMENTS
CROSS_LINGUAL_RETRIEVAL_RISK
TOKENIZATION_LENGTH_RISK
VIETNAMESE_SOURCE_NOT_CHECKED
```

## Safe repair

Safe repair may:

- narrow scope;
- split large source into nodes;
- request current Notion source or exact packet;
- list checked source segments;
- expand Vietnamese target variants;
- return FOUND / NOT FOUND / UNCERTAIN separately;
- hand off to Claim Verification, Corpus Topic / Thread Discovery, POLARIS quality check, Readiness, or Editorial Director.

Safe repair must not:

- invent evidence;
- infer absence from silence in summary;
- use English summary as Vietnamese source;
- call readiness, Human Chapter Pass, or Publication Lock;
- create scripts, workflows, reports, issues, boards, databases, automations, or live manuscript copies.

## Output labels

```text
LONG_CONTEXT_RETRIEVAL_READY
LONG_CONTEXT_RETRIEVAL_NEEDS_SOURCE
LONG_CONTEXT_RETRIEVAL_NEEDS_SCOPE
LONG_CONTEXT_RETRIEVAL_NEEDS_TARGET
LONG_CONTEXT_RETRIEVAL_BLOCKED
FOUND_WITH_ANCHOR
ABSENCE_CLAIM_NOT_ALLOWED
CLAIM_VERIFICATION_HANDOFF
TOPIC_DISCOVERY_HANDOFF
READINESS_HANDOFF
```