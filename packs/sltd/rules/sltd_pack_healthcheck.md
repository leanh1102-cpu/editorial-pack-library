# SLTD Pack Healthcheck

Use this rule to check SLTD pack health after version changes.

This is a manual agent check. It does not create management artifacts.

## Check manifest

Verify version, required files, allowed tasks, source priority, and fail-closed status.

## Check source fidelity

Verify source fidelity rule and source surface prompt exist and exact prose/status routes require source surface before patching or verdict.

## Check context capsule and lore retrieval discipline

Verify Context Capsule files exist, task is allowed, Entry and Router place Context Capsule after Source Preflight and before downstream roles when current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope.

## Check human expert AI-smell explanation discipline

Verify the rule, prompt, and calibration sample exist, are listed in manifest, and `human_expert_ai_smell_explanation_check` is listed in allowed_tasks.

Verify Task Router and Role Entry Index route this as a span-based reader-effect explanation role for synthetic surface, same-voice dialogue, over-clean prose, outline labels, false-positive risk, and repair direction.

Verify the gate requires span, reason, false-positive risk, source/canon/voice separation, and next route; it must not become source truth, authorship verdict, detector score, rewrite permission, Human Chapter Pass, readiness, Publication Lock, or project-management artifact.

## Check multilingual long-context retrieval and OneRuler discipline

Verify Multilingual Long-Context Source Retrieval rule/prompt/sample exist, task is allowed, route blocks compressed-source-only not-found claims, chat-memory retrieval, legacy-source-as-current risk, aggregation without segments, cross-lingual retrieval risk, and Vietnamese source not checked.

## Check reference-anchored longform story quality and POLARIS discipline

Verify Reference-Anchored Longform Story Quality rule/prompt/sample exist, task is allowed, route is a quality stress test only, and it does not become source truth, rewrite permission, Human Chapter Pass, readiness, or Publication Lock.

## Check corpus topic / thread discovery and TopicGPT discipline

Verify Corpus Topic / Thread Discovery rule/prompt/sample exist, task is allowed, routes are map-level only, quote/evidence anchors are required, and topic maps do not authorize readiness, lock, canon verdict, or rewrite permission.

## Check narrative claim verification and CLIPPER discipline

Verify Narrative Claim Verification rule/prompt/sample exist, task is allowed, Entry and Router place it after Source/Context/Retrieval when claims control the route, and route governance blocks claim verification from becoming readiness, lock, detector scoring, or gate cascade.

## Check multi-constraint instruction ledger and Suri discipline

Verify Multi-Constraint Ledger rule/prompt/sample exist, task is allowed, Entry and Router place it after Source/Context/Retrieval/Claim Verification and before rewrite, author-aligned drafting, human surface polish, readiness, or lock when multiple constraints control output.

## Check editorial harm anticipation and AHA vignette matrix

Verify Editorial Harm rule/prompt/sample exist, task is allowed, Entry and Router place it after Source/Context/Retrieval/Claim Verification/Multi-Constraint when harm risk is in scope and before large rewrite, REDTEAM/PREMORTEM, readiness, lock, or packet decision.

## Check narrative feature and structural idiosyncrasy discipline

Verify Narrative Feature rule/prompt/sample exist, task is allowed, and Entry/Router place it before draft, line surgery, human surface polish, copyedit, readiness, or publication lock when story-decision AI smell is in scope.

## Check author writing sheet and claim-evidence style memory

Verify Author Writing Sheet rule/prompt/sample exist, task is allowed, Entry places it before Author Voice Fingerprint and Author-Aligned Drafting when style claims or prompt-specific story rules are in scope.

## Check author voice fingerprint and ghostwriter discipline

Verify Author Voice / Author-Aligned Drafting files exist, tasks are allowed, Author Voice Fingerprint follows Author Writing Sheet when style evidence is needed, and these roles cannot override source, canon, POV, character voice, Human Chapter Pass, or Publication Lock.

## Check human surface polish and anti-synthetic prose discipline

Verify Human Surface Polish files exist, task is allowed, route runs after source/context/retrieval/AI-smell explanation/story/voice/style/constraint/harm/topic-map/reference-quality blockers, and it cannot authorize new canon, scene outcome changes, readiness, Human Chapter Pass, Publication Lock, or project-management artifacts.

## Check role boundary and role entry index

Verify Role Entry Index includes Human Expert AI-Smell Explanation and the other prompt-routed roles where applicable, and role boundary contracts still prevent silent Notion/GitHub/source writes and role mixing.

## Check character voice, dialogue, relationship memory, and location staging

Verify voice/staging files exist, task is allowed, route ends with node checkpoint, and rewrite/readiness/packet/matrix routes call the gate when dialogue, relationship, multi-character presence, location staging, or tone integrity is at stake.

## Check general + chapter feedback matrix

Verify matrix rule/prompt/sample exist, task is allowed, route ends with node checkpoint, and matrix output requires source used, source status, general feedback, chapter feedback, evidence check, node ledger, and next node.

## Check tracking, structural spine, Vietnamese surface, supernatural residue, and protagonist route

Verify these gates remain listed and routed when their scope is in play.

## Check route governance

Verify one primary route before secondary gates, evidence-backed secondary gates, explicit stop conditions, context capsule requirements, retrieval requirements, AI-smell explanation requirements, reference quality requirements, corpus topic/thread requirements, claim verification requirements, multi-constraint ledger requirements, editorial harm requirements, narrative feature requirements, author writing sheet requirements, author voice / drafting requirements, human surface polish requirements, and no gate cascade.

## Check orphan risk

Mark a file as possible orphan when it exists but is not listed in manifest, is listed but cannot be fetched, defines a task with no route, duplicates another rule without reason, or is missing from its route.

## Output labels

```text
PACK_HEALTH_OK
PACK_HEALTH_WARN
PACK_HEALTH_FAIL
```