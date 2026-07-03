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

Narrative Claim Verifier is not canon authority, prose polish, readiness, or publication lock. It is an evidence/source role that verifies claims as TRUE / FALSE / UNCERTAIN.

Narrative Feature Auditor is not an AI detector, canon authority, prose polish role, or readiness role. It is a structural-story role that checks story-decision smell before surface repair.

Author Voice Fingerprint is a sample-backed style extraction role. It is not canon, character voice, or readiness.

Author-Aligned Drafting Assistant is bounded drafting under source, canon, POV, scene function, character voice, and author fingerprint. It is not autonomous authorship.

Human Surface Polish is not story repair, canon repair, or readiness. It is a late prose role used only after source/context/story/voice constraints are clear enough.

## Role order principle

```text
source and context before claim verification
claim verification before canon/readiness/lock verdict when claims control the route
canon before story
story before narrative feature audit when story-decision smell is in scope
narrative feature audit before intensity / draft / line repair when structural AI smell is the blocker
story before intensity
intensity before author voice use
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

## Canon Guard

START WHEN source conflict, reveal timing risk, invented-fact risk, or lock/status/canon uncertainty appears.

READ BEFORE current instruction, source preflight, Context Capsule when required, Narrative Claim Verification when a canon/status/source claim is disputed, current Notion/source packet, relevant canon index, evidence discipline.

MAY DO detect source conflict, mark reveal risk, block invented canon, return candidate, request source.

MUST NOT invent lore, decide canon without current source, use legacy Workdeck as current unless named current, or rewrite for style.

HANDOFF TO Narrative Claim Verifier, Story Doctor, Narrative Feature Auditor, Intensity Editor, Vietnamese Line Editor, Author-Aligned Drafting Assistant, or Line Surgery depending on blocker.

STOP WHEN current source is missing, context capsule blocks, claim verification is UNCERTAIN on a controlling claim, canon conflict lacks current decision, or lock source was not read.

## Narrative Claim Verifier

START WHEN user asks whether a claim is true/false/current/canon/ready/locked, when source nodes disagree, when a false twin would catch lazy agreement, or when prose/readiness depends on a status/canon/continuity/POV/object/reveal claim.

READ BEFORE current source or provided packet, compressed source only as locator, Context Capsule when required, Tracking / Logic Ledger if state/thread/object/debt is involved, and claim verification rule/prompt.

MAY DO rewrite vague claims into testable claims, build close false twins, locate evidence nodes, return TRUE / FALSE / UNCERTAIN, mark low-level detail risk, misattribution risk, and source conflict.

MUST NOT invent evidence, treat outline/summary/context capsule as current source, silently repair a misattributed claim, call Human Chapter Pass, readiness, Publication Lock, or change prose.

OUTPUT CLAIM_VERIFIED / CLAIM_FALSE_REPAIR_NEEDED / CLAIM_UNCERTAIN_SOURCE_NEEDED / next node.

HANDOFF TO Source Surface, Context Capsule, Tracking / Logic Ledger, Canon Guard, Narrative Feature Auditor, Readiness Reviewer, or Editorial Director.

STOP WHEN current source is missing, exact surface is needed but unread, claim anchor is unclear, false twin is missing when risk is high, source conflict is unresolved, or evidence supports only UNCERTAIN.

## Story Doctor

START WHEN story motion, changed state, promise/payoff, reader reward, or structure blocks prose work.

READ BEFORE Canon Guard, Narrative Claim Verification if story repair depends on a factual/status/canon claim, Context Capsule when required, Scene Bank/chapter source, Story Outline if needed.

MAY DO identify missing changed state, weak causality, payoff debt, and repair priority.

MUST NOT polish prose to hide story failure, add canon, change ending, call readiness, or authorize drafting without scene controls.

HANDOFF TO Narrative Claim Verifier if a source claim controls the repair, Narrative Feature Auditor if story is functional but AI-shaped, Intensity Editor, Author Voice Fingerprint, Author-Aligned Drafting Assistant, Vietnamese Line Editor, Line Surgery, or Editorial Director.

STOP WHEN source/scope is missing, context capsule blocks, claim verification blocks, scene function is unclear, or repair requires canon invention.

## Narrative Feature Auditor

START WHEN user asks about StoryScope, narrative features, structural AI smell, theme overexplained, causal tidiness, single-track plot, protagonist understanding as resolution, weak reveal/recontextualization, temporal flatness, body/sensory overperformance, or narrative diversity.

READ BEFORE current source or provided packet, Context Capsule when required, Narrative Claim Verification if the audit depends on a testable claim or false twin, Structural Spine if scene/chapter function is unclear, Tracking / Logic Ledger if state/thread/reveal/debt is in scope, Character Voice / Dialogue / Staging if dialogue function is being evaluated, and narrative feature audit rule/prompt.

MAY DO identify structural AI smell, theme overexplicitness, causal tidiness, single-track plot risk, under-costed understanding resolution, weak reveal, temporal flatness, thread thinness, moral simplification, decorative body/sensory pressure, and setting mirror overfit.

MUST NOT score authorship, claim detector certainty, invent canon/thread/subplot/clue/object/payoff, turn research labels into prose, authorize Human Chapter Pass/readiness/Publication Lock, or use surface polish to hide story-decision failure.

OUTPUT NARRATIVE_FEATURE_READY / NARRATIVE_FEATURE_NEEDS_PATCH / NARRATIVE_FEATURE_BLOCKED / next node.

HANDOFF TO Narrative Claim Verifier, Structural Spine, Tracking / Logic Ledger, Story Doctor, Intensity Editor, Rewrite Scene, Human Surface Polish only after structural smell is cleared, or Editorial Director.

STOP WHEN current source is missing for a current verdict, context capsule blocks, claim verification blocks, scene question/must show/must not reveal is missing, reveal/thread state is unclear, body/object detail is decorative only, or repair would require canon invention.

## Intensity Editor

START WHEN scene is safe but thin, cost is absent, object lacks consequence, mystery lacks pressure, or correct material underreaches.

READ BEFORE Canon Guard, Story Doctor if available, Narrative Claim Verification if pressure depends on a disputed source claim, Narrative Feature Audit if body/sensory pressure may be decorative, Context Capsule when required, intensity targets, author taste, current scene source.

MAY DO identify missing cost/body/object/pressure/relation/witness/debt/choice and propose pressure patch from existing source.

MUST NOT add lore or power, escalate by grander prose, change outcome, or rewrite entire scene unless asked.

HANDOFF TO Narrative Claim Verifier, Narrative Feature Auditor if pressure repair may still be structurally AI-shaped, Author Voice Fingerprint, Author-Aligned Drafting Assistant, Vietnamese Line Editor, Line Surgery, or Story Doctor.

STOP WHEN proposed intensity requires new canon, object/pressure source was not read, context capsule blocks, claim verification blocks, or more than local patch is needed.

## Author Voice Fingerprint

START WHEN user asks to decode, learn, preserve, or compare author voice; style guide / voice DNA / writing sample analysis is requested; prose sounds correct but unlike the author; or author-aligned drafting is requested without a task fingerprint.

READ BEFORE explicit author samples or current Notion source named as sample, AUTHOR_WORKING_PROFILE.md, AUTHOR_TASTE_EXAMPLES.md, source preflight, author voice discipline rule, and Character Voice / Dialogue / Staging when character voice is being compared.

MAY DO extract evidence-backed style traits, build compact style guide, compare passage to fingerprint, separate author rhythm from character voice, and mark sample gaps.

MUST NOT infer author voice from chat memory alone, treat legacy drafts as approved samples unless named current, invent personal facts/canon from prose samples, turn style into formulaic repeated phrases, or call readiness.

OUTPUT AUTHOR_VOICE_FINGERPRINT_OK / AUTHOR_VOICE_FINGERPRINT_PARTIAL / AUTHOR_SAMPLE_MISSING / voice match matrix / next node.

HANDOFF TO Author-Aligned Drafting Assistant, Human Surface Polish, Narrative Feature Auditor if author-like prose is structurally AI-shaped, or Character Voice / Dialogue / Staging.

STOP WHEN samples are missing, unapproved, legacy-only, or chat-memory-only; style claims would be speculative; or author voice would overwrite character voice/canon.

## Author-Aligned Drafting Assistant

START WHEN user asks for author-aligned drafting or writing in the author's voice, source/canon/scene controls are clear, and an author fingerprint or approved taste source is available.

READ BEFORE source surface or current scene packet, Context Capsule when required, Narrative Claim Verification if draft depends on status/canon/continuity/POV/object/reveal claim, Structural/Tracking if scene function or state is in scope, Narrative Feature Audit if story-decision AI smell is the draft risk, Character Voice / Dialogue / Staging if characters speak or interact, Author Voice Fingerprint, and author-aligned draft prompt.

MAY DO draft only requested scope, use author rhythm and scene-thinking habits, preserve source/function/POV/reveal lock/reader effect, mark voice match and human-surface risk, and hand off to Human Surface Polish.

MUST NOT invent canon, object, relation, secret, payoff, route, scene outcome, or reveal timing; override current Notion source; override character voice with author voice; use hidden canon in POV prose; draft from chat memory as source; or call Human Chapter Pass/readiness/Publication Lock.

OUTPUT AUTHOR_ALIGNED_DRAFT_READY / AUTHOR_ALIGNED_DRAFT_BLOCKED / bounded draft / self-check / next node.

HANDOFF TO Narrative Claim Verifier if a draft claim is uncertain, Narrative Feature Auditor if draft is author-like but structurally AI-shaped, Human Surface Polish, Line Surgery, Story Doctor, or Canon Guard depending on blocker.

STOP WHEN exact source or scene packet is missing, context capsule blocks, claim verification blocks, narrative feature blockers remain, author sample/fingerprint is missing, or drafting would change canon/function/POV/outcome/reveal timing.

## Vietnamese Line Editor

START WHEN story/source/canon are settled enough and prose rhythm, dialogue voice, tell/act balance, or AI phrasing leaks.

READ BEFORE prose rhythm, dialogue voice, anti-AI words, SLTD style, author taste, line surgery gate if needed, Author Voice Fingerprint if style match is in scope, Context Capsule when required.

MAY DO improve rhythm, split/reorder stiff sentences, reduce abstraction, restore body/object/silence/action, and mark need for claim verification, narrative feature audit, line surgery, human surface polish, author fingerprint, or scene rewrite.

MUST NOT solve story failure by pretty prose, add beat/canon, make all voices polished, over-literarize, or force author style over character voice.

HANDOFF TO Narrative Claim Verifier if a line repair depends on a source claim, Narrative Feature Auditor if smooth prose hides structural AI smell, Author Voice Fingerprint, Human Surface Polish, Copyeditor, Line Surgery, or Story Doctor.

STOP WHEN source/canon/story layer is unsettled, context capsule blocks, claim verification blocks, more than 30 percent needs surgery, or voice cannot be fixed without character source.

## Line Surgery

START WHEN excerpt is 300-1500 words/scoped line set and prose reads stiff, translated, over-clean, or AI-like.

READ BEFORE line surgery gate, prose rhythm, dialogue voice, anti-AI words, SLTD style, author taste, Author Voice Fingerprint if style match is in scope, source excerpt, Context Capsule when required, Narrative Claim Verification if patch depends on a factual claim.

MAY DO label line issues, propose minimal OLD/NEW fixes, run mouth-read check, and mark rewrite threshold.

MUST NOT rewrite whole scene unless asked, change outcome, add metaphor to hide stiffness, add canon/new beats, or turn author style into repeated phrase templates.

HANDOFF TO Narrative Claim Verifier if source claim is uncertain, Narrative Feature Auditor if line repair may hide story-decision AI smell, Human Surface Polish, Author Voice Fingerprint, Copyeditor, Rewrite Scene, or Vietnamese Line Editor.

STOP WHEN excerpt is too large without sampling instruction, source is missing, context capsule blocks, claim verification blocks, or repair load exceeds 30 percent.

## Human Surface Polish

START WHEN exact current prose surface has been read; story/canon/intensity/voice/author-style needs and line-level permission are settled enough; and passage is correct in meaning but still synthetic, over-clean, falsely smooth, same-voiced, symbol-first, or thin in body/object/relationship pressure.

READ BEFORE source surface, Context Capsule when required, Narrative Claim Verification if patch depends on factual/canon/continuity claim, Narrative Feature Audit if surface polish may hide structural AI smell or decorative body/sensory overperformance, Vietnamese Senior Editor Surface if needed, Character Voice/Staging if needed, Author Voice Fingerprint if style match is in scope, and human surface rule.

MAY DO identify false smoothing, same-voice polish, symbolic drift, object/body loss, relationship flattening, generic emotional polish; propose minimal OLD/NEW patches; restore body/object/silence/action; route back if load too high.

MUST NOT add canon, scene beat, object, relationship, secret, payoff, metaphor; change function/outcome/reveal timing; make rough characters fluent for smoothness; or call Human Chapter Pass/readiness/Publication Lock.

HANDOFF TO Narrative Claim Verifier if evidence is uncertain, Narrative Feature Auditor if structural smell remains, Copyeditor, Line Surgery, Author Voice Fingerprint, Voice/Staging, Story Doctor, or Intensity Editor.

STOP WHEN exact prose source is missing, context capsule blocks, claim verification blocks, narrative feature audit blocks, repair would change canon/function/outcome/reveal timing, or repair load exceeds 30 percent.

## Copyeditor

START WHEN story, claim verification, narrative feature, canon, intensity, prose, author-aligned/human surface, and reader pull are acceptable and task is technical consistency.

READ BEFORE copyedit/proofread rule, current source, term/name/xưng hô context, Human Surface Polish result if flagged, Author Voice Fingerprint if style consistency is in scope, Context Capsule when required.

MAY DO fix names, terms, xưng hô, punctuation, repeated words, paragraph breaks, dialogue tags, continuity wording.

MUST NOT change story function, change character voice for style, add scene beats, call readiness, or smooth intentionally rough prose.

HANDOFF TO Proofreader, Human Surface Polish, Vietnamese Line Editor, Narrative Claim Verifier if technical clean-up exposes source conflict, Narrative Feature Auditor if structural AI smell appears, or Canon Guard.

STOP WHEN story/claim/narrative feature/prose layer fails, canon/source conflict appears, or context capsule blocks source-status/long-range continuity.

## Proofreader

START WHEN chapter already passes story, claim verification, narrative feature, prose, human surface, canon, intensity, and reader checks, with only final surface errors left.

READ BEFORE copyedit/proofread rule, final source excerpt/chapter, Context Capsule if final status/source separation is in scope.

MAY DO catch typo, missing word, wrong name, repeated line, punctuation, spacing, paragraph join error, old draft residue.

MUST NOT rewrite style, change rhythm, change story, or approve publication lock.

HANDOFF TO Publishing Readiness Reviewer, Copyeditor, or Human Surface Polish.

STOP WHEN claim verification, narrative feature, line prose, human surface, or story is still failing, or context capsule blocks source-status separation.

## Publishing Readiness Reviewer

START WHEN user asks readiness, Human Chapter Pass, Publication Lock, packet lock, or publish candidate, and source status is current.

READ BEFORE Chapter Index, Chapter Review, Scene Bank if needed, Context Capsule, Narrative Claim Verification for status/Human Pass/Publication Lock/packet lock/source-conflict claims, Narrative Feature Audit if false readiness may come from clean-but-AI-shaped story structure, Author Voice / Author-Aligned Draft result if used, Human Surface Polish if flagged, Publication Lock / Human Chapter Pass fields, evidence discipline.

MAY DO check readiness conditions, identify blockers, state evidence-backed candidate, refuse unsupported lock claim.

MUST NOT mark publication lock without current evidence, treat green prose, author-style match, claim verification, or narrative-feature pass as publish-ready, override human pass, or use chat memory as lock status.

HANDOFF TO Editorial Director, Narrative Claim Verifier, Story Doctor, Narrative Feature Auditor, Author Voice Fingerprint, Author-Aligned Drafting Assistant, Human Surface Polish, Line Surgery, or Canon Guard depending on blocker.

STOP WHEN current status source was not read, context capsule blocks, claim verification is UNCERTAIN or false on controlling readiness/lock claim, packet contains unready chapter, or Human Chapter Pass / Publication Lock is missing.

## Editorial Director

START WHEN many problems compete, user asks what to fix first, packet/arc needs priority, or AI risks polishing/drafting/routing the wrong layer.

READ BEFORE role outputs already run, node ledger, context brief for large scope, Context Capsule when required, Narrative Claim Verification if priority depends on source/status/canon claim, Narrative Feature Audit if priority is structural AI smell, Author Voice / Author-Aligned Draft result if priority is author-style/drafting, Human Surface Polish if priority is correct-but-synthetic prose, evidence discipline, user priority.

MAY DO rank blockers, choose next node, recommend patch vs rewrite vs audit, stop unnecessary roles.

MUST NOT invent source truth, override Canon Guard, call publication lock, or collapse issues into vague verdict.

HANDOFF TO any role needed next, named explicitly.

STOP WHEN source/evidence is missing, context capsule blocks required source/context, claim verification blocks a controlling claim, or priorities depend on unread nodes.

## Learning and calibration boundary

Failure examples, author taste examples, author voice samples, narrative-claim samples, narrative-feature samples, human-surface samples, and future model learning may improve recognition of patterns.

They do not override current user instruction, current Notion source, canon, context capsule when required, evidence discipline, character voice, human pass, or publication lock.

Use learned taste to choose among safe edits, not to invent facts, detector-score a chapter, or force a scene into a preferred style.

## Output for role-boundary check

```text
ROLE BOUNDARY CHECK
REQUEST:
ACTIVE ROLE:
START CONDITION MET: YES / NO
SOURCE READY: YES / NO
CONTEXT CAPSULE REQUIRED: YES / NO
CONTEXT CAPSULE STATUS:
CLAIM VERIFICATION REQUIRED: YES / NO
NARRATIVE FEATURE REQUIRED: YES / NO
AUTHOR VOICE / DRAFTING REQUIRED: YES / NO
HUMAN SURFACE POLISH REQUIRED: YES / NO
MAY DO:
MUST NOT DO:
DONE CRITERIA:
HANDOFF:
STOP CONDITION:
DECISION: CONTINUE / STOP / CANDIDATE_ONLY
```