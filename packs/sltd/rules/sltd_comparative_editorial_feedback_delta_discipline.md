# SLTD Comparative Editorial Feedback Delta Discipline

This rule adapts comparative language feedback research for SLTD editorial work.

It converts user/editor feedback into a bounded editorial delta: what to increase, decrease, preserve, prohibit, compare, repair, and verify after revision.

## Core rule

No feedback delta without target scope.

No rewrite from vague preference.

No `better` without saying better along which dimension.

This is a feedback-translation and revision-routing discipline. It is not source authority, not canon authority, not a rewrite role by itself, not Human Chapter Pass, not readiness, and not Publication Lock.

## Use when

- the user gives comparative or directional feedback such as stronger, thinner, less AI, more human, more agency, less explanation, more object pressure, preserve X, do not reveal Y, or fix only this scene;
- feedback compares two outputs, an old version and a new version, a draft and target effect, or current prose and author taste;
- the user feedback contains mixed directions that must be separated before rewriting;
- rewrite, polish, human surface, author-aligned draft, packet review, readiness risk, or AI-smell explanation needs a precise delta ledger;
- the task needs to preserve user editorial intent instead of turning it into a generic style law.

## Authority

Run after:

```text
source preflight
source surface when exact span/current output is being judged
multilingual long-context retrieval when feedback depends on found/not-found/aggregation across long source
context capsule when current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, reveal timing, or long-range continuity is in scope
human expert AI-smell explanation when the feedback concerns synthetic reader effect
narrative claim verification when feedback depends on factual/status/canon/continuity evidence
multi-constraint instruction ledger when feedback contains several controlling constraints
```

Run before:

```text
rewrite
author-aligned draft
human surface polish
line surgery
readiness / lock route when feedback affects acceptance criteria
packet review result
```

## Required distinction

```text
FEEDBACK = user/editor language as given
DELTA = structured editorial change request extracted from feedback
INCREASE = feature to make more present, visible, costly, concrete, agentic, tense, or distinct
DECREASE = feature to reduce, cut, soften, compress, or move later
PRESERVE = source/canon/voice/object/reader-effect element that must remain
PROHIBIT = change that must not happen
COMPARE = relation between old/new, A/B, source/output, or current/target effect
REPAIR = safe next action, not automatic rewrite permission
```

Do not turn one instance of feedback into a permanent style law unless the user explicitly says it is a standing rule.

## Output schema

```text
SLTD COMPARATIVE EDITORIAL FEEDBACK DELTA CHECK
SCOPE:
SOURCE USED:
SOURCE STATUS:
FEEDBACK USED:
TARGET SPAN / SCENE / CHAPTER:
FEEDBACK TYPE: INCREASE / DECREASE / PRESERVE / PROHIBIT / COMPARE / REPAIR / MIXED
INCREASE:
DECREASE:
PRESERVE:
PROHIBIT:
COMPARE AGAINST:
IMPLICIT PREFERENCE:
SOURCE / CANON LIMIT:
POV / REVEAL LIMIT:
VOICE / CHARACTER LIMIT:
STYLE / SURFACE LIMIT:
READER EFFECT TARGET:
REVISION TEST:
REWRITE / POLISH PERMISSION: YES / NO / CANDIDATE_ONLY
BLOCKERS:
NEXT NODE:
```

## Delta extraction rules

Extract feedback into:

```text
what changes
where it changes
why it changes
what must remain
what must not be touched
how to test the revision
```

If any of these are missing, mark the delta partial instead of drafting from intuition.

## Common SLTD deltas

```text
increase object pressure
increase body/action cost
increase protagonist agency
increase relationship memory
increase silence/interruption
increase witness/debt/resource pressure
increase Vietnamese human rhythm

decrease explanation
decrease symbol-first prose
decrease outline label
decrease same-voice dialogue
decrease generic dread
decrease over-clean transitions
decrease author-style over character

preserve canon
preserve POV knowledge limit
preserve Must Show
preserve Must Not Reveal
preserve scene question
preserve reader effect
preserve current Notion source status

prohibit full-chapter rewrite
prohibit reveal leak
prohibit new canon
prohibit smoothing away rough character voice
prohibit changing scene outcome
```

## Comparison rules

When comparing versions, separate:

```text
A is better at X
B is better at Y
A fails because Z
B fails because W
next candidate should preserve A:X and B:Y while prohibiting Z/W
```

Do not collapse comparison into a single winner if the user feedback contains mixed preference.

## Blockers

```text
scope missing
target span missing
feedback too vague
source missing when source/canon/POV/status is affected
current source required but unread
comparison target missing
feedback conflicts with canon/POV/reveal lock
feedback conflicts with user instruction
feedback would cause full rewrite beyond requested scope
implicit preference not separated from source rule
rewrite requested before preserve/prohibit list is clear
```

## Failure labels

```text
FEEDBACK_DELTA_READY
FEEDBACK_DELTA_PARTIAL
FEEDBACK_DELTA_BLOCKED
SCOPE_REQUIRED_FOR_DELTA
TARGET_SPAN_REQUIRED_FOR_DELTA
VAGUE_FEEDBACK_BLOCKED
PRESERVE_LIST_MISSING
PROHIBIT_LIST_MISSING
IMPLICIT_PREFERENCE_UNSEPARATED
GENERIC_STYLE_LAW_RISK
REWRITE_PERMISSION_BLOCKED
```

## Safe repair

Safe repair may:

- restate feedback as delta;
- separate increase/decrease/preserve/prohibit;
- identify implicit preference and revision test;
- recommend rewrite, trim, line edit, human surface polish, AI-smell explanation, narrative feature audit, voice/staging, or readiness route;
- propose bounded patch only when the user asks for it and source constraints are clear.

Safe repair must not:

- invent user preference;
- convert feedback into universal style law;
- change canon, POV, reveal, scene outcome, or current source status to satisfy preference;
- polish before preserve/prohibit boundaries are clear;
- create scripts, workflows, reports, issues, boards, databases, automations, or live manuscript copies.

## Output labels

```text
FEEDBACK_DELTA_READY
FEEDBACK_DELTA_NEEDS_SCOPE
FEEDBACK_DELTA_NEEDS_TARGET
FEEDBACK_DELTA_NEEDS_SOURCE
FEEDBACK_DELTA_BLOCKED
REWRITE_HANDOFF
HUMAN_SURFACE_HANDOFF
AI_SMELL_EXPLANATION_HANDOFF
NARRATIVE_FEATURE_HANDOFF
VOICE_STAGING_HANDOFF
```