# SLTD Webnovel Paragraphing & Layout Rhythm Gate

This gate controls paragraphing, line breaks, mobile readability, and visible layout rhythm.

## Core rule

Paragraph is reader breath, not decoration.

Line break is a structural signal, not artificial emphasis.

```text
PARAGRAPH = reader-breath unit
LINE BREAK = speaker, action, focus, turn, interruption, aftershock, location, time, or scene-beat shift
LAYOUT RHYTHM = paragraph length variation matching scene pressure and mobile readability
```

## Use when

- prose uses many one-sentence paragraphs;
- short lines appear in dense sequence;
- every sentence gets its own line;
- line breaks create artificial punch or suspense;
- dialogue beats are over-fragmented;
- action is split into too many isolated lines;
- a chapter has uniform breath rhythm;
- mobile reading feels choppy or tiring;
- paragraphs are too dense for webnovel reading.

## Paragraph length guidance

```text
1 sentence: sparing use for turn, hook, silence, aftershock, interruption, or earned emphasis
2-4 sentences: default safe zone for webnovel prose
5-7 sentences: allowed for slow pressure, immersion, description, memory, or reflection with internal movement
8+ sentences: mobile fatigue risk unless voice or immersion needs density
```

Three or more consecutive one-sentence paragraphs are a red flag unless rapid dialogue or action requires them.

## Line break purpose test

Each line break should serve at least one purpose:

```text
speaker change
main action change
focus shift
turn / reveal / interruption
real silence / aftershock
mobile breath pause
time / location / scene beat shift
```

## Failure labels

```text
RANDOM_LINE_BREAKS
SHORT_LINE_OVERUSE
ONE_SENTENCE_PARAGRAPH_ABUSE
FAKE_EMPHASIS_BY_LINEBREAK
UNIFORM_BREATH_RHYTHM
DIALOGUE_OVER_FRAGMENTED
ACTION_OVER_FRAGMENTED
AFTERSHOCK_LINE_OVERUSE
WALL_OF_TEXT_RISK
MOBILE_READING_FATIGUE
AI_LAYOUT_SIGNATURE
PARAGRAPH_DENSITY_FLAT
```

## Safe repair

Safe repair may merge isolated sentences that share one breath, split dense paragraphs at real focus or action shifts, keep dialogue and small action tags together when they are one spoken breath, preserve one-line aftershock only when earned, and vary paragraph length to match pressure.

Safe repair must not change plot or canon, make all paragraphs the same length, remove all white space, create new punchlines, or use layout to hide weak prose.

## Layout audit

```text
WEBNOVEL PARAGRAPHING & LAYOUT CHECK
SCOPE:
SOURCE USED:
SOURCE SURFACE:
SCENE / CHAPTER TYPE:
PARAGRAPH LENGTH MAP:
SHORT-LINE DENSITY:
LINE BREAK PURPOSE:
DIALOGUE LAYOUT:
ACTION PARAGRAPH FLOW:
AFTERSHOCK LINE USE:
MOBILE FATIGUE RISK:
AI-LAYOUT RISK:
FAILURE LABELS:
REPAIR PRINCIPLE:
ROLE HANDOFF:
NEXT NODE:
```

## Patch rule

```text
OLD:
LAYOUT FAILURE:
WHY IT HURTS READER BREATH:
NEW:
WHAT WAS MERGED:
WHAT WAS SPLIT:
RISK:
```

If exact source text is missing, run Source Surface Check before patching.

## Handoff

If layout exposes weak prose, hand off to Scene-First Prose Judgment or First-Pass Editorial Workflow.

If short-line rhythm flattens cadence, hand off to Dynamic Range Check.

If register is the real issue, hand off to Vietnamese Register Check.

If chapter surface flow is overloaded, hand off to Chapter Assembly & Split Check.

## Output labels

```text
LAYOUT_RHYTHM_OK
LAYOUT_RHYTHM_PARTIAL
AI_LAYOUT_SIGNATURE_DETECTED
SHORT_LINE_OVERUSE_DETECTED
WALL_OF_TEXT_RISK_DETECTED
REFORMAT_REQUIRED
SOURCE_SURFACE_REQUIRED
```