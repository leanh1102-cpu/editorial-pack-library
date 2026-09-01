# Promotion Rules

Knowledge/corpus lifecycle: `CANDIDATE → VALIDATED → CORE`.
Operational-rule lifecycle: `CANDIDATE GAP → CANDIDATE REPAIR → TARGETED TEST → REGRESSION → STABLE / REJECT / ROLLBACK`.

Do not create a heuristic from one ordinary miss. Require at least two distinct cases with the same causal failure mechanism, unless a Constitution-level hard fail occurs.

Promote only when target failures improve and linked preservation counter-cases do not regress.
Record version, evidence set, benchmark delta, scope/non-scope, and rollback path.
Frequency in a corpus is not proof of quality and must not become taste by default.
