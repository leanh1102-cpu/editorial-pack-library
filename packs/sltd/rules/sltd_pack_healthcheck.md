# SLTD Pack Healthcheck

Use this rule to check SLTD pack health after version changes.

This is a manual agent check. It does not create management artifacts.

## Check manifest

Verify version, required files, allowed tasks, source priority, and fail-closed status.

## Check source fidelity

Verify source fidelity rule and source surface prompt exist and exact prose/status routes require source surface before patching or verdict.

## Check character voice, dialogue, relationship memory, and location staging

Verify:

- `rules/sltd_character_voice_dialogue_relationship_location_gate.md` exists and is listed in manifest;
- `prompts/character_voice_dialogue_staging_check.md` exists and is listed in manifest;
- `samples/character_voice_dialogue_staging_calibration.md` exists and is listed in manifest;
- character_voice_dialogue_staging_check is listed in allowed_tasks;
- voice/staging route ends with node checkpoint;
- rewrite, readiness, packet review, and matrix routes call the gate when dialogue, relationship, multi-character presence, location staging, or tone integrity is at stake;
- the gate defines character voice, dialogue weight, unsaid content, relationship memory, presence trace, location stage, usable objects, task-while-speaking, and tone integrity;
- the gate blocks same-voice dialogue, static talk, character dropout, silence without reason, missing relationship memory, location as backdrop, vague scene input, and style-mismatched sound/action handling;
- the gate does not authorize invented voice profiles, relationships, secrets, habits, location objects, or canon.

## Check general + chapter feedback matrix

Verify matrix rule/prompt/sample exist, task is allowed, route ends with node checkpoint, and matrix output requires source used, source status, general feedback, chapter feedback, evidence check, node ledger, and next node.

## Check tracking, structural spine, Vietnamese surface, supernatural residue, and protagonist route

Verify these gates remain listed and routed when their scope is in play.

## Check route governance

Verify one primary route before secondary gates, evidence-backed secondary gates, explicit stop conditions, and no gate cascade.

## Check orphan risk

Mark a file as possible orphan when it exists but is not listed in manifest, is listed but cannot be fetched, defines a task with no route, duplicates another rule without reason, or is missing from its route.

## Output labels

```text
PACK_HEALTH_OK
PACK_HEALTH_WARN
PACK_HEALTH_FAIL
```
