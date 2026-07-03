# SLTD Role Boundary Contracts

This rule defines where each editorial role starts, stops, hands off, and must not act.

It prevents role mixing, false authority, and polishing the wrong layer.

## Global contract

Every role must obey current user instruction, current Notion source or current packet, source preflight, context capsule when required, decision safety, evidence discipline, canon guard, and node checkpoint.

A role may produce a candidate. It may not silently update Notion, GitHub, or manuscript source.

Review modes change the lens. They do not become roles.

Context Capsule is not a prose, story, line, canon, or readiness role.

Reference-Anchored Longform Story Quality is not source authority, canon authority, prose polish, rewrite permission, Human Chapter Pass, readiness, or Publication Lock. It checks whether long draft/rewrite/chapter/packet output sustains source-safe quality across length.

Corpus Topic / Thread Discovery is not source authority, canon authority, prose polish, rewrite permission, Human Chapter Pass, readiness, or Publication Lock. It maps topics, motifs, repeated patterns, and threads with quote/evidence anchors.

Narrative Claim Verifier is not canon authority, prose polish, readiness, or Publication Lock. It verifies claims as TRUE / FALSE / UNCERTAIN.

Multi-Constraint Instruction Ledger is not source authority, canon authority, prose polish, Human Chapter Pass, readiness, or Publication Lock. It tracks output constraints and drift risk.

Editorial Harm Anticipation is not source authority, canon authority, prose polish, Human Chapter Pass, readiness, or Publication Lock. It builds REDTEAM/PREMORTEM risk vignettes.

Narrative Feature Auditor is not an AI detector, canon authority, prose polish role, or readiness role. It checks story-decision smell before surface repair.

Author Writing Sheet is claim-evidence style memory. It is not canon authority, character voice authority, readiness, or Publication Lock.

Author Voice Fingerprint is a sample-backed style synthesis role. It is not canon, character voice, or readiness.

Author-Aligned Drafting Assistant is bounded drafting under source, canon, POV, scene function, character voice, multi-constraint ledger, harm anticipation when relevant, reference-quality check when relevant, author writing sheet, and author fingerprint.

Human Surface Polish is not story repair, canon repair, or readiness.

## Role order principle

```text
source and context before topic/thread discovery or longform quality when current evidence matters
longform quality before chapter/packet acceptance when quality across length is in scope
topic/thread discovery before packet/arc/series map verdict when map-level navigation is in scope
claim verification before canon/readiness/lock verdict when claims control the route
multi-constraint ledger before rewrite/draft/polish/readiness when multiple constraints control output
editorial harm anticipation before REDTEAM/PREMORTEM/readiness/lock/high-risk rewrite decisions when failure cost is in scope
story before narrative feature audit when story-decision smell is in scope
author writing sheet before author voice fingerprint when style claims need evidence
author voice fingerprint before author-aligned drafting
line surgery before human surface polish
human surface polish before copyedit
copyedit before proofread
readiness before publication lock claim
```

If a later role discovers an earlier-layer failure, stop and hand back.

## Reference-Anchored Longform Story Quality

START WHEN POLARIS-style story quality, long rewrite quality, chapter assembly quality, packet candidate quality, length adherence, bloat, drift, over-summary, over-explanation, late-output collapse, or reference-anchored quality is in scope.

READ BEFORE current instruction, current source or packet, exact output being judged, Context Capsule when current source or long-range context is in scope, Narrative Claim Verification when quality depends on factual/status/canon evidence, Multi-Constraint Ledger when output constraints control the draft, Editorial Harm Anticipation when false quality/readiness harm is in scope, Corpus Topic / Thread Discovery when packet/arc map-level quality is in scope, and the POLARIS rule/prompt.

MAY DO assess positive and negative quality dimensions, check target/actual length, mark Must Show preservation, identify bloat/drift/over-summary/late collapse, use only user-approved/current anchors, and recommend next route.

MUST NOT use a quality score without source, reward length when Must Show is cut, use an unauthorized anchor, treat generated or legacy text as anchor unless approved, call Human Chapter Pass/readiness/Publication Lock, or copy protected reference text.

HANDOFF TO Source Surface, Context Capsule, Narrative Claim Verifier, Multi-Constraint Ledger, Editorial Harm Anticipation, Corpus Topic / Thread Discovery, Narrative Feature Auditor, Human Surface Polish, Readiness Reviewer, or Editorial Director.

STOP WHEN source is missing, output is missing, exact prose is required but unread, anchor is required but unauthorized, Must Show source is missing, length target is needed but missing, quality depends on unverified source/canon/status claim, or the result is being used as readiness substitute.

## Corpus Topic / Thread Discovery

START WHEN TopicGPT-style topic modeling, packet/arc/part/series map, motif clusters, thread discovery, topic gaps, topic drift, repeated pattern clusters, or source assignments with quote anchors are in scope.

MAY DO build scoped topic/thread map, assign source nodes to topic labels with quote/evidence anchors, mark duplicate/merge candidates, split too-broad topics, flag low-frequency-but-important topics, identify topic gaps and thread drift, and hand off to packet/arc review.

