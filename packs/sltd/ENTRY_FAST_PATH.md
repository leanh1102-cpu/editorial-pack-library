# SLTD Entry Fast Path

Use this file to choose the smallest SLTD route.

## Always read

```text
manifest.yml
DESIGN.md
PACK.md
AGENT_IDENTITY.md
rules/sltd_runtime_loop.md
rules/sltd_source_preflight.md
rules/sltd_decision_safety.md
```

## Pipeline order

```text
0. Source Preflight
1. Context Capsule
2. Narrative Claim Verification when status/canon/continuity/lock claim is in scope
3. Spine Lock
4. Tracking / Logic Ledger
5. Borderbound
6. Life-Task Bound
7. Story Movement
8. Scene-First Prose Judgment
9. Narrative Feature / Structural Idiosyncrasy Audit when story-decision AI smell is in scope
10. Voice / Dialogue / Staging
11. Author Voice Fingerprint when author style matching is in scope
12. Draft / Rewrite / Author-Aligned Ghostwriter Draft
13. Line / Voice / Rhythm
14. Human Surface Polish
15. Composite Risk Check
16. Feedback Matrix / Report
17. Seam / Chapter Assembly
18. Readiness / Lock
```

Do not run later gears to hide failure in earlier gears. Do not draft, ghostwrite, polish, copyedit, or claim readiness before source, context capsule, claim verification, spine, tracking, border, narrative-feature, and scene staging are clear when continuity, hidden canon, object state, relationship memory, author voice, dialogue, reveal, status, lock, or story-decision smell is at stake. Stop at the first real blocker.

## Fast paths

### Context capsule / lore retrieval discipline

```text
rules/sltd_source_preflight.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_context_capsule_lore_retrieval_discipline.md
rules/sltd_narrative_claim_verification_clipper_discipline.md if current status, canon, continuity, readiness, lock, or source conflict claim is in scope
rules/sltd_tracking_logic_ledger_traceability_gate.md if state, knowledge, object, residue, thread, pass trace, or downstream risk is affected
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md if scene function, chapter card, scene packet, or border is unclear
rules/sltd_narrative_feature_structural_idiosyncrasy_audit.md if story-decision AI smell, reveal value, thematic explicitness, or causal tidiness is in scope
rules/sltd_character_voice_dialogue_relationship_location_gate.md if voice, relationship, silence, presence, or location staging is affected
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md if exact Vietnamese surface, Human Chapter Pass, or Publication Lock is in scope
prompts/context_capsule_preflight.md
prompts/node_checkpoint.md
```

### Narrative claim verification / CLIPPER discipline

```text
rules/sltd_source_preflight.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_context_capsule_lore_retrieval_discipline.md if current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope
rules/sltd_tracking_logic_ledger_traceability_gate.md if state, object, debt, residue, thread, claim anchor, or downstream risk is affected
rules/sltd_narrative_claim_verification_clipper_discipline.md
rules/sltd_narrative_feature_structural_idiosyncrasy_audit.md if the claim concerns story-decision AI smell or structural idiosyncrasy
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md if Human Chapter Pass, Publication Lock, or exact Vietnamese surface is in scope
prompts/narrative_claim_verification_check.md
prompts/node_checkpoint.md
```

### Narrative feature / structural idiosyncrasy audit

```text
rules/sltd_source_preflight.md
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_context_capsule_lore_retrieval_discipline.md if current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, reveal timing, or long-range continuity is in scope
rules/sltd_narrative_claim_verification_clipper_discipline.md if a story-decision verdict depends on a testable claim or false twin
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md if scene/chapter function or prose permission is unclear
rules/sltd_tracking_logic_ledger_traceability_gate.md if state, object, debt, residue, thread, reveal, or downstream risk is affected
rules/sltd_character_voice_dialogue_relationship_location_gate.md if dialogue function, character presence, or relationship pressure is in scope
rules/sltd_author_voice_fingerprint_ghostwriter_discipline.md if author-style match or author-aligned draft is being evaluated
rules/sltd_human_surface_polish_anti_synthetic_gate.md if the next node may be surface polish
rules/sltd_narrative_feature_structural_idiosyncrasy_audit.md
prompts/narrative_feature_audit.md
prompts/node_checkpoint.md
```

