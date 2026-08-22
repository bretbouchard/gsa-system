# Modeled World

The Modeled World is GSA's authoritative representation of the system and project state.

A language model never owns this state. Instead, the system projects only the relevant slice of the Modeled World into a model session.

## Responsibilities

The Modeled World may hold:

- entities and relationships
- requirements and constraints
- current project state
- decisions and rationale
- plans and dependencies
- permissions and capabilities
- evidence and verification state
- unresolved unknowns
- external resource references
- outcomes and historical context

## Projection

Models receive controlled projections rather than unrestricted access to every fact. Projections should be purpose-specific, bounded, and reconstructible from authoritative state.

## Mutation

State mutation occurs through explicit operations. Proposed mutations may require validation, policy checks, evidence, or approval before commitment.

## Recovery

Because authoritative state exists outside the model context, a failed or replaced model session does not erase the system's understanding of the project.
