# Model Boundary

GSA treats models as replaceable reasoning processors, not privileged system components.

## What a model may do

A model may:

- inspect an authorized projection of state
- reason about goals and constraints
- identify unknowns
- request specialist investigation
- propose plans
- call explicit tools
- suggest state mutations
- explain evidence and tradeoffs

## What a model does not own

A model does not own:

- authoritative persistent state
- permissions
- approval policy
- evidence validity
- external side effects
- user identity or credentials
- irreversible decisions

## Tool boundary

```text
Model
  |
  | structured request
  v
Tool Contract
  |
  v
Authorization / Policy
  |
  v
Bounded Operation
  |
  v
Verification / Evidence
  |
  v
State Mutation or Result
```

Tool contracts are explicit and inspectable. Arbitrary execution is not the default capability model.

## Model independence

The architecture is designed so that local models, hosted frontier models, and specialized domain models can be substituted without transferring ownership of state or policy to the provider.
