# SLTD Multi-Constraint Instruction Ledger & Suri Discipline

This rule adapts Suri-style multi-constraint instruction following for SLTD.

It turns a rewrite, audit, polish, or readiness request into an explicit constraint ledger so long-form output does not satisfy some requirements while quietly breaking source, canon, POV, reveal timing, character voice, word target, or reader effect.

## Core rule

No rewrite without named constraints.

A draft may sound good and still fail if it violates a hidden or late constraint. Every high-risk task must name its constraints before drafting, patching, readiness, or lock verdict.

## Use when

- the user asks for rewrite, edit, audit, readiness, lock, packet review, or author-aligned draft with multiple constraints;
- Scene Question, Must Show, Must Not Reveal, Reader Effect, POV knowledge, canon lock, object state, word target, author taste, or surface quality must be preserved together;
- prior output fixed one layer but broke another;
- a task has more than one controlling instruction;
- the user asks about Suri, multi-constraint instruction following, constraint satisfaction, corrupted instructions, or instruction ledger;
- AI risks following the visible prompt while missing a source/canon/style/voice constraint.

## Authority

Run after:

```text
source preflight
context capsule when current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope
narrative claim verification if a constraint depends on a factual/status/canon claim
source surface when exact prose, status, patch, or output anchor is required
```

Run before:

```text
rewrite
line surgery
human surface polish
author-aligned drafting
readiness verdict
Human Chapter Pass claim
Publication Lock claim
```

## Required distinction

```text
CONSTRAINT = a requirement that the output must satisfy or must not violate
CORRUPTED CONSTRAINT = a near-plausible wrong version of a high-risk constraint
CLAIM VERIFICATION = TRUE/FALSE/UNCERTAIN evidence check for story/status/canon claims
NARRATIVE FEATURE AUDIT = story-decision smell check
AUTHOR WRITING SHEET = claim-evidence style memory
HUMAN SURFACE POLISH = late prose surface repair
```

A corrupted constraint is not a claim verdict. It is a trapdoor used to catch drift during drafting or review.

## Constraint types

Use compact types:

```text
SOURCE
CANON
POV
SCENE_FUNCTION
MUST_SHOW
MUST_NOT_REVEAL
READER_EFFECT
OBJECT_STATE
THREAD_DEBT
RELATIONSHIP_MEMORY
CHARACTER_VOICE
AUTHOR_STYLE
VIETNAMESE_SURFACE
WORDCOUNT
READINESS
PUBLICATION_LOCK
```

## Output schema

```text
SLTD MULTI-CONSTRAINT INSTRUCTION LEDGER
SCOPE:
SOURCE USED:
SOURCE STATUS:
TASK TYPE:
PRIMARY USER INSTRUCTION:
CONSTRAINT LIST:
- ID:
  TYPE:
  MUST SATISFY:
  MUST NOT:
  CORRUPTED CONSTRAINT:
  PRIORITY:
  EVIDENCE / OUTPUT ANCHOR:
  STATUS: SATISFIED / PARTIAL / NOT SATISFIED / UNCERTAIN
CONSTRAINT CONFLICTS:
LOW-LEVEL DETAIL RISK:
DRAFT / REWRITE PERMISSION:
REPAIR TARGET:
NEXT NODE:
```

Use the full schema for rewrites/readiness/packet review. For small line work, use a compressed ledger.

## Corrupted constraint rules

Every high-risk constraint needs a corrupted twin when drift is plausible.

Good corrupted constraints are close enough to tempt agreement:

- keep origin unrevealed -> hint origin for clarity;
- dog stays wrongly silent -> dog barks to warn;
- POV only feels local pressure -> POV names high law;
- Human Pass is NO -> green gate labels make it ready;
- poor household object acts as pressure -> object becomes symbolic label;
- character hides knowledge through task -> character explains emotion directly.

Do not create silly or unrelated corrupted constraints.

## Conflict handling

If constraints conflict, stop before drafting.

Examples:

- wordcount target requires cutting a Must Show;
- author style rule would flatten character voice;
- human surface polish would reveal hidden canon;
- readiness request conflicts with current Publication Lock evidence;
- style imitation requires sample not approved.

Return conflict and next node instead of forcing output.

## Evidence / output anchor

Each constraint needs an anchor:

- source node / field / scene packet item;
- exact scene line or excerpt when exact prose is in scope;
- user instruction;
- author sample / Author Writing Sheet claim;
- output paragraph or patch location after drafting.

If anchor is missing, status is `UNCERTAIN`, not satisfied.

## Prose and readiness blockers

```text
source missing
current source not read for current-status claim
constraint list missing
high-risk corrupted constraint missing
constraint conflict unresolved
exact output anchor missing
constraint status uncertain on canon/source/POV/reveal/readiness
word target would delete Must Show
style constraint lacks evidence
AI constraint satisfaction used as Human Chapter Pass
```

## Failure labels

```text
MULTI_CONSTRAINT_LEDGER_OK
MULTI_CONSTRAINT_LEDGER_PARTIAL
MULTI_CONSTRAINT_LEDGER_BLOCKED
CONSTRAINT_LIST_MISSING
CORRUPTED_CONSTRAINT_MISSING
CONSTRAINT_CONFLICT
CONSTRAINT_ANCHOR_MISSING
CONSTRAINT_STATUS_UNCERTAIN
SOURCE_CONSTRAINT_BROKEN
CANON_CONSTRAINT_BROKEN
POV_CONSTRAINT_BROKEN
REVEAL_CONSTRAINT_BROKEN
CHARACTER_VOICE_CONSTRAINT_BROKEN
STYLE_CONSTRAINT_UNEVIDENCED
WORDCOUNT_OVERREPAIR_RISK
READINESS_NOT_AUTHORIZED
PUBLICATION_LOCK_NOT_AUTHORIZED
```

## Safe repair

Safe repair may:

- extract constraints from current user instruction and source packet;
- add corrupted constraints for high-risk items;
- mark conflicts before drafting;
- check draft output against constraints;
- route failed constraints to Source Surface, Claim Verification, Tracking Ledger, Structural Spine, Character Voice, Author Writing Sheet, Human Surface, or Readiness route;
- produce a bounded repair target.

Safe repair must not:

- invent source constraints;
- treat AI self-evaluation as human pass;
- override source priority;
- call Publication Lock;
- hide a broken constraint under smooth prose;
- create scripts, workflows, reports, boards, databases, automations, or live manuscript copies.

## Output labels

```text
CONSTRAINT_LEDGER_READY
CONSTRAINT_LEDGER_NEEDS_SOURCE
CONSTRAINT_LEDGER_CONFLICT_BLOCKED
CONSTRAINT_CHECK_FAILED
DRAFT_PERMISSION_GRANTED
DRAFT_PERMISSION_BLOCKED
REWRITE_PERMISSION_GRANTED
REWRITE_PERMISSION_BLOCKED
READINESS_NOT_AUTHORIZED
```