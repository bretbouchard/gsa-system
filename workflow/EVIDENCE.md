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
- runtime telemetry
- logs and traces
- user behavior signals
- incidents and regressions
- observed outcomes

## Two evidence classes

GSA distinguishes implementation evidence from outcome evidence.

### Implementation evidence

Implementation evidence answers:

> Was the requested change implemented correctly?

Examples include builds, unit tests, integration tests, static analysis, deterministic validation, artifact hashes, and domain verification.

### Outcome evidence

Outcome evidence answers:

> Did the change produce the intended effect in reality?

Examples include runtime behavior, user behavior, performance measurements, production incidents, field measurements, simulation-to-reality comparison, support feedback, workflow changes, and other observed consequences.

A successful implementation verification must not be treated as successful outcome validation.

## Evidence requirements

Claims that matter to a decision should identify:

- what was tested or observed
- whether the evidence concerns implementation or outcome
- source or producer
- timestamp/version where relevant
- expected outcome or hypothesis where applicable
- confidence or limitations
- the decision, requirement, Change, or outcome it supports

## Signals and interpretation

Raw observations are evidence, not automatic truth.

A signal may trigger an unknown, investigation, or finding. Interpretation should preserve provenance and uncertainty so later governance can distinguish measurement from inference and inference from decision.

## Staleness

Evidence may become stale when requirements, dependencies, environment, implementation, user behavior, operating conditions, or the intended outcome changes. GSA can mark dependent decisions as needing re-verification or re-observation rather than silently treating old evidence as current.
