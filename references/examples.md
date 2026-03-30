# Examples

Use these examples to recognize the full decision-clarity sequence.

Pattern:

- Surface question
- Real issue
- Assumptions
- Facts and constraints
- Simplified options
- Best current move

## Example 1: Startup idea confusion

### Surface question
Is this a good startup idea?

### Real issue
Is there a painful enough problem, for a clear enough buyer, with economics that could work?

### Assumptions
- the market is big enough
- users care enough
- the current alternatives are weak
- more features will improve competitiveness

### Facts and constraints
- pain level and urgency matter more than narrative quality
- switching costs may be high
- buyer trust may be the bottleneck
- limited resources force prioritization

### Simplified options
- broad product for many users
- narrow product for one painful job

### Best current move
Test the narrowest painful job first with a simple value promise.

---

## Example 2: Overbuilt MVP

### Surface question
What should we include in the MVP?

### Real issue
What is the smallest product that can create a meaningful result and produce evidence of demand?

### Assumptions
- users expect breadth
- competitor parity matters immediately
- missing secondary features will kill adoption

### Facts and constraints
- the core promised outcome must work
- resources are limited
- extra features increase confusion and development drag

### Simplified options
- multi-feature launch
- narrow outcome-first launch

### Best current move
Ship the smallest version that solves one painful outcome clearly and measure activation plus repeat usage.

---

## Example 3: Heavy content workflow

### Surface question
Why does making tutorials take so long?

### Real issue
Which parts of the workflow create audience value, and which parts only create production drag?

### Assumptions
- high effort equals high quality
- each tutorial needs a unique process
- heavy editing is necessary

### Facts and constraints
- correctness and clarity matter
- proof and pacing matter
- much polish does not materially improve understanding

### Simplified options
- full custom production each time
- repeatable pipeline with reuse

### Best current move
Create one reusable tutorial pipeline and compare production time against audience response.

---

## Example 4: Bloated workflow

### Surface question
Why is this process so slow?

### Real issue
Which steps are real risk controls, and which are inherited organizational friction?

### Assumptions
- each approval is necessary
- more oversight always reduces risk
- current sequencing is safest

### Facts and constraints
- some steps exist only because of old incidents
- handoffs increase cycle time
- only some approvals are tied to real risk

### Simplified options
- keep full workflow
- remove duplicate approvals and merge low-value handoffs

### Best current move
Simplify one low-risk version of the process and compare cycle time plus error rate.

---

## Example 5: Quick Reframe — Security architecture question

### Mode A output

**Real issue:** The question is not "which framework" but "what is the actual threat model, and does the defense need to match it?"

**Hidden assumption:** More security layers always means more security. In practice, unused or misconfigured layers increase attack surface.

**Main constraint:** Limited security engineering time must be allocated to the threats that actually matter.

**Simpler conclusion:** Map the real threat model first. Defend against the top 3 realistic attack vectors. Remove security theater that consumes resources without reducing risk.

**Next move:** List the top 3 attack vectors by likelihood and impact, then check whether current defenses address them.

---

## Example 6: Incomplete information — Startup market entry

### Surface question
Should I enter the enterprise market or stay with SMBs?

### Handling incomplete information

**Key ambiguity:** We don't know the user's current revenue, team size, or sales capability — all of which determine whether enterprise is viable.

**Most likely interpretations:**
1. User has some SMB traction and is considering moving upmarket
2. User is pre-revenue and choosing an initial market

**Assumptions made explicit:** Assuming interpretation 1 (some SMB traction exists). If interpretation 2, the answer changes — start with SMBs because the feedback loop is faster.

### Real issue
Is the unit economics improvement from enterprise deals worth the longer sales cycle and higher support cost?

### Assumptions
- enterprise customers will pay enough to justify the sales cycle
- the product is mature enough for enterprise requirements (security, compliance, SLAs)
- the team can handle the support burden

### Facts and constraints
- enterprise sales cycles are typically 3-12 months
- enterprise deals require security audits, compliance, and dedicated support
- SMB retention may be the real lever if churn is the problem

### Simplified options
- stay SMB, fix retention
- move upmarket with one pilot enterprise customer

### Best current move
Run one enterprise pilot while measuring SMB retention. The pilot tests enterprise viability without abandoning the current base.

**What fact would most change this recommendation:** If SMB churn is below 5% monthly, the enterprise move is less urgent. If above 10%, enterprise may be necessary for survival.

---

## Example 7: Personal decision — Career transition

### Surface question
Should I leave my security research job to start a startup?

### Real issue
Can I test the startup hypothesis without an irreversible career move?

### Assumptions
- starting a startup requires quitting the job immediately
- the startup idea is validated enough to justify full commitment
- security research and startup building are mutually exclusive
- financial runway is sufficient

### Facts and constraints
- startup ideas need validation before full commitment
- security expertise is a differentiator that could be the startup itself
- leaving a job is a one-way door; starting a side project is a two-way door
- financial runway determines how much risk is rational

### Simplified options
- quit and go all-in (one-way door)
- validate on the side while employed (two-way door)
- negotiate reduced hours or sabbatical (partial door)

### Best current move
Spend 4 weekends validating the core hypothesis (do potential customers have the pain you think they have, and will they pay for a solution?). If validation succeeds, then negotiate a transition. Do not quit before you have evidence that the problem is real and someone will pay.

---

## Example 8: Technical architecture — Build vs. buy

### Surface question
Should we build our own auth system or use a third-party provider?

### Real issue
What is the total cost of ownership for each option, given our actual security requirements and team capability?

### Assumptions
- building our own gives us more control
- third-party auth is "good enough" for our security needs
- the team has the expertise to build and maintain auth securely
- integration cost with a third-party is low

### Facts and constraints
- auth is a security-critical component where mistakes have severe consequences
- custom auth requires ongoing maintenance (vulnerability patches, protocol updates)
- third-party providers handle compliance certifications (SOC2, etc.)
- the team's core competency is the product, not identity infrastructure

### Simplified options
- build custom (high control, high maintenance, high risk if team lacks auth expertise)
- use third-party provider (lower control, lower maintenance, transfers auth risk)
- hybrid: third-party for standard auth, custom for domain-specific authorization rules

### Best current move
Use a third-party provider for authentication (the part where getting it wrong is catastrophic) and build custom authorization logic only for domain-specific access rules. Revisit if the third-party becomes a constraint on functionality you actually need — not hypothetically might need.
