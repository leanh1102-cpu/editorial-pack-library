# SLTD Narrative Feature & Structural Idiosyncrasy Audit

This rule adapts narrative-feature research for SLTD without using detector-bypass goals.

It catches AI-like structure at the story-decision layer: theme over-explained, causality too tidy, plot too single-track, protagonist understanding used as resolution, reveal without recontextualization, and sensory/body detail that performs style without changing action, relation, resource, evidence, or cost.

## Core rule

Do not fix AI-like story structure by polishing sentences.

A passage can sound human at the line level and still fail at the narrative-feature level if the story is too clean, too explanatory, too single-route, too morally simple, or too resolved by understanding instead of cost.

Narrative Feature Audit is not an AI detector. It is a structural smell audit for scene/chapter/packet decisions.

## Use when

- prose sounds good but the story decision feels synthetic;
- a scene has correct facts but weak reread value;
- theme is spoken by narration instead of pressured by event;
- causality is too clean, convenient, or single-route;
- protagonist comprehension replaces action, debt, witness, or cost;
- body/sensory detail is abundant but does not alter choice, relation, evidence, or risk;
- setting mirrors emotion too neatly;
- reveal does not recontextualize prior evidence;
- a chapter/packet feels readable but generic, soft, or AI-shaped;
- user asks about StoryScope, narrative features, structural AI smell, or story idiosyncrasy.

## Authority

Run after:

```text
source preflight
source surface when exact scene/chapter prose is required
context capsule when current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope
structural spine / tracking / voice gates when their blockers are in scope
```

Run before:

```text
rewrite
line surgery
human surface polish
copyedit
readiness
publication lock claim
```

If Narrative Feature Audit finds a structural smell, do not send the passage directly to Human Surface Polish or Copyedit. Hand back to structural, tracking, story doctor, intensity, or rewrite.

## Required distinction

```text
NARRATIVE FEATURE AUDIT = checks story-decision patterns and structural idiosyncrasy
STRUCTURAL SPINE = checks scene/chapter function and prose permission
TRACKING / LOGIC LEDGER = checks continuity, state, debt, residue, and downstream effects
HUMAN SURFACE POLISH = repairs correct-but-synthetic surface after story structure is safe
ANTI-AI COMPOSITE = broad smell check, not a detailed narrative-feature matrix
```

## What to inspect

Inspect only features useful for SLTD editorial decisions:

- thematic explicitness;
- causal tidiness;
- single-track plot risk;
- protagonist agency shape;
- temporal complexity;
- reveal / recontextualization;
- subplot or thread integration;
- moral ambiguity;
- dialogue function;
- body / sensory overperformance;
- setting as psychological mirror;
- narrative diversity;
- changed-state and reread value.

Do not import a large research taxonomy wholesale. Keep the audit compact and task-bounded.

## SLTD-specific cautions

Body/object detail is not automatically human.

```text
Body/object detail passes only when it changes action, relation, resource, evidence, witness, debt, risk, or choice.
```

For SLTD, concrete pressure remains preferred, but it must work inside the scene. Do not add hands, breath, cold, smell, silence, shadow, or weather as decorative proof of human prose.

## Output schema

```text
SLTD NARRATIVE FEATURE AUDIT
SCOPE:
SOURCE USED:
SOURCE STATUS:
CONTEXT CAPSULE STATUS:
SCENE / CHAPTER QUESTION:
THEMATIC EXPLICITNESS:
CAUSAL TIDINESS:
SINGLE-TRACK PLOT RISK:
PROTAGONIST AGENCY SHAPE:
TEMPORAL COMPLEXITY:
REVEAL / RECONTEXTUALIZATION:
SUBPLOT / THREAD INTEGRATION:
MORAL AMBIGUITY:
DIALOGUE FUNCTION:
BODY / SENSORY OVERPERFORMANCE:
SETTING AS PSYCHOLOGICAL MIRROR:
NARRATIVE DIVERSITY:
CHANGED-STATE / REREAD VALUE:
AI-STRUCTURAL SMELL:
SAFE REPAIR:
PROSE PERMISSION:
NEXT NODE:
```

Use only fields needed by the scope. For a short scene, keep the audit short.

## Prose permission blockers

```text
source or current scene/chapter surface missing
context capsule blocked
scene question unclear
must show / must not reveal missing
thread/debt state unclear
reveal timing unclear
AI-structural smell remains unresolved
body/object detail is decorative only
repair would require canon invention
```

## Failure labels

```text
NARRATIVE_FEATURE_OK
NARRATIVE_FEATURE_PARTIAL
NARRATIVE_FEATURE_BLOCKED
THEME_OVEREXPLAINED
CAUSAL_TIDINESS_RISK
SINGLE_TRACK_PLOT_RISK
UNDERCOSTED_UNDERSTANDING_RESOLUTION
REVEAL_WITHOUT_RECONTEXTUALIZATION
TEMPORAL_FLATNESS
SUBPLOT_THREAD_THINNESS
MORAL_SIMPLIFICATION
BODY_SENSORY_OVERPERFORMANCE
SETTING_MIRROR_OVERFIT
NARRATIVE_DIVERSITY_LOW
STRUCTURAL_AI_SMELL
PROSE_PERMISSION_BLOCKED
```

## Safe repair

Safe repair may:

- mark the strongest narrative-feature smell;
- route back to Structural Spine, Tracking / Logic Ledger, Story Doctor, Intensity Editor, or Rewrite;
- propose a source-safe structural repair candidate;
- reduce over-explicit theme;
- make body/object detail consequential;
- add pressure only from existing source/canon/scene controls;
- preserve hidden canon and POV restraint.

Safe repair must not:

- invent canon, thread, subplot, clue, object, relation, institution, or payoff;
- turn research labels into prose labels;
- score authorship or claim detector certainty;
- use a decorative percentage;
- authorize Human Chapter Pass, readiness, or Publication Lock;
- create scripts, workflows, reports, boards, databases, automations, or live manuscript copies.

## Output labels

```text
NARRATIVE_FEATURE_READY
NARRATIVE_FEATURE_NEEDS_PATCH
NARRATIVE_FEATURE_BLOCKED
STRUCTURAL_REWRITE_REQUIRED
TRACKING_REPAIR_REQUIRED
HUMAN_SURFACE_NOT_YET_AUTHORIZED
READINESS_NOT_AUTHORIZED
```