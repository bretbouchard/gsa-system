# GSA — Governed Stewardship Architecture

**A public architecture for agentic systems that can reason, investigate, and act without allowing a language model to become the authority over state, permissions, evidence, or reality.**

GSA is the general architecture behind domain systems such as White Room and Volta. It is designed for long-running, tool-using AI systems where models may change, fail, disagree, or hallucinate while the surrounding system must remain trustworthy.

## Core rule

**Models are interchangeable processors. The system owns reality.**

A model receives a controlled projection of authoritative state. It may investigate, plan, call explicit tools, and propose changes. It does not own persistent truth, permissions, policy, evidence, or side effects.

```text
                         MODEL(S)
                            |
                    controlled projection
                            |
                            v
                   +-----------------+
                   |  Modeled World  |
                   | authoritative   |
                   | state           |
                   +--------+--------+
                            |
          +-----------------+------------------+
          |                 |                  |
          v                 v                  v
      Elenchus           Council          Historian
      unknowns          expertise          memory
          |                 |                  |
          +-----------------+------------------+
                            v
                           GSD
                     sequences work
                            |
                            v
                        Obdurate
                    governs actions
                            |
                            v
                          Tools
                            |
                            v
                         REALITY
```

## System roles

- **Modeled World** — authoritative structured state that models can inspect but do not own.
- **GSD** — sequences work into explicit, dependency-aware, verifiable steps.
- **Elenchus** — hunts unknowns, assumptions, missing evidence, and unresolved risk.
- **Council** — domain professionals investigate decisions from distinct professional viewpoints and return evidence-backed findings.
- **Historian** — preserves epistemic state, decisions, precedent, outcomes, and the evidence behind them.
- **Obdurate** — governs what may actually happen, including permissions, approvals, irreversible actions, and external side effects.
- **Tools** — explicit capabilities through which models read state, perform bounded operations, verify claims, and request changes.

## Why this architecture exists

Traditional agent loops often collapse reasoning, memory, permissions, execution, and truth into one conversational context. That works for demos but becomes fragile as systems gain tools, persistence, multiple models, long-running projects, and real-world consequences.

GSA separates those concerns so that:

1. a model can be replaced without replacing the system,
2. evidence can outlive the model session that produced it,
3. side effects remain governed even when a model is confident,
4. unknowns become explicit work rather than silent assumptions,
5. multiple professional viewpoints can challenge a proposed decision,
6. state remains inspectable and recoverable after failures,
7. deterministic verification can override model confidence.

## Execution pattern

```text
Intent
  |
  v
Authoritative State
  |
  +--> Unknown discovery
  |
  +--> Specialist investigation
  |
  v
Plan / work graph
  |
  v
Tool contract
  |
  v
Policy / approval
  |
  v
Domain operation
  |
  v
Verification + evidence
  |
  v
Authoritative state update
```

## Public applications

- [White Room System](https://github.com/bretbouchard/white-room-system) — governed AI applied to a real-time creative/music system.
- [Volta System](https://github.com/bretbouchard/volta-system) — governed AI applied to electronics design, validation, and manufacturing.

These repositories show how the same architecture changes shape in very different domains while preserving the same state, evidence, tooling, and governance principles.

## What this repository contains

This is a public architectural repository. It documents concepts, contracts, workflows, and examples without exposing private implementation code, prompts, project state, credentials, or user-specific data.

Start with:

- [Architecture Overview](architecture/OVERVIEW.md)
- [Modeled World](architecture/MODELED_WORLD.md)
- [Model Boundary](architecture/MODEL_BOUNDARY.md)
- [Execution Flow](architecture/EXECUTION_FLOW.md)
- [GSD](workflow/GSD.md)
- [Evidence](workflow/EVIDENCE.md)
- [Decision Lifecycle](workflow/DECISION_LIFECYCLE.md)
- [Elenchus](intelligence/ELENCHUS.md)
- [Council](intelligence/COUNCIL.md)
- [Historian](intelligence/HISTORIAN.md)
- [Obdurate](governance/OBDURATE.md)

## Status

GSA is under active development. The production implementation and application-specific state remain private; this repository is the public systems architecture and portfolio surface.
