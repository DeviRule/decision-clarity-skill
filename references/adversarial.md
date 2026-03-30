# Adversarial

Use this file for decisions in adversarial contexts — security threats, competitive moves, negotiation, hostile information environments, and situations where another party is actively trying to influence your decision.

## Core orientation

Adversarial decisions differ from normal decisions because:

- the information environment may be deliberately manipulated
- the simplest explanation may be the one the adversary wants you to reach
- your actions change the adversary's behavior (game-theoretic feedback)
- the cost of being wrong is often asymmetric (defender must succeed every time; attacker only once)
- time pressure is often artificial and imposed by the adversary

## When to activate adversarial reasoning

Use this lens when any of these are true:

- another party benefits from your decision going a specific way
- the information you are acting on could have been planted or shaped
- your decision will be observed and reacted to by a competitor or adversary
- the stakes are asymmetric (your downside is larger than their cost to attack)
- you are under time pressure you did not create

## Key inversions from normal reasoning

In adversarial contexts, invert these default rules:

| Normal default | Adversarial inversion |
|---|---|
| Prefer simpler explanation (Occam's) | Ask: who benefits from me choosing the simple explanation? |
| Prefer lower assumption load | Assume the worst case until evidence rules it out |
| Treat soft constraints as challengeable | Some "soft constraints" may be adversary-imposed traps |
| Bias toward action on reversible choices | Even "reversible" actions may reveal information to the adversary |

## Strong questions

- Who benefits from me making this specific decision?
- What would the adversary want me to believe, and does the available evidence conveniently support it?
- If I take this action, what information does it reveal to the other party?
- What is the adversary's cost to exploit my mistake vs. my cost to recover?
- Am I under time pressure because the situation demands it, or because someone imposed it?
- What would I do differently if I assumed the most pessimistic interpretation?

## Security-specific lenses

For security decisions specifically:

- **Threat model first:** What is the actual threat actor, capability, and intent? Do not defend against hypothetical threats at the expense of real ones.
- **Supply chain risk:** What is the blast radius if this dependency (library, vendor, CI provider) is compromised?
- **Disclosure timing:** Is the vulnerability being actively exploited? What is the cost of waiting vs. the cost of premature disclosure?
- **Defense asymmetry:** The defender must get everything right; the attacker only needs one gap. Where is the one gap?
- **Attribution confidence:** How reliable is the threat intelligence? Could the source be compromised or incentivized to mislead?
- **Incident velocity:** In active incidents, the cost of analysis delay may exceed the cost of imperfect action. Name the time constraint explicitly.

## Typical outputs

- identification of adversary incentives and likely responses
- reframed risk assessment that accounts for deliberate manipulation
- recommendation that minimizes information leakage to adversary
- detection of artificial urgency or planted evidence
- action plan that assumes pessimistic scenario until ruled out
