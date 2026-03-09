# Layer 3: Behavioral Dynamics

**Framework**: Teresa Torres 6-Layer Problem Definition Framework — Layer 3
**Core Question**: "What frictions, incentives, norms, habits, or power dynamics are blocking or reinforcing current behaviors?"

---

## What This Layer Is For

Layer 3 explains the gap between *stated intent* and *actual behavior*. Customers say they want something; they don't do it. Or they do something you didn't expect. Layer 3 is where you find out why.

This is the most analytically demanding layer because it requires going beyond what people say and examining the invisible forces — cognitive, social, organizational — that govern what people actually do.

Three frameworks are indispensable here:

---

## Behavioral Frameworks

### The Fogg Behavior Model (B=MAP)

Developed by BJ Fogg at Stanford's Behavior Design Lab, this model holds that a behavior occurs only when **Motivation**, **Ability**, and a **Prompt** converge simultaneously. If any one is absent, the behavior doesn't happen — regardless of how much the user wants it.

**B = Motivation × Ability × Prompt**

| Component | High | Low |
|-----------|------|-----|
| **Motivation** | User actively wants to do this | User knows it exists but doesn't care enough |
| **Ability** | Behavior is easy to perform | Too many steps, too much cognitive load |
| **Prompt** | A trigger surfaces at the right moment | No trigger, or trigger at the wrong time |

**Three prompt types** (Fogg, *Tiny Habits*, 2020):
- **Spark**: raises motivation when it's low ("This saved 2 hours on average")
- **Facilitator**: makes the behavior easier when motivation is high but ability is low ("One click to try")
- **Signal**: simply reminds when both motivation and ability are already present

**Diagnostic use**: If adoption is failing, identify *which* component is missing before designing an intervention. Missing motivation → spark prompt. Too much friction → facilitator. User forgets → signal.

