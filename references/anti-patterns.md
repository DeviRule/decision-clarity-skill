# Anti-Patterns

Use this file to avoid turning decision clarity into abstract, bloated, or misleading reasoning.

## Core warning

This skill should not become:

- endless questioning
- contrarian theater
- empty abstraction
- false simplicity
- analysis without action
- "it depends" used as an escape

The goal is better judgment, not more intellectual performance.

## Common failure modes

### 1. Endless inquiry

Bad pattern:
Asking many questions without improving understanding.

Correction:
Ask at most 2-3 clarifying questions. If you cannot determine which question matters most, state your best interpretation and proceed. Questions that don't change the recommendation are wasted.

### 2. Solving the wrong question well

Bad pattern:
Accepting the user's framing without checking whether it is the real issue.

Correction:
Clarify the actual goal before analyzing solutions.

### 3. Abstract decomposition

Bad pattern:
Talking about fundamentals without naming actual facts, constraints, costs, incentives, or mechanisms.

Correction:
Reduce the problem into concrete parts.

### 4. False simplicity

Bad pattern:
Removing complexity by ignoring important evidence or constraints.

Correction:
Simplicity must preserve adequacy.

### 5. Contrarian posturing

Bad pattern:
Rejecting norms automatically because they are conventional.

Correction:
Reject only what fails decomposition or necessity.

### 6. No recommendation

Bad pattern:
The answer is insightful but leaves the user with no clearer move.

Correction:
Always end with a recommendation, next step, or decision rule.

### 7. Overbuilding the answer

Bad pattern:
The analysis becomes more complex than the problem.

Correction:
Use the lightest structure that still improves the decision.

### 8. Premature certainty

Bad pattern:
Presenting a confident recommendation when the information is genuinely insufficient to decide.

Correction:
If the recommendation depends heavily on an unverified assumption, say so. "Delay and gather X" is a legitimate recommendation when the cost of being wrong exceeds the cost of waiting.

### 9. Assumption smuggling

Bad pattern:
Replacing the user's hidden assumptions with your own hidden assumptions during analysis. The output looks rigorous but has swapped one set of unexamined beliefs for another.

Correction:
Label every assumption explicitly — including your own. Distinguish "the user assumes X" from "I am assuming Y based on general knowledge." Mark inferences as inferences.

### 10. Reframing as deflection

Bad pattern:
Reframing the question so aggressively that the original question never gets answered. The user asks "Should I use React or Vue?" and gets "The real question is what user outcome you're trying to achieve" without ever returning to the concrete choice.

Correction:
Reframing must circle back. After clarifying the real question, answer the original question through the new lens. The user should get both the reframe and the answer.

### 11. Trusting the simple story in adversarial contexts

Bad pattern:
Applying Occam's razor in situations where an adversary may be shaping the information environment. Choosing the simplest explanation when someone benefits from you reaching that conclusion.

Correction:
In adversarial contexts, prefer the pessimistic interpretation until evidence rules it out. Ask "who benefits from me believing this?" before accepting the simplest explanation. See `references/adversarial.md`.

## Self-check before finalizing

Ask:

- Did I identify the real question?
- Did I expose the main assumption?
- Did I separate facts from inertia?
- Did I simplify without deleting reality?
- Did I end with a useful next move?
- Am I presenting my inferences as verified facts?
- Is the analysis proportionate to the stakes and reversibility?
- If I reframed the question, did I also answer it?
- Does my output name at least one way the recommendation could fail? (pre-mortem check)
- If this decision involves an adversary, did I consider their incentives and likely response?

If any answer is no, revise.
