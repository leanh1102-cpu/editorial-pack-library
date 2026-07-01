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

## Check source fidelity

Verify source fidelity rule and source surface prompt exist, are listed in manifest, and line-level routes require exact source surface before patching.

## Check first-pass editorial workflow

Verify first-pass rule and prompt exist, task is allowed, route ends with node checkpoint, source fidelity is respected, and targeted gates run only after initial prose judgment.

## Check chapter assembly and split control

Verify chapter assembly rule and prompt exist, task is allowed, route ends with node checkpoint, source fidelity is respected, and it separates scene edit unit from chapter reader unit.

## Check Vietnamese register and Viet Dao calibration

Verify Vietnamese register rule, prompt, and calibration sample exist, task is allowed, route ends with node checkpoint, source fidelity is respected, and the gate separates Vietnamese life layer from Sino-Vietnamese concept layer.

## Check webnovel paragraphing and layout rhythm

Verify webnovel paragraphing rule and prompt exist, task is allowed, route ends with node checkpoint, source fidelity is respected, paragraph is reader breath, line break is structural signal, and the gate checks short-line density, dialogue layout, mobile fatigue, and wall-text risk.

## Check character distinctiveness and iceberg profile

Verify:

- `rules/sltd_character_distinctiveness_iceberg_gate.md` exists and is listed in manifest;
- `prompts/character_distinctiveness_check.md` exists and is listed in manifest;
- character_distinctiveness_check is listed in allowed_tasks;
- character distinctiveness route ends with node checkpoint;
- character distinctiveness route references source fidelity before patching;
- the gate separates agency from distinctiveness;
- the gate checks voice signature, body/gesture signature, object/clothing signature, habit under pressure, private want, private fear, concealment strategy, relation-specific behavior, iceberg trace, personalized cost, and interchangeability risk;
- the gate prevents function-only characters, cast voice collapse, decorative quirks, and backstory explained rather than embodied;
- the gate does not authorize trauma, backstory, motive, symbol, title, relation, or canon invention.

## Check scene-first prose judgment

Verify scene-first rule and prompt exist, task is allowed, route ends with node checkpoint, source fidelity is respected, one governing scene pressure is required, and checklist is later verification rather than writing method.

## Check anti-AI composite

Verify anti-AI composite rule and prompt exist, task is allowed, route ends with node checkpoint, source fidelity is respected, and it blocks texture-as-cover and readiness-from-green-sub-passes.

## Check character agency

Verify character agency rule and prompt exist, task is allowed, route ends with node checkpoint, source fidelity is respected, and want/fear/knowledge limit/pressure/choice/visible cost are checked.

## Check dynamic range

Verify dynamic range rule and prompt exist, task is allowed, route ends with node checkpoint, source fidelity is respected, and cadence/pressure are not flattened.

## Check handoff continuity

Verify handoff continuity rule is listed, session_handoff reads it, handoff route ends with node checkpoint, and handoff is navigation rather than source truth.

## Check calibration cases

Verify calibration discipline and sample files are listed, calibration route ends with node checkpoint, and calibration remains example data rather than canon/current manuscript.

Required calibration files:

```text
samples/viet_dao_prose_calibration.md
samples/line_surgery_calibration.md
samples/dialogue_voice_calibration.md
samples/underreach_calibration.md
samples/readiness_false_positive.md
```

## Check routes

Verify each allowed task has a route or prompt, large routes use context brief when needed, node-changing routes end with node checkpoint or result report, and routes reference their required gate files:

```text
source-surface routes -> sltd_source_fidelity_anti_compression.md
first-pass routes -> sltd_first_pass_editorial_workflow.md
chapter assembly routes -> sltd_chapter_assembly_split_control_gate.md
Vietnamese register routes -> sltd_vietnamese_register_viet_dao_gate.md
webnovel paragraphing routes -> sltd_webnovel_paragraphing_layout_rhythm_gate.md
character distinctiveness routes -> sltd_character_distinctiveness_iceberg_gate.md
scene-first routes -> sltd_scene_first_prose_judgment_gate.md
anti-AI composite routes -> sltd_anti_ai_composite_failure_gate.md
character agency routes -> sltd_character_agency_anti_ooc_gate.md
dynamic range routes -> sltd_dynamic_range_cadence_gate.md
handoff routes -> sltd_handoff_continuity_protocol.md
```

## Check role boundaries

Verify later roles do not overwrite earlier-layer blockers and learned taste/calibration/gates/workflows do not override current source, canon, evidence, or human lock.

## Check orphan risk

Mark a file as possible orphan when it exists but is not listed in manifest, is listed but cannot be fetched, defines a task with no route, duplicates another rule without reason, or is missing from its route.

## Output labels

```text
PACK_HEALTH_OK
PACK_HEALTH_WARN
PACK_HEALTH_FAIL
```

A warning does not block all work, but a fail blocks new skill expansion until fixed.
