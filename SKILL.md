---
name: decision-clarity
description: Improve decision quality by clarifying the real problem, exposing hidden assumptions, reasoning from fundamental facts, reducing unnecessary complexity, and ending with a cleaner recommendation or next step. Use when the user is confused, comparing options, overcomplicating a problem, questioning assumptions, trying to identify the real bottleneck, or asking things like "what am I missing?", "does this really have to be this way?", "what should I remove?", "what is the simplest explanation that still fits?", or "help me think this through".
---

# Decision Clarity

Use this skill to turn ambiguous, high-value, complexity-prone problems into clearer decisions.

This skill combines three reasoning modes in a practical sequence:

1. Socratic questioning to clarify the real issue
2. First-principles thinking to reduce the issue to facts and constraints
3. Occam-style simplification to remove unnecessary complexity

Do not use this skill to sound philosophical. Use it to improve judgment.

## Core objective

Produce answers that:

1. identify the real question
2. expose hidden assumptions
3. reduce the issue to facts, constraints, and causal structure
4. compare options by complexity and assumption load
5. remove false complexity
6. end with a clear recommendation, next step, or test

A strong answer should make the user feel:

- "the real problem is clearer now"
- "you found the assumption I was missing"
- "this is simpler than I thought"
- "I know what to do next"

## Operating stance

Default to clarity before confidence.

Ask:

- What is the user actually trying to decide or understand?
- Which parts of the problem are vague, inherited, or untested?
- What facts and hard constraints actually matter?
- Which explanation or plan requires fewer unnecessary assumptions?
- What is the simplest path that still respects reality?

## Best-fit use cases

This skill is especially useful for:

- startup and business decisions
- product and MVP decisions
- content and creator workflow design
- operations and process simplification
- strategy questions with multiple plausible options
- personal decisions where confusion, self-justification, or complexity are distorting judgment
- argument and reasoning audits

## Not a good fit for

Do not use this skill for:

- simple factual lookup
- purely mechanical execution tasks
- obvious low-stakes choices
- cases where the user explicitly wants only conventional guidance without reframing

## Workflow routing

State which workflow and mode you selected and why before producing output.

Route by the strongest signal in the user's input:

1. **User cannot articulate what they are deciding** → `Workflows/Clarify.md`
   - Signals: vague language, undefined terms, goal-method confusion, "I'm not sure what to do"
2. **User has a clear question but it involves multiple factors, mechanics, or hidden structure** → `Workflows/Deconstruct.md`
   - Signals: "why is this happening?", black-box problems, accepted costs without decomposition
3. **User has a clear question with too many options, steps, or moving parts** → `Workflows/Simplify.md`
   - Signals: "this feels overbuilt", comparison of named options, "what can I remove?"
4. **User needs a recommendation among known options or a next move** → `Workflows/Decide.md`
   - Signals: "which should I pick?", "what should I do?", analysis already done, conversation at risk of stalling

**Tiebreaker:** If signals overlap, prefer Clarify. Clarity unlocks everything downstream.

**Full sequence:** For non-trivial problems where no single workflow is sufficient, run:
1. Clarify → 2. Deconstruct → 3. Simplify → 4. Decide

For simpler problems, compress the sequence. See `references/examples.md` Example 5 (Quick Reframe) for what compressed output looks like.

**Urgency modifier:** When the decision is time-critical (active incident, closing window, expiring deadline), compress to Mode A regardless of complexity. The cost of delayed analysis can exceed the cost of a suboptimal decision. Name the time constraint explicitly: "This must be decided by X because Y."

**Adversarial modifier:** When the decision involves an adversary (security threats, competitive moves, negotiation, hostile information environments), invert some defaults:
- **Prefer higher assumption load** — assume the worst case, not the simplest explanation. Occam's razor can be weaponized: the simplest explanation for anomalous behavior may be what the adversary wants you to believe.
- **Treat simple explanations with suspicion** — ask "who benefits from me reaching this conclusion?"
- **Model the adversary's decision tree** — what will they do in response to each of your options?
- Read `references/adversarial.md` for adversarial reasoning lenses.

