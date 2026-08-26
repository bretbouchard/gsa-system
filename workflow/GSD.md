# GSD — Get Shit Done

GSD is the execution-planning layer of GSA. It turns intent or accepted evidence-backed findings into a visible work graph with dependencies, verification criteria, expected outcomes, and state transitions.

## GSD is not a prompt

A plan should persist independently of the model that authored it. Work items can be resumed, reassigned, blocked, invalidated, or re-planned as evidence changes.

## Work entry paths

GSD may receive work from deliberate human intent or from the Reality Feedback Loop.

Evidence-originated work follows:

```text
Signal
  ↓
Investigation
  ↓
Finding
  ↓
Decision
  ↓
Governed GSD work
```

A raw observation must not automatically become a ticket, requirement, or Change. Elenchus, Council, Historian, or another governed process first establishes what the signal means and whether action is warranted.

## Work item shape

A useful work item includes:

- goal
- expected outcome
- inputs
- dependencies
- required capabilities
- acceptance criteria
- implementation evidence requirements
- outcome observation requirements where applicable
- risk/autonomy classification
- status
- blockers
- outputs

## Implementation state

```text
Not Started → Executing → Implemented → Verified
```

`Verified` means the requested implementation passed its defined verification obligations.

## Outcome state

Where a work item asserts a real-world effect, track outcome separately:

```text
Not Observed → Observing → Outcome Validated | Outcome Failed | Inconclusive
```

GSD must never equate `Verified` with `Outcome Validated`.

Outcome failure or inconclusive evidence may create new unknowns, investigations, or replanning without erasing the fact that the original implementation was correctly executed.

## Flow

```text
Intent or accepted finding
  ↓
Decompose
  ↓
Identify dependencies
  ↓
Expose unknowns
  ↓
Define verification + expected outcome
  ↓
Sequence work
  ↓
Govern
  ↓
Execute bounded operations
  ↓
Verify implementation
  ↓
Commit verified state
  ↓
Observe outcome where applicable
  ↓
Validate outcome / fail / remain inconclusive
  ↓
Commit learning / re-plan
```

## Why this matters

Long-running agentic work fails when planning exists only inside a model transcript or when passing tests are treated as proof that the change was worthwhile. GSD makes the remaining work inspectable, lets new evidence change the plan without losing project continuity, and preserves the distinction between implementation correctness and outcome success.
