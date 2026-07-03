# SLTD Narrative Feature Audit

Use this prompt when a scene/chapter/packet may be source-correct and line-readable but still AI-shaped at the story-decision layer.

This is not an AI detector prompt. It is a structural idiosyncrasy and narrative-feature audit for SLTD.

## Read first

```text
manifest.yml
rules/sltd_source_preflight.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_context_capsule_lore_retrieval_discipline.md if current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md if scene/chapter function or prose permission is unclear
rules/sltd_tracking_logic_ledger_traceability_gate.md if state, object, debt, residue, thread, reveal, or downstream risk is affected
rules/sltd_character_voice_dialogue_relationship_location_gate.md if dialogue function, character presence, or relationship pressure is in scope
rules/sltd_author_voice_fingerprint_ghostwriter_discipline.md if author-style match or author-aligned draft is being evaluated
rules/sltd_human_surface_polish_anti_synthetic_gate.md if the next node may be surface polish
rules/sltd_narrative_feature_structural_idiosyncrasy_audit.md
AUTHOR_TASTE_EXAMPLES.md
```

## Source requirement

Read current source or the user-provided current packet before giving a verdict.

If current source is missing, return:

```text
SOURCE NOT READ / EVIDENCE MISSING
```

If exact prose is not needed and the user asks for map-level assessment, use the current chapter card / scene packet / outline source and mark source surface as not read.

## Output

```text
SLTD NARRATIVE FEATURE AUDIT
SCOPE:
SOURCE USED:
SOURCE STATUS:
CONTEXT CAPSULE STATUS:
SCENE / CHAPTER QUESTION:
THEMATIC EXPLICITNESS:
CAUSAL TIDINESS:
SINGLE-TRACK PLOT RISK:
PROTAGONIST AGENCY SHAPE:
TEMPORAL COMPLEXITY:
REVEAL / RECONTEXTUALIZATION:
SUBPLOT / THREAD INTEGRATION:
MORAL AMBIGUITY:
DIALOGUE FUNCTION:
BODY / SENSORY OVERPERFORMANCE:
SETTING AS PSYCHOLOGICAL MIRROR:
NARRATIVE DIVERSITY:
CHANGED-STATE / REREAD VALUE:
AI-STRUCTURAL SMELL:
SAFE REPAIR:
PROSE PERMISSION:
NEXT NODE:
```

## Rules

- Do not use a detector score.
- Do not report a decorative percentage.
- Do not punish clarity; punish clarity that removes pressure, ambiguity, debt, or reread value.
- Do not treat body/sensory detail as automatically human.
- Do not add canon or subplot to avoid a single-track plot.
- Do not turn research feature names into prose language.
- Do not call Human Chapter Pass, readiness, or Publication Lock.
- If the audit exposes story failure, route back before Human Surface Polish.

## Minimal scene check

For a single scene, the audit may be compressed to:

```text
PRIMARY STRUCTURAL SMELL:
EVIDENCE:
RISK:
SAFE REPAIR:
NEXT NODE:
```

## Source gap output

```text
NARRATIVE FEATURE SOURCE GAP
SCOPE:
REQUEST:
SOURCE NEEDED:
WHY NEEDED:
SAFE CLAIM NOW:
NEXT NODE:
```