### Character voice / dialogue / relationship / location staging

```text
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_context_capsule_lore_retrieval_discipline.md if current source, hidden canon, POV knowledge, object state, relationship memory, or long-range context is in scope
rules/sltd_narrative_claim_verification_clipper_discipline.md if a voice/knowledge/status claim needs evidence
rules/sltd_narrative_feature_structural_idiosyncrasy_audit.md if dialogue is structurally decorative, causality is too tidy, or body/sensory pressure performs without consequence
rules/sltd_character_voice_dialogue_relationship_location_gate.md
samples/character_voice_dialogue_staging_calibration.md
rules/sltd_tracking_logic_ledger_traceability_gate.md if relationship memory, knowledge state, object state, or downstream risk is affected
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md if scene function or border is unclear
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md if exact Vietnamese dialogue surface is in scope
rules/sltd_author_voice_fingerprint_ghostwriter_discipline.md if author voice may overwrite character voice
rules/sltd_character_distinctiveness_iceberg_gate.md if voice profile is unclear
rules/sltd_living_world_community_motion_gate.md if group presence or community motion is in scope
prompts/character_voice_dialogue_staging_check.md
prompts/node_checkpoint.md
```

### Author voice fingerprint / ghostwriter discipline

```text
rules/sltd_source_preflight.md
rules/sltd_source_fidelity_anti_compression.md
AUTHOR_WORKING_PROFILE.md
AUTHOR_TASTE_EXAMPLES.md
rules/sltd_author_voice_fingerprint_ghostwriter_discipline.md
rules/sltd_context_capsule_lore_retrieval_discipline.md if current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope
rules/sltd_narrative_claim_verification_clipper_discipline.md if author-aligned draft depends on status/canon/continuity claim
rules/sltd_narrative_feature_structural_idiosyncrasy_audit.md if author-aligned prose may be structurally AI-shaped
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md if scene function or prose permission is unclear
rules/sltd_tracking_logic_ledger_traceability_gate.md if state, object, debt, residue, thread, or downstream risk is affected
rules/sltd_character_voice_dialogue_relationship_location_gate.md if dialogue, character voice, relationship, silence, presence, or staging is in scope
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md if exact Vietnamese surface is in scope
prompts/author_voice_fingerprint_check.md for sample/style extraction or voice match
prompts/author_aligned_ghostwriter_draft.md for bounded source-safe drafting
prompts/node_checkpoint.md
```

### General + chapter feedback matrix

```text
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_context_capsule_lore_retrieval_discipline.md if current source, packet scope, canon status, or long-range context is in scope
rules/sltd_narrative_claim_verification_clipper_discipline.md if packet/status/canon/continuity claims need TRUE/FALSE/UNCERTAIN verdicts
rules/sltd_general_chapter_feedback_matrix_output_protocol.md
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md if spine/source status is in scope
rules/sltd_tracking_logic_ledger_traceability_gate.md if state/thread/object/pass/downstream logic is in scope
rules/sltd_narrative_feature_structural_idiosyncrasy_audit.md if story-decision AI smell, thematic overexplicitness, causal tidiness, or narrative diversity is a packet issue
rules/sltd_character_voice_dialogue_relationship_location_gate.md if dialogue, relationship, or staging is a packet issue
rules/sltd_author_voice_fingerprint_ghostwriter_discipline.md if author voice match is a packet issue
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md if human surface or pass integrity is in scope
prompts/general_chapter_feedback_matrix_check.md
prompts/node_checkpoint.md
```

### Tracking / structural / surface / prose work

```text
source_surface_check when exact prose or status is required
context_capsule_preflight when current source, hidden canon, POV knowledge, object state, relationship memory, lore retrieval, or long-range continuity is in scope
rules/sltd_narrative_claim_verification_clipper_discipline.md when a status/canon/continuity/source-conflict claim controls the route
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md when spine or border is in scope
rules/sltd_tracking_logic_ledger_traceability_gate.md when logic continuity is affected
rules/sltd_narrative_feature_structural_idiosyncrasy_audit.md when story-decision AI smell, thematic overexplicitness, causal tidiness, reveal value, body/sensory overperformance, or narrative diversity is in scope
rules/sltd_character_voice_dialogue_relationship_location_gate.md when voice, relationship, or location staging is affected
rules/sltd_author_voice_fingerprint_ghostwriter_discipline.md when author voice, style match, or ghostwriter drafting is in scope
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md when human surface or pass integrity is affected
rules/sltd_human_surface_polish_anti_synthetic_gate.md when exact prose is source-safe but still reads synthetic, over-clean, same-voiced, or falsely smooth
relevant primary gate only when evidence requires it
prompts/node_checkpoint.md
```

