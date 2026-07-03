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

Context Capsule is not a prose, story, line, canon, or readiness role. It is a pre-role source/context gate.

Corpus Topic / Thread Discovery is not source authority, canon authority, prose polish, rewrite permission, Human Chapter Pass, readiness, or publication lock. It maps topics, motifs, repeated patterns, and threads with quote/evidence anchors for packet/arc/series navigation.

Narrative Claim Verifier is not canon authority, prose polish, readiness, or publication lock. It verifies claims as TRUE / FALSE / UNCERTAIN.

Multi-Constraint Instruction Ledger is not source authority, canon authority, prose polish, Human Chapter Pass, readiness, or publication lock. It tracks output constraints and drift risk.

Editorial Harm Anticipation is not source authority, canon authority, prose polish, Human Chapter Pass, readiness, or publication lock. It builds AHA-style impact-target / failure-behavior / vignette / harm matrices for REDTEAM, PREMORTEM, readiness risk, packet risk, and high-risk rewrite planning.

Narrative Feature Auditor is not an AI detector, canon authority, prose polish role, or readiness role. It checks story-decision smell before surface repair.

Author Writing Sheet is claim-evidence style memory. It is not canon authority, character voice authority, readiness, or publication lock.

Author Voice Fingerprint is a sample-backed style synthesis role. It is not canon, character voice, or readiness.

Author-Aligned Drafting Assistant is bounded drafting under source, canon, POV, scene function, character voice, multi-constraint ledger, harm anticipation when relevant, author writing sheet, and author fingerprint. It is not autonomous authorship.

Human Surface Polish is not story repair, canon repair, or readiness.

## Role order principle

```text
source and context before topic/thread discovery when current map status matters
topic/thread discovery before packet/arc/series map verdict when map-level navigation is in scope
source and context before claim verification
claim verification before canon/readiness/lock verdict when claims control the route
multi-constraint ledger before rewrite/draft/polish/readiness when multiple constraints control output
editorial harm anticipation before REDTEAM/PREMORTEM/readiness/lock/high-risk rewrite decisions when failure cost is in scope
canon before story
story before narrative feature audit when story-decision smell is in scope
narrative feature audit before intensity / draft / line repair when structural AI smell is the blocker
story before intensity
intensity before author writing sheet use when style claims are in scope
author writing sheet before author voice fingerprint when style claims need evidence
author voice fingerprint before author-aligned drafting
author-aligned draft before line surgery when drafting is requested
line surgery before human surface polish
human surface polish before copyedit
copyedit before proofread
proofread before readiness
readiness before publication lock claim
editorial director chooses priority, not canon truth
```

If a later role discovers an earlier-layer failure, stop and hand back.

## Corpus Topic / Thread Discovery

START WHEN TopicGPT-style topic modeling, packet/arc/part/series map, motif clusters, thread discovery, topic gaps, topic drift, repeated AI-smell clusters, or source assignments with quote anchors are in scope.

READ BEFORE current instruction, context brief for large scope, current source or provided packet, Context Capsule when hidden canon/reveal timing/POV knowledge/source-status separation/long-range continuity is in scope, Source Surface when exact source assignment is required, and corpus topic/thread rule/prompt.

MAY DO build scoped topic/thread map, assign source nodes to topic labels with quote/evidence anchors, mark duplicate/merge candidates, split too-broad topics, flag low-frequency-but-important topics, identify topic gaps and thread drift, and hand off to packet/arc review.

MUST NOT invent canon, invent future payoff, treat topic labels as evidence, use summary-only assignments as final source, delete low-frequency topics without canon/reveal/payoff check, call readiness/Publication Lock, or rewrite from topic labels.

OUTPUT CORPUS_TOPIC_MAP_READY / CORPUS_TOPIC_MAP_NEEDS_SOURCE / CORPUS_TOPIC_MAP_PARTIAL / THREAD_DISCOVERY_HANDOFF / PACKET_REVIEW_HANDOFF / next node.

