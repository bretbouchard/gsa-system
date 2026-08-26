# Historian

The Historian preserves the epistemic state of the system over time.

It records more than events. It preserves what was believed, why it was believed, what evidence supported it, what decision followed, what outcome was expected, and what happened afterward.

## Responsibilities

- decision history
- evidence provenance
- prior assumptions
- superseded beliefs
- expected outcomes
- observed outcomes
- precedent
- reversals and corrections
- links between decisions and later consequences
- links between verified implementation and later outcome validation or failure
- lessons that should constrain future planning

## Outcome history

Historian must preserve the difference between:

- `the change was implemented correctly`; and
- `the change produced the intended effect`.

Implementation verification closes an engineering obligation. Outcome validation closes a hypothesis about reality.

For consequential Changes, Historian should be able to reconstruct:

1. the original intent;
2. the expected outcome;
3. assumptions and unknowns at decision time;
4. the implementation Change;
5. verification evidence;
6. later observed evidence;
7. whether the outcome was validated, failed, or remained inconclusive;
8. any follow-up Change, reversal, supersession, or learned constraint.

## Why this matters

A long-running agentic system should not repeatedly rediscover the same lesson or silently rewrite its own history. The Historian lets future work distinguish current truth from prior belief and compare decisions against outcomes.

This also prevents a common failure mode in autonomous software work: treating a passing test suite or successful deployment as proof that the product or architectural decision itself was correct.
