# SLTD Pack Healthcheck

Use this rule to check SLTD pack health after version changes.

This is a manual agent check. It does not create management artifacts.

## Check manifest

Verify version, required files, allowed tasks, source priority, and fail-closed status.

## Check source fidelity

Verify source fidelity rule and source surface prompt exist and exact prose/status routes require source surface before patching or verdict.

## Check context capsule and lore retrieval discipline

Verify Context Capsule files exist, task is allowed, Entry and Router place Context Capsule after Source Preflight and before downstream roles when current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope.

## Check reference-anchored longform story quality and POLARIS discipline

Verify:

- `rules/sltd_reference_anchored_longform_quality_polaris_discipline.md` exists and is listed in manifest;
- `prompts/reference_anchored_story_quality_check.md` exists and is listed in manifest;
- `samples/reference_anchored_story_quality_calibration.md` exists and is listed in manifest;
- `reference_anchored_story_quality_check` is listed in allowed_tasks;
- Entry Fast Path routes Reference-Anchored Longform Story Quality after Source/Context/Claim/Constraint/Harm/Topic when quality across length is in scope;
- Task Router has a dedicated route for long rewrite, chapter assembly, packet candidate, length adherence, bloat, drift, over-summary, over-explanation, and late-output collapse;
- Route Governance blocks quality-score overreach and prevents longform quality from becoming source truth, rewrite permission, Human Chapter Pass, readiness, or Publication Lock;
- Role Boundary treats Reference-Anchored Longform Story Quality as a quality stress test, not source authority, canon authority, prose polish, or readiness;
- the gate blocks source missing, output missing, unauthorized anchor, Must Show cut for length, wordcount padding, bloat, local coherence failure, late-output collapse, and quality-as-readiness;
- the gate does not authorize training, fine-tuning, scraping, protected-text copying, workflows, scripts, reports, boards, automations, or live manuscript copies.

## Check corpus topic / thread discovery and TopicGPT discipline

Verify Corpus Topic / Thread Discovery rule/prompt/sample exist, task is allowed, routes are map-level only, quote/evidence anchors are required, and topic maps do not authorize readiness, lock, canon verdict, or rewrite permission.

## Check narrative claim verification and CLIPPER discipline

Verify Narrative Claim Verification rule/prompt/sample exist, task is allowed, Entry and Router place it after Source/Context and before prose/readiness/lock/canon verdict when claims control the route, and route governance blocks claim verification from becoming readiness, lock, detector scoring, or gate cascade.

## Check multi-constraint instruction ledger and Suri discipline

Verify Multi-Constraint Ledger rule/prompt/sample exist, task is allowed, Entry and Router place it after Source/Context/Claim Verification and before rewrite, author-aligned drafting, human surface polish, readiness, or lock when multiple constraints control output, and the gate blocks unnamed constraints, missing corrupted constraints, conflicts, missing anchors, and AI constraint satisfaction as Human Chapter Pass.

## Check editorial harm anticipation and AHA vignette matrix

Verify Editorial Harm rule/prompt/sample exist, task is allowed, Entry and Router place it after Source/Context/Claim Verification/Multi-Constraint when harm risk is in scope and before large rewrite, REDTEAM/PREMORTEM, readiness, lock, or packet decision, and the gate blocks missing scope, missing source, invented canon vignettes, unverified harm claims, matrix overload, and harm anticipation as readiness substitute.

## Check narrative feature and structural idiosyncrasy discipline

Verify Narrative Feature rule/prompt/sample exist, task is allowed, and Entry/Router place it before draft, line surgery, human surface polish, copyedit, readiness, or publication lock when story-decision AI smell is in scope.

## Check author writing sheet and claim-evidence style memory

Verify Author Writing Sheet rule/prompt/sample exist, task is allowed, Entry places it before Author Voice Fingerprint and Author-Aligned Drafting when style claims or prompt-specific story rules are in scope, and it blocks style claims without evidence, chat-memory-only samples, generated-only samples, phrase mining, author voice over character voice, and style-memory canon drift.

## Check author voice fingerprint and drafting discipline

Verify Author Voice / Author-Aligned Drafting files exist, tasks are allowed, Author Voice Fingerprint follows Author Writing Sheet when style evidence is needed, and these roles cannot override source, canon, POV, character voice, Human Chapter Pass, or Publication Lock.

## Check human surface polish and anti-synthetic prose discipline

Verify Human Surface Polish files exist, task is allowed, route runs after source/context/story/voice/style/constraint/harm/topic-map/reference-quality blockers, and it cannot authorize new canon, scene outcome changes, readiness, Human Chapter Pass, Publication Lock, workflows, scripts, reports, boards, automations, or live manuscript copies.

## Check role boundary and role entry index

Verify Role Entry Index and role boundary contracts include Context Capsule, Reference-Anchored Longform Story Quality, Corpus Topic / Thread Discovery, Narrative Claim Verifier, Multi-Constraint Instruction Ledger, Editorial Harm Anticipation, Narrative Feature Auditor, Author Writing Sheet, Author Voice Fingerprint, Author-Aligned Drafting, and Human Surface Polish boundaries, and still prevent silent Notion/GitHub/source writes and role mixing.

## Check character voice, dialogue, relationship memory, and location staging

Verify voice/staging files exist, task is allowed, route ends with node checkpoint, and rewrite/readiness/packet/matrix routes call the gate when dialogue, relationship, multi-character presence, location staging, or tone integrity is at stake.

## Check general + chapter feedback matrix

Verify matrix rule/prompt/sample exist, task is allowed, route ends with node checkpoint, and matrix output requires source used, source status, general feedback, chapter feedback, evidence check, node ledger, and next node.

## Check tracking, structural spine, Vietnamese surface, supernatural residue, and protagonist route

Verify these gates remain listed and routed when their scope is in play.

## Check route governance

Verify one primary route before secondary gates, evidence-backed secondary gates, explicit stop conditions, context capsule requirements, reference quality requirements, corpus topic/thread requirements, claim verification requirements, multi-constraint ledger requirements, editorial harm requirements, narrative feature requirements, author writing sheet requirements, author voice / drafting requirements, human surface polish requirements, and no gate cascade.

## Check orphan risk

Mark a file as possible orphan when it exists but is not listed in manifest, is listed but cannot be fetched, defines a task with no route, duplicates another rule without reason, or is missing from its route.

## Output labels

```text
PACK_HEALTH_OK
PACK_HEALTH_WARN
PACK_HEALTH_FAIL
```