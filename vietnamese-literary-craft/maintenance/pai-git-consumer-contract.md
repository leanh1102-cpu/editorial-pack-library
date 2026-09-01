# PAI Git Consumer Contract — VLC Narrative Dynamics + Author-Taste v0.1

**Status:** `DOWNSTREAM CONSUMER CONTRACT / RUNTIME-VALIDATED SOURCE PACKAGE`

## Purpose
This file defines how a downstream PAI consumer may pin and load the validated Vietnamese Literary Craft runtime package. It does not modify, configure, or certify any PAI repository by itself.

## Source repository
- Repository: `leanh1102-cpu/editorial-pack-library`
- Runtime ref: `install/vietnamese-literary-craft-narrative-dynamics-author-taste-v0.1-runtime`
- Exact validated runtime commit: `40608c73103dab76d83b7fc3b34b4b1dea293f84`
- Package status: `RUNTIME-VALIDATED / COMPOSITE PASS / HARD FAIL 0`
- Skill entry root: `SKILL.md`

## Package boundary
The runtime ref is package-only. A consumer must load the branch root as the VLC skill root.

Required runtime content includes the packaged `SKILL.md`, `CONSTITUTION.md`, `analysis/`, `craft/`, `curriculum/`, `drills/`, `evaluation/`, `glossary/`, `maintenance/`, `register/`, `runtime/`, and `theory/` trees present at the pinned commit.

The consumer must **not** expect or import `harness/`, evaluator/golden material, or candidate corpus material from this runtime ref. Validation artifacts remain outside the installed skill package.

## Validation receipt
The pinned runtime snapshot was validated with:
- Narrative Dynamics / Author-Taste focused runtime gate: `RV-01..RV-08 = 16/16 / HARD FAIL 0`;
- runtime install smoke: `RS-01..RS-04 = 8/8 / HARD FAIL 0`;
- previously frozen Author-Taste holdout and blast-radius composite evidence with current hard fail 0.

This receipt applies only to the exact runtime package identified above. It is not a general certification of arbitrary later commits or of a downstream PAI integration.

## Downstream integration contract
A PAI consumer must:
1. pin the exact runtime commit above rather than floating on an unverified branch head;
2. treat `SKILL.md` as the package entry point and preserve its progressive-loading routes;
3. keep VLC evaluation/golden harnesses outside the runtime prompt/package;
4. preserve the runtime evidence/source boundaries, including `HOLD-INSUFFICIENT_EVIDENCE`, sentence-local `MIN_EDIT`, sensory no-invention, and source-grounded chapter/arc intervention;
5. run its own downstream C0–C4 checks, UAT, and integration receipt before claiming PAI-side production readiness;
6. record the exact VLC commit used in the downstream receipt.

## Rollback
Validated rollback ref:
- `install/vietnamese-literary-craft-dialogue-texture-v0.1-runtime`
- known runtime snapshot commit: `b4a64b0845e7006837cea864fb9bbac5c0f68f06`

Rollback is a consumer operation. This repository does not automatically alter any downstream installation.

## Non-coupling rule
VLC remains the source package and rule memory. PAI remains a downstream Git consumer. Do not merge repositories, mirror PAI control-plane files into VLC, or treat this contract as permission for autonomous cross-repository writes.

## Revalidation trigger
A new VLC runtime pin requires downstream revalidation when behavior-bearing package content changes. A new source commit, branch movement, or metadata-only change does not inherit this runtime receipt automatically unless the runtime package is demonstrated byte/behavior equivalent or is revalidated.