### Human surface polish / anti-synthetic prose

```text
source_surface_check when exact prose is being patched
rules/sltd_source_fidelity_anti_compression.md
rules/sltd_context_capsule_lore_retrieval_discipline.md if current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope
rules/sltd_narrative_claim_verification_clipper_discipline.md if the patch depends on a factual/canon/continuity claim
rules/sltd_structural_spine_outline_preprose_borderbound_gate.md if scene function or prose permission is unclear
rules/sltd_tracking_logic_ledger_traceability_gate.md if state, object, debt, residue, thread, or downstream risk is affected
rules/sltd_narrative_feature_structural_idiosyncrasy_audit.md if surface polish may hide structural AI smell or decorative body/sensory overperformance
rules/sltd_character_voice_dialogue_relationship_location_gate.md if voice, relationship, silence, presence, dialogue, or location staging is in scope
rules/sltd_author_voice_fingerprint_ghostwriter_discipline.md if author voice match or ghostwriter output is being polished
rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md
rules/sltd_human_surface_polish_anti_synthetic_gate.md
prompts/human_surface_polish_pass.md
prompts/node_checkpoint.md
```

## Rule

Run `context_capsule_preflight.md` when the task concerns current/latest source, Notion current manuscript, lock, readiness, Human Chapter Pass, Publication Lock, packet verdict, canon conflict, hidden canon, POV knowledge, object/location/body/debt state, relationship memory, lore retrieval, legacy source risk, summary-vs-source risk, or long-range continuity.

Run `narrative_claim_verification_check.md` when the task concerns CLIPPER-style claim verification, true/false claims, false twins, status claims, canon claims, continuity claims, POV knowledge claims, source conflicts, readiness claims, Human Chapter Pass, Publication Lock, or whether a claim is TRUE/FALSE/UNCERTAIN.

Run `narrative_feature_audit.md` when the task concerns StoryScope-style narrative features, structural AI smell, theme overexplained, causal tidiness, single-track plot risk, protagonist understanding as resolution, temporal flatness, weak reveal/recontextualization, decorative body/sensory detail, or narrative diversity.

Run `character_voice_dialogue_staging_check.md` when the task concerns dialogue, multi-character scenes, character voice, relationship memory, silence, interruptions, location staging, usable objects, tone, comedy, grief, or physical action.

Run `author_voice_fingerprint_check.md` when the task concerns author voice, voice DNA, style guide, writing sample analysis, voice match, personal style, or prose that sounds unlike the author.

Run `author_aligned_ghostwriter_draft.md` only when source/canon/scene controls are clear and the user asks for author-aligned drafting, ghostwriter-style drafting, or writing in the author's voice.

Run `general_chapter_feedback_matrix_check.md` when the task asks for general feedback plus chapter-by-chapter feedback, packet/arc/hồi review, or matrix-style review output.

Run `tracking_logic_ledger_check.md` when the task concerns logic continuity, state trace, knowledge state, object/residue/thread tracking, payoff debt, status/pass trace, downstream risk, or verify target.

Run `structural_spine_outline_preprose_check.md` when act/arc/hồi/chapter/scene, Story Outline, Chapter by Chapter Outline, Chapter Card, Scene Packet, borderbound, or prose permission is in scope.

Run `vietnamese_senior_editor_surface_check.md` when senior Vietnamese reading, từng chữ, semantic load, repeated AI smell, pass metadata, Human Chapter Pass, candidate-ready, or Publication Lock is in scope.

Run `human_surface_polish_pass.md` when exact prose is source-safe and story/voice constraints are settled enough, but the passage still reads synthetic, over-clean, falsely smooth, same-voiced, symbol-first, or human-surface thin. Do not use it for detector bypass, structure repair, canon repair, or readiness.
