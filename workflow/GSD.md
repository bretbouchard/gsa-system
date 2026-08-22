# GSD — Get Shit Done

GSD is the execution-planning layer of GSA. It turns intent into a visible work graph with dependencies, verification criteria, and state transitions.

## GSD is not a prompt

A plan should persist independently of the model that authored it. Work items can be resumed, reassigned, blocked, invalidated, or re-planned as evidence changes.

## Work item shape

A useful work item includes:

- goal
- inputs
- dependencies
- required capabilities
- acceptance criteria
- evidence requirements
- status
- blockers
- outputs

## Flow

```text
Intent
  ↓
Decompose
  ↓
Identify dependencies
  ↓
Expose unknowns
  ↓
Sequence work
  ↓
Execute bounded operations
  ↓
Verify
  ↓
Commit outcome / re-plan
```

## Why this matters

Long-running agentic work fails when planning exists only inside a model transcript. GSD makes the remaining work inspectable and lets new evidence change the plan without losing project continuity.
