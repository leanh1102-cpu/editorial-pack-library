# SLTD Reference-Anchored Longform Story Quality & POLARIS Discipline

This rule adapts POLARIS-style long-form story quality evaluation for SLTD editorial work.

It checks whether a long rewrite, draft, chapter assembly, or packet candidate sustains story quality across length while preserving source, constraints, scene function, character voice, and human-surface integrity.

## Core rule

No story-quality score without source.

No length reward if Must Show is cut.

This is a quality stress test. It is not RL training, not a detector, not a Human Chapter Pass, not readiness, and not Publication Lock.

## Use when

- the user asks about POLARIS, longform quality, story-quality rubric, long rewrite quality, chapter rewrite quality, length adherence, bloat, drift, or quality across length;
- a scene/chapter/packet draft is long enough to risk early strength and late collapse;
- a rewrite meets wordcount but may be bloated, over-explained, generic, or incoherent;
- a draft is short/clean but may cut Must Show or reduce scene function;
- author-aligned drafting, chapter assembly, packet review, readiness risk, or human surface polish needs longform stress testing;
- a user-approved reference/anchor is available and style/quality comparison is explicitly in scope.

Do not use this as a generic line edit gate or as a substitute for source surface, claim verification, multi-constraint ledger, harm anticipation, narrative feature audit, or readiness.

## Authority

Run after:

```text
source preflight
source surface when exact prose/output is being judged
context capsule when current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope
narrative claim verification when a quality claim depends on factual/status/canon evidence
multi-constraint instruction ledger when output constraints control the draft
editorial harm anticipation when high-risk failure cost is in scope
corpus topic/thread discovery only when packet/arc/series map-level quality is in scope
```

Run before:

```text
readiness verdict
large rewrite acceptance
chapter assembly acceptance
packet candidate acceptance
human surface polish when the problem may be longform quality rather than surface
copyedit/proofread
```

## Required distinction

```text
SOURCE = current Notion source or user-provided current packet/excerpt
OUTPUT = draft, rewrite, assembled chapter, or packet candidate being evaluated
REFERENCE / ANCHOR = user-approved current sample or benchmark passage used for calibration, not source truth
TARGET LENGTH = requested or expected length
ACTUAL LENGTH = observed output length
QUALITY CHECK = rubric-based stress test, not readiness
```

A reference anchor must be user-approved/current. Do not use legacy drafts, generated passages, chat memory, or protected text as an anchor unless the user explicitly provides/approves it for this task.

## Positive dimensions

Assess with evidence from the output:

```text
PROMPT / SCENE FUNCTION FULFILLMENT
SCENE REALIZATION
NARRATIVE ARC / PACING
CHARACTER DEPTH / AGENCY
VOICE / STYLE DISTINCTIVENESS
THEMATIC / EMOTIONAL PRESSURE
READER EFFECT
```

Positive dimensions pass only when they are source-safe and sustained across the output, not merely strong in the opening segment.

## Negative dimensions

Actively check:

```text
SOURCE / PROMPT VIOLATION
COHERENCE / POV BREAK
GENERIC LANGUAGE
OVER-SUMMARY
OVER-EXPLANATION
DRIFT / BLOAT
DIALOGUE PROBLEM
PREDICTABILITY / CLICHE
OVERWROUGHT PROSE
LOCAL CONTRADICTION
LATE-OUTPUT COLLAPSE
MUST_SHOW_CUT_FOR_LENGTH
WORDCOUNT_PADDING
```

## Output schema

