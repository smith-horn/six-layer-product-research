# Layer 6: Feasible Influence

**Framework**: Teresa Torres 6-Layer Problem Definition Framework — Layer 6
**Core Question**: "What can we realistically change, given our constraints?"

---

## What This Layer Is For

Layer 6 is the reality filter. Layers 1–5 have produced a rich picture of the problem — customer voice, ecosystem dynamics, behavioral barriers, the graveyard of prior attempts, and the technologies that make new solutions possible. Layer 6 asks: **given all of that, what can your specific team actually change?**

This layer prevents two failure modes:
- **Over-ambition**: Building a solution that requires changing things outside your control (platform APIs, competitor behavior, regulatory frameworks, user psychology that requires years to shift)
- **Under-ambition**: Scoping so conservatively that the solution doesn't address the root problem

The output of Layer 6 is a scoped problem statement — the subset of the full problem that your team can realistically address, with a clear rationale for what is in and out of scope.

---

## What "Feasible Influence" Means

Feasible influence does not mean "easy." It means:

1. **You have access to the leverage point** — you can build, partner, or influence your way to addressing it
2. **The constraint can be moved in your time horizon** — not "eventually possible" but "achievable in the next 12–18 months"
3. **You have or can acquire the required resources** — technical, partnership, go-to-market
4. **The ecosystem will allow it** — actors from Layer 2 won't block it; behavioral dynamics from Layer 3 don't make it impossible

Things that are outside feasible influence are not failures — they are scope boundaries. Document them clearly.

---

## Research Questions to Answer

### Internal Constraint Assessment

1. **What is your team's actual technical reach?**
   - What can you build vs. what requires partnerships or platform cooperation?
   - What would require capabilities (data, infrastructure, relationships) you don't have?

2. **What is your time horizon?**
   - What must be true in 3 months? 12 months? 3 years?
   - Different constraints apply at different horizons.

3. **What are your distribution constraints?**
   - How do you reach your target customer? What channels are available, and which aren't?
   - From Layer 2: who has distribution that you could partner with vs. compete against?

### Ecosystem Constraint Assessment

4. **Which ecosystem actors can you influence, and which will resist?**
   - From Layer 2: map each actor as ally, neutral, or potential blocker.
   - Allies can be leveraged. Neutrals can be ignored for now. Blockers must be managed.

5. **What platform dependencies constrain your solution?**
   - If your solution depends on a platform (API, marketplace, OS), what happens if that platform changes the rules?
   - Identify single points of failure in your distribution or delivery.

6. **What industry standards or protocols are forming that you must align with?**
   - From Layer 5: which emerging standards will define who is "in" and who is "out" of the ecosystem?
   - Being outside an emerging standard is an existential constraint.

### Behavioral Constraint Assessment

7. **Which behavioral barriers from Layer 3 can you change, and which must you design around?**
   - Some behaviors can be shifted (friction can be removed, prompts can be added)
   - Others are structural (users will never check a dashboard proactively; design for ambient, not active)
   - Be honest. "We'll change user behavior through education" is almost always wrong.

8. **What does the customer have to believe or do differently for your solution to work?**
   - Each required behavior change is a risk. Minimize required behavior changes.
   - The most robust solutions work *with* existing habits, not against them.

### Strategic Window Assessment

9. **Is there a timing constraint that makes now the right moment?**
   - Ecosystem consolidation windows (when a market is forming standards) close quickly
   - Partner relationships have finite availability
   - Competitor gaps are temporary
   - Document what specifically creates a timing advantage, and when it closes

10. **What is the minimum viable influence?**
    - What is the smallest set of changes that would make a meaningful difference?
    - This becomes your MVP thesis.

---

## Synthesis Framework: The In/Out/Later Table

After completing research, categorize every potential intervention:

| Category | Definition | Example |
|----------|------------|---------|
| **In scope** | You can influence this in your time horizon | Reducing discovery friction at the point of use |
| **Out of scope (not feasible)** | Requires resources, access, or behavior change you can't achieve | Changing platform API behavior |
| **Out of scope (not necessary)** | True, but solving it doesn't move your core metric | Fixing a problem that only affects 2% of users |
| **Later** | Feasible but requires a foundation you're building now | Federation with other registries after single-registry validation |

Be honest about "Out of scope (not feasible)." Teams that put things in "Later" when they mean "Never" build roadmaps that mislead.

---

## The Scoped Problem Statement

Layer 6 culminates in a scoped problem statement — the version of the problem your team will actually address.

**Structure**:
> [Target user] in [specific context] cannot [specific action or outcome] because [root cause your team can address], and existing solutions fail to solve this because [structural gap]. Our team can address this because [specific feasible leverage point], within the constraint that [explicit scope boundary].

**What separates a scoped statement from a vague one**:
- It names who is NOT included (scope boundary)
- It names what root cause is NOT being addressed (and why)
- It is falsifiable — you can test whether the problem is solved

---

## Common Mistakes in Layer 6

**Scope set by ambition rather than constraint**: "We'll solve the whole problem" is a funding pitch, not a feasibility assessment. Be specific about what you can't do.

**Ignoring ecosystem blockers**: If a major ecosystem actor benefits from the problem persisting (Layer 2), they will resist your solution. "We'll win on quality" is not a strategy for dealing with an incumbent with distribution.

**Underestimating behavior change costs**: Every behavior change required of users reduces adoption. Each one is a risk. Minimize them, don't plan for multiple simultaneous behavior changes.

**Treating "Later" as a safe category**: "Later" should mean "we have a concrete plan for when Later arrives." If you don't, it should be "Out of scope."

**Skipping the timing assessment**: If there's a strategic window, document when it closes and what happens if you miss it. This focuses execution.

---

## Completing the Framework

After Layer 6, you have everything you need to write:

1. **The full problem statement** — grounded in all 6 layers, scoped by feasibility
2. **The solution direction** — what the research points toward (this is still not a spec)
3. **The opportunity statement** for Torres' Opportunity Solution Tree

**Full problem statement structure**:
> [Customer, in their words from Layer 1] face [problem, described through behavioral lens from Layer 3], compounded by [ecosystem dynamic from Layer 2]. Existing solutions fail because [failure mode pattern from Layer 4]. New technical capabilities [from Layer 5] now make a different class of solution possible. Our team can address [specific subset from Layer 6], within the constraint that [scope boundary].

**Solution direction** (not a spec — a direction):
> Build [solution type] that [addresses specific Layer 3 friction], leveraging [specific Layer 5 capability], positioned as [ecosystem role from Layer 2 analysis], moving quickly to [strategic window from Layer 6].

---

## Output

Produce two documents:

1. **Raw research document** (`layer-6-feasibility-research.md`) — constraint inventory, ecosystem blocker map, timing analysis.
2. **Layer 6 synthesis** (use `templates/layer-synthesis-template.md`) — In/Out/Later table, scoped problem statement, solution direction.

Then produce the final cross-layer document (use `templates/cross-layer-template.md`) — the culmination of all six layers.

When writing files, the default output path is `docs/research/` in your current project. Claude will confirm the location with you before writing.
