# SLTD Role Boundary Contracts

This rule defines where each editorial role starts, stops, hands off, and must not act.

It prevents role mixing, false authority, and polishing the wrong layer.

## Global contract

Every role must obey:

- user current instruction;
- current Notion source or user-provided current packet;
- source preflight;
- context capsule preflight when current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope;
- decision safety;
- evidence discipline;
- canon guard;
- node checkpoint.

A role may produce a candidate. It may not silently update Notion, GitHub, or manuscript source.

Review modes change the lens. They do not become roles.

Context Capsule is not a prose, story, line, canon, or readiness role. It is a pre-role source/context gate. If it blocks, later roles must stop instead of continuing from memory or plausible continuity.

Human Surface Polish is not detector bypass, story repair, canon repair, or readiness. It is a late prose role used only after source/context/story/voice constraints are clear enough.

## Role order principle

```text
source and context before canon
canon before story
story before intensity
intensity before line surgery
line surgery before human surface polish
human surface polish before copyedit
copyedit before proofread
proofread before readiness
readiness before publication lock claim
editorial director chooses priority, not canon truth
```

If a later role discovers an earlier-layer failure, stop and hand back.

## Contract format

Each role must be understood through:

```text
ROLE:
START WHEN:
READ BEFORE:
MAY DO:
MUST NOT DO:
OUTPUT:
DONE WHEN:
HANDOFF TO:
STOP WHEN:
```

## Canon Guard

ROLE: Canon Guard

START WHEN:
- source conflict appears;
- reveal timing may be wrong;
- rewrite or patch may invent facts;
- lock/status/canon is unclear.

READ BEFORE:
- current user instruction;
- source preflight result;
- context capsule preflight result when current source, hidden canon, POV knowledge, source-status separation, or long-range continuity is in scope;
- current Notion source or user-provided source;
- relevant canon index if available;
- evidence discipline.

MAY DO:
- detect source conflict;
- mark reveal timing risk;
- block invented canon;
- return canon patch candidate;
- request missing source.

MUST NOT DO:
- invent lore to solve a scene;
- decide canon without current source;
- use legacy Workdeck as current source unless named current;
- rewrite for style.

OUTPUT:
- canon risk;
- source conflict;
- safe claim;
- candidate only.

DONE WHEN:
- canon risk is cleared, blocked, or narrowed;
- next role knows what must not be changed.

HANDOFF TO:
- Story Doctor if story motion is the issue;
- Intensity Editor if underreach is the issue;
- Vietnamese Line Editor or Line Surgery if prose is the issue.

STOP WHEN:
- current source is missing;
- context capsule blocks current source, hidden canon, POV knowledge, or source-status separation;
- canon conflict lacks current decision;
- user asks for lock but lock source was not read.

## Story Doctor

ROLE: Story Doctor

START WHEN:
- scene or chapter is correct but does not pull;
- changed state is missing;
- promise/payoff is weak;
- reader reward is low;
- structure blocks line polish.

READ BEFORE:
- Canon Guard result;
- Context Capsule result if current source, hidden canon, POV knowledge, relationship memory, object state, or long-range continuity is in scope;
- Scene Bank or chapter source;
- Story Outline if needed;
- Webnovel Momentum Benchmark if packet pull is asked.

MAY DO:
- identify missing changed state;
- mark weak causality;
- find promise/payoff debt;
- propose scene-level repair priority;
- recommend rewrite when structure is wrong.

MUST NOT DO:
- polish prose to hide story failure;
- add new canon;
- change ending without user request;
- call readiness.

OUTPUT:
- story blocker;
- repair priority;
- rewrite candidate;
- next scene/chapter node.

DONE WHEN:
- the story layer is passable or marked for rewrite;
- line roles know whether polishing is allowed.

HANDOFF TO:
- Intensity Editor if story is functional but thin;
- Vietnamese Line Editor or Line Surgery if story is settled;
- Editorial Director if multiple blockers compete.

STOP WHEN:
- source or scope is missing;
- context capsule blocks required source/context;
- scene function is unclear;
- repair would require canon invention.

## Intensity Editor

ROLE: Intensity Editor

START WHEN:
- scene is safe but thin;
- cost is absent;
- object exists without consequence;
- mystery lacks pressure;
- correct material underreaches.

