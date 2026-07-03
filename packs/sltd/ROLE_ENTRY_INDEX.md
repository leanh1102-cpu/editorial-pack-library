# SLTD Role Entry Index

This index is the entry point for role-specific editorial work.

Role entry cards do not replace `rules/sltd_role_boundary_contracts.md`.

Context Capsule is a pre-role source/context gate.

Reference-Anchored Longform Story Quality is a prompt-routed quality stress-test role. It is not source authority, canon authority, prose polish, rewrite permission, Human Chapter Pass, readiness, or Publication Lock.

Corpus Topic / Thread Discovery is a prompt-routed map-level navigation role. It is not source authority, canon authority, prose polish, rewrite permission, Human Chapter Pass, readiness, or Publication Lock.

Narrative Claim Verifier checks TRUE / FALSE / UNCERTAIN claims. Multi-Constraint Instruction Ledger tracks output constraints. Editorial Harm Anticipation builds REDTEAM/PREMORTEM vignettes. Narrative Feature Auditor checks story-decision smell. Author Writing Sheet builds evidence-backed style memory. Author Voice Fingerprint and Author-Aligned Drafting remain bounded by source, canon, POV, character voice, constraints, and readiness rules. Human Surface Polish is not story repair or readiness.

## Role cards

```text
Canon Guard -> roles/canon_guard.md
Story Doctor -> roles/story_doctor.md
Intensity Editor -> roles/intensity_editor.md
Vietnamese Line Editor -> roles/vietnamese_line_editor.md
Line Surgery -> roles/line_surgery.md
Copyeditor -> roles/copyeditor.md
Proofreader -> roles/proofreader.md
Publishing Readiness Reviewer -> roles/publishing_readiness_reviewer.md
Editorial Director -> roles/editorial_director.md
```

## Prompt-routed roles without standalone role cards

```text
Reference-Anchored Longform Story Quality -> prompts/reference_anchored_story_quality_check.md + rules/sltd_reference_anchored_longform_quality_polaris_discipline.md
Corpus Topic / Thread Discovery -> prompts/corpus_topic_thread_discovery_check.md + rules/sltd_corpus_topic_thread_discovery_topicgpt_discipline.md
Narrative Claim Verifier -> prompts/narrative_claim_verification_check.md + rules/sltd_narrative_claim_verification_clipper_discipline.md
Multi-Constraint Instruction Ledger -> prompts/multi_constraint_instruction_check.md + rules/sltd_multi_constraint_instruction_ledger_suri_discipline.md
Editorial Harm Anticipation -> prompts/editorial_harm_anticipation_check.md + rules/sltd_editorial_harm_anticipation_aha_vignette_matrix.md
Narrative Feature Auditor -> prompts/narrative_feature_audit.md + rules/sltd_narrative_feature_structural_idiosyncrasy_audit.md
Author Writing Sheet -> prompts/author_writing_sheet_check.md + rules/sltd_author_writing_sheet_claim_evidence_discipline.md
Author Voice Fingerprint -> prompts/author_voice_fingerprint_check.md + rules/sltd_author_voice_fingerprint_ghostwriter_discipline.md
Author-Aligned Drafting Assistant -> prompts/author_aligned_ghostwriter_draft.md + rules/sltd_author_voice_fingerprint_ghostwriter_discipline.md
Human Surface Polish -> prompts/human_surface_polish_pass.md + rules/sltd_human_surface_polish_anti_synthetic_gate.md
```

## Use rule

```text
1. Read manifest and boot path.
2. Read this index.
3. Read role boundary contracts.
4. Run source preflight / source surface as required.
5. Run context capsule preflight when current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope.
6. Run reference-anchored longform story quality when long rewrite/chapter/packet quality, length adherence, bloat, drift, over-summary, or late-output collapse needs source-backed stress testing.
7. Run corpus topic / thread discovery when packet/arc/series map, motif clusters, repeated pattern clusters, topic gaps, or thread drift need quote/evidence anchors.
8. Run claim verification, multi-constraint ledger, harm anticipation, narrative feature audit, author writing sheet, author voice, drafting, or human surface only when their source/evidence scope is actually in play.
9. End with node checkpoint or result report.
```

## Conflict rule

If Reference-Anchored Longform Story Quality blocks because source, output, anchor authorization, Must Show source, or exact output is missing, do not use the quality check as readiness, lock, canon verdict, or rewrite permission.

If Corpus Topic / Thread Discovery blocks, do not use the topic map as readiness, canon verdict, or rewrite permission.

If Claim Verification, Multi-Constraint Ledger, Editorial Harm Anticipation, Narrative Feature Audit, Author Writing Sheet, or Author Voice blocks, do not continue into later roles to hide that failure.

If Author-Aligned Drafting would change canon, scene function, POV, character voice, outcome, or reveal timing, stop and hand back.

## Output

```text
ROLE ENTRY
REQUEST:
ACTIVE ROLE:
ROLE CARD / PROMPT READ:
BOUNDARY READ:
CONTEXT CAPSULE REQUIRED:
CONTEXT CAPSULE STATUS:
REFERENCE-ANCHORED STORY QUALITY REQUIRED:
CORPUS TOPIC / THREAD DISCOVERY REQUIRED:
CLAIM VERIFICATION REQUIRED:
MULTI-CONSTRAINT LEDGER REQUIRED:
EDITORIAL HARM ANTICIPATION REQUIRED:
NARRATIVE FEATURE REQUIRED:
AUTHOR WRITING SHEET REQUIRED:
AUTHOR VOICE / DRAFTING REQUIRED:
SOURCE READY:
ROUTE:
OUTPUT:
HANDOFF:
```