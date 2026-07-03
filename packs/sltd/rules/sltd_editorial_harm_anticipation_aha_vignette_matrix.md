# SLTD Editorial Harm Anticipation & AHA Vignette Matrix

This rule adapts AHA-style harm anticipation for SLTD editorial work.

It uses a bounded matrix of impact targets, editorial failure behaviors, and concrete vignettes to anticipate how an edit, rewrite, polish, packet verdict, readiness claim, or lock claim may damage the manuscript.

## Core rule

No harm matrix without scope.

Editorial harm anticipation supports REDTEAM, PREMORTEM, readiness review, packet review, and high-risk rewrite planning. It does not repair prose by itself and does not authorize Human Chapter Pass, readiness, or Publication Lock.

## Use when

- the user asks REDTEAM, PREMORTEM, failure analysis, harm anticipation, AHA, risk matrix, readiness risk, or lock risk;
- a chapter/packet may be falsely ready;
- a rewrite may improve one layer while damaging another;
- source, canon, POV, reveal timing, character voice, object state, relationship memory, author style, wordcount, or reader effect could be harmed;
- multi-constraint ledger shows high-risk constraints;
- prior AI output satisfied surface constraints but broke function, canon, or human read;
- a large rewrite, chapter readiness, packet review, canon conflict, or publication decision needs top failure vignettes.

## Authority

Run after:

```text
source preflight
context capsule when current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope
narrative claim verification when the harm depends on a status/canon/continuity claim
multi-constraint instruction ledger when constraints control output
source surface when exact prose/output is being judged
```

Run before:

```text
large rewrite
REDTEAM report
PREMORTEM report
readiness verdict
Publication Lock claim
packet decision
high-risk human surface polish
```

## Required distinction

```text
IMPACT TARGET = reader, scene function, character voice, canon, object state, relationship memory, future payoff, Human Pass, Publication Lock, or other manuscript target that may be harmed
EDITORIAL FAILURE BEHAVIOR = the way an edit or verdict may go wrong
VIGNETTE = concrete mini-scenario showing how the failure happens
HARM = consequence of that failure for manuscript/readers/downstream work
REPAIR / PREVENTION = route or blocker that prevents the harm
```

A harm vignette must stay source-safe. Do not invent canon, scene beats, or future events as if they are source.

## Impact targets

Use compact targets:

```text
READER_EFFECT
SCENE_FUNCTION
PROTAGONIST_ROUTE
CHARACTER_VOICE
CANON_REVEAL
POV_KNOWLEDGE
OBJECT_STATE
RELATIONSHIP_MEMORY
THREAD_PAYOFF
VIETNAMESE_SURFACE
AUTHOR_STYLE
HUMAN_CHAPTER_PASS
PUBLICATION_LOCK
DOWNSTREAM_CHAPTER
```

## Editorial failure behaviors

Use compact behaviors:

```text
SOURCE_DRIFT
COMPRESSED_SOURCE_REPLACES_CURRENT
FALSE_READINESS
REVEAL_LEAK
POV_LEAK
CANON_DRIFT
OVER_POLISH
STYLE_OVER_CHARACTER_VOICE
LORE_FRONTLOAD
WORDCOUNT_CUTS_MUST_SHOW
CONSTRAINT_SURFACE_PASS_EFFECT_FAIL
OBJECT_TO_SYMBOL_LABEL
RELATIONSHIP_FLATTENING
DIALOGUE_SAME_VOICE
AI_SMOOTHING_HOUSEHOLD_PRESSURE
```

## Output schema

```text
SLTD EDITORIAL HARM ANTICIPATION MATRIX
SCOPE:
SOURCE USED:
SOURCE STATUS:
TASK TYPE:
MATRIX MODE: UPFRONT / SECONDARY-CHECK
IMPACT TARGETS:
EDITORIAL FAILURE BEHAVIORS:
VIGNETTES:
- TARGET:
  FAILURE BEHAVIOR:
  FAILURE VIGNETTE:
  LIKELY HARM:
  SOURCE / CONSTRAINT ANCHOR:
  SEVERITY: LOW / MEDIUM / HIGH / CRITICAL
  DETECTABILITY: EASY / MODERATE / HARD
  REPAIR / PREVENTION:
BLOCKERS:
ROUTE DECISION:
NEXT NODE:
```

For broad tasks, return the top 3 harms by severity unless the user asks for a full matrix.

## Matrix modes

```text
UPFRONT = before rewrite/readiness/lock to anticipate risk
SECONDARY-CHECK = after a draft, polish, or verdict to inspect what may have been harmed
```

Use secondary-check when an AI output already exists.

## Vignette rules

A useful vignette must be concrete enough to test.

Good vignettes name:

- the scene/chapter/packet affected;
- the failure behavior;
- what the edit/verdict would do;
- who or what absorbs the harm;
- downstream consequence.

Bad vignettes:

- vague warnings;
- invented canon;
- generic AI-safety categories;
- harm lists with no scene/source anchor;
- readiness claims without current status source.

## Review overload rule

Do not generate a huge matrix by default.

If the matrix expands beyond useful scope, stop and return:

```text
TOP 3 HARMS BY SEVERITY
```

Then hand off to the one route that prevents the highest harm.

## Blockers

```text
scope missing
source missing for current/readiness/lock claim
impact target unclear
failure behavior unclear
vignette would invent canon
matrix creates review overload
harm depends on unverified claim
constraint anchor missing
AI harm anticipation used as readiness substitute
```

## Failure labels

```text
EDITORIAL_HARM_MATRIX_OK
EDITORIAL_HARM_MATRIX_PARTIAL
EDITORIAL_HARM_MATRIX_BLOCKED
SCOPE_MISSING
SOURCE_REQUIRED_FOR_HARM_MATRIX
VIGNETTE_CANON_DRIFT
HARM_OVERLOAD_RISK
UNVERIFIED_HARM_CLAIM
FALSE_READINESS_HARM
REVEAL_LEAK_HARM
OVERPOLISH_HARM
STYLE_OVER_CHARACTER_VOICE_HARM
READINESS_NOT_AUTHORIZED
PUBLICATION_LOCK_NOT_AUTHORIZED
```

## Safe repair

Safe repair may:

- build a scoped harm matrix;
- create top 3 failure vignettes;
- rank severity and detectability;
- identify repair/prevention route;
- hand off to Source Surface, Claim Verification, Multi-Constraint Ledger, Narrative Feature Audit, Character Voice, Author Writing Sheet, Human Surface Polish, Readiness, or Editorial Director.

Safe repair must not:

- invent future canon as harm evidence;
- turn harm anticipation into prose repair;
- use harm matrix as Human Chapter Pass;
- call Publication Lock;
- create scripts, workflows, reports, boards, databases, automations, or live manuscript copies.

## Output labels

```text
EDITORIAL_HARM_MATRIX_READY
EDITORIAL_HARM_MATRIX_NEEDS_SOURCE
EDITORIAL_HARM_MATRIX_OVERLOAD_TRIMMED
EDITORIAL_HARM_MATRIX_BLOCKED
REDTEAM_HANDOFF
PREMORTEM_HANDOFF
READINESS_NOT_AUTHORIZED
```