HANDOFF TO Source Surface, Context Capsule, Narrative Claim Verifier, Tracking / Logic Ledger, Narrative Feature Auditor, Editorial Harm Anticipation, Packet Review, or Editorial Director.

STOP WHEN scope is missing, current source is required but unread, quote/evidence anchor is missing, assignment is summary-only, low-frequency deletion lacks canon/reveal/payoff check, or map is being used as readiness/canon/rewrite permission.

## Canon Guard

START WHEN source conflict, reveal timing risk, invented-fact risk, or lock/status/canon uncertainty appears.

READ BEFORE current instruction, source preflight, Context Capsule when required, Corpus Topic / Thread Discovery when map-level topic/thread assignment may affect canon/reveal, Narrative Claim Verification when a canon/status/source claim is disputed, Multi-Constraint Ledger when canon is one of several output constraints, Editorial Harm Anticipation when canon failure has downstream harm, current Notion/source packet, relevant canon index, evidence discipline.

MAY DO detect source conflict, mark reveal risk, block invented canon, return candidate, request source.

MUST NOT invent lore, decide canon without current source, use legacy Workdeck as current unless named current, or rewrite for style.

HANDOFF TO Corpus Topic / Thread Discovery, Narrative Claim Verifier, Multi-Constraint Instruction Ledger, Editorial Harm Anticipation, Story Doctor, Narrative Feature Auditor, Intensity Editor, Vietnamese Line Editor, Author-Aligned Drafting Assistant, or Line Surgery depending on blocker.

STOP WHEN current source is missing, context capsule blocks, topic assignment lacks evidence, claim verification is UNCERTAIN on a controlling claim, constraint conflict remains unresolved, harm vignette would invent canon, canon conflict lacks current decision, or lock source was not read.

## Narrative Claim Verifier

START WHEN user asks whether a claim is true/false/current/canon/ready/locked, source nodes disagree, a false twin would catch lazy agreement, topic assignment is disputed, or prose/readiness depends on a status/canon/continuity/POV/object/reveal claim.

READ BEFORE current source or provided packet, compressed source only as locator, Context Capsule when required, Tracking / Logic Ledger if state/thread/object/debt is involved, Corpus Topic / Thread Discovery if the claim concerns topic/thread assignment, and claim verification rule/prompt.

MAY DO rewrite vague claims into testable claims, build close false twins, locate evidence nodes, return TRUE / FALSE / UNCERTAIN, and mark low-level detail/misattribution/source conflict risk.

MUST NOT invent evidence, treat outline/summary/context capsule/topic label as current source, silently repair a misattributed claim, call Human Chapter Pass, readiness, Publication Lock, or change prose.

HANDOFF TO Source Surface, Context Capsule, Corpus Topic / Thread Discovery if the claim concerns topic/thread assignment, Multi-Constraint Instruction Ledger if verified claims become output constraints, Editorial Harm Anticipation when false/uncertain claims create harm, Tracking / Logic Ledger, Canon Guard, Narrative Feature Auditor, Readiness Reviewer, or Editorial Director.

STOP WHEN current source is missing, exact surface is needed but unread, claim anchor is unclear, false twin is missing when risk is high, source conflict is unresolved, or evidence supports only UNCERTAIN.

## Multi-Constraint Instruction Ledger

START WHEN rewrite, edit, author-aligned draft, line surgery, human surface polish, readiness, lock, packet review, or audit must preserve multiple source/canon/POV/scene/style/surface/wordcount/readiness constraints together.

READ BEFORE current instruction, current source or provided packet, Context Capsule when required, Narrative Claim Verification if a constraint depends on factual/status/canon evidence, Corpus Topic / Thread Discovery if constraints come from packet/arc/series map, Source Surface if exact output anchor is required, and multi-constraint rule/prompt.

MAY DO extract constraints, assign types and priorities, create corrupted constraints for high-risk items, mark evidence/output anchors, detect conflicts, and grant or block draft/rewrite permission.

