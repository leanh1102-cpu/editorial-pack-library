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
- fast path does not replace boot, manifest, design, or source preflight.

## Check routes

Verify:

- each allowed task has a route or prompt;
- each route has a safety step;
- large routes use context brief when needed;
- node-changing routes end with node checkpoint or result report;
- role-overlap routes reference `rules/sltd_role_boundary_contracts.md`.

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
- it defines a role or task without boundary, route, or output.

## Output labels

```text
PACK_HEALTH_OK
PACK_HEALTH_WARN
PACK_HEALTH_FAIL
```

A warning does not block all work, but a fail blocks new skill expansion until fixed.
