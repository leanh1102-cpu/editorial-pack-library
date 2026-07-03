# SLTD Context Memory Lifecycle Check

Use this prompt when prior handoff, context brief, node ledger, chat memory, feedback delta, route note, risk note, topic map, style note, or readiness note may affect current work.

This is a lifecycle and provenance discipline. It is not source authority, canon authority, readiness, Publication Lock, or rewrite permission.

## Read first

```text
manifest.yml
rules/sltd_source_preflight.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_multilingual_long_context_retrieval_oneruler_discipline.md if memory depends on found/not-found/aggregation evidence
rules/sltd_context_capsule_lore_retrieval_discipline.md if current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, reveal timing, or long-range continuity is in scope
rules/sltd_narrative_claim_verification_clipper_discipline.md if the context entry contains a factual/status/canon/continuity claim
rules/sltd_comparative_editorial_feedback_delta_discipline.md if the entry captures user/editor feedback
rules/sltd_agent_native_context_memory_lifecycle_byterover_discipline.md
```

## Source requirement

If the context entry is used for current status, canon, readiness, lock, source absence, or exact manuscript claim, current source or current user packet must be read.

If provenance is missing, return:

```text
CONTEXT_MEMORY_NEEDS_PROVENANCE
```

If source is required but missing, return:

```text
CONTEXT_MEMORY_NEEDS_SOURCE
```

## Output

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

## Rules

- No context entry without provenance.
- No stale handoff as current source.
- No GitHub live manuscript memory.
- No chat memory as source truth.
- No mature/stable label without source or rule basis.
- No current-status verdict from context memory.
- No hidden recency decay.
- If memory contains claim, hand off to Narrative Claim Verification when verdict matters.
- If memory contains source absence or distributed evidence, hand off to Long-Context Retrieval.
- If memory contains user feedback, hand off to Comparative Feedback Delta before rewrite.

## Minimal output

```text
CONTEXT MEMORY BRIEF
SCOPE:
ENTRY:
PROVENANCE:
MATURITY:
RECENCY:
SOURCE-TRUTH LIMIT:
DECISION:
NEXT NODE:
```

## Source gap output

```text
CONTEXT MEMORY SOURCE GAP
REQUEST:
CONTEXT ENTRY:
SOURCE NEEDED:
PROVENANCE NEEDED:
WHY NEEDED:
SAFE CLAIM NOW:
NEXT NODE:
```