READ BEFORE:
- Canon Guard result;
- Story Doctor result if available;
- Context Capsule result if object/location/body/debt state, relationship memory, hidden canon, or long-range continuity is in scope;
- intensity rules and targets;
- author taste examples;
- current scene source.

MAY DO:
- identify missing cost, body, object, pressure, relation, witness, debt, or choice;
- propose pressure patch using existing source material;
- mark underreach;
- rank intensity fixes.

MUST NOT DO:
- add new lore or power;
- escalate by making prose grander;
- change scene outcome;
- rewrite entire scene unless asked.

OUTPUT:
- underreach finding;
- pressure patch candidate;
- cost/consequence gap;
- next node.

DONE WHEN:
- visible cost or pressure is present, or the scene is marked for rewrite.

HANDOFF TO:
- Vietnamese Line Editor if prose can now be shaped;
- Line Surgery if issue is sentence-level AI smell;
- Story Doctor if pressure failure is structural.

STOP WHEN:
- proposed intensity requires new canon;
- object/pressure source was not read;
- context capsule blocks required object/location/body/debt state;
- more than local patch is needed.

## Vietnamese Line Editor

ROLE: Vietnamese Line Editor

START WHEN:
- story, source, and canon are settled enough to work at prose level;
- rhythm is stiff;
- dialogue has one voice;
- scene tells instead of acts;
- AI phrasing leaks.

READ BEFORE:
- prose rhythm rules;
- dialogue voice rules;
- anti-AI words;
- SLTD style rules;
- author taste examples;
- line surgery gate if prose smell is line-level;
- Context Capsule result if voice, relationship memory, POV knowledge, hidden canon, or source-status separation is in scope.

MAY DO:
- improve Vietnamese rhythm;
- split or reorder stiff sentences;
- reduce abstract phrasing;
- restore body, object, silence, and action;
- mark need for line surgery, human surface polish, or scene rewrite.

MUST NOT DO:
- solve story failure by pretty prose;
- add beat or canon;
- make all voices polished;
- over-literarize the sentence.

OUTPUT:
- prose issue;
- minimal patch;
- line surgery or human surface polish recommendation;
- voice risk.

DONE WHEN:
- prose reads naturally for the scoped passage, or failure is escalated.

HANDOFF TO:
- Human Surface Polish if prose is correct but still synthetic, over-clean, same-voiced, or falsely smooth;
- Copyeditor if line prose and human surface pass;
- Line Surgery if sentence-level repair is needed;
- Story Doctor if prose failure is structural.

STOP WHEN:
- source/canon/story layer is unsettled;
- context capsule blocks POV knowledge, hidden canon, relationship memory, or source-status separation;
- more than 30 percent of excerpt needs surgery;
- voice cannot be fixed without character source.

## Line Surgery

ROLE: Line Surgery

START WHEN:
- excerpt is 300-1500 words or a scoped line set;
- prose reads stiff, translated, over-clean, or AI-like;
- user asks for line audit or minimal OLD/NEW patch.

READ BEFORE:
- Vietnamese Line Surgery Gate;
- prose rhythm;
- dialogue voice;
- anti-AI words;
- SLTD style rules;
- author taste examples;
- source excerpt;
- Context Capsule result if current source, hidden canon, POV knowledge, relationship memory, or source-status separation is in scope.

MAY DO:
- label line issues;
- propose minimal OLD/NEW fixes;
- run mouth-read check;
- mark rewrite threshold.

MUST NOT DO:
- rewrite whole scene unless asked;
- change scene outcome;
- add metaphor to hide stiffness;
- add canon or new beats.

OUTPUT:
- LINE_SURGERY_PASS;
- NEEDS_LINE_SURGERY;
- NEEDS_SCENE_REWRITE;
- OLD/NEW patches.

DONE WHEN:
- scoped lines pass mouth-read check or are escalated.

HANDOFF TO:
- Human Surface Polish if the line set is repaired but still falsely smooth, same-voiced, or synthetic-surface thin;
- Copyeditor if pass and human surface is already clean;
- Rewrite Scene if over threshold;
- Vietnamese Line Editor if broad prose rhythm still needs work.

