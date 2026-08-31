# Vietnamese Literary Craft Corpus Index

## Status model

Public corpus uses three states only:

- `CANDIDATE` — mechanism extracted and sanitized; not yet validated for general use.
- `VALIDATED` — passed targeted blind validation and relevant regressions.
- `CORE` — repeatedly validated across distinct source spans / holdouts and safe for broad routing.

Promotion is evidence-based and rollbackable. Frequency is not quality.

## Privacy and source boundary

This repository is public. Corpus files MUST NOT contain:

- private manuscript bodies or long verbatim excerpts;
- project canon, character names, private URLs, workspace IDs, or hidden source metadata;
- unreviewed AI output represented as author-approved evidence.

Private provenance remains in authorized Notion/Drive staging. Public entries retain only a coarse `SOURCE_CLASS`, observable mechanism, anonymized case, transfer risk, and validation status.

## Current corpus nodes

### Candidate

- `candidate/author-taste-vietnamese-prose-v0.1.md` — human-approved Vietnamese prose mechanisms + production-observed failure boundaries, sanitized for cross-project use.

### Validated

None yet for this corpus family.

### Core

None yet for this corpus family.

## Promotion contract

`CANDIDATE → VALIDATED` requires:

1. frozen blind runner + evaluator;
2. targeted suite pass with hard fail 0, or a documented narrow closure that does not broaden the rule;
3. no private-source leakage or surface imitation;
4. relevant blast-radius regressions clean/composite-closed.

`VALIDATED → CORE` additionally requires:

1. separate holdout source span not used to author the mechanism;
2. transfer pass without surface imitation;
3. repeated production evidence or multiple independent source classes;
4. no unresolved material regression.

TRAIN/REFERENCE material is never by itself evidence of generalization.
