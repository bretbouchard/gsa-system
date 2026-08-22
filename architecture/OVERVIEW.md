# Architecture Overview

GSA separates five concerns that are often collapsed into one agent loop: state, reasoning, workflow, governance, and evidence.

## Layers

1. **Modeled World** — authoritative structured state.
2. **Intelligence** — models and specialist processes that reason over controlled projections of state.
3. **Workflow** — GSD turns intent into dependency-aware, verifiable work.
4. **Governance** — Obdurate evaluates whether proposed actions may occur.
5. **Evidence** — verification results, decisions, outcomes, and provenance that persist beyond any model session.

## Architectural invariant

No model response becomes authoritative merely because it was generated. State changes require an explicit operation and, where appropriate, verification, policy checks, and approval.

## Why this matters

This lets the system tolerate model swaps, model failures, disagreement, retries, and partial execution without losing the underlying project state or weakening safety boundaries.
