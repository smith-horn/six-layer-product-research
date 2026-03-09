# Layer 4: Status Quo Attempts

**Framework**: Teresa Torres 6-Layer Problem Definition Framework — Layer 4
**Core Question**: "What have people already tried, and why did it fail?"

---

## What This Layer Is For

Every meaningful problem has a graveyard of prior attempts. Layer 4 is where you study it.

Before designing a new solution, you need to understand:
- What solutions already exist (and why they're insufficient)
- What solutions have been abandoned (and what killed them)
- What workarounds people have built themselves (these are the richest signal of all)

The goal is not to avoid the graveyard — it's to learn from it. Teams that skip Layer 4 often rebuild failed solutions with minor variations and wonder why history repeats.

> "The most dangerous assumption in product development is that a problem exists because no one has tried to solve it. Usually, it exists because everyone who tried failed for the same reason."
>
> — Common pattern in post-mortem analysis

---

## Three Types of Status Quo Evidence

### Type 1: Existing Solutions That Persist

These are solutions that partially address the problem and are actively used. They persist because they're *good enough* — not because they're optimal.

Understanding existing solutions reveals:
- What the market has already validated (people paid for or adopted this)
- Where the persistent gaps are (what users complain about or work around)
- What ecosystem norms have formed around the solution

### Type 2: Abandoned Attempts

Solutions that were built and then died. Abandonments are more revealing than failures:
- The team got far enough to see what worked and what didn't
- Users made a considered decision to stop (rather than never starting)
- Post-mortem reasoning often exists in public

Common causes of abandonment:
- **Curation burnout**: Solutions requiring manual ongoing effort die when maintainers lose interest
- **Cold start failure**: Two-sided markets that never achieved critical mass on both sides
- **Trust deficit**: Solutions requiring trust that wasn't established before asking for it
- **Complexity overshoot**: Solutions that solved the problem theoretically but were too hard in practice
- **Scope creep**: Solutions that started focused but expanded until they became unwieldy

### Type 3: User-Built Workarounds

These are the richest signal in Layer 4. When users build their own solution — a spreadsheet, a custom script, a manual process — it tells you:
- The problem is real enough to justify effort
- The existing solutions are insufficient
- This is the "Job to Be Done" in its most honest form — users hired whatever they built to do a specific job

> Workarounds reveal the user's mental model of the ideal solution. The form of the workaround is often the shape of the product you should build.

---

## Research Sources for This Layer

| Source | What to find | How to search |
|--------|-------------|--------------|
| GitHub repositories (archived) | Abandoned tools with post-mortems in issues | Search `<domain> archived:true` |
| GitHub repository README files | "Why this exists" sections that describe what failed before | Look for "motivation" and "alternatives" sections |
| Hacker News "Show HN" history | Products that launched and disappeared | Site:news.ycombinator.com + product domain |
| Reddit post history | Threads asking "why did X die?" | r/<domain> + "discontinued" / "dead" / "abandoned" |
| Product Hunt graveyard | Products with votes but no traction | Older PH listings with low follower counts |
| App store reviews | What users hate about the current leader | Sort by 1-star and 2-star reviews |
| Blog post-mortems | Founders writing "why we shut down" | Google: `site:medium.com "<domain>" "shut down"` |
| User forums / Discord | Current workarounds people share | Look for pinned "how do you do X?" threads |
| Your own customer interviews | What did you try before this? | Add "what have you already tried?" to every interview |

---

## Research Questions to Answer

### Existing Solutions

1. **What solutions currently exist that address this problem, even partially?**
   - List them. Include manual processes, not just software.

2. **For each existing solution: what does it do well, and what do users consistently complain about?**
   - Source this from reviews, forums, and interviews — not from the product's own marketing.

3. **Why hasn't the most popular existing solution solved the problem?**
   - Is it structural (the solution can't solve it by design) or executory (it could, but hasn't)?

4. **What is the "good enough" threshold that keeps users from switching?**
   - What would have to change for a user to leave the current solution?

### Abandoned Attempts

5. **What solutions existed and no longer do?**
   - When did they shut down? What reasons were given?

6. **What patterns appear across multiple abandonments?**
   - If three tools all failed for similar reasons, that's a structural constraint, not a product flaw.

7. **Which anti-patterns keep reappearing?**
   - Document each anti-pattern with evidence. These become design constraints.

8. **What did abandoned solutions get right?**
   - Failed products often had one excellent insight surrounded by bad execution. Identify the insight.

### Workarounds

9. **What do users do *today* to cope with the problem?**
   - Manual processes, scripts, custom configs, social workarounds (asking a colleague).

10. **How much effort do users invest in their workarounds?**
    - A workaround that users invest significant effort in = a problem they genuinely want solved.
    - A workaround that users tolerate passively = a problem they'd like solved but won't pay much for.

11. **What does the shape of the workaround tell you about the shape of the ideal solution?**
    - If everyone builds a spreadsheet, they need structure + flexibility + offline access.
    - If everyone asks a colleague, they need social proof + explanation, not documentation.

---

## Anti-Pattern Catalog

Build a personal anti-pattern catalog for your domain during Layer 4. For each anti-pattern:
- **Name**: A memorable label
- **Description**: What it looks like
- **Why it fails**: The structural reason it doesn't work
- **Evidence**: At least two examples

Common anti-patterns across many domains:
- **The Directory Problem**: Comprehensive lists lose maintainability as they scale; curators burn out
- **The Trust-Before-Value Trap**: Asking users to trust before demonstrating value
- **The Two-Sided Cold Start**: Requiring both supply and demand before either has reason to join
- **The Power User Trap**: Optimizing for heavy users while losing the majority at first contact
- **The Integration Prerequisite**: Requiring users to set up a complex integration before seeing any value

---

## Synthesis Prompts

1. **What is the most important thing existing solutions get right?** (Preserve this.)
2. **What is the most consistent gap in existing solutions?** (This is your opportunity.)
3. **What is the #1 pattern across abandoned attempts?** (This is your first constraint.)
4. **What does the most common workaround tell you about what users actually need?**
5. **List the anti-patterns you must avoid.** State each as a design constraint: "We will not build a solution that requires X."

---

## Output

Produce two documents:

1. **Raw research document(s)** — existing solutions (`layer-4-existing-solutions.md`), abandoned attempts and workarounds (`layer-4-abandoned-patterns.md`). Include sources, links, quotes.
2. **Layer 4 synthesis** (use `templates/layer-synthesis-template.md`) — anti-pattern catalog, opportunity gaps, design constraints.

When writing files, the default output path is `docs/research/` in your current project. Claude will confirm the location with you before writing.