## Mode selection

Choose the lightest response mode that still improves the decision.

### Mode A: Quick Reframe

**When:** Short or single-factor questions. The user needs a perspective shift, not a deep analysis.
**Typical with:** Any single workflow, or compressed full sequence.

Output (from `references/output-patterns.md` Pattern 1):

- Real issue
- Hidden assumption
- Main constraint
- Simpler conclusion
- Next move

### Mode B: Structured Decision Analysis

**When:** Multi-factor decisions with real stakes — startup, product, operations, technical architecture, life choices.
**Typical with:** Full sequence or Deconstruct + Decide.

Output (from `references/output-patterns.md` Pattern 2):

- Real goal
- Assumptions
- Basic facts
- Hard constraints
- Soft constraints
- Simpler options
- Recommendation
- First test or next step

### Mode C: Reasoning Audit

**When:** The user presents their own argument, thesis, plan, or decision path for review.
**Typical with:** Any workflow. The key signal is that the user is asking you to *evaluate* their reasoning, not generate your own.

Output (from `references/output-patterns.md` Pattern 3):

- Real question
- Weak assumptions
- Missing evidence or contradiction
- Simpler interpretation
- Refined judgment
- Next checkpoint

For specialized output structures (option comparisons, workflow simplifications), see Patterns 4-5 in `references/output-patterns.md`.

Do not force a long analysis when a shorter one is enough.

## Required reasoning rules

### 1. Clarify before solving

Do not solve the wrong problem well.

Restate the issue in outcome terms, not only in the user's current framing.

Examples:

- "Should I build an app?" may really mean "what is the best delivery mechanism for this user outcome?"
- "How do I make this more professional?" may really mean "how do I increase trust, clarity, conversion, or authority?"
- "Why is this so hard?" may really mean "which part is actually the bottleneck?"

If the question is framed at the wrong level, say so and correct it.

### 2. Surface assumptions explicitly

Look for assumptions in:

- the user's wording
- inherited workflows
- industry norms
- default best practices
- preferred tools or formats
- emotional preferences presented as logic

Useful prompts to yourself:

- What is being treated as necessary?
- What would have to be true for this conclusion to hold?
- What is being accepted without evidence?
- Which assumption is carrying the most weight?

### 3. Reduce the issue to facts and constraints

Break the problem into:

- goals
- user behavior
- incentives
- cost structure
- time requirements
- dependencies
- information flow
- causal drivers
- legal or technical boundaries
- real risks

Prefer mechanism over narrative.

Do not say "this is just how the market works" unless you explain the actual mechanics.

### 4. Distinguish hard constraints from soft constraints

#### Hard constraints
Treat these as real unless evidence suggests otherwise:

- physical limits
- legal or regulatory limits
- hard technical boundaries
- fixed budgets or capacities
- immovable deadlines already fixed in reality

#### Soft constraints
Treat these as challengeable by default:

- industry conventions
- legacy process steps
- default tool choices
- current org boundaries
- aesthetic expectations
- existing architecture
- "this is how it is usually done"

Never present a soft constraint as immutable without justification.

### 5. Prefer lower assumption load

When comparing explanations or options, prefer the one that:

- requires fewer speculative assumptions
- introduces fewer moving parts
- adds less coordination cost
- preserves the real goal with less structure
- still adequately fits the facts and constraints

Do not simplify by deleting reality. Simplicity must remain sufficient.

**Exception:** In adversarial contexts, invert this rule — assume the worst case, not the simplest explanation. See the adversarial modifier in Workflow routing.

### 6. End with a decision

Always end with one of:

- a recommendation
- a decision rule
- a priority order
- a smallest useful experiment
- a first implementation step
- a short list of what to answer next

Do not end with abstract reflection alone.

### 7. Assess reversibility

Before recommending, ask: is this action a one-way door or a two-way door?

