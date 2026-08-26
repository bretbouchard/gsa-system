# Reality Feedback Loop

GSA does not treat successful execution as proof that a change was the right change.

A governed system must compare intended outcomes with observed reality and feed those consequences back into the Modeled World.

## Core lifecycle

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

This loop is continuous. Runtime behavior, user behavior, measurements, failures, regressions, tests, simulations, external changes, and human feedback may all become evidence.

## Two completion dimensions

Implementation state and outcome state are intentionally separate.

### Implementation state

```text
Not Started → Executing → Implemented → Verified
```

`Verified` means the requested change was implemented correctly and its verification obligations passed.

### Outcome state

```text
Not Observed → Observing → Outcome Validated | Outcome Failed | Inconclusive
```

`Outcome Validated` means evidence supports that the change produced its intended real-world effect.

A change may therefore be:

- correctly implemented but outcome failed;
- correctly implemented but still awaiting observation;
- technically imperfect yet directionally successful;
- inconclusive because available evidence is insufficient.

## Signal is not truth

Observations are evidence, not automatic requirements.

A crash, repeated workflow, usage pattern, failed measurement, complaint, benchmark movement, or anomalous trace may trigger investigation. It must not silently become a ticket, requirement, policy, or autonomous change.

Elenchus may frame the unknown. Council may investigate where specialist judgment matters. Historian provides prior decisions and consequences. GSD turns an accepted finding into governed work. Obdurate decides what may proceed autonomously and what requires human authority.

## Risk-based autonomy

Autonomy is determined by consequence, confidence, reversibility, evidence quality, and policy—not by whether AI generated the change.

Low-risk, reversible, strongly verifiable changes may proceed with little or no human review. Architectural, security, privacy, destructive, externally visible, expensive, or product-intent changes require stronger governance and may require explicit human approval.

## Modeled World integration

The Modeled World should preserve links among:

- original intent;
- expected outcome;
- requirements and constraints;
- implementation Change;
- verification evidence;
- observed outcome evidence;
- resulting findings;
- follow-up Changes;
- reversals, supersession, or learned constraints.

The system must be able to answer both:

> Was this change implemented correctly?

and:

> Did this change actually work?

Those are different questions and must never collapse into one status.
