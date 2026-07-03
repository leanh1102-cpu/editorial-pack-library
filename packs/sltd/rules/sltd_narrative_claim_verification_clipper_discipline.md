# SLTD Narrative Claim Verification & CLIPPER Discipline

This rule adapts CLIPPER-style narrative claim verification for SLTD.

It uses compressed source only to locate and structure evidence. It does not let outlines, summaries, chapter cards, or context capsules replace the current source.

## Core rule

Compressed source helps locate evidence. Compressed source does not replace source.

A claim about manuscript status, canon, continuity, character knowledge, reveal timing, object state, debt, lock, or readiness must be verified against current Notion source or an explicitly provided current packet before it becomes a verdict.

## Use when

- the user asks whether a claim about SLTD is true, false, uncertain, current, locked, ready, canon, or contradicted;
- a rewrite depends on a factual/canon/continuity claim;
- a packet review risks relying on green labels, summaries, or memory;
- source nodes disagree;
- current status, Human Chapter Pass, Publication Lock, packet lock, or canon conflict is in scope;
- a false twin would catch lazy agreement;
- claim verification / CLIPPER / true-false pair / evidence-backed reasoning is requested.

## Authority

Run after:

```text
source preflight
source surface when exact scene/chapter/status is required
context capsule when current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope
tracking / logic ledger when state, object, debt, residue, thread, or downstream risk is affected
```

Run before:

```text
rewrite that depends on the claim
readiness verdict
Human Chapter Pass claim
Publication Lock claim
canon decision
packet verdict
```

If evidence is missing, verdict is `UNCERTAIN`, not guessed.

## Required distinction

```text
SOURCE = current Notion source or user-provided current packet
COMPRESSED SOURCE = chapter outline, chapter card, context capsule, summary, ledger, or packet brief
CLAIM = a testable statement about story/status/canon/continuity
FALSE TWIN = a close counterclaim designed to catch lazy agreement
VERDICT = TRUE / FALSE / UNCERTAIN, based on evidence
```

Compressed source may:

- locate likely evidence;
- define claim scope;
- help build false twins;
- expose missing source;
- compress handoff.

Compressed source must not:

- become current manuscript evidence by itself;
- override scene surface;
- override Chapter Index / Scene Bank / Chapter Review current fields;
- authorize readiness or lock;
- invent a missing link.

## Claim types

Use compact claim types:

```text
STATUS_CLAIM
CANON_CLAIM
CONTINUITY_CLAIM
POV_KNOWLEDGE_CLAIM
OBJECT_STATE_CLAIM
THREAD_DEBT_CLAIM
REVEAL_TIMING_CLAIM
READINESS_CLAIM
PUBLICATION_LOCK_CLAIM
SOURCE_CONFLICT_CLAIM
```

## Output schema

```text
SLTD NARRATIVE CLAIM VERIFICATION
SCOPE:
SOURCE USED:
SOURCE STATUS:
COMPRESSED SOURCE USED:
CLAIM:
CLAIM TYPE:
TRUE / FALSE / UNCERTAIN:
EVIDENCE:
COUNTERCLAIM / FALSE TWIN:
CHAPTER / SCENE ANCHOR:
LOW-LEVEL DETAIL RISK:
MISATTRIBUTION RISK:
CANON / CONTINUITY IMPACT:
VERDICT:
PROSE / READINESS PERMISSION:
NEXT NODE:
```

Use only fields needed by the task. For simple claims, keep the output short.

## False twin rules

A useful false twin must be close enough to tempt agreement.

Good false twins change one story-sensitive element:

- ready vs not ready;
- Human Pass yes vs no;
- scene reveals vs withholds;
- dog barks vs dog stays wrongly silent;
- object is explained vs object remains pressured and unnamed;
- character knows high law vs only feels local pressure;
- source says current vs legacy material says old status.

Do not build silly or unrelated false twins.

## Low-level detail caution

Compressed outlines can lose small but decisive details.

If a claim depends on exact wording, object behavior, line-level reveal, dialogue nuance, xưng hô, silence, gesture, or sensory action, read exact source surface before verdict.

## Misattribution caution

When a claim names a chapter, scene, character, object, or field, verify the anchor.

If evidence appears in a different node than claimed, mark `MISATTRIBUTION_RISK` and do not silently repair the claim.

## Prose / readiness permission blockers

```text
current source missing
compressed source only
exact scene surface needed but not read
claim anchor unclear
false twin not checked when risk is high
source conflict unresolved
low-level detail risk unresolved
claim is TRUE but readiness still lacks Human Chapter Pass / Publication Lock evidence
claim verification used as readiness substitute
```

## Failure labels

```text
CLAIM_VERIFICATION_OK
CLAIM_VERIFICATION_PARTIAL
CLAIM_VERIFICATION_BLOCKED
CLAIM_TRUE
CLAIM_FALSE
CLAIM_UNCERTAIN
COMPRESSED_SOURCE_ONLY
FALSE_TWIN_MISSING
LOW_LEVEL_DETAIL_RISK
MISATTRIBUTION_RISK
SOURCE_CONFLICT_RISK
LAZY_AGREEMENT_RISK
READINESS_NOT_AUTHORIZED
PUBLICATION_LOCK_NOT_AUTHORIZED
```

## Safe repair

Safe repair may:

- rewrite a vague claim into a testable claim;
- create a close false twin;
- locate likely evidence nodes;
- mark evidence gaps;
- return TRUE / FALSE / UNCERTAIN;
- route to source surface, context capsule, tracking ledger, canon guard, narrative feature audit, or readiness route.

Safe repair must not:

- invent evidence;
- treat outline/summary/capsule as current source;
- use claim verification as Human Chapter Pass;
- call Publication Lock;
- create scripts, workflows, reports, boards, databases, automations, or live manuscript copies.

## Output labels

```text
CLAIM_VERIFIED
CLAIM_FALSE_REPAIR_NEEDED
CLAIM_UNCERTAIN_SOURCE_NEEDED
SOURCE_SURFACE_REQUIRED
TRACKING_LEDGER_REQUIRED
CANON_GUARD_REQUIRED
READINESS_NOT_AUTHORIZED
```