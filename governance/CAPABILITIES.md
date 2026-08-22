# Capabilities

Capabilities are explicit, bounded permissions granted to tools or actors.

A capability should describe what may be done, to which resource, under what constraints, and for how long.

## Examples

- read a project file
- run a deterministic verifier
- propose a code patch
- write within a specific workspace
- send an approval request
- export a manufacturing artifact

## Why capabilities matter

Agentic systems become difficult to govern when the default primitive is unrestricted shell or account access. Capability-oriented tools make authority inspectable and revocable and let policy reason about concrete actions instead of vague agent intent.
