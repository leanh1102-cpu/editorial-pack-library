# SLTD Role Entry Index

This index is the entry point for role-specific editorial work.

Use it when a user names a role directly or when task routing needs a precise role card.

Role entry cards do not replace `rules/sltd_role_boundary_contracts.md`. They are short doors into each role, while the boundary file remains the authority for role limits.

Context Capsule is not a role card. It is a pre-role source/context gate used when current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope.

Narrative Claim Verifier may be routed as a prompt-based evidence/source role. It is not readiness, canon authority, prose polish, or publication lock authority.

Narrative Feature Auditor may be routed as a prompt-based structural-story role. It is not an AI detector, canon authority, prose polish role, or readiness authority.

Author Writing Sheet may be routed as a prompt-based claim-evidence style memory role. It is not canon authority, character voice authority, readiness, or publication lock authority.

Author Voice Fingerprint and Author-Aligned Drafting Assistant may be routed as roles through boundary contracts and prompts. They do not become authorial authority, canon authority, character voice authority, or readiness authority.

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
Narrative Claim Verifier -> prompts/narrative_claim_verification_check.md + rules/sltd_narrative_claim_verification_clipper_discipline.md
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
6. Run narrative claim verification when status/canon/continuity/POV/object/reveal/readiness/lock/source-conflict claims need TRUE/FALSE/UNCERTAIN evidence.
7. Run narrative feature audit before surface repair when story-decision AI smell, thematic overexplicitness, causal tidiness, weak reveal, decorative body/sensory pressure, or narrative diversity is in scope.
8. Run author writing sheet when style claims, sample-backed author profile, or prompt-specific story rules need claim-evidence support.
9. Run author voice fingerprint before author-aligned drafting when style matching is in scope.
10. Read the requested role card or prompt-routed role.
11. Read source/evidence files needed by the role.
12. Execute the smallest safe task.
13. End with node checkpoint or result report.
```

## Conflict rule

If a role card and role boundary contracts disagree, use `rules/sltd_role_boundary_contracts.md`.

If Context Capsule blocks, do not continue into a later role to hide the source/context failure.

If Narrative Claim Verification returns UNCERTAIN or disproves a status/lock/readiness/canon claim, do not continue into readiness, Publication Lock, or prose repair to hide the evidence failure.

If Narrative Feature Audit blocks because story-decision smell remains unresolved, do not continue into Human Surface Polish, Copyedit, Readiness, or Publication Lock to hide the structural failure.

If Author Writing Sheet blocks because author samples or style evidence are missing, do not use style adjectives or chat memory as a substitute.

If Author Voice Fingerprint blocks because samples are missing, do not draft from chat memory or plausible style.

If Author-Aligned Drafting would change canon, scene function, POV, character voice, outcome, or reveal timing, stop and hand back.

If a later role finds an earlier-layer blocker, stop and hand back.

## Output

```text
ROLE ENTRY
REQUEST:
ACTIVE ROLE:
ROLE CARD / PROMPT READ:
BOUNDARY READ:
CONTEXT CAPSULE REQUIRED:
CONTEXT CAPSULE STATUS:
CLAIM VERIFICATION REQUIRED:
NARRATIVE FEATURE REQUIRED:
AUTHOR WRITING SHEET REQUIRED:
AUTHOR VOICE / DRAFTING REQUIRED:
SOURCE READY:
ROUTE:
OUTPUT:
HANDOFF:
```