# SLTD Pack Healthcheck

Use this rule to check SLTD pack health after version changes.

This is a manual agent check. It does not create management artifacts.

## Check manifest

Verify version, required files, allowed tasks, source priority, and fail-closed status.

## Check source fidelity

Verify source fidelity rule and source surface prompt exist and exact prose/status routes require source surface before patching or verdict.

## Check context capsule and lore retrieval discipline

Verify:

- `rules/sltd_context_capsule_lore_retrieval_discipline.md` exists and is listed in manifest;
- `prompts/context_capsule_preflight.md` exists and is listed in manifest;
- `samples/context_capsule_calibration.md` exists and is listed in manifest;
- `context_capsule_preflight` is listed in allowed_tasks;
- Entry Fast Path places Context Capsule after Source Preflight and before Spine, Tracking, Voice/Staging, Rewrite, Matrix, and Readiness when source status or long-range context is in scope;
- task router calls Context Capsule for current/latest source, Notion current manuscript, lock, readiness, Publication Lock, Human Chapter Pass, packet verdict, canon conflict, hidden canon, POV knowledge, legacy source risk, summary-vs-source risk, and long-range continuity;
- route governance requires Context Capsule before downstream gates when current source, hidden canon, POV knowledge, source-status separation, or long-range continuity is in scope;
- role boundary contracts require Context Capsule before later roles when source/context scope needs it;
- the gate blocks chat memory, summary, raw draft, legacy source, hidden canon leakage, unclear POV knowledge, unclear object/location/body/debt state, and unresolved canon conflict from becoming prose or verdict;
- the gate does not authorize autonomous lore updates, new canon, new databases, workflows, scripts, reports, project boards, automations, or live manuscript copies in GitHub.

## Check human surface polish and anti-synthetic prose discipline

Verify:

- `rules/sltd_human_surface_polish_anti_synthetic_gate.md` exists and is listed in manifest;
- `prompts/human_surface_polish_pass.md` exists and is listed in manifest;
- `samples/human_surface_polish_calibration.md` exists and is listed in manifest;
- `human_surface_polish_pass` is listed in allowed_tasks;
- Entry Fast Path places Human Surface Polish after source/context/structure/tracking/voice/Vietnamese surface blockers and before copyedit, proofread, readiness, or publication lock;
- task router has a dedicated human surface polish route and can call it in readiness only when source-safe prose still has synthetic-surface risk;
- route governance defines budget and stop conditions so Human Surface Polish does not become gate cascade, detector bypass, structure repair, or over-polish;
- role boundary contracts treat Human Surface Polish as a role between Line Surgery and Copyeditor;
- the gate blocks detector-bypass framing, false smoothing, same-voice polish, object/body loss, relationship flattening, hidden canon leak, and repair load above 30 percent;
- the gate does not authorize new canon, scene outcome changes, readiness, Human Chapter Pass, Publication Lock, workflows, scripts, reports, boards, automations, or live manuscript copies.

## Check role boundary and role entry index

Verify:

- `ROLE_ENTRY_INDEX.md` exists and is listed in manifest;
- `rules/sltd_role_boundary_contracts.md` exists and is listed in manifest;
- Role Entry Index states Context Capsule is not a role card and must run before role cards when current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope;
- role boundary contracts include Context Capsule in the global contract, role order, key role READ BEFORE / STOP WHEN clauses, learning boundary, and role-boundary output;
- role boundaries still prevent silent Notion/GitHub/source writes and role mixing.

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

Verify one primary route before secondary gates, evidence-backed secondary gates, explicit stop conditions, context capsule requirements when needed, human surface polish requirements when needed, and no gate cascade.

## Check orphan risk

Mark a file as possible orphan when it exists but is not listed in manifest, is listed but cannot be fetched, defines a task with no route, duplicates another rule without reason, or is missing from its route.

## Output labels

```text
PACK_HEALTH_OK
PACK_HEALTH_WARN
PACK_HEALTH_FAIL
```
