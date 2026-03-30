# Simplify Workflow

Use this workflow to reduce unnecessary complexity while preserving adequacy.

## When to use

Use this workflow when:

- there are too many options
- the proposed solution feels overbuilt
- the explanation has too many assumptions
- the workflow contains too many steps
- the system has too many moving parts
- the user asks what can be removed

## Core question

What is the simplest path, explanation, or design that still works?

## Process

### Step 1: Define adequacy

State the minimum thing the explanation or system must do.

To define adequacy well:
- List the outcomes the simplified version must still deliver
- List the constraints it must still respect
- List at least one failure mode it must still survive
- If you cannot list a failure mode, your adequacy definition is probably too narrow

Do not simplify before defining what must be preserved. If components and constraints are not yet clear, run Deconstruct first.

### Step 2: List current options or moving parts

Make the competing explanations, features, steps, or structures explicit.

### Step 3: Measure assumption load

For each option or component, ask:

- how many extra assumptions it requires
- how many dependencies it adds
- how many actors or handoffs it introduces
- whether it exists for a real function or just for reassurance
- whether it is compensating for another weak part of the system

### Step 4: Remove non-essential complexity

Prefer removing:

- decorative complexity
- speculative additions
- duplicate layers
- workaround-driven structure
- optional steps with low payoff

**Sanity check:** For each item marked for removal, state why its removal is safe. If you cannot articulate why, do not remove it.

### Step 5: Compare simplified candidates

Prefer the option that:

- still fits the facts
- still satisfies the real goal
- uses fewer assumptions
- adds less coordination cost
- is easier to test or execute

### Step 6: State what would force more complexity

Name the specific evidence, metric, or event that would make the current simplification insufficient. Be concrete — what would you see, measure, or learn?

Bad: "if requirements change significantly"
Good: "if monthly active users exceed 10,000, the single-server architecture needs a load balancer"

Name 1-2 specific triggers, not a vague list.

## Output format

- What must be preserved
- Current options or moving parts
- Assumption load
- What can be removed
- Simplest sufficient option
- What would justify more complexity later

## Quality bar

A good simplification should:
- handle every requirement in the adequacy definition
- use fewer assumptions, dependencies, or coordination steps than alternatives considered
- name what was removed and why it was safe to remove
- feel cleaner and more direct without becoming naive
