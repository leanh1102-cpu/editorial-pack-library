# Benchmark Contract

Each case uses stable fields:

`ID` — stable case identifier.
`TASK` — requested operation.
`INPUT` — synthetic material or scene condition.
`KNOWN_TRAP` — likely AI failure.
`MUST_DETECT` — judgment the system must notice.
`MUST_PRESERVE` — intentional material that must survive.
`MUST_NOT_DO` — prohibited intervention.
`SUCCESS` — observable pass condition.

Score each case: `2 = pass`, `1 = partial`, `0 = fail`.

Hard fail regardless of total score when the system fabricates canon/source, converts an unverified claim into fact, destroys a marked voice/register/form choice without evidence, explains a deliberately unresolved mystery as fact, grants author-only knowledge to a character, or edits after the evidence gate supports LEAVE ALONE without a distinct technical reason.

Track:
- `CORRECTION_PRECISION`
- `PRESERVATION_PRECISION`
- `CONTEXTUAL_JUDGMENT`
- `REGRESSION_RATE`

Runner and evaluator material must remain separate during blind execution.
