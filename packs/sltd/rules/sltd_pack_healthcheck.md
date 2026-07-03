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
- task router has a dedicated author writing sheet route and can call it from author voice, author drafting, packet, readiness, character voice, and human surface routes only when evidence requires it;
- route governance defines budget and stop conditions so Author Writing Sheet does not become style overfitting or gate cascade;
- role boundary contracts treat Author Writing Sheet as claim-evidence style memory, not canon authority, character voice authority, readiness, or publication lock;
- the gate blocks style claims without evidence, chat-memory-only samples, generated-only samples, plot/development claims with weak evidence, phrase mining, author voice over character voice, and style-memory canon drift;
- the gate does not authorize new canon, scene outcome changes, Notion/GitHub/source writes, workflows, scripts, reports, boards, automations, or live manuscript copies.

## Check author voice fingerprint and ghostwriter discipline

Verify:

- `rules/sltd_author_voice_fingerprint_ghostwriter_discipline.md` exists and is listed in manifest;
- `prompts/author_voice_fingerprint_check.md` exists and is listed in manifest;
- `prompts/author_aligned_ghostwriter_draft.md` exists and is listed in manifest;
- `samples/author_voice_fingerprint_calibration.md` exists and is listed in manifest;
- `author_voice_fingerprint_check` and `author_aligned_ghostwriter_draft` are listed in allowed_tasks;
- Entry Fast Path places Author Voice Fingerprint after Author Writing Sheet when style claims need evidence and before Author-Aligned Drafting / Human Surface Polish;
- task router has dedicated routes for author voice fingerprint and author-aligned drafting;
- role boundary contracts treat Author Voice Fingerprint and Author-Aligned Drafting as bounded roles that do not override source, canon, POV, character voice, Human Chapter Pass, or Publication Lock.

## Check human surface polish and anti-synthetic prose discipline

Verify Human Surface Polish files exist, task is allowed, route runs after source/context/story/voice/style blockers, and it cannot authorize new canon, scene outcome changes, readiness, Human Chapter Pass, Publication Lock, workflows, scripts, reports, boards, automations, or live manuscript copies.

## Check role boundary and role entry index

Verify Role Entry Index and role boundary contracts include Context Capsule, Narrative Claim Verifier, Narrative Feature Auditor, Author Writing Sheet, Author Voice Fingerprint, Author-Aligned Drafting, and Human Surface Polish boundaries, and still prevent silent Notion/GitHub/source writes and role mixing.

## Check character voice, dialogue, relationship memory, and location staging

Verify voice/staging files exist, task is allowed, route ends with node checkpoint, and rewrite/readiness/packet/matrix routes call the gate when dialogue, relationship, multi-character presence, location staging, or tone integrity is at stake.

## Check general + chapter feedback matrix

Verify matrix rule/prompt/sample exist, task is allowed, route ends with node checkpoint, and matrix output requires source used, source status, general feedback, chapter feedback, evidence check, node ledger, and next node.

## Check tracking, structural spine, Vietnamese surface, supernatural residue, and protagonist route

Verify these gates remain listed and routed when their scope is in play.

## Check route governance

Verify one primary route before secondary gates, evidence-backed secondary gates, explicit stop conditions, context capsule requirements, claim verification requirements, narrative feature requirements, author writing sheet requirements, author voice / drafting requirements, human surface polish requirements, and no gate cascade.

## Check orphan risk

Mark a file as possible orphan when it exists but is not listed in manifest, is listed but cannot be fetched, defines a task with no route, duplicates another rule without reason, or is missing from its route.

## Output labels

```text
PACK_HEALTH_OK
PACK_HEALTH_WARN
PACK_HEALTH_FAIL
```