MUST NOT invent constraints, treat AI self-evaluation as Human Chapter Pass, override source priority, call Publication Lock, or smooth prose over a broken constraint.

OUTPUT CONSTRAINT_LEDGER_READY / CONSTRAINT_LEDGER_NEEDS_SOURCE / CONSTRAINT_LEDGER_CONFLICT_BLOCKED / DRAFT_PERMISSION_GRANTED / DRAFT_PERMISSION_BLOCKED / next node.

HANDOFF TO Source Surface, Narrative Claim Verifier, Corpus Topic / Thread Discovery if constraints come from packet/arc/series map, Editorial Harm Anticipation when constraint failure has high harm, Tracking / Logic Ledger, Structural Spine, Character Voice / Dialogue / Staging, Author Writing Sheet, Human Surface Polish, Readiness Reviewer, or Editorial Director.

STOP WHEN constraints are missing, high-risk corrupted constraints are missing, constraints conflict, output anchors are missing, exact source is required but unread, source/canon/POV/reveal/readiness constraint is UNCERTAIN, or word target would delete Must Show.

## Editorial Harm Anticipation

START WHEN REDTEAM, PREMORTEM, readiness risk, lock risk, packet failure, topic/thread drift harm, high-risk rewrite failure, false readiness, reveal leak, over-polish harm, style-over-character harm, or AHA-style harm anticipation is in scope.

READ BEFORE current instruction, current source or packet, Context Capsule when required, Narrative Claim Verification when harm depends on status/canon/continuity claim, Multi-Constraint Ledger when constraints control output or prevention, Corpus Topic / Thread Discovery when harm is topic/thread drift, Source Surface when exact output is judged, and harm anticipation rule/prompt.

MAY DO build scoped impact-target / failure-behavior matrix, create concrete failure vignettes, rank severity and detectability, return top 3 harms by severity, and recommend prevention route.

MUST NOT invent future canon as harm evidence, turn harm anticipation into prose repair, use harm matrix as Human Chapter Pass, call readiness/Publication Lock, or create review overload by default.

OUTPUT EDITORIAL_HARM_MATRIX_READY / EDITORIAL_HARM_MATRIX_NEEDS_SOURCE / EDITORIAL_HARM_MATRIX_OVERLOAD_TRIMMED / REDTEAM_HANDOFF / PREMORTEM_HANDOFF / next node.

HANDOFF TO Source Surface, Narrative Claim Verifier, Corpus Topic / Thread Discovery when harm is topic/thread drift, Multi-Constraint Ledger, Narrative Feature Auditor, Character Voice / Dialogue / Staging, Author Writing Sheet, Human Surface Polish, Readiness Reviewer, or Editorial Director.

STOP WHEN scope is missing, current source is required but unread, impact target or failure behavior is unclear, harm depends on unverified claim, vignette would invent canon, matrix creates review overload, or harm anticipation is being used as readiness substitute.

## Story Doctor

START WHEN story motion, changed state, promise/payoff, reader reward, or structure blocks prose work.

READ BEFORE Canon Guard, Narrative Claim Verification if story repair depends on a factual/status/canon claim, Corpus Topic / Thread Discovery if map-level patterns matter, Multi-Constraint Ledger if story repair must preserve multiple constraints, Editorial Harm Anticipation if story failure has downstream harm, Context Capsule when required, Scene Bank/chapter source, Story Outline if needed.

MAY DO identify missing changed state, weak causality, payoff debt, and repair priority.

MUST NOT polish prose to hide story failure, add canon, change ending, call readiness, or authorize drafting without scene controls.

HANDOFF TO Corpus Topic / Thread Discovery if map-level patterns matter, Narrative Claim Verifier, Multi-Constraint Instruction Ledger, Editorial Harm Anticipation, Narrative Feature Auditor, Intensity Editor, Author Writing Sheet, Author Voice Fingerprint, Author-Aligned Drafting Assistant, Vietnamese Line Editor, Line Surgery, or Editorial Director.

