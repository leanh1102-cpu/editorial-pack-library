# SLTD Pack Healthcheck

Use this rule to check the health of the SLTD pack after version changes.

This is a manual agent check. It does not create scripts, workflow files, issues, boards, or reports.

## Check manifest

Verify:

- manifest version matches the requested release;
- every new file is listed in `required_files`;
- every new task is listed in `allowed_tasks`;
- no forbidden task was added;
- priority order still keeps current user instruction and Notion live source above the pack.

## Check entries

Verify root entry, pack entry, runtime entry, fast path, and role entry index.

## Check source fidelity

Verify source fidelity rule and source surface prompt exist, are listed in manifest, and line-level routes require exact source surface before patching.

## Check scene-first prose judgment

Verify:

- `rules/sltd_scene_first_prose_judgment_gate.md` exists and is listed in manifest;
- `prompts/scene_first_prose_judgment.md` exists and is listed in manifest;
- scene_first_prose_judgment is listed in allowed_tasks;
- scene-first route ends with node checkpoint;
- scene-first route references source fidelity before patching;
- scene-first gate requires one governing scene pressure before repair;
- scene-first gate treats checklist as later verification, not the writing method;
- scene-first gate prevents adding required-looking body/object/silence/cost beats to hide checklist-first prose.

## Check anti-AI composite

Verify:

- `rules/sltd_anti_ai_composite_failure_gate.md` exists and is listed in manifest;
- `prompts/anti_ai_composite_check.md` exists and is listed in manifest;
- anti_ai_composite_check is listed in allowed_tasks;
- anti-AI composite route ends with node checkpoint;
- anti-AI composite route references source fidelity before patching;
- anti-AI composite gate checks scene-card visibility, object force, dialogue duty, narrator voice, consequence trace, repair collage, false human texture, and readiness conflict;
- anti-AI composite gate prevents adding more texture to hide synthetic structure;
- anti-AI composite gate does not authorize canon invention or readiness claims from green sub-passes alone.

## Check character agency

Verify character agency rule and prompt exist, task is allowed, route ends with node checkpoint, source fidelity is respected, and want/fear/knowledge limit/pressure/choice/visible cost are checked.

## Check dynamic range

Verify dynamic range rule and prompt exist, task is allowed, route ends with node checkpoint, source fidelity is respected, and cadence/pressure are not flattened.

## Check handoff continuity

Verify handoff continuity rule is listed, session_handoff reads it, handoff route ends with node checkpoint, and handoff is navigation rather than source truth.

## Check role entry cards

Required role cards:

```text
roles/canon_guard.md
roles/story_doctor.md
roles/intensity_editor.md
roles/vietnamese_line_editor.md
roles/line_surgery.md
roles/copyeditor.md
roles/proofreader.md
roles/publishing_readiness_reviewer.md
roles/editorial_director.md
```

Each role card must have role, trigger, read-first list, source required, run, do, do not, output, done, handoff, and fail-closed.

## Check iteration loop

Verify iteration loop and checkpoint are listed, route ends with node checkpoint, and the loop requires source, scope, role, route, verification gate, and stop condition.

## Check calibration cases

Verify calibration discipline and sample files are listed, calibration route ends with node checkpoint, and calibration remains example data rather than canon/current manuscript.

Required calibration files:

```text
samples/line_surgery_calibration.md
samples/dialogue_voice_calibration.md
samples/underreach_calibration.md
samples/readiness_false_positive.md
```

## Check routes

Verify each allowed task has a route or prompt, large routes use context brief when needed, node-changing routes end with node checkpoint or result report, and routes reference their required gate files:

```text
source-surface routes -> sltd_source_fidelity_anti_compression.md
scene-first routes -> sltd_scene_first_prose_judgment_gate.md
anti-AI composite routes -> sltd_anti_ai_composite_failure_gate.md
character agency routes -> sltd_character_agency_anti_ooc_gate.md
dynamic range routes -> sltd_dynamic_range_cadence_gate.md
handoff routes -> sltd_handoff_continuity_protocol.md
```

## Check role boundaries

Verify later roles do not overwrite earlier-layer blockers and learned taste/calibration/gates do not override current source, canon, evidence, or human lock.

## Check orphan risk

Mark a file as possible orphan when it exists but is not listed in manifest, is listed but cannot be fetched, defines a task with no route, duplicates another rule without reason, or is missing from its route.

## Output labels

```text
PACK_HEALTH_OK
PACK_HEALTH_WARN
PACK_HEALTH_FAIL
```

A warning does not block all work, but a fail blocks new skill expansion until fixed.
