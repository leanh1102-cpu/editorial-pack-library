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

## Use when

- the user asks to audit many chapters at once;
- the user asks line-level work over a packet or arc;
- the user asks rewrite or patch without exact excerpt;
- the source is summary, digest, old chat memory, or legacy Workdeck;
- the AI is at risk of compressing prose into plot summary;
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
- scene rhythm is judged from summary.

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
```

## Output labels

```text
SOURCE_SURFACE_OK
SOURCE_SURFACE_PARTIAL
SOURCE_SURFACE_MISSING
COMPRESSION_RISK_HIGH
COMPRESSION_BLOCKED
SAFE_DOWNGRADE_REQUIRED
```
