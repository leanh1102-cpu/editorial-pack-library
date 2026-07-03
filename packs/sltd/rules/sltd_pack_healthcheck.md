# SLTD Pack Healthcheck

Use this rule to check SLTD pack health after version changes.

This is a manual agent check. It does not create scripts, workflow files, issues, boards, or reports.

## Check manifest

Verify version, required files, allowed tasks, source priority, and fail-closed status.

## Check source fidelity

Verify source fidelity rule and source surface prompt exist and exact prose/status routes require source surface before patching or verdict.

## Check structural spine, outline pre-prose, and borderbound

Verify rule/prompt/sample exist, are listed in manifest, task is allowed, routes end with node checkpoint, and rewrite/readiness routes reference structural spine when outline, card, packet, or borderbound affects prose permission.

## Check Vietnamese senior editor surface and pass integrity

Verify:

- `rules/sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md` exists and is listed in manifest;
- `prompts/vietnamese_senior_editor_surface_check.md` exists and is listed in manifest;
- `samples/vietnamese_senior_editor_surface_calibration.md` exists and is listed in manifest;
- vietnamese_senior_editor_surface_check is listed in allowed_tasks;
- Vietnamese surface route ends with node checkpoint;
- the gate defines Vietnamese surface, semantic load, pass integrity, read-aloud friction, object-function visibility, and human breath space;
- the gate blocks false readiness from Anti-AI Pass, candidate-ready notes, formal status updates, conflicting notes, Human Chapter Pass NO, and Publication Lock Not Ready;
- the gate requires exact prose for sentence-level verdict or repair.

## Check supernatural event residue and dread amplitude

Verify supernatural residue rule/prompt/sample, allowed task, source fidelity route, node checkpoint, and blockers for mood-only fog/cold/silence, underpowered dread, folklore without incident, generic beast threat, relic decoration, and early deep-lore reveal.

## Check protagonist inquiry and advancement

Verify protagonist inquiry and advancement rule/prompt/sample files, allowed tasks, source fidelity routes, node checkpoints, and blockers for passive protagonist, adult system reasoning, source-unsupported growth, and Notion-label prose.

## Check entry route governance

Verify one primary route before secondary gates, evidence-backed secondary gates, explicit stop conditions, and no gate cascade.

## Check routes

Verify each allowed task has a route or prompt, node-changing routes end with node checkpoint or result report, and routes reference required gate files:

```text
source-surface routes -> sltd_source_fidelity_anti_compression.md
entry governance routes -> sltd_entry_route_governance_gate_budget_protocol.md
structural spine routes -> sltd_structural_spine_outline_preprose_borderbound_gate.md
Vietnamese surface routes -> sltd_vietnamese_senior_editor_surface_pass_integrity_gate.md
supernatural residue routes -> sltd_supernatural_event_residue_dread_amplitude_gate.md
protagonist inquiry routes -> sltd_protagonist_inquiry_inner_reasoning_clue_chain_gate.md
protagonist advancement routes -> sltd_protagonist_advancement_growth_route_gate.md
```

## Check role boundaries

Verify later roles do not overwrite earlier-layer blockers and learned gates do not override current source, canon, evidence, or human lock.

## Check orphan risk

Mark a file as possible orphan when it exists but is not listed in manifest, is listed but cannot be fetched, defines a task with no route, duplicates another rule without reason, or is missing from its route.

## Output labels

```text
PACK_HEALTH_OK
PACK_HEALTH_WARN
PACK_HEALTH_FAIL
```
