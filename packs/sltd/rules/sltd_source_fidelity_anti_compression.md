# SLTD Source Fidelity & Anti-Compression Gate

This rule prevents the AI from editing or judging prose from compressed memory, summary, digest, or inferred source.

It protects the exact surface of Vietnamese fiction: sentence order, rhythm, dialogue breaks, object placement, and small bodily or sensory beats.

## Core rule

```text
SOURCE TEXT > DERIVED DIGEST > CHAT MEMORY
```

Exact source text is required for line edit, line surgery, copyedit, proofread, and exact OLD/NEW patch.

A digest can guide navigation, prioritization, or map-level audit. It cannot be treated as source text.

Chat memory can provide context. It cannot be used as current source evidence or prose surface.

## A-source survival rawness guard

When A-source material is used as benchmark / draft-material reference, do not compress away its raw survival pressure.

A-source is not automatically live canon, but its rough life-force can be a protected source signal. Editorial prose must not become prettier, cleaner, more symbolic, or more lore-labeled by removing the survival impulse that caused the action.

```text
SURVIVAL IMPULSE > LORE LABEL
RAW LIFE COST > BEAUTIFUL SURFACE
ACTION FROM NEED > ACTION FROM THEME
OBJECT / BODY / HUNGER / DEBT / FEAR > ABSTRACT EXPLANATION
```

For SLTD, the visible urge should usually come from survival first:

- hunger;
- medicine shortage;
- breath failure;
- cold / fog / rain / mud;
- debt pressure;
- family body-cost;
- someone watching or misnaming;
- food, water, fire, tool, road, paper, animal, or witness pressure;
- the need to hide, carry, trade, refuse, ask, or delay.

The underlying lore law may shape the world, but scene action should not look like characters moving to illustrate lore. A scene fails if every beat is correct in outline but the human body has no immediate reason to move.

## Editorial smoothing failure

Flag an editorial draft when it:

```text
A_SOURCE_RAWNESS_COMPRESSED
SURVIVAL_IMPULSE_LOST
ROUGH_LIFE_COST_REMOVED
LORE_LAW_OVER_SURVIVAL_ACTION
SYMBOLIC_POLISH_OVER_BODY_NEED
PRETTY_SCENE_FALSE_GAIN
ACTION_FROM_THEME_NOT_NEED
A_SOURCE_BEAT_BEAUTIFIED_AWAY
```

This failure is especially dangerous in chapters where the source contains poverty, hunger, illness, rough trade, dirty medicine, animal signs, mud, torn tools, unpaid debt, family embarrassment, small theft/temptation, or a physically ugly survival choice.

## A-source-to-editorial check

Before accepting an editorial rewrite derived from A-source or old draft material, check:

```text
A-SOURCE SURVIVAL CHECK
SOURCE USED:
EDITORIAL VERSION USED:
RAW SURVIVAL DRIVER IN A-SOURCE:
WHAT BODY / OBJECT / DEBT / HUNGER / FEAR MOVES THE ACTION:
WHAT THE EDITORIAL VERSION REMOVED:
WHAT WAS BEAUTIFIED OR SYMBOLIZED:
LORE LAW PRESENT: YES / NO
LORE LAW OVERWRITES SURVIVAL: YES / NO
SCENE ACTION STILL STARTS FROM NEED: YES / NO
SAFE REPAIR:
```

Safe repair should restore pressure through concrete need before adding lore clarity.

Do not solve the problem by adding explanation. Restore the missing object, body cost, hunger, debt, family risk, witness risk, route pressure, or dirty practical choice.

## Use when

- the user asks to audit many chapters at once;
- the user asks line-level work over a packet or arc;
- the user asks rewrite or patch without exact excerpt;
- the source is summary, digest, old chat memory, or legacy Workdeck;
- the AI is at risk of compressing prose into plot summary;
- the editorial version may have smoothed, prettified, or symbolized rough A-source survival pressure;
- context window limits may affect source fidelity.

## Task level rule

```text
map-level review = may use digest, cannot patch prose
packet review = may use digest plus sampled exact source, cannot line edit whole packet
chapter readiness = requires current chapter source and status evidence
scene rewrite = requires source scene or current scene packet
line surgery = requires exact excerpt, best 300-1500 words
copyedit/proofread = requires exact current text
publication readiness = requires current Notion evidence
```

## Source surface types

```text
EXACT_SOURCE_TEXT
CURRENT_NOTION_SOURCE
USER_PROVIDED_EXCERPT
DERIVED_DIGEST_NOT_SOURCE
LEGACY_REFERENCE_NOT_CURRENT
CHAT_MEMORY_NOT_SOURCE
MISSING_SOURCE_SURFACE
```