STOP WHEN source/scope is missing, context capsule blocks, topic map blocks when required, claim verification blocks, constraint ledger blocks, harm matrix blocks, scene function is unclear, or repair requires canon invention.

## Narrative Feature Auditor

START WHEN user asks about StoryScope, narrative features, structural AI smell, theme overexplained, causal tidiness, single-track plot, protagonist understanding as resolution, weak reveal/recontextualization, temporal flatness, body/sensory overperformance, or narrative diversity.

READ BEFORE current source or provided packet, Context Capsule when required, Corpus Topic / Thread Discovery when map-level repetition, motif clusters, or narrative diversity are in scope, Narrative Claim Verification if the audit depends on a testable claim or false twin, Multi-Constraint Ledger if audit findings become draft constraints, Structural Spine if scene/chapter function is unclear, Tracking / Logic Ledger if state/thread/reveal/debt is in scope, Character Voice / Dialogue / Staging if dialogue function is being evaluated, and narrative feature audit rule/prompt.

MAY DO identify structural AI smell and route to structural/tracking/story/intensity repair.

MUST NOT score authorship, claim detector certainty, invent canon/thread/subplot/clue/object/payoff, turn research labels into prose, authorize Human Chapter Pass/readiness/Publication Lock, or use surface polish to hide story-decision failure.

HANDOFF TO Corpus Topic / Thread Discovery when map-level repetition, motif clusters, or narrative diversity are in scope, Narrative Claim Verifier, Multi-Constraint Instruction Ledger, Editorial Harm Anticipation when structural smell creates downstream harm, Structural Spine, Tracking / Logic Ledger, Story Doctor, Intensity Editor, Author Writing Sheet, Rewrite Scene, Human Surface Polish only after structural smell is cleared, or Editorial Director.

STOP WHEN current source is missing for a current verdict, context capsule blocks, topic map blocks when required, claim verification blocks, constraint ledger blocks, harm matrix blocks, scene question/must show/must not reveal is missing, reveal/thread state is unclear, body/object detail is decorative only, or repair would require canon invention.

## Intensity Editor

START WHEN scene is safe but thin, cost is absent, object lacks consequence, mystery lacks pressure, or correct material underreaches.

READ BEFORE Canon Guard, Story Doctor if available, Narrative Claim Verification if pressure depends on a disputed source claim, Multi-Constraint Ledger if pressure repair must preserve several constraints, Editorial Harm Anticipation if failure has downstream harm, Narrative Feature Audit if body/sensory pressure may be decorative, Context Capsule when required, intensity targets, author taste, current scene source.

MAY DO identify missing cost/body/object/pressure/relation/witness/debt/choice and propose pressure patch from existing source.

MUST NOT add lore or power, escalate by grander prose, change outcome, or rewrite entire scene unless asked.

HANDOFF TO Narrative Claim Verifier, Multi-Constraint Instruction Ledger, Editorial Harm Anticipation, Narrative Feature Auditor, Author Writing Sheet, Author Voice Fingerprint, Author-Aligned Drafting Assistant, Vietnamese Line Editor, Line Surgery, or Story Doctor.

STOP WHEN proposed intensity requires new canon, object/pressure source was not read, context capsule blocks, claim verification blocks, constraint ledger blocks, harm matrix blocks, or more than local patch is needed.

## Author Writing Sheet

START WHEN user asks for Author Writing Sheet, claim-evidence style memory, sample-backed author profile, prompt-specific story rules, or author-style claims need evidence before fingerprint/drafting.

READ BEFORE approved/current author samples, AUTHOR_WORKING_PROFILE.md, AUTHOR_TASTE_EXAMPLES.md, source preflight, Narrative Claim Verification if a style claim depends on factual/status/canon evidence, Multi-Constraint Ledger if style is one of several output constraints, Corpus Topic / Thread Discovery when style/thread clusters are map-level, Character Voice / Dialogue / Staging if character voice may be affected, and author writing sheet rule/prompt.

