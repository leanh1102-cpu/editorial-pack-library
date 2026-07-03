# SLTD Corpus Topic / Thread Discovery & TopicGPT Discipline

This rule adapts TopicGPT-style topic modeling for SLTD map-level editorial work.

It discovers, refines, and assigns corpus-level topics, motifs, thread clusters, and repeated failure patterns with quote/evidence anchors.

## Core rule

No topic without quote or evidence anchor.

A topic map helps packet, arc, and series navigation. It does not authorize rewrite, canon verdict, readiness, Human Chapter Pass, or Publication Lock.

## Use when

- the user asks for packet, arc, part, or series-level map;
- the user asks about TopicGPT, topic modeling, thread discovery, motif clusters, repeated AI smell clusters, or source assignment;
- C001-C030 / C001-C120 or larger scope needs thematic/thread navigation;
- repeated motifs, dread patterns, household pressure, debt, reveal timing, character voice patterns, or AI-smell patterns need grouping;
- a packet review needs topic/thread coverage before targeted gates;
- a low-frequency motif may be important but easy to discard.

Do not use this for line edit, local scene rewrite, or readiness verdict by itself.

## Authority

Run after:

```text
source preflight
context brief for large scope
source surface or current Notion source when current manuscript status matters
context capsule when hidden canon, reveal timing, POV knowledge, source-status separation, or long-range continuity is in scope
narrative claim verification when a topic assignment depends on a factual/status/canon claim
```

Run before:

```text
packet review
arc review
series navigation
thread drift audit
narrative feature audit when map-level repetition is the issue
tracking / logic ledger when thread state is the issue
```

## Required distinction

```text
TOPIC = recurring subject, motif, pressure pattern, failure pattern, or thread cluster
THREAD = story/canon/relationship/reveal line that continues across scenes or chapters
TOPIC ASSIGNMENT = source node assigned to a topic with evidence quote/anchor
TOPIC REFINEMENT = merge, split, rename, or mark topic as too broad/too narrow
LOW-FREQUENCY IMPORTANT = rare topic that may matter for canon, reveal, payoff, or author taste
```

A topic label is not evidence. A quote or source anchor is required.

## Map levels

Use compact levels:

```text
SCENE
CHAPTER
PACKET
ARC
PART
SERIES
```

For 100+ chapters, use map-level review only. Do not line edit.

## Output schema

```text
SLTD CORPUS TOPIC / THREAD DISCOVERY MAP
SCOPE:
SOURCE USED:
SOURCE STATUS:
MAP LEVEL: SCENE / CHAPTER / PACKET / ARC / PART / SERIES
SEED TOPICS:
DISCOVERED TOPICS:
- TOPIC LABEL:
  DESCRIPTION:
  SOURCE ASSIGNMENTS:
  QUOTE / EVIDENCE ANCHORS:
  SPECIFICITY: TOO BROAD / OK / TOO NARROW
  DUPLICATE / MERGE CANDIDATE:
  LOW-FREQUENCY BUT IMPORTANT: YES / NO / UNCERTAIN
  CANON / REVEAL RISK:
  EDITORIAL USE:
TOPIC GAPS:
TOPIC DRIFT:
ROUTE DECISION:
NEXT NODE:
```

For broad tasks, return top clusters and topic gaps. Do not exhaustively list every chapter unless asked.

## Topic refinement rules

Safe refinement may:

- merge duplicate topics;
- split topics that are too broad;
- rename unclear labels;
- mark a low-frequency topic as important;
- create seed topics from user instruction or current packet;
- assign source nodes to topics with quotes/anchors.

Safe refinement must not:

- delete a low-frequency topic without canon/reveal/payoff check;
- treat summary-only topic labels as evidence;
- merge canon thread with decorative motif because words overlap;
- infer current status from old Workdeck/raw draft;
- call readiness or Publication Lock.

## Evidence anchors

Accepted anchors:

- current Notion source node;
- user-provided current packet;
- exact chapter/scene excerpt;
- explicit Chapter Card / Scene Packet fields;
- user-approved source summary only as locator, not final evidence.

Not accepted as final evidence:

- chat memory;
- vague summary;
- generated passage;
- topic label alone;
- old Workdeck unless user names it current/source sample.

## Low-frequency topic guard

Rare topics can be important.

Before discarding a topic because it appears once or twice, check:

```text
canon/reveal risk
future payoff
character-route relevance
object-state relevance
relationship-memory relevance
author-taste relevance
reader-effect relevance
```

If this check was not run, mark:

```text
LOW-FREQUENCY BUT IMPORTANT: UNCERTAIN
```

## Blockers

```text
scope missing
source missing for current map
quote/evidence anchor missing
topic assignment from summary only
low-frequency deletion without canon/reveal check
map used as readiness/lock verdict
map used as rewrite permission
topic refinement causes source drift
```

## Failure labels

```text
CORPUS_TOPIC_MAP_OK
CORPUS_TOPIC_MAP_PARTIAL
CORPUS_TOPIC_MAP_BLOCKED
TOPIC_WITHOUT_EVIDENCE
SUMMARY_ONLY_TOPIC_RISK
LOW_FREQUENCY_IMPORTANT_UNCHECKED
TOPIC_MERGE_CANON_DRIFT
TOPIC_TOO_BROAD
TOPIC_TOO_NARROW
THREAD_DRIFT_DETECTED
MAP_USED_AS_READINESS
MAP_USED_AS_REWRITE_PERMISSION
SOURCE_REQUIRED_FOR_TOPIC_MAP
```

## Safe repair

Safe repair may:

- build a scoped topic/thread map;
- assign source nodes to topics with quote/evidence anchors;
- identify topic gaps and thread drift;
- mark topics for merge/split without deleting source truth;
- hand off to Tracking Ledger, Narrative Feature Audit, Claim Verification, Harm Anticipation, Packet Review, or Editorial Director.

Safe repair must not:

- invent canon or future payoff;
- use topic map as source truth;
- call Human Chapter Pass, readiness, or Publication Lock;
- rewrite scenes from topic labels;
- create scripts, workflows, reports, boards, databases, automations, or live manuscript copies.

## Output labels

```text
CORPUS_TOPIC_MAP_READY
CORPUS_TOPIC_MAP_NEEDS_SOURCE
CORPUS_TOPIC_MAP_PARTIAL
CORPUS_TOPIC_MAP_BLOCKED
THREAD_DISCOVERY_HANDOFF
PACKET_REVIEW_HANDOFF
SERIES_MAP_HANDOFF
READINESS_NOT_AUTHORIZED
```