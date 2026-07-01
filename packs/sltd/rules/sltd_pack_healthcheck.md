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

## Check first-pass editorial workflow

Verify first-pass rule and prompt exist, task is allowed, route ends with node checkpoint, source fidelity is respected, and targeted gates run only after initial prose judgment.

## Check chapter assembly and split control

Verify:

- `rules/sltd_chapter_assembly_split_control_gate.md` exists and is listed in manifest;
- `prompts/chapter_assembly_split_check.md` exists and is listed in manifest;
- chapter_assembly_split_check is listed in allowed_tasks;
- chapter assembly route ends with node checkpoint;
- chapter assembly route references source fidelity before verdict;
- chapter assembly gate separates scene edit unit from chapter reader unit;
- chapter assembly gate checks length type, reader question, governing chapter pressure, major turns, payoff points, loops, and natural breakpoints;
- chapter assembly gate warns on word-count risk without splitting mechanically by word count alone;
- chapter assembly gate does not authorize silent live manuscript split, renumbering, deletion, or Notion update.

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
first-pass routes -> sltd_first_pass_editorial_workflow.md
chapter assembly routes -> sltd_chapter_assembly_split_control_gate.md
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
