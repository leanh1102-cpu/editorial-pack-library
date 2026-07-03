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

Verify Narrative Claim Verification rule/prompt/sample exist, task is allowed, Entry and Router place it after Source/Context and before prose/readiness/lock/canon verdict when claims control the route, and route governance blocks claim verification from becoming readiness, lock, detector scoring, or gate cascade.

## Check multi-constraint instruction ledger and Suri discipline

Verify Multi-Constraint Ledger rule/prompt/sample exist, task is allowed, Entry and Router place it after Source/Context/Claim Verification and before rewrite, author-aligned drafting, human surface polish, readiness, or lock when multiple constraints control output, and the gate blocks unnamed constraints, missing corrupted constraints, conflicts, missing anchors, and AI constraint satisfaction as Human Chapter Pass.

## Check editorial harm anticipation and AHA vignette matrix

Verify:

- `rules/sltd_editorial_harm_anticipation_aha_vignette_matrix.md` exists and is listed in manifest;
- `prompts/editorial_harm_anticipation_check.md` exists and is listed in manifest;
- `samples/editorial_harm_anticipation_calibration.md` exists and is listed in manifest;
- `editorial_harm_anticipation_check` is listed in allowed_tasks;
- Entry Fast Path places Editorial Harm Anticipation after Source/Context/Claim Verification/Multi-Constraint when harm risk is in scope and before large rewrite, REDTEAM/PREMORTEM, readiness, lock, or packet decision;
- task router has a dedicated editorial harm route and can call it from context capsule, claim verification, multi-constraint ledger, narrative feature, character voice, author writing sheet, author drafting, matrix, tracking, structural, senior surface, human surface, readiness, and packet routes only when evidence requires it;
- route governance defines budget and stop conditions so harm anticipation does not become review overload, prose repair, Human Chapter Pass, readiness, or Publication Lock;
- role boundary contracts treat Editorial Harm Anticipation as AHA-style risk/vignette analysis, not source authority, canon authority, prose polish, Human Chapter Pass, readiness, or publication lock;
- the gate blocks missing scope, missing source for current/readiness/lock claims, invented canon vignettes, unverified harm claims, matrix overload, and harm anticipation as readiness substitute;
- the gate does not authorize new canon, invented future events, Human Chapter Pass, Publication Lock, workflows, scripts, reports, boards, automations, or live manuscript copies.

## Check narrative feature and structural idiosyncrasy discipline

Verify Narrative Feature rule/prompt/sample exist, task is allowed, and Entry/Router place it before draft, line surgery, human surface polish, copyedit, readiness, or publication lock when story-decision AI smell is in scope.

## Check author writing sheet and claim-evidence style memory

Verify Author Writing Sheet rule/prompt/sample exist, task is allowed, Entry places it before Author Voice Fingerprint and Author-Aligned Drafting when style claims or prompt-specific story rules are in scope, and it blocks style claims without evidence, chat-memory-only samples, generated-only samples, phrase mining, author voice over character voice, and style-memory canon drift.

## Check author voice fingerprint and ghostwriter discipline

Verify Author Voice / Author-Aligned Drafting files exist, tasks are allowed, Author Voice Fingerprint follows Author Writing Sheet when style evidence is needed, and these roles cannot override source, canon, POV, character voice, Human Chapter Pass, or Publication Lock.

## Check human surface polish and anti-synthetic prose discipline

Verify Human Surface Polish files exist, task is allowed, route runs after source/context/story/voice/style/constraint/harm blockers, and it cannot authorize new canon, scene outcome changes, readiness, Human Chapter Pass, Publication Lock, workflows, scripts, reports, boards, automations, or live manuscript copies.

## Check role boundary and role entry index

Verify Role Entry Index and role boundary contracts include Context Capsule, Narrative Claim Verifier, Multi-Constraint Instruction Ledger, Editorial Harm Anticipation, Narrative Feature Auditor, Author Writing Sheet, Author Voice Fingerprint, Author-Aligned Drafting, and Human Surface Polish boundaries, and still prevent silent Notion/GitHub/source writes and role mixing.

## Check character voice, dialogue, relationship memory, and location staging

Verify voice/staging files exist, task is allowed, route ends with node checkpoint, and rewrite/readiness/packet/matrix routes call the gate when dialogue, relationship, multi-character presence, location staging, or tone integrity is at stake.

## Check general + chapter feedback matrix

Verify matrix rule/prompt/sample exist, task is allowed, route ends with node checkpoint, and matrix output requires source used, source status, general feedback, chapter feedback, evidence check, node ledger, and next node.

## Check tracking, structural spine, Vietnamese surface, supernatural residue, and protagonist route

Verify these gates remain listed and routed when their scope is in play.

## Check route governance

Verify one primary route before secondary gates, evidence-backed secondary gates, explicit stop conditions, context capsule requirements, claim verification requirements, multi-constraint ledger requirements, editorial harm requirements, narrative feature requirements, author writing sheet requirements, author voice / drafting requirements, human surface polish requirements, and no gate cascade.

## Check orphan risk

Mark a file as possible orphan when it exists but is not listed in manifest, is listed but cannot be fetched, defines a task with no route, duplicates another rule without reason, or is missing from its route.

## Output labels

```text
PACK_HEALTH_OK
PACK_HEALTH_WARN
PACK_HEALTH_FAIL
```