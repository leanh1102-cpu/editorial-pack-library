# SLTD Pack Healthcheck

Use this rule to check SLTD pack health after version changes.

This is a manual agent check. It does not create management artifacts.

## Check manifest

Verify version, required files, allowed tasks, source priority, and fail-closed status.

## Check source fidelity

Verify source fidelity rule and source surface prompt exist and exact prose/status routes require source surface before patching or verdict.

## Check context capsule and lore retrieval discipline

Verify Context Capsule files exist, task is allowed, and Router places Context Capsule before downstream roles when current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope.

## Check context memory lifecycle and ByteRover discipline

Verify the rule, prompt, and calibration sample exist, are listed in manifest, and `context_memory_lifecycle_check` is listed in allowed_tasks.

Verify Router and Role Entry Index route it as a provenance, maturity, recency, and source-truth-limit discipline for handoff, context brief, node ledger, route note, feedback delta, topic map, source-status note, and chat-memory reuse.

Verify it rejects context entries without provenance, stale handoff as current source, chat memory as source truth, legacy source as current without instruction, unsupported maturity labels, hidden recency risk, semantic drift, GitHub live manuscript memory, and management artifacts.

## Check comparative editorial feedback delta discipline

Verify Comparative Editorial Feedback Delta rule/prompt/sample exist, task is allowed, and route translates feedback into bounded increase/decrease/preserve/prohibit deltas without rewrite permission from feedback alone.

## Check human expert AI-smell explanation discipline

Verify Human Expert AI-Smell Explanation rule/prompt/sample exist, task is allowed, and route explains reader-facing synthetic effects without detector score, authorship accusation, or readiness authority.

## Check multilingual long-context retrieval and OneRuler discipline

Verify Multilingual Long-Context Source Retrieval rule/prompt/sample exist, task is allowed, and route guards against compressed-source-only not-found claims, chat-memory retrieval, legacy-source-as-current risk, aggregation without segments, cross-lingual retrieval risk, and Vietnamese source not checked.

## Check reference-anchored longform story quality and POLARIS discipline

Verify Reference-Anchored Longform Story Quality rule/prompt/sample exist, task is allowed, and route remains a quality stress test only.

## Check corpus topic / thread discovery and TopicGPT discipline

Verify Corpus Topic / Thread Discovery rule/prompt/sample exist, task is allowed, routes are map-level only, and quote/evidence anchors are required.

## Check claim, constraint, harm, feature, style, voice, surface, and tracking gates

Verify their files remain listed, routes remain present, and none of these gates becomes source truth, canon authority, rewrite permission, Human Chapter Pass, readiness, or Publication Lock.

## Check role boundary and role entry index

Verify Role Entry Index includes Context Memory Lifecycle and other prompt-routed roles where applicable, and role boundary contracts still prevent silent Notion/GitHub/source writes and role mixing.

## Check route governance

Verify one primary route before secondary gates, evidence-backed secondary gates, explicit stop conditions, context capsule requirements, context memory requirements, retrieval requirements, feedback delta requirements, AI-smell explanation requirements, reference quality requirements, corpus topic/thread requirements, claim verification requirements, multi-constraint ledger requirements, editorial harm requirements, narrative feature requirements, author writing sheet requirements, author voice / drafting requirements, human surface polish requirements, and no gate cascade.

## Check orphan risk

Mark a file as possible orphan when it exists but is not listed in manifest, is listed but cannot be fetched, defines a task with no route, duplicates another rule without reason, or is missing from its route.

## Output labels

```text
PACK_HEALTH_OK
PACK_HEALTH_WARN
PACK_HEALTH_FAIL
```