STOP WHEN:
- excerpt is too large and no sampling instruction exists;
- source is missing;
- context capsule blocks required source/context;
- repair load exceeds 30 percent.

## Human Surface Polish

ROLE: Human Surface Polish

START WHEN:
- exact current prose surface has been read;
- story, canon, intensity, voice, and line-level permission are settled enough;
- the passage is correct in meaning but still reads synthetic, over-clean, falsely smooth, same-voiced, symbol-first, or thin in body/object/relationship pressure;
- user asks for human surface, humanize, anti-synthetic polish, văn nghe người hơn, đúng ý nhưng giả, or mượt giả.

READ BEFORE:
- source surface result for the exact prose;
- Context Capsule result when current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope;
- Vietnamese Senior Editor Surface result if human surface or pass integrity is in scope;
- Character Voice / Dialogue / Staging result if voice, relationship, silence, presence, or location staging is in scope;
- AUTHOR_TASTE_EXAMPLES.md;
- `rules/sltd_human_surface_polish_anti_synthetic_gate.md`.

MAY DO:
- identify false smoothing, same-voice polish, symbolic drift, object/body loss, relationship flattening, or generic emotional polish;
- propose minimal OLD/NEW patches;
- restore body, object, silence, action, and read-aloud Vietnamese using only existing source pressure;
- mark detector-bypass framing as blocked;
- route back to Line Surgery or Rewrite Scene if repair load is too high.

MUST NOT DO:
- bypass AI detectors or frame the task as detector evasion;
- add canon, scene beat, object, relationship, secret, payoff, or metaphor;
- change scene function, outcome, or reveal timing;
- make rough characters fluent because polish wants smoothness;
- call Human Chapter Pass, readiness, or Publication Lock.

OUTPUT:
- HUMAN_SURFACE_READY;
- HUMAN_SURFACE_NEEDS_PATCH;
- HUMAN_SURFACE_BLOCKED;
- OLD/NEW patches;
- next node.

DONE WHEN:
- the scoped passage keeps source meaning, pressure, voice, and reveal locks while reading as lived Vietnamese prose;
- or the pass blocks and hands back to the earlier role.

HANDOFF TO:
- Copyeditor if human surface passes;
- Line Surgery if sentence-level repair remains;
- Voice / Dialogue / Staging if same-voice or relationship loss remains;
- Story Doctor or Intensity Editor if the polish exposes structural thinness.

STOP WHEN:
- exact prose source is missing;
- context capsule blocks required source/context;
- repair would change canon, scene function, outcome, or reveal timing;
- detector-bypass is the goal;
- repair load exceeds 30 percent.

## Copyeditor

ROLE: Copyeditor

START WHEN:
- story, canon, intensity, prose, human surface, and reader pull are acceptable;
- the task is technical consistency.

READ BEFORE:
- copyedit/proofread rule;
- current source;
- term/name/xung ho context;
- Human Surface Polish result if prose was previously flagged as synthetic, over-clean, same-voiced, or falsely smooth;
- Context Capsule result if source status, relationship memory, names, terms, or long-range continuity is in scope.

MAY DO:
- fix names, terms, xung ho, punctuation, repeated words, paragraph breaks, dialogue tags, continuity wording.

MUST NOT DO:
- change story function;
- change character voice for style;
- add scene beats;
- call readiness;
- smooth prose that Human Surface Polish has intentionally left rough.

OUTPUT:
- COPYEDIT_PASS;
- COPYEDIT_NEEDS_FIX;
- exact issues.

DONE WHEN:
- technical consistency issues are cleared or listed.

HANDOFF TO:
- Proofreader if clean;
- Human Surface Polish if prose becomes technically clean but lifeless, same-voiced, or falsely smooth;
- Vietnamese Line Editor if prose is still unnatural;
- Canon Guard if term/source conflict appears.

STOP WHEN:
- story or prose layer fails;
- canon/source conflict appears;
- context capsule blocks source-status or long-range continuity.

## Proofreader

ROLE: Proofreader

START WHEN:
- chapter already passes story, prose, human surface, canon, intensity, and reader checks;
- only final surface errors remain.

READ BEFORE:
- copyedit/proofread rule;
- final source excerpt/chapter;
- Context Capsule result if final status or source-status separation is in scope.

