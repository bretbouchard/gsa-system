# Evidence

GSA treats evidence as durable state rather than prose embedded in a model response.

## Evidence can include

- deterministic test results
- measurements
- simulation output
- external source facts
- tool execution records
- approvals
- artifact hashes
- human review
- observed outcomes

## Evidence requirements

Claims that matter to a decision should identify:

- what was tested or observed
- source or producer
- timestamp/version where relevant
- confidence or limitations
- the decision or requirement it supports

## Staleness

Evidence may become stale when requirements, dependencies, environment, or implementation change. GSA can mark dependent decisions as needing re-verification rather than silently treating old evidence as current.
