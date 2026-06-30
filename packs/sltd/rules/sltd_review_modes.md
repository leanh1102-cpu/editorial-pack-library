# SLTD Review Modes

Review modes are command prefixes that change how an existing skill route is used.

They are not separate editors and they do not replace source preflight, decision safety, evidence discipline, or node checkpoint.

## Core modes

### TRUEMODE

Use when the user wants only grounded claims.

Route:

```text
source_preflight -> sltd_evidence_discipline -> sltd_decision_safety -> result_report
```

Rules:

- make only claims supported by opened or provided source;
- lower confidence when a source node was not read;
- stop instead of guessing current status;
- separate fact, inference, and recommendation.

### REDTEAM

Use when the user wants the conclusion attacked.

Route:

```text
editorial_director_review -> sltd_publishing_readiness -> sltd_pack_healthcheck -> node_checkpoint
```

Rules:

- look for hidden blockers;
- test the weakest assumption;
- find source conflict, canon risk, false readiness, thin stakes, and route gaps;
- do not rewrite unless the user asks.

### PREMORTEM

Use when the user wants to know why a chapter, packet, or decision may fail.

Route:

```text
audit_story_arc -> chapter_readiness_check -> sltd_publishing_readiness -> editorial_director_review
```

Rules:

- assume the work failed;
- list likely failure causes;
- rank them by impact;
- name the source needed to confirm each cause;
- give next audit node.

### SOCRATES

Use when the user wants questions before verdict.

Route:

```text
task_intake -> context_brief -> mindmap_review -> node_checkpoint
```

Rules:

- ask targeted questions that expose assumptions;
- avoid long generic question lists;
- ask about source, scope, canon, scene function, cost, and reader effect;
- end with the smallest next step.

## Support modes

### SOURCELOCK

Use only current source named by the user. If current source is missing, stop.

### CANONLOCK

Do not add canon. Detect conflict or return patch candidate.

### TASTELOCK

Apply `AUTHOR_TASTE_EXAMPLES.md` to line edit, rewrite, or underreach fixes. Taste does not override canon or source.

### UNDERREACH

Find where a correct passage lacks cost, body, object, relation, witness, debt, choice, or pressure.

### DIFFMODE

Compare two named sources or versions. Do not infer a diff from memory.

### READINESS

Check whether a chapter or packet can move toward Human Chapter Pass or Publication Lock. Evidence is required.

### NODETRACE

Return source nodes read, role nodes run, blockers, open loops, and next node.

### HANDOFF

Compress the current task into a session handoff for the next chat.

## Combining modes

Modes may be combined when they do not conflict.

Examples:

```text
TRUEMODE + PREMORTEM
REDTEAM + READINESS
SOURCELOCK + CANONLOCK
TASTELOCK + UNDERREACH
NODETRACE + HANDOFF
```

If modes conflict, choose the safer one and explain the drop.

## Output

```text
REVIEW MODE:
BASE ROUTE:
SOURCE RULE:
EVIDENCE RULE:
FINDINGS:
BLOCKERS:
NEXT NODE:
```
