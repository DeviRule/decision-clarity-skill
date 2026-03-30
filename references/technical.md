# Technical

Use this file for research direction, architecture choices, build-vs-buy, migration timing, security posture, and technical tradeoff questions.

## Core orientation

Most technical confusion comes from:

- solving for elegance instead of the actual constraint
- premature abstraction or optimization
- inherited architecture treated as immutable
- build-vs-buy decisions driven by ego rather than economics
- security theater replacing actual threat modeling
- research direction chosen by interest rather than impact
- supply chain dependencies accepted without blast-radius analysis
- decisions made under artificial urgency imposed by external pressure

## Key lenses

Examine:

- actual constraint (performance, security, correctness, cost, time)
- reversibility of the choice
- maintenance burden over time
- team capability and context-switching cost
- attack surface and threat model
- assumption load of each approach
- what evidence exists vs. what is hypothesized
- supply chain blast radius (what happens if this dependency is compromised?)
- adversary economics (what does the attacker's cost/benefit look like?)
- temporal sensitivity (is there a closing window that changes the calculus?)
- information leakage (does this decision reveal something to a competitor or adversary?)

## Strong questions

- What is the actual technical constraint we are solving for?
- Is this architecture chosen because it fits, or because it is familiar?
- What is the threat model, and does the defense match it?
- Build-vs-buy: what is the total cost of ownership, not just the build cost?
- What would we do if this decision turns out to be wrong in 6 months?
- Which part of this system is actually load-bearing, and which is decorative?
- What is the simplest architecture that handles the real (not hypothetical) load?
- What is the blast radius if our most critical dependency is compromised tomorrow?
- Are we defending against the actual threat model or against compliance checkbox requirements?
- What would an attacker target first in this architecture?
- Is this time pressure real, or is it artificially imposed?

## Typical outputs

- simpler architecture that fits actual constraints
- clearer build-vs-buy decision based on total cost
- tighter research focus based on impact rather than novelty
- more realistic threat model replacing security theater
- reversible technical choice replacing premature commitment
- security investment matched to actual threat model rather than compliance theater
- supply chain risk assessment with concrete blast-radius bounds
- decision that accounts for adversary response
