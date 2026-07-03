# SLTD Author Voice Fingerprint & Ghostwriter Discipline

This rule lets SLTD learn an author's usable writing fingerprint from source-backed samples, then draft in an author-aligned way without taking authorial authority.

It adapts author-voice and ghostwriter ideas for long-form SLTD editing. It does not replace source discipline, canon guard, character voice, or human approval.

## Core rule

Ghostwriter may imitate author rhythm. Ghostwriter may not imitate author authority.

Author voice is evidence, not permission. A style match can guide diction, rhythm, paragraph breath, restraint, and pressure handling, but it cannot decide canon, scene function, reveal timing, Human Chapter Pass, or Publication Lock.

## Use when

- the user asks to decode, learn, match, or preserve the author's voice;
- the user asks for style guide, voice DNA, author fingerprint, or sample-based style extraction;
- prose sounds correct but not like the author;
- AI keeps writing generic Vietnamese prose instead of SLTD taste;
- the user asks for ghostwriter / viết thay / viết theo giọng tôi / viết như tôi;
- a rewrite needs author-aligned draft after source, context, scene function, and voice constraints are clear.

## Authority

Run Author Voice Fingerprint only from explicit source samples:

```text
current user-provided sample
current Notion source named as author sample
AUTHOR_TASTE_EXAMPLES.md
AUTHOR_WORKING_PROFILE.md
approved manuscript excerpt named by the user
```

Do not infer author voice from chat memory, summaries, old Workdecks, raw drafts, or generic assumptions unless the user explicitly names them as sample material.

Run Author-Aligned Ghostwriter Draft after:

```text
source preflight
source surface when exact prose/source is required
context capsule when current source, hidden canon, POV knowledge, source-status separation, object/location/body/debt state, relationship memory, or long-range continuity is in scope
structural / tracking / voice / Vietnamese senior surface gates when their blockers are in scope
author voice fingerprint when style matching is in scope
```

Run it before:

```text
human surface polish
copyedit
proofread
readiness
publication lock claim
```

## Required distinction

```text
AUTHOR VOICE FINGERPRINT = extracts author habits from approved samples
AUTHOR STYLE GUIDE = compact operating summary of the fingerprint
AUTHOR THINKING MODEL = how the author tends to build scene pressure and withhold information
AUTHOR-ALIGNED GHOSTWRITER DRAFT = drafts prose under source/canon/POV/scene limits using the fingerprint
HUMAN SURFACE POLISH = repairs correct-but-synthetic prose after drafting or line work
```

## What to learn

Learn only actionable, evidence-backed traits:

- sentence length range and break pattern;
- paragraph breath and mobile reading rhythm;
- concrete object habits;
- body-pressure habits;
- silence and withheld information;
- dialogue roughness and xưng hô behavior;
- emotional restraint;
- how mystery is delayed;
- how scene pressure starts;
- what the author avoids;
- repeated AI-like patterns the author dislikes.

Do not learn private facts, hidden canon, or unverifiable personal claims from style samples.

## Ghostwriter permission

Ghostwriter drafting is allowed only when a bounded scene or passage has:

```text
SOURCE USED
SOURCE STATUS
CONTEXT CAPSULE STATUS when required
SCENE QUESTION
MUST SHOW
MUST NOT REVEAL
READER EFFECT
POV
CHARACTERS PRESENT
AUTHOR VOICE FINGERPRINT USED
DRAFT SCOPE
```

If any required source/control is missing, return a source gap or fingerprint gap instead of drafting.

## Must not do

The Ghostwriter must not:

- invent canon, scene function, character secret, relation, object, payoff, law, institution, or route;
- override current Notion source;
- override character voice with author voice;
- leak hidden canon because it knows the wider plan;
- draft from chat memory as if it were source;
- turn style guide into formulaic repeated phrasing;
- make prose smoother at the cost of body/object pressure;
- call Human Chapter Pass, readiness, or Publication Lock;
- update Notion, GitHub, or source files without explicit write instruction.

## Author voice fingerprint schema

```text
AUTHOR VOICE FINGERPRINT
SCOPE:
SOURCE USED:
AUTHOR SAMPLES USED:
SAMPLE STATUS:
GENRE / MODE:
NARRATION RHYTHM:
PARAGRAPH BREATH:
DIALOGUE HABITS:
XUNG HO / REGISTER:
OBJECT / BODY HABITS:
MYSTERY HANDLING:
EMOTION HANDLING:
TRANSITION HABITS:
SCENE PRESSURE HABITS:
DO:
DO NOT:
VOICE RISKS:
STYLE GUIDE VERDICT:
NEXT NODE:
```

Use concise bullets. Do not create a bloated style bible unless the user asks.

## Author-aligned ghostwriter draft schema

```text
AUTHOR-ALIGNED GHOSTWRITER DRAFT
SCOPE:
SOURCE USED:
SOURCE STATUS:
CONTEXT CAPSULE STATUS:
SCENE QUESTION:
MUST SHOW:
MUST NOT REVEAL:
READER EFFECT:
AUTHOR VOICE FINGERPRINT USED:
POV:
CHARACTERS PRESENT:
DRAFT PERMISSION:
DRAFT:
SELF-CHECK:
VOICE MATCH RISK:
HUMAN SURFACE RISK:
NEXT NODE:
```

## Voice match scoring

Do not report a single decorative percentage. Use a bounded diagnostic matrix:

```text
AUTHOR RHYTHM MATCH:
VIETNAMESE MOUTH-FEEL:
OBJECT / BODY PRESSURE:
SCENE PRESSURE:
DIALOGUE DIFFERENCE:
POV RESTRAINT:
CANON SAFETY:
FALSE SMOOTHING RISK:
VERDICT:
```

A passage can fail even when it sounds author-like if it violates canon, POV, source status, character voice, or scene function.

## Failure labels

```text
AUTHOR_SAMPLE_MISSING
AUTHOR_SAMPLE_UNAPPROVED
CHAT_MEMORY_STYLE_RISK
STYLE_GUIDE_OVERFITTING
AUTHOR_VOICE_OVER_CHARACTER_VOICE
GHOSTWRITER_CANON_DRIFT
GHOSTWRITER_SOURCE_DRIFT
HIDDEN_CANON_LEAK
SCENE_FUNCTION_INVENTED
VOICE_MATCH_FALSE_POSITIVE
FORMULAIC_AUTHOR_STYLE
DRAFT_PERMISSION_BLOCKED
HUMAN_SURFACE_HANDOFF_REQUIRED
```

## Safe repair

Safe repair may:

- request approved author samples;
- extract a compact fingerprint;
- compare a passage against the fingerprint;
- produce a bounded source-safe draft;
- mark style risk separately from canon/source risk;
- hand off to Human Surface Polish after drafting.

Safe repair must not:

- create Notion databases, GitHub workflows, reports, project boards, automations, or live manuscript copies;
- convert sample analysis into permanent canon;
- update style guides in source memory without explicit write permission;
- use detector-bypass framing;
- treat author voice match as readiness.

## Output labels

```text
AUTHOR_VOICE_FINGERPRINT_OK
AUTHOR_VOICE_FINGERPRINT_PARTIAL
AUTHOR_VOICE_FINGERPRINT_BLOCKED
AUTHOR_ALIGNED_DRAFT_READY
AUTHOR_ALIGNED_DRAFT_BLOCKED
GHOSTWRITER_SOURCE_SAFE
GHOSTWRITER_NEEDS_HUMAN_SURFACE_POLISH
READINESS_NOT_AUTHORIZED
```