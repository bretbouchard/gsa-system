# Execution Flow

GSA turns intent into governed, evidence-producing work rather than a single opaque agent loop.

## Normal flow

1. Capture intent, expected outcome, and current authoritative state.
2. Run unknown discovery to surface assumptions and missing information.
3. Engage specialist review where domain judgment matters.
4. Build a dependency-aware GSD work graph.
5. Apply Obdurate policy and approval checks before governed actions.
6. Execute work through explicit tools.
7. Run deterministic or domain-specific verification where possible.
8. Store implementation evidence.
9. Commit verified implementation state.
10. Observe runtime, user, measurement, simulation, or external consequences where applicable.
11. Store outcome evidence and classify the result as validated, failed, or inconclusive.
12. Update authoritative state and preserve the decision, evidence, and consequences in the Historian.
13. Re-plan when outcome evidence reveals a new unknown, regression, failed hypothesis, or changed requirement.

## Reality Feedback Loop

Execution is one segment of a larger lifecycle:

```text
Observe
  ↓
Evidence
  ↓
Interpret
  ↓
Investigate
  ↓
Decide
  ↓
Plan
  ↓
Govern
  ↓
Execute
  ↓
Verify
  ↓
Observe
```

The loop may begin from deliberate human intent or from evidence that something in reality deserves investigation.

A signal never automatically becomes a requirement or ticket. It enters governed investigation first.

## Completion

Successful execution and successful outcome are different claims.

A Change can be `Verified` when its implementation and verification obligations pass while its outcome remains `Not Observed` or `Observing`.

Only later evidence can establish `Outcome Validated`, `Outcome Failed`, or `Inconclusive`.

## Failure flow

A failed tool call, failed verification, rejected approval, newly discovered unknown, failed outcome, regression, or contradictory observation does not disappear into conversational context. It becomes explicit state that can change the plan.

## Long-running work

Because state, decisions, evidence, expected outcomes, and observed consequences persist independently of the active model session, work may pause, resume, change models, or branch without relying on one conversation transcript as the system of record.