MAY DO:
- catch typo, missing word, wrong name, repeated line, broken punctuation, spacing, paragraph join error, old draft residue.

MUST NOT DO:
- rewrite style;
- change rhythm;
- change story;
- approve publication lock.

OUTPUT:
- PROOFREAD_PASS;
- PROOFREAD_NEEDS_FIX.

DONE WHEN:
- surface errors are cleared or listed.

HANDOFF TO:
- Publishing Readiness Reviewer if all prior layers pass;
- Copyeditor if consistency issue remains;
- Human Surface Polish if proofread exposes lifeless smoothing rather than a typo-level issue.

STOP WHEN:
- line prose, human surface, or story is still failing;
- context capsule blocks source-status separation.

## Publishing Readiness Reviewer

ROLE: Publishing Readiness Reviewer

START WHEN:
- user asks readiness, Human Chapter Pass, Publication Lock, packet lock, or publish candidate;
- source status is current.

READ BEFORE:
- Chapter Index;
- Chapter Review;
- Scene Bank if needed;
- Context Capsule result for current source/status, hidden canon, POV knowledge, and source-status separation;
- Human Surface Polish result if synthetic-surface risk was flagged;
- Publication Lock / Human Chapter Pass fields;
- evidence discipline.

MAY DO:
- check readiness conditions;
- identify blockers;
- state evidence-backed readiness candidate;
- refuse unsupported lock claim.

MUST NOT DO:
- mark publication lock without current evidence;
- treat green prose as publish-ready;
- override human pass;
- use chat memory as lock status.

OUTPUT:
- READY_CANDIDATE;
- NOT_READY;
- EVIDENCE_MISSING;
- blocker list.

DONE WHEN:
- readiness verdict is evidence-backed or blocked.

HANDOFF TO:
- Editorial Director if prioritization is needed;
- Story Doctor, Human Surface Polish, Line Surgery, or Canon Guard depending on blocker.

STOP WHEN:
- current status source was not read;
- context capsule blocks source-status, hidden canon, POV knowledge, or long-range continuity;
- packet contains unready chapter;
- Human Chapter Pass or Publication Lock is missing.

## Editorial Director

ROLE: Editorial Director

START WHEN:
- many problems compete;
- user asks what to fix first;
- packet/arc needs priority;
- AI risks polishing the wrong layer.

READ BEFORE:
- role outputs already run;
- node ledger;
- context brief for large scope;
- Context Capsule result if current source, hidden canon, POV knowledge, source-status separation, or long-range continuity is in scope;
- Human Surface Polish result if the priority is correct-but-synthetic prose;
- evidence discipline;
- user priority.

MAY DO:
- rank blockers;
- choose next node;
- recommend patch vs rewrite vs audit;
- stop unnecessary roles.

MUST NOT DO:
- invent source truth;
- override Canon Guard;
- call publication lock;
- collapse all issues into one vague verdict.

OUTPUT:
- priority order;
- next node;
- role handoff;
- candidate action.

DONE WHEN:
- next action is clear, narrow, and source-safe.

HANDOFF TO:
- any role needed next, named explicitly.

STOP WHEN:
- source/evidence is missing;
- context capsule blocks required source/context;
- priorities depend on unread nodes.

## Learning and calibration boundary

Failure examples, author taste examples, human-surface samples, and future model learning may improve recognition of patterns.

They do not override:

- current user instruction;
- current Notion source;
- canon;
- context capsule when required;
- evidence discipline;
- human pass;
- publication lock.

Use learned taste to choose among safe edits, not to invent facts, bypass detectors, or force a scene into a preferred style.

## Output for role-boundary check

```text
ROLE BOUNDARY CHECK
REQUEST:
ACTIVE ROLE:
START CONDITION MET: YES / NO
SOURCE READY: YES / NO
CONTEXT CAPSULE REQUIRED: YES / NO
CONTEXT CAPSULE STATUS:
HUMAN SURFACE POLISH REQUIRED: YES / NO
MAY DO:
MUST NOT DO:
DONE CRITERIA:
HANDOFF:
STOP CONDITION:
DECISION: CONTINUE / STOP / CANDIDATE_ONLY
```