MAY DO build claim-evidence style memory, classify claims by Plot / Creativity / Development / Language Use, mark counter-average, task fit, and prompt-specific story rules.

MUST NOT infer style from chat memory alone, treat generated text as author sample, turn phrases into style law, override character voice, add canon/object/payoff/reveal, use topic labels as draft controls, or call readiness/Publication Lock.

HANDOFF TO Corpus Topic / Thread Discovery when style/thread clusters are map-level, Multi-Constraint Instruction Ledger when style becomes an output constraint, Editorial Harm Anticipation when style-over-character harm is in scope, Author Voice Fingerprint, Author-Aligned Drafting Assistant, Character Voice / Dialogue / Staging, Human Surface Polish, or Editorial Director.

STOP WHEN samples are missing, unapproved, generated-only, legacy-only, chat-memory-only, style claims lack evidence, Plot/Development claims are under-evidenced, or task fit is unclear.

## Author Voice Fingerprint

START WHEN user asks to decode, learn, preserve, or compare author voice; style guide / voice DNA / writing sample analysis is requested; prose sounds correct but unlike the author; or author-aligned drafting is requested without a task fingerprint.

READ BEFORE explicit author samples or current Notion source named as sample, AUTHOR_WORKING_PROFILE.md, AUTHOR_TASTE_EXAMPLES.md, Author Writing Sheet when style claims need evidence, Multi-Constraint Ledger when style is one of several output constraints, Corpus Topic / Thread Discovery when author-style thread/topic clusters are in scope, source preflight, author voice discipline rule, and Character Voice / Dialogue / Staging when character voice is being compared.

MAY DO extract evidence-backed style traits, build compact style guide, compare passage to fingerprint, separate author rhythm from character voice, and mark sample gaps.

MUST NOT infer author voice from chat memory alone, treat legacy drafts as approved samples unless named current, invent personal facts/canon from prose samples, turn style into formulaic repeated phrases, or call readiness.

HANDOFF TO Author Writing Sheet if evidence is missing, Multi-Constraint Instruction Ledger when fingerprint becomes output constraint, Editorial Harm Anticipation when author-like prose creates high harm risk, Corpus Topic / Thread Discovery when style/thread clusters are map-level, Author-Aligned Drafting Assistant, Human Surface Polish, Narrative Feature Auditor if author-like prose is structurally AI-shaped, or Character Voice / Dialogue / Staging.

STOP WHEN samples are missing, unapproved, legacy-only, chat-memory-only, style claims would be speculative, or author voice would overwrite character voice/canon.

## Author-Aligned Drafting Assistant

START WHEN user asks for author-aligned drafting or writing in the author's voice, source/canon/scene controls are clear, constraints are clear, and author fingerprint or approved taste source is available.

READ BEFORE source surface or current scene packet, Context Capsule when required, Narrative Claim Verification if draft depends on status/canon/continuity/POV/object/reveal claim, Multi-Constraint Ledger for source/canon/POV/scene/style/surface/wordcount constraints, Editorial Harm Anticipation if draft failure risk is high, Author Writing Sheet when style memory or prompt-specific story rules are used, Structural/Tracking if scene function or state is in scope, Narrative Feature Audit if story-decision AI smell is draft risk, Character Voice / Dialogue / Staging if characters speak or interact, Author Voice Fingerprint, and author-aligned draft prompt.

MAY DO draft only requested scope, use author rhythm and scene-thinking habits, preserve source/function/POV/reveal lock/reader effect, mark voice match and human-surface risk, and hand off to Human Surface Polish.

MUST NOT invent canon, object, relation, secret, payoff, route, scene outcome, or reveal timing; override current Notion source; override character voice with author voice; use hidden canon in POV prose; draft from chat memory as source; use topic labels as draft controls; or call Human Chapter Pass/readiness/Publication Lock.

HANDOFF TO Narrative Claim Verifier if a draft claim is uncertain, Multi-Constraint Instruction Ledger if constraints are missing or fail, Editorial Harm Anticipation if draft failure risk is high, Author Writing Sheet if style evidence is missing, Narrative Feature Auditor if draft is author-like but structurally AI-shaped, Human Surface Polish, Line Surgery, Story Doctor, or Canon Guard.