MUST NOT invent canon, invent future payoff, treat topic labels as evidence, use summary-only assignments as final source, delete low-frequency topics without canon/reveal/payoff check, call readiness/Publication Lock, or rewrite from topic labels.

STOP WHEN scope is missing, current source is required but unread, quote/evidence anchor is missing, assignment is summary-only, low-frequency deletion lacks canon/reveal/payoff check, or map is being used as readiness/canon/rewrite permission.

## Claim / Constraint / Harm roles

Narrative Claim Verifier verifies current/source/canon/continuity/POV/object/reveal/readiness/lock/topic/quality claims as TRUE / FALSE / UNCERTAIN. It must not invent evidence or call readiness.

Multi-Constraint Instruction Ledger extracts constraints, corrupted constraints, priorities, and output anchors. It must not invent constraints, smooth over broken constraints, or call readiness.

Editorial Harm Anticipation builds scoped impact-target / failure-behavior / vignette / harm matrices. It must not invent future canon, become prose repair, or call readiness.

Each of these roles hands off to the next smallest source-safe route and stops at missing source, missing anchor, unresolved conflict, or readiness substitution.

## Story / feature / voice / author / surface roles

Story Doctor handles changed state, promise/payoff, reader reward, and story motion. It must not polish prose to hide story failure.

Narrative Feature Auditor checks story-decision smell, over-tidy causality, weak reveal, temporal flatness, decorative body/sensory pressure, and narrative diversity. It is not a detector or readiness role.

Character Voice / Dialogue / Staging handles dialogue, relationship memory, silence, location staging, and character presence. It must not flatten character voice under author style.

Author Writing Sheet builds evidence-backed style memory. It must not infer style from chat memory alone or override character voice/canon.

Author Voice Fingerprint compares and summarizes sample-backed style. It must not turn style into formula or call readiness.

Author-Aligned Drafting Assistant drafts only requested scope after source, context, claim, constraint, harm, reference-quality when relevant, author evidence, and character voice controls are clear.

Vietnamese Line Editor, Line Surgery, Copyeditor, Proofreader, and Human Surface Polish operate only after source/canon/story/topic/claim/constraint/harm/quality blockers are clear enough for their layer.

## Publishing Readiness Reviewer

START WHEN readiness, Human Chapter Pass, Publication Lock, packet lock, or publish candidate is requested and source status is current.

READ BEFORE Chapter Index, Chapter Review, Scene Bank if needed, Context Capsule, Narrative Claim Verification for status/Human Pass/Publication Lock/packet lock/source-conflict claims, Multi-Constraint Ledger for readiness constraints, Editorial Harm Anticipation for false readiness / lock / downstream harm, Reference-Anchored Longform Story Quality only as readiness-risk evidence when requested, Corpus Topic / Thread Discovery only if packet/arc map is requested, Narrative Feature Audit when clean-but-false readiness is possible, Human Surface Polish if flagged, and evidence discipline.

MAY DO check readiness conditions, identify blockers, state evidence-backed candidate, and refuse unsupported lock claim.

MUST NOT mark Publication Lock without current evidence, treat topic coherence, longform quality, author-style match, claim verification, constraint ledger, harm matrix, writing sheet, or narrative-feature pass as publish-ready, override human pass, or use chat memory as lock status.

STOP WHEN current status source was not read, context capsule blocks, quality check is being used as readiness substitute, topic map is being used as readiness substitute, claim verification is UNCERTAIN or false on controlling readiness/lock claim, constraint ledger blocks, harm matrix blocks, packet contains unready chapter, or Human Chapter Pass / Publication Lock is missing.

## Editorial Director

START WHEN many problems compete, user asks what to fix first, packet/arc needs priority, or AI risks polishing/drafting/routing the wrong layer.

MAY DO rank blockers, choose next node, recommend patch vs rewrite vs audit, and stop unnecessary roles.

MUST NOT invent source truth, override Canon Guard, call Publication Lock, or collapse issues into vague verdict.

STOP WHEN source/evidence is missing, context capsule blocks required source/context, quality check blocks, topic map blocks, claim verification blocks a controlling claim, constraint ledger blocks, harm matrix blocks, or priorities depend on unread nodes.

## Learning and calibration boundary

Failure examples, author taste examples, reference-quality samples, corpus topic samples, multi-constraint samples, editorial harm samples, author writing sheet samples, author voice samples, narrative-claim samples, narrative-feature samples, and human-surface samples may improve recognition of patterns.

They do not override current user instruction, current Notion source, canon, context capsule when required, evidence discipline, character voice, human pass, or Publication Lock.

## Output for role-boundary check

```text
ROLE BOUNDARY CHECK
REQUEST:
ACTIVE ROLE:
START CONDITION MET: YES / NO
SOURCE READY: YES / NO
CONTEXT CAPSULE REQUIRED: YES / NO
CONTEXT CAPSULE STATUS:
REFERENCE-ANCHORED STORY QUALITY REQUIRED: YES / NO
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