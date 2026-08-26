# Modeled World

The Modeled World is GSA's authoritative representation of the system and project state.

A language model never owns this state. Instead, the system projects only the relevant slice of the Modeled World into a model session.

## Responsibilities

The Modeled World may hold:

- entities and relationships
- intent, requirements, constraints, and preferences
- current project state
- decisions and rationale
- plans and dependencies
- permissions and capabilities
- implementation and verification state
- expected outcomes
- observed outcome evidence
- unresolved unknowns
- external resource references
- historical context and consequences

## Reality Feedback Loop

The Modeled World is not only an input to execution. It is updated by evidence from what actually happens afterward.

```text
Observe → Evidence → Interpret → Investigate → Decide → Plan → Govern → Execute → Verify → Observe
```

Observations may come from tests, runtime telemetry, logs, traces, measurements, simulations, user behavior, human feedback, incidents, regressions, or external state.

An observation is evidence, not truth. It does not silently become a requirement, policy, or work item. It may instead create an unknown or finding that Elenchus, Council, Historian, GSD, and Obdurate process through normal governance.

## Completion semantics

The Modeled World must preserve implementation state separately from outcome state.

Implementation may be `Not Started`, `Executing`, `Implemented`, or `Verified`.

Outcome may be `Not Observed`, `Observing`, `Outcome Validated`, `Outcome Failed`, or `Inconclusive`.

`Verified` means the requested change was implemented correctly and its verification obligations passed. It does not mean the change produced the intended real-world effect.

The world model should preserve links from intent and expected outcome through implementation and verification evidence to later observations, consequences, follow-up work, reversals, and learned constraints.

## Projection

Models receive controlled projections rather than unrestricted access to every fact. Projections should be purpose-specific, bounded, and reconstructible from authoritative state.

## Mutation

State mutation occurs through explicit operations. Proposed mutations may require validation, policy checks, evidence, or approval before commitment.

Observed signals may update evidence or create investigation state, but must not bypass governance to mutate requirements, architecture, policy, or product intent.

## Recovery

Because authoritative state exists outside the model context, a failed or replaced model session does not erase the system's understanding of the project.