STOP WHEN exact source or scene packet is missing, context capsule blocks, claim verification blocks, constraint ledger blocks, harm matrix blocks when required, author writing sheet blocks when style memory is used, narrative feature blockers remain, author sample/fingerprint is missing, or drafting would change canon/function/POV/outcome/reveal timing.

## Vietnamese Line Editor

START WHEN story/source/canon are settled enough and prose rhythm, dialogue voice, tell/act balance, or AI phrasing leaks.

READ BEFORE prose rhythm, dialogue voice, anti-AI words, SLTD style, author taste, line surgery gate if needed, Multi-Constraint Ledger when line repair must preserve several constraints, Editorial Harm Anticipation if over-polish/false-surface harm is in scope, Author Writing Sheet / Author Voice Fingerprint if style match is in scope, Context Capsule when required.

MAY DO improve rhythm, split/reorder stiff sentences, reduce abstraction, restore body/object/silence/action, and mark need for claim verification, multi-constraint ledger, narrative feature audit, author writing sheet, line surgery, human surface polish, author fingerprint, or scene rewrite.

MUST NOT solve story failure by pretty prose, add beat/canon, make all voices polished, over-literarize, or force author style over character voice.

HANDOFF TO Narrative Claim Verifier, Multi-Constraint Instruction Ledger, Editorial Harm Anticipation, Narrative Feature Auditor, Author Writing Sheet, Author Voice Fingerprint, Human Surface Polish, Copyeditor, Line Surgery, or Story Doctor.

STOP WHEN source/canon/story layer is unsettled, context capsule blocks, claim verification blocks, constraint ledger blocks, harm matrix blocks when required, more than 30 percent needs surgery, or voice cannot be fixed without character source.

## Line Surgery

START WHEN excerpt is 300-1500 words/scoped line set and prose reads stiff, translated, over-clean, or AI-like.

READ BEFORE line surgery gate, prose rhythm, dialogue voice, anti-AI words, SLTD style, author taste, Multi-Constraint Ledger if patch must preserve several constraints, Editorial Harm Anticipation if over-polish/false-surface harm is in scope, Author Writing Sheet / Author Voice Fingerprint if style match is in scope, source excerpt, Context Capsule when required, Narrative Claim Verification if patch depends on a factual claim.

MAY DO label line issues, propose minimal OLD/NEW fixes, run mouth-read check, and mark rewrite threshold.

MUST NOT rewrite whole scene unless asked, change outcome, add metaphor to hide stiffness, add canon/new beats, or turn author style into repeated phrase templates.

HANDOFF TO Narrative Claim Verifier, Multi-Constraint Instruction Ledger, Editorial Harm Anticipation, Narrative Feature Auditor, Human Surface Polish, Author Writing Sheet, Author Voice Fingerprint, Copyeditor, Rewrite Scene, or Vietnamese Line Editor.

STOP WHEN excerpt is too large without sampling instruction, source is missing, context capsule blocks, claim verification blocks, constraint ledger blocks, harm matrix blocks when required, or repair load exceeds 30 percent.

## Human Surface Polish

START WHEN exact current prose surface has been read; story/canon/intensity/voice/author-style needs and line-level permission are settled enough; constraints are clear; harm risk is addressed when relevant; topic-map blockers are not controlling the local surface; and passage is correct in meaning but still synthetic, over-clean, falsely smooth, same-voiced, symbol-first, or thin in body/object/relationship pressure.

READ BEFORE source surface, Context Capsule when required, Narrative Claim Verification if patch depends on factual/canon/continuity claim, Multi-Constraint Ledger if polish must preserve multiple constraints, Editorial Harm Anticipation if over-polish or false-surface harm is in scope, Corpus Topic / Thread Discovery only if the surface issue is actually map-level repetition/thread drift, Narrative Feature Audit if surface polish may hide structural AI smell or decorative body/sensory overperformance, Author Writing Sheet if style memory is used, Vietnamese Senior Editor Surface if needed, Character Voice/Staging if needed, Author Voice Fingerprint if style match is in scope, and human surface rule.