**Source**: [behaviormodel.org](https://www.behaviormodel.org/) — BJ Fogg, Stanford Persuasive Tech Lab

---

### Technology Acceptance Model (TAM)

Proposed by Fred Davis (1989), TAM identifies two primary determinants of whether a user adopts a technology:

- **Perceived Usefulness (PU)**: "Will this actually help me do my job better?"
- **Perceived Ease of Use (PEOU)**: "Will this be too hard to learn or use?"

Both must be sufficiently positive for adoption to occur. The relationship is directional: PEOU affects PU (if it's easier, it seems more useful), and PU more strongly drives adoption intention than PEOU.

**Practical implication**: Users who believe a tool is useful will tolerate more friction. Users who are uncertain of usefulness will not invest effort to learn it. This means the first experience must demonstrate value *before* asking for any effort.

**Sources**:
- Davis, F.D. (1989). "Perceived Usefulness, Perceived Ease of Use, and User Acceptance of Information Technology." *MIS Quarterly*, 13(3), 319–340. [doi:10.2307/249008](https://doi.org/10.2307/249008)
- Developer tools application: [Explaining Software Development Tool Use with TAM](https://www.tandfonline.com/doi/abs/10.1080/08874417.2001.11647015)

---

### Diffusion of Innovations (Rogers)

Everett Rogers identified five attributes that determine how quickly a new technology spreads through a population:

| Attribute | Definition | Implication |
|-----------|------------|-------------|
| **Relative Advantage** | Is it clearly better than the alternative? | Must be demonstrably superior, not just different |
| **Compatibility** | Does it fit existing values and practices? | Solutions that require workflow disruption face higher resistance |
| **Complexity** | How hard is it to understand and use? | Simpler = faster adoption, even if less powerful |
| **Trialability** | Can people experiment with low commitment? | Low-stakes trials accelerate adoption |
| **Observability** | Can people see others using it successfully? | Social proof drives the majority who follow early adopters |

Rogers also identified the S-curve of adoption: Innovators (2.5%) → Early Adopters (13.5%) → Early Majority (34%) → Late Majority (34%) → Laggards (16%). Solutions stall most often at the "chasm" between Early Adopters and Early Majority, where social proof becomes the dominant adoption driver.

**Source**: [*Diffusion of Innovations*](https://en.wikipedia.org/wiki/Diffusion_of_innovations), 5th ed., Everett M. Rogers, 2003

---

## Research Questions to Answer

### Frictions

1. **What specific friction points prevent the desired behavior?**
   - Cognitive friction: too many decisions, unclear interface
   - Time friction: too slow, too many steps
   - Social friction: requires getting others involved
   - Trust friction: uncertainty about quality or reliability

2. **At what point in the workflow does the behavior need to occur?** And is that a high-friction moment (deep in a task) or a low-friction moment (idle, onboarding)?

3. **What is the cognitive load of the current situation?** Users under high cognitive load default to familiar behaviors. If your desired behavior requires learning, it will be deferred.
   - Research: Gloria Mark (UC Irvine) found that context-switching recovery takes an average of 23 minutes. [FastCompany](https://www.fastcompany.com/944128/worker-interrupted-cost-task-switching)
   - Microsoft study (2006): 90% of features users requested already existed — they simply didn't know. Feature awareness is a behavioral problem, not just a communication problem.

### Incentives

4. **What reinforces the current (undesired) behavior?** There is always a reason people do what they do. Find it before designing an intervention.

5. **What immediate rewards exist for the desired behavior?** BJ Fogg's research shows that immediate reinforcement (even tiny — a checkmark, a confirmation) dramatically increases habit formation. *Tiny Habits*, Chapter 5.

6. **What does the social environment reward?** If peers are celebrated for moving fast and the desired behavior looks like slowing down, social incentives work against you.

### Norms and Habits

7. **What is the existing habit that the desired behavior needs to replace or attach to?**
   - Rogers: Compatibility with existing habits is the second-strongest predictor of adoption.
   - Fogg: New behaviors attach most durably when anchored to existing habits ("After I do X, I will do Y").

8. **What are the professional or community norms around this behavior?** Open source communities have different norms than enterprise dev teams. Research both.

9. **What percentage of users have ever changed a relevant default setting?** Studies consistently show 85–95% of users never change defaults. Design for defaults; treat customization as edge case.

### Power Dynamics

10. **Who has approval authority over adoption?** In B2B, the person who benefits from your product often isn't the person who approves it. Document the approval chain.

11. **Are there status dynamics at play?** In developer communities, early adoption of new tools signals expertise. In conservative enterprise teams, adoption of unvetted tools signals poor judgment. Same behavior, opposite status signals.

---

## Synthesis Prompts

1. **Which Fogg component is the primary blocker?** Motivation, Ability, or Prompt? (Most problems have a primary blocker — identify it before designing interventions.)
2. **What is the TAM diagnosis?** Is low adoption driven by low Perceived Usefulness or low Perceived Ease of Use?
3. **Where on Rogers' S-curve is adoption currently?** Which chasm is the product stuck at?
4. **What is the single biggest behavioral blocker?**
5. **What behavior does your desired behavior need to replace, and what does that behavior currently reward the user with?**
6. **What would a "Facilitator Prompt" look like for your context?** (Reduces friction at the moment of highest motivation)

---

## Common Mistakes in Layer 3

**Treating behavioral blockers as communication problems**: "We just need better docs/marketing" is almost always wrong. If people know about a feature and aren't using it, the blocker is behavioral, not informational.

**Skipping to intervention design**: Identify which Fogg component is missing *before* designing solutions. Spark prompts don't fix low Ability; Facilitators don't fix low Motivation.

**Ignoring social proof**: Rogers' Observability is underweighted by most product teams. Watching someone else use a tool successfully is the most powerful adoption trigger for the majority of users — not feature lists or documentation.

**Over-engineering the first experience**: TAM says Perceived Usefulness drives adoption more than Perceived Ease of Use. The first experience must demonstrate genuine value quickly, even if imperfect. Polished empty experiences don't build habit.

---

## Output

Produce two documents:

1. **Raw research document(s)** — per source type (e.g., `layer-3-academic-research.md`, `layer-3-behavioral-interviews.md`). Sources, quotes, framework applications.
2. **Layer 3 synthesis** (use `templates/layer-synthesis-template.md`) — Fogg diagnosis, TAM diagnosis, Rogers stage, unified behavioral barrier, strategic implication.

When writing files, the default output path is `docs/research/` in your current project. Claude will confirm the location with you before writing.
