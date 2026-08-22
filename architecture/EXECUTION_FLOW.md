# Execution Flow

GSA turns intent into governed, evidence-producing work rather than a single opaque agent loop.

## Normal flow

1. Capture intent and current authoritative state.
2. Run unknown discovery to surface assumptions and missing information.
3. Engage specialist review where domain judgment matters.
4. Build a dependency-aware GSD work graph.
5. Execute work through explicit tools.
6. Apply Obdurate policy and approval checks before governed actions.
7. Run deterministic or domain-specific verification where possible.
8. Store evidence and outcomes.
9. Update authoritative state.
10. Preserve the decision and result in the Historian.

## Failure flow

A failed tool call, failed verification, rejected approval, or newly discovered unknown does not disappear into conversational context. It becomes explicit state that can change the plan.

## Long-running work

Because state, decisions, and evidence persist independently of the active model session, work may pause, resume, change models, or branch without relying on one conversation transcript as the system of record.
