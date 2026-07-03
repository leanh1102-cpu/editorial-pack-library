# SLTD Pack Healthcheck

Use this rule to check SLTD pack health after version changes.

This is a manual agent check. It does not create management artifacts.

## Check manifest

Verify version, required files, allowed tasks, source priority, and fail-closed status.

## Check source fidelity

Verify source fidelity rule and source surface prompt exist and exact prose/status routes require source surface before patching or verdict.

## Check context capsule and lore retrieval discipline

Verify Context Capsule files exist, task is allowed, Entry and Router place Context Capsule after Source Preflight and before downstream roles when current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope.

## Check narrative claim verification and CLIPPER discipline

Verify:

- `rules/sltd_narrative_claim_verification_clipper_discipline.md` exists and is listed in manifest;
- `prompts/narrative_claim_verification_check.md` exists and is listed in manifest;
- `samples/narrative_claim_verification_calibration.md` exists and is listed in manifest;
- `narrative_claim_verification_check` is listed in allowed_tasks;
- Entry and Router place Narrative Claim Verification after Source/Context and before prose, readiness, lock, or canon verdict when claims control the route;
- route governance blocks claim verification from becoming readiness, lock, detector scoring, or gate cascade.

## Check multi-constraint instruction ledger and Suri discipline

Verify:

- `rules/sltd_multi_constraint_instruction_ledger_suri_discipline.md` exists and is listed in manifest;
- `prompts/multi_constraint_instruction_check.md` exists and is listed in manifest;
- `samples/multi_constraint_instruction_calibration.md` exists and is listed in manifest;
- `multi_constraint_instruction_check` is listed in allowed_tasks;
- Entry Fast Path places Multi-Constraint Instruction Ledger after Source/Context/Claim Verification and before rewrite, author-aligned drafting, human surface polish, readiness, or lock when multiple constraints control output;
- task router has a dedicated multi-constraint route and can call it from context capsule, claim verification, narrative feature, voice, author writing sheet, author drafting, matrix, tracking, structural, senior surface, human surface, readiness, and packet routes only when evidence requires it;
- route governance defines budget and stop conditions so the ledger does not become gate cascade or AI self-approval;
- role boundary contracts treat Multi-Constraint Instruction Ledger as constraint tracking, not source authority, canon authority, prose polish, Human Chapter Pass, readiness, or Publication Lock;
- the gate blocks unnamed constraints, missing corrupted constraints, constraint conflicts, missing output anchors, uncertain high-risk constraints, wordcount overrepair, and AI constraint satisfaction as Human Chapter Pass;
- the gate does not authorize new canon, invented source constraints, Human Chapter Pass, Publication Lock, workflows, scripts, reports, boards, automations, or live manuscript copies.

## Check narrative feature and structural idiosyncrasy discipline

Verify:

- `rules/sltd_narrative_feature_structural_idiosyncrasy_audit.md` exists and is listed in manifest;
- `prompts/narrative_feature_audit.md` exists and is listed in manifest;
- `samples/narrative_feature_calibration.md` exists and is listed in manifest;
- `narrative_feature_audit` is listed in allowed_tasks;
- Entry and Router place Narrative Feature Audit before draft, line surgery, human surface polish, copyedit, readiness, or publication lock when story-decision AI smell is in scope.

## Check author writing sheet and claim-evidence style memory

Verify:

- `rules/sltd_author_writing_sheet_claim_evidence_discipline.md` exists and is listed in manifest;
- `prompts/author_writing_sheet_check.md` exists and is listed in manifest;
- `samples/author_writing_sheet_calibration.md` exists and is listed in manifest;
- `author_writing_sheet_check` is listed in allowed_tasks;
- Entry Fast Path places Author Writing Sheet before Author Voice Fingerprint and Author-Aligned Drafting when style claims or prompt-specific story rules are in scope;
- the gate blocks style claims without evidence, chat-memory-only samples, generated-only samples, plot/development claims with weak evidence, phrase mining, author voice over character voice, and style-memory canon drift.

## Check author voice fingerprint and ghostwriter discipline

Verify Author Voice / Author-Aligned Drafting files exist, tasks are allowed, Author Voice Fingerprint follows Author Writing Sheet when style evidence is needed, and these roles cannot override source, canon, POV, character voice, Human Chapter Pass, or Publication Lock.

## Check human surface polish and anti-synthetic prose discipline

Verify Human Surface Polish files exist, task is allowed, route runs after source/context/story/voice/style/constraint blockers, and it cannot authorize new canon, scene outcome changes, readiness, Human Chapter Pass, Publication Lock, workflows, scripts, reports, boards, automations, or live manuscript copies.

## Check role boundary and role entry index

Verify Role Entry Index and role boundary contracts include Context Capsule, Narrative Claim Verifier, Multi-Constraint Instruction Ledger, Narrative Feature Auditor, Author Writing Sheet, Author Voice Fingerprint, Author-Aligned Drafting, and Human Surface Polish boundaries, and still prevent silent Notion/GitHub/source writes and role mixing.

## Check character voice, dialogue, relationship memory, and location staging

Verify voice/staging files exist, task is allowed, route ends with node checkpoint, and rewrite/readiness/packet/matrix routes call the gate when dialogue, relationship, multi-character presence, location staging, or tone integrity is at stake.

## Check general + chapter feedback matrix

Verify matrix rule/prompt/sample exist, task is allowed, route ends with node checkpoint, and matrix output requires source used, source status, general feedback, chapter feedback, evidence check, node ledger, and next node.

## Check tracking, structural spine, Vietnamese surface, supernatural residue, and protagonist route

Verify these gates remain listed and routed when their scope is in play.

## Check route governance

Verify one primary route before secondary gates, evidence-backed secondary gates, explicit stop conditions, context capsule requirements, claim verification requirements, multi-constraint ledger requirements, narrative feature requirements, author writing sheet requirements, author voice / drafting requirements, human surface polish requirements, and no gate cascade.

## Check orphan risk

Mark a file as possible orphan when it exists but is not listed in manifest, is listed but cannot be fetched, defines a task with no route, duplicates another rule without reason, or is missing from its route.

## Output labels

```text
PACK_HEALTH_OK
PACK_HEALTH_WARN
PACK_HEALTH_FAIL
```