MAY DO identify false smoothing, same-voice polish, symbolic drift, object/body loss, relationship flattening, generic emotional polish; propose minimal OLD/NEW patches; restore body/object/silence/action; route back if load too high.

MUST NOT add canon, scene beat, object, relationship, secret, payoff, metaphor; change function/outcome/reveal timing; make rough characters fluent for smoothness; or call Human Chapter Pass/readiness/Publication Lock.

HANDOFF TO Corpus Topic / Thread Discovery if surface issue is actually map-level repetition/thread drift, Narrative Claim Verifier, Multi-Constraint Instruction Ledger, Editorial Harm Anticipation when over-polish harm is in scope, Narrative Feature Auditor, Author Writing Sheet, Copyeditor, Line Surgery, Author Voice Fingerprint, Voice/Staging, Story Doctor, or Intensity Editor.

STOP WHEN exact prose source is missing, context capsule blocks, topic map blocks when required, claim verification blocks, constraint ledger blocks, harm matrix blocks when required, author writing sheet blocks when style memory is used, narrative feature audit blocks, repair would change canon/function/outcome/reveal timing, or repair load exceeds 30 percent.

## Copyeditor

START WHEN story, claim verification, constraints, harm, narrative feature, canon, intensity, prose, author-aligned/human surface, and reader pull are acceptable and task is technical consistency.

READ BEFORE copyedit/proofread rule, current source, term/name/xưng hô context, Multi-Constraint Ledger if technical changes must preserve constraints, Editorial Harm Anticipation if technical polish may cause harm, Human Surface Polish result if flagged, Author Writing Sheet / Author Voice Fingerprint if style consistency is in scope, Context Capsule when required.

MAY DO fix names, terms, xưng hô, punctuation, repeated words, paragraph breaks, dialogue tags, continuity wording.

MUST NOT change story function, change character voice for style, add scene beats, call readiness, or smooth intentionally rough prose.

HANDOFF TO Proofreader, Human Surface Polish, Vietnamese Line Editor, Narrative Claim Verifier, Multi-Constraint Instruction Ledger, Editorial Harm Anticipation, Narrative Feature Auditor, or Canon Guard.

STOP WHEN story/claim/constraint/harm/narrative feature/prose layer fails, canon/source conflict appears, or context capsule blocks source-status/long-range continuity.

## Proofreader

START WHEN chapter already passes story, claim verification, constraint ledger, harm check when relevant, narrative feature, prose, human surface, canon, intensity, and reader checks, with only final surface errors left.

READ BEFORE copyedit/proofread rule, final source excerpt/chapter, Context Capsule if final status/source separation is in scope.

MAY DO catch typo, missing word, wrong name, repeated line, punctuation, spacing, paragraph join error, old draft residue.

MUST NOT rewrite style, change rhythm, change story, or approve publication lock.

HANDOFF TO Publishing Readiness Reviewer, Copyeditor, or Human Surface Polish.

STOP WHEN claim verification, constraints, harm, narrative feature, line prose, human surface, or story is still failing, or context capsule blocks source-status separation.

## Publishing Readiness Reviewer

START WHEN user asks readiness, Human Chapter Pass, Publication Lock, packet lock, or publish candidate, and source status is current.

READ BEFORE Chapter Index, Chapter Review, Scene Bank if needed, Context Capsule, Narrative Claim Verification for status/Human Pass/Publication Lock/packet lock/source-conflict claims, Multi-Constraint Ledger for readiness constraints/corrupted constraints, Editorial Harm Anticipation for false readiness / lock / downstream harm, Corpus Topic / Thread Discovery only if packet/arc topic/thread map is explicitly requested, Narrative Feature Audit if false readiness may come from clean-but-AI-shaped story structure, Author Writing Sheet / Author Voice / Author-Aligned Draft result if used, Human Surface Polish if flagged, Publication Lock / Human Chapter Pass fields, evidence discipline.

