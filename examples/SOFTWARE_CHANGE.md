# Example — Governed Software Change

This simplified example shows the GSA pattern without depending on a specific implementation.

## Intent

> Add a capability to an existing application without regressing its current behavior.

## Flow

1. The Modeled World provides current requirements, architecture, repository state, and known constraints.
2. Elenchus identifies missing acceptance criteria and compatibility assumptions.
3. GSD creates implementation, test, and verification work items.
4. A model receives only the state needed for the assigned work and proposes changes through bounded tools.
5. Tests and static checks produce evidence.
6. A failed check blocks completion and becomes explicit work.
7. Obdurate controls merge, release, or other externally consequential actions.
8. The Historian records the decision, evidence, and outcome.

The key property is that a successful-looking model response never substitutes for the actual verification result.
