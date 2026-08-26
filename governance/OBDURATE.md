# Obdurate

Obdurate is GSA's governance boundary: the component that decides whether a proposed action may actually happen.

Reasoning and permission are intentionally separate. A model may be correct about what it wants to do and still lack authority to do it.

## Responsibilities

Obdurate can evaluate:

- actor and capability
- target resource
- action class
- reversibility
- cost
- privacy or security impact
- external visibility
- architectural or product-intent impact
- expected consequence
- confidence and evidence quality
- required evidence
- required approval
- policy constraints

## Risk-based autonomy

Autonomy is determined by consequence, confidence, reversibility, evidence quality, and policy—not by whether a human or AI authored the change.

Low-risk, reversible, strongly verifiable work may be delegated for autonomous execution and merge.

Higher-risk work requires progressively stronger controls. Architectural invariant changes, destructive actions, security/privacy changes, expensive actions, external releases, product-intent changes, and other consequential operations may require explicit human authority even when an agent can implement and verify them autonomously.

No amount of model confidence alone may bypass a governance boundary.

## Outcome feedback

Outcome evidence can alter future authority decisions. A class of changes that repeatedly produces failed or inconclusive outcomes may require stronger verification, reduced autonomy, new constraints, or human approval.

Conversely, strong historical evidence may justify safe delegation where policy permits it.

Historian and the Modeled World provide the evidence and precedent; Obdurate applies the policy.

## Outcomes

A proposed action can be:

- allowed
- denied
- constrained
- redirected to a safer capability
- held for approval
- held for additional evidence
- allowed only with post-execution outcome observation

## Principle

The model proposes. Governance decides. Tools execute only within the granted capability.

Humans govern consequences, not keystrokes.
