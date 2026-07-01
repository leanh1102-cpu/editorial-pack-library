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

Verify:

- root entry is still `AI_ENTRY.md`;
- pack entry is still `packs/sltd/manifest.yml`;
- runtime entry is still `prompts/boot_task.md`;
- fast path does not replace boot, manifest, design, or source preflight;
- `ROLE_ENTRY_INDEX.md` lists every role card.

## Check source fidelity

Verify:

- `rules/sltd_source_fidelity_anti_compression.md` exists and is listed in manifest;
- `prompts/source_surface_check.md` exists and is listed in manifest;
- source_surface_check is listed in allowed_tasks;
- line edit, line surgery, copyedit, proofread, rewrite, readiness, and exact patch routes require source surface when exact text/current source may be missing;
- digest is labeled as not source text;
- exact OLD is required before OLD/NEW patch;
- missing source surface downgrades to map-level review, packet risk scan, or source request.

## Check character agency

Verify:

- `rules/sltd_character_agency_anti_ooc_gate.md` exists and is listed in manifest;
- `prompts/character_agency_check.md` exists and is listed in manifest;
- character_agency_check is listed in allowed_tasks;
- character agency route ends with node checkpoint;
- character agency route references source fidelity before patching;
- character agency gate checks want, fear, knowledge limit, pressure, choice, and visible cost;
- character agency gate prevents characters from serving plot, clue, scene card, or explanation duty without source pressure;
- character agency gate does not authorize canon invention or locked outcome changes.

## Check dynamic range

Verify:

- `rules/sltd_dynamic_range_cadence_gate.md` exists and is listed in manifest;
- `prompts/dynamic_range_check.md` exists and is listed in manifest;
- dynamic_range_check is listed in allowed_tasks;
- dynamic range route ends with node checkpoint;
- dynamic range route references source fidelity before patching;
- dynamic range gate separates what must stay quiet from what needs stronger scene pressure;
- dynamic range gate prevents all scenes from being forced into the same restrained cadence;
- dynamic range gate does not authorize canon invention or locked outcome changes.

## Check handoff continuity

Verify:

- `rules/sltd_handoff_continuity_protocol.md` exists and is listed in manifest;
- `prompts/session_handoff.md` reads the handoff continuity protocol;
- handoff_continuity_check is listed in allowed_tasks;
- handoff route ends with node checkpoint;
- handoff separates FACT, INFERENCE, RECOMMENDATION, CANDIDATE, and UNVERIFIED;
- handoff contains source, role, node, decision, patch, and error ledgers;
- handoff contains CARRY FORWARD and DO NOT CARRY;
- handoff tells next AI to verify current source before verdict;
- handoff is marked as navigation, not source truth.

## Check role entry cards

Verify each role card exists, is listed in manifest, and has:

- Role;
- When user says;
- Read first;
- Source required;
- Run;
- Do;
- Do not;
- Output;
- Done;
- Handoff;
- Fail closed.

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

## Check iteration loop

Verify:

- `rules/sltd_agentic_iteration_loop.md` exists and is listed in manifest;
- `prompts/iteration_checkpoint.md` exists and is listed in manifest;
- iteration tasks are listed in allowed_tasks;
- iteration route ends with node checkpoint;
- loop requires source, scope, role, route, verification gate, and stop condition;
- loop ends with next node or stop;
- loop does not authorize automation, scripts, workflows, reports, boards, or silent writes.

## Check calibration cases

Verify:

- `rules/sltd_calibration_discipline.md` exists and is listed in manifest;
- calibration task is listed in allowed_tasks;
- calibration sample files exist and are listed in manifest;
- calibration route ends with node checkpoint;
- calibration cases use BAD / WHY BAD / RULE HIT / PREFERRED / PATCH PRINCIPLE;
- calibration is marked as example, not canon or current manuscript;
- user rejection creates a calibration candidate, not a silent write.

Required calibration files:

```text
samples/line_surgery_calibration.md
samples/dialogue_voice_calibration.md
samples/underreach_calibration.md
samples/readiness_false_positive.md
```

## Check routes

Verify:

- each allowed task has a route or prompt;
- each named role has a role card route;
- each route has a safety step;
- large routes use context brief when needed;
- node-changing routes end with node checkpoint or result report;
- role-overlap routes reference `rules/sltd_role_boundary_contracts.md`;
- iteration routes reference `rules/sltd_agentic_iteration_loop.md`;
- calibration routes reference `rules/sltd_calibration_discipline.md`;
- source-surface routes reference `rules/sltd_source_fidelity_anti_compression.md`;
- character agency routes reference `rules/sltd_character_agency_anti_ooc_gate.md`;
- dynamic range routes reference `rules/sltd_dynamic_range_cadence_gate.md`;
- handoff routes reference `rules/sltd_handoff_continuity_protocol.md`.

## Check role boundaries

Verify:

- each active editorial role has start condition, allowed actions, must-not-do, done criteria, stop condition, and handoff;
- later roles do not overwrite earlier-layer blockers;
- review modes remain lenses, not roles;
- learned taste, calibration, character agency checks, and dynamic range checks do not override current source, canon, evidence, or human lock.

## Check orphan risk

Mark a file as possible orphan when:

- it exists but is not listed in manifest;
- it is listed in manifest but cannot be fetched;
- it describes a task that no route uses;
- it duplicates another rule without a clear reason;
- it defines a role or task without boundary, route, or output;
- a role card exists but is missing from `ROLE_ENTRY_INDEX.md`;
- an iteration file exists but is missing from manifest or route;
- a calibration file exists but is missing from manifest or route;
- a source-surface file exists but is missing from manifest or route;
- a character-agency file exists but is missing from manifest or route;
- a dynamic range file exists but is missing from manifest or route;
- a handoff-continuity file exists but is missing from manifest or route.

## Output labels

```text
PACK_HEALTH_OK
PACK_HEALTH_WARN
PACK_HEALTH_FAIL
```

A warning does not block all work, but a fail blocks new skill expansion until fixed.