MAY DO check readiness conditions, identify blockers, state evidence-backed candidate, refuse unsupported lock claim.

MUST NOT mark publication lock without current evidence, treat green prose, topic coherence, author-style match, claim verification, constraint ledger, harm matrix, writing sheet, or narrative-feature pass as publish-ready, override human pass, or use chat memory as lock status.

HANDOFF TO Editorial Director, Corpus Topic / Thread Discovery when packet map is requested, Narrative Claim Verifier, Multi-Constraint Ledger, Editorial Harm Anticipation, Story Doctor, Narrative Feature Auditor, Author Writing Sheet, Author Voice Fingerprint, Author-Aligned Drafting Assistant, Human Surface Polish, Line Surgery, or Canon Guard.

STOP WHEN current status source was not read, context capsule blocks, topic map is being used as readiness substitute, claim verification is UNCERTAIN or false on controlling readiness/lock claim, constraint ledger blocks, harm matrix blocks, packet contains unready chapter, or Human Chapter Pass / Publication Lock is missing.

## Editorial Director

START WHEN many problems compete, user asks what to fix first, packet/arc needs priority, or AI risks polishing/drafting/routing the wrong layer.

READ BEFORE role outputs already run, node ledger, context brief for large scope, Context Capsule when required, Corpus Topic / Thread Discovery if packet/arc map informs priority, Narrative Claim Verification if priority depends on source/status/canon claim, Multi-Constraint Ledger if priority depends on constraints, Editorial Harm Anticipation if priority depends on failure cost, Narrative Feature Audit if priority is structural AI smell, Author Writing Sheet / Author Voice / Author-Aligned Draft result if priority is style/drafting, Human Surface Polish if priority is correct-but-synthetic prose, evidence discipline, user priority.

MAY DO rank blockers, choose next node, recommend patch vs rewrite vs audit, stop unnecessary roles.

MUST NOT invent source truth, override Canon Guard, call publication lock, or collapse issues into vague verdict.

HANDOFF TO any role needed next, named explicitly.

STOP WHEN source/evidence is missing, context capsule blocks required source/context, topic map blocks, claim verification blocks a controlling claim, constraint ledger blocks, harm matrix blocks, or priorities depend on unread nodes.

## Learning and calibration boundary

Failure examples, author taste examples, corpus topic samples, multi-constraint samples, editorial harm samples, author writing sheet samples, author voice samples, narrative-claim samples, narrative-feature samples, human-surface samples, and future model learning may improve recognition of patterns.

They do not override current user instruction, current Notion source, canon, context capsule when required, evidence discipline, character voice, human pass, or publication lock.

Use learned taste and topic maps to choose among safe routes, not to invent facts, detector-score a chapter, or force a scene into a preferred style.

## Output for role-boundary check

```text
ROLE BOUNDARY CHECK
REQUEST:
ACTIVE ROLE:
START CONDITION MET: YES / NO
SOURCE READY: YES / NO
CONTEXT CAPSULE REQUIRED: YES / NO
CONTEXT CAPSULE STATUS:
CORPUS TOPIC / THREAD DISCOVERY REQUIRED: YES / NO
CLAIM VERIFICATION REQUIRED: YES / NO
MULTI-CONSTRAINT LEDGER REQUIRED: YES / NO
EDITORIAL HARM ANTICIPATION REQUIRED: YES / NO
NARRATIVE FEATURE REQUIRED: YES / NO
AUTHOR WRITING SHEET REQUIRED: YES / NO
AUTHOR VOICE / DRAFTING REQUIRED: YES / NO
HUMAN SURFACE POLISH REQUIRED: YES / NO
MAY DO:
MUST NOT DO:
DONE CRITERIA:
HANDOFF:
STOP CONDITION:
DECISION: CONTINUE / STOP / CANDIDATE_ONLY
```