```text
SLTD REFERENCE-ANCHORED LONGFORM STORY QUALITY CHECK
SCOPE:
SOURCE USED:
SOURCE STATUS:
OUTPUT TYPE: SCENE / CHAPTER / PACKET / DRAFT / REWRITE
TARGET LENGTH:
ACTUAL LENGTH:
REFERENCE / ANCHOR USED:
ANCHOR STATUS:
POSITIVE DIMENSIONS:
- PROMPT / SCENE FUNCTION FULFILLMENT:
- SCENE REALIZATION:
- NARRATIVE ARC / PACING:
- CHARACTER DEPTH / AGENCY:
- VOICE / STYLE DISTINCTIVENESS:
- THEMATIC / EMOTIONAL PRESSURE:
- READER EFFECT:
NEGATIVE DIMENSIONS:
- SOURCE / PROMPT VIOLATION:
- COHERENCE / POV BREAK:
- GENERIC LANGUAGE:
- OVER-SUMMARY:
- OVER-EXPLANATION:
- DRIFT / BLOAT:
- DIALOGUE PROBLEM:
- PREDICTABILITY / CLICHE:
- OVERWROUGHT PROSE:
- LOCAL CONTRADICTION:
- LATE-OUTPUT COLLAPSE:
LENGTH ADHERENCE:
MUST SHOW PRESERVATION:
LOCAL COHERENCE CHECK:
QUALITY VERDICT: PASS / PARTIAL / FAIL / BLOCKED
DRAFT / REWRITE PERMISSION:
BLOCKERS:
NEXT NODE:
```

## Length rules

Length adherence is not quality by itself.

Mark failure when:

- output reaches target length by padding, explanation, generic atmosphere, repeated beats, or recap;
- output preserves style but cuts Must Show, scene question, Reader Effect, object state, relationship memory, or reveal lock;
- output starts strong but loses coherence, voice, object pressure, or pacing later;
- output is concise but undercuts scene function.

## Reference anchor rules

A reference anchor may help calibrate quality, density, rhythm, pressure, or human-surface expectation.

It must not:

- replace current source;
- override canon, POV, scene function, or character voice;
- become a style law;
- be copied, paraphrased closely, scraped, or used as training data;
- authorize readiness.

If anchor status is unclear, write:

```text
ANCHOR STATUS: NOT AUTHORIZED
```

and continue without anchor or block if the task requires one.

## Blockers

```text
source missing
output missing
scope missing
exact prose needed but not read
reference anchor required but not authorized
Must Show source missing
length target missing when length adherence is requested
quality claim depends on unverified status/canon claim
multi-constraint ledger needed but missing
harm/risk gate needed but missing
longform quality used as readiness substitute
```

## Failure labels

```text
LONGFORM_QUALITY_OK
LONGFORM_QUALITY_PARTIAL
LONGFORM_QUALITY_FAIL
LONGFORM_QUALITY_BLOCKED
SOURCE_REQUIRED_FOR_QUALITY
OUTPUT_REQUIRED_FOR_QUALITY
ANCHOR_NOT_AUTHORIZED
MUST_SHOW_CUT_FOR_LENGTH
WORDCOUNT_PADDING
DRIFT_BLOAT_RISK
OVER_SUMMARY_RISK
OVER_EXPLANATION_RISK
LOCAL_COHERENCE_FAILURE
LATE_OUTPUT_COLLAPSE
VOICE_STYLE_OVERLOAD
READINESS_NOT_AUTHORIZED
PUBLICATION_LOCK_NOT_AUTHORIZED
```

## Safe repair

Safe repair may:

- identify quality blockers;
- mark length adherence problems;
- separate bloat from necessary scene pressure;
- compare to approved anchor at a high level;
- recommend rewrite, trim, source surface, multi-constraint ledger, narrative feature audit, human surface polish, or readiness route.

Safe repair must not:

- train, fine-tune, scrape, or copy protected reference text;
- use LLM judge result as Human Chapter Pass;
- call readiness or Publication Lock;
- invent source facts, canon, object state, relationship memory, or future payoff;
- reward length when Must Show is cut;
- create scripts, workflows, reports, boards, databases, automations, or live manuscript copies.

## Output labels

```text
LONGFORM_QUALITY_READY
LONGFORM_QUALITY_NEEDS_SOURCE
LONGFORM_QUALITY_NEEDS_OUTPUT
LONGFORM_QUALITY_BLOCKED
REWRITE_PERMISSION_BLOCKED
HUMAN_SURFACE_HANDOFF
NARRATIVE_FEATURE_HANDOFF
READINESS_NOT_AUTHORIZED
```