## Allowed actions by source type

### EXACT_SOURCE_TEXT / USER_PROVIDED_EXCERPT

Allowed:

- line surgery;
- OLD/NEW patch;
- prose rhythm check;
- dialogue voice check;
- copyedit/proofread if scope fits;
- source-surface-based audit.

### CURRENT_NOTION_SOURCE

Allowed:

- current-state verdict;
- readiness check;
- canon/status check;
- scene/chapter audit;
- exact patch only if exact text is opened and quoted.

### DERIVED_DIGEST_NOT_SOURCE

Allowed:

- navigation;
- context brief;
- packet map;
- risk prioritization;
- choose next exact source to open.

Forbidden:

- line edit;
- line surgery;
- OLD/NEW patch;
- proofread;
- prose naturalness verdict;
- current status claim.

### LEGACY_REFERENCE_NOT_CURRENT

Allowed:

- history comparison when named;
- DIFFMODE if paired with named current source;
- background context.

Forbidden:

- current status claim;
- current readiness claim;
- direct manuscript patch unless user names it as current source.

### CHAT_MEMORY_NOT_SOURCE

Allowed:

- orientation;
- safe narrow claim;
- source request.

Forbidden:

- current status verdict;
- canon verdict;
- exact prose patch;
- readiness verdict.

## Compression risk levels

```text
LOW = exact source in context and scope is small
MEDIUM = exact source partly available, digest used for navigation
HIGH = packet/arc scope, only summary/digest/memory available, or line-level task over large scope
BLOCKING = no exact source for requested line/rewrite/readiness task
```

## Source surface check

Before editing prose, return or internally confirm:

```text
SOURCE SURFACE CHECK
REQUEST:
SCOPE:
TASK LEVEL: map / packet / chapter / scene / excerpt / line
SOURCE TYPE:
SURFACE AVAILABLE: YES / NO
COMPRESSION RISK: LOW / MEDIUM / HIGH / BLOCKING
ALLOWED ACTION:
FORBIDDEN ACTION:
NEXT NODE:
```

## Exact patch rule

For every patch:

```text
OLD:
[exact source text]
PROBLEM:
[label]
NEW:
[patch]
VERIFY:
old text found: YES / NO
meaning preserved: YES / NO
canon risk: NONE / POSSIBLE / BLOCKING
surface risk: LOW / MEDIUM / HIGH
```

If `old text found` is NO, stop. Do not approximate.

## Digest rule

Every digest must be labeled:

```text
DERIVED DIGEST — NOT SOURCE TEXT
```

A digest may answer:

- what to open next;
- which chapter may be risky;
- which role should run;
- what open loops exist;
- what packet-level blocker may exist.

A digest must not answer:

- what exact prose says;
- whether a sentence reads naturally;
- whether a line edit is correct;
- whether current status is locked;
- whether canon conflict is resolved.

## Safe downgrade

If request scope exceeds source surface, downgrade safely:

```text
SOURCE SURFACE MISSING
SAFE TASK:
- map-level review only
- packet risk scan only
- choose chapter priority
- request exact scene/excerpt
NEEDED SOURCE:
NEXT NODE:
```

## Anti-compression warnings

Flag high risk when:

- the answer summarizes instead of citing/opening exact source;
- line edit is requested over many chapters;
- rewrite is requested from digest;
- patch is proposed without exact OLD;
- readiness is inferred from prose quality;
- current status is inferred from chat memory;
- scene rhythm is judged from summary;
- A-source survival material is replaced by cleaner symbolic editorial prose;
- scene action is explained by lore law before body/object survival need exists;
- rough living details are removed because they look dirty, repetitive, ordinary, or not elegant enough.

## Stop rule

Stop when:

```text
SOURCE_SURFACE_MISSING
EXACT_OLD_NOT_FOUND
DIGEST_USED_AS_SOURCE
MEMORY_USED_AS_CURRENT_STATUS
LINE_TASK_OVER_PACKET_SCOPE
REWRITE_WITHOUT_SCENE_SOURCE
READINESS_WITHOUT_CURRENT_NOTION
A_SOURCE_RAWNESS_COMPRESSED
SURVIVAL_IMPULSE_LOST
LORE_LAW_OVER_SURVIVAL_ACTION
```

## Output labels

```text
SOURCE_SURFACE_OK
SOURCE_SURFACE_PARTIAL
SOURCE_SURFACE_MISSING
COMPRESSION_RISK_HIGH
COMPRESSION_BLOCKED
SAFE_DOWNGRADE_REQUIRED
A_SOURCE_SURVIVAL_RESTORE_REQUIRED
EDITORIAL_SMOOTHING_BLOCKED
```