**One-way doors** (hard to reverse): signing contracts, public launches, deleting data, burning bridges, spending limited capital. These need more certainty before acting.

**Two-way doors** (easy to reverse): experiments, feature flags, prototype tests, temporary hires, soft launches. These need less certainty — bias toward action.

When the best option is a one-way door, look for a two-way-door version first (pilot, prototype, limited test). Only recommend the irreversible version when no reversible alternative exists.

### 8. Name what you don't know

Distinguish between:
- **facts you can verify** from the user's input or context
- **claims the user made** that you are treating as true
- **inferences you are making** based on general knowledge
- **gaps** where you have no information

Do not present inferences as facts. When a recommendation depends on an unverified claim, say so.

### 9. Run a pre-mortem

Before committing to a recommendation, assume it was implemented and failed. Ask:
- What went wrong?
- Which assumption turned out to be false?
- What did we not see coming?

This is not risk assessment (which is prospective). A pre-mortem uses prospective hindsight — imagining the failure as already happened — which increases the ability to identify failure modes by ~30%. If the pre-mortem reveals a plausible, high-consequence failure path, either mitigate it or reconsider the recommendation.

### 10. Check the outside view

Before finalizing, ask: how do similar decisions turn out for similar people in similar situations?

- For startup decisions: most startups fail. What makes this one different?
- For career transitions: what is the base rate of success for this type of move?
- For technical bets: what happened to others who made this same architectural choice?

The "inside view" (analyzing your specific situation) tends toward overconfidence. The "outside view" (reference class forecasting) provides calibration. Use both.

## If information is incomplete

Do not stall. Instead:

1. name the key ambiguity
2. state the most likely interpretations
3. make the minimum necessary assumptions explicit
4. proceed with the best current interpretation
5. say what fact would most change the recommendation

## Before finalizing output

Run these structural checks. Each must be mechanically verifiable, not subjective:

1. **Reframe check:** Does my output contain a reframed question or goal that differs from the user's surface phrasing? If not, I may be solving the stated problem without checking if it is the real one.
2. **Assumption label check:** Does my output contain at least one item explicitly labeled as an assumption (not presented as fact)? If not, I may be smuggling assumptions.
3. **Action check:** Does my last section contain a concrete action with a verb and an object — not a reflection or a vague aspiration? ("Run one enterprise pilot" not "consider exploring options")
4. **Proportionality check:** Is my response length proportionate to the stakes? Mode A questions should get ~150 words. Mode B should not exceed the complexity of the problem itself.
5. **Circle-back check:** If I reframed the question, did I also answer the original question through the new lens?
6. **Pre-mortem check:** Did I name at least one plausible way the recommendation could fail?

If any check fails, fix it before outputting. See `references/anti-patterns.md` for the full failure mode list.

## Domain references

Read only the relevant references when useful:

- `references/business.md` for startup, pricing, growth, distribution, and strategy
- `references/product.md` for MVP, feature decisions, onboarding, user jobs, and scope
- `references/content.md` for tutorials, creator workflows, content quality, and production systems
- `references/operations.md` for SOPs, approvals, handoffs, and workflow simplification
- `references/technical.md` for research direction, architecture choices, build-vs-buy, and technical tradeoffs
- `references/adversarial.md` for decisions in adversarial contexts — security, competition, negotiation, hostile information
- `references/personal.md` for career, life transitions, personal strategy, and value-alignment decisions
- `references/trigger-questions.md` for transforming vague user prompts into sharper analysis frames
- `references/output-patterns.md` for stable response structure
- `references/examples.md` for concrete high-value examples
- `references/anti-patterns.md` whenever the reasoning risks becoming overly abstract, endlessly inquisitive, falsely simple, or non-actionable

## Quality bar

A strong answer produced with this skill should:

- identify the real decision or question
- expose the hidden assumption
- separate facts from inertia
- reduce unnecessary complexity
- preserve adequacy
- leave the user with a cleaner next step

If the answer sounds clever but does not improve the user's decision quality, it is not good enough.
