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

## Check routes

Verify:

- each allowed task has a route or prompt;
- each named role has a role card route;
- each route has a safety step;
- large routes use context brief when needed;
- node-changing routes end with node checkpoint or result report;
- role-overlap routes reference `rules/sltd_role_boundary_contracts.md`;
- iteration routes reference `rules/sltd_agentic_iteration_loop.md`.

## Check role boundaries

Verify:

- each active editorial role has start condition, allowed actions, must-not-do, done criteria, stop condition, and handoff;
- later roles do not overwrite earlier-layer blockers;
- review modes remain lenses, not roles;
- learned taste does not override current source, canon, evidence, or human lock.

## Check orphan risk

Mark a file as possible orphan when:

- it exists but is not listed in manifest;
- it is listed in manifest but cannot be fetched;
- it describes a task that no route uses;
- it duplicates another rule without a clear reason;
- it defines a role or task without boundary, route, or output;
- a role card exists but is missing from `ROLE_ENTRY_INDEX.md`;
- an iteration file exists but is missing from manifest or route.

## Output labels

```text
PACK_HEALTH_OK
PACK_HEALTH_WARN
PACK_HEALTH_FAIL
```

A warning does not block all work, but a fail blocks new skill expansion until fixed.
