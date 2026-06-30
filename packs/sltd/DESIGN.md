# SLTD Pack Design

This file is the human-readable architecture contract for the SLTD pack.

`manifest.yml` is the machine-readable entry. `DESIGN.md` explains why the pack is shaped this way and how to extend it without turning GitHub into a workflow system.

## Purpose

The SLTD pack turns AI into a controlled editorial agent for a long Vietnamese web novel project.

It should help the agent:

- read the right source;
- choose the right skill;
- keep canon stable;
- avoid AI-looking Vietnamese prose;
- work by chapter, scene, packet, and node;
- leave evidence, checkpoints, and handoff;
- avoid creating extra management structure.

## Source of truth

```text
Notion = live manuscript state
GitHub = editorial rules, skills, router, evidence discipline
User instruction = current task and final authority for writes
```

Legacy Google Docs or Workdecks may be useful as history. They are not current manuscript unless the user says so.

## System topology

```text
AI_ENTRY.md
  -> packs/sltd/manifest.yml
  -> packs/sltd/PACK.md
  -> packs/sltd/AGENT_IDENTITY.md
  -> packs/sltd/ENTRY_FAST_PATH.md
  -> packs/sltd/prompts/boot_task.md
  -> packs/sltd/rules/sltd_runtime_loop.md
```

The pack is split into:

- identity files;
- source discipline;
- task router;
- competency map;
- mindmap and node traversal;
- context-window strategy;
- evidence discipline;
- healthcheck;
- task prompts;
- examples.

## Runtime loop

```text
boot_task
source_preflight
task_intake
task_router
decision_safety
task-specific prompt
node_checkpoint
result_report
```

Use the smallest route that answers the user request.

## Context strategy

The agent must not try to hold the whole novel in the chat window.

For each task, build a small working context:

```text
current source
scope
local chapter or scene
relevant canon
active skills
node ledger
open loops
```

Large work must split by chapter, scene, packet, role, or source layer.

## Editorial competency model

The main editorial roles are:

- Canon Guard;
- Story Doctor;
- Intensity Editor;
- Vietnamese Line Editor;
- Copyeditor;
- Proofreader;
- Publishing Readiness Reviewer;
- Editorial Director.

Roles should be routed by task. Do not run every role for every request.

## Mindmap and node traversal

Mindmap files define source nodes, role nodes, output nodes, and blocking nodes.

Node traversal exists to show:

- what was read;
- what was not read;
- which role ran;
- what blocked the conclusion;
- what node comes next.

## Evidence discipline

Current-state claims require current evidence.

Claims about Chapter Index, Human Chapter Pass, Publication Lock, Scene Bank readiness, packet lock, canon conflict, or pass validity must name source and node.

Chat memory, old audit, old Google Doc, or a prior assistant claim is not enough.

## Healthcheck discipline

Before adding a new skill, run entry healthcheck.

Check:

- manifest version;
- required files;
- allowed tasks;
- route coverage;
- evidence coverage;
- orphan risk;
- changelog.

If pack health fails, patch the entry before adding skills.

## Extension policy

Add new files only when they improve editorial reading, rewriting, routing, evidence, context handling, or pack health.

Allowed file types:

- rule;
- prompt;
- sample;
- design note;
- manifest update;
- changelog entry.

Do not add scripts, workflows, boards, reports, project management files, or live manuscript copies.

## Non-goals

The SLTD pack must not become:

- a Notion replacement;
- a live manuscript store;
- a project board;
- an automation system;
- a GitHub Actions workflow;
- a place where AI invents canon;
- a place where AI silently updates Notion.

## 1000+ chapter operating model

For a very long series, operate by slice:

```text
1 scene = rewrite unit
1 chapter = readiness unit
10 chapters = packet check
30 chapters = arc or part check
100+ chapters = map-level review
1000+ chapters = series-level navigation, not line edit
```

The agent should always prefer retrieval, context brief, node checkpoint, and session handoff over trying to remember everything.

## Invariants

These rules should remain stable across versions:

- Notion is the live manuscript state.
- GitHub is editorial memory and rules.
- User instruction outranks the pack.
- AI does not invent canon.
- AI does not update Notion without a clear write request.
- AI does not claim readiness without evidence.
- AI uses fast path for normal tasks.
- AI splits large work by node.
- Manifest is machine-readable entry.
- Design is human-readable architecture contract.
