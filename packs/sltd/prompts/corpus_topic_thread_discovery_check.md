# SLTD Corpus Topic / Thread Discovery Check

Use this prompt for packet, arc, part, or series-level topic/thread discovery.

This is a map-level navigation pass, not a line edit, rewrite pass, canon verdict, or readiness pass.

## Read first

```text
manifest.yml
rules/sltd_source_preflight.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_context_capsule_lore_retrieval_discipline.md if current source, hidden canon, POV knowledge, source-status separation, reveal timing, or long-range continuity is in scope
rules/sltd_corpus_topic_thread_discovery_topicgpt_discipline.md
rules/sltd_narrative_claim_verification_clipper_discipline.md if topic assignment depends on factual/status/canon evidence
rules/sltd_tracking_logic_ledger_traceability_gate.md if thread state or payoff debt is in scope
rules/sltd_narrative_feature_structural_idiosyncrasy_audit.md if repeated structural AI smell or narrative diversity is in scope
rules/sltd_editorial_harm_anticipation_aha_vignette_matrix.md if topic/thread drift creates downstream harm
```

## Source requirement

Use current Notion source or a user-provided current packet when current manuscript status matters.

If source is missing, return:

```text
CORPUS_TOPIC_MAP_NEEDS_SOURCE
```

Do not create topic assignments from summary alone when current source status matters.

## Output

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

## Rules

- No topic without quote/evidence anchor.
- Do not delete low-frequency topics without canon/reveal/payoff check.
- Do not use a topic map as readiness, lock, canon verdict, or rewrite permission.
- Do not line edit from topic labels.
- Mark summary-only topic assignments as partial.
- For 100+ chapters, map only; do not line edit.
- For broad tasks, return top clusters, topic gaps, and next route.

## Minimal output

For quick packet navigation:

```text
TOPIC / THREAD MAP BRIEF
SCOPE:
SOURCE USED:
TOP CLUSTERS:
LOW-FREQUENCY IMPORTANT:
TOPIC GAPS:
THREAD DRIFT:
NEXT NODE:
```

## Source gap output

```text
CORPUS TOPIC SOURCE GAP
SCOPE:
REQUEST:
SOURCE NEEDED:
WHY NEEDED:
SAFE MAP CLAIM NOW:
NEXT NODE:
```