# Layer 1: Customer Mental Models

**Framework**: Teresa Torres 6-Layer Problem Definition Framework — Layer 1
**Core Question**: "What problem does the customer say they have, in their own words?"

---

## What This Layer Is For

Layer 1 captures the customer's *self-reported* problem in their own language. You are not interpreting yet — you are listening. The goal is to surface the vocabulary, metaphors, and emotional framing customers use when they describe their pain.

This is the voice-of-customer layer. It deliberately excludes your team's interpretation. That comes later.

> Torres caution: Teams almost always already have a hypothesis about what the problem is. Layer 1's job is to surface what customers *actually say*, not to confirm what you already believe. Approach sources without a predetermined conclusion.
>
> — Teresa Torres, *Continuous Discovery Habits*, Chapter 4

---

## Research Sources for This Layer

These are the most productive sources for capturing unfiltered customer voice:

| Source | What to look for | Tips |
|--------|-----------------|------|
| Reddit communities | How customers describe the problem in casual language | Search for complaints, frustration posts, "why doesn't X..." threads |
| Hacker News threads | More technical voice; strong signal on mental model mismatch | Search Show HN, Ask HN, and comment threads on product launches |
| Twitter / X threads | Condensed pain expression; see what gets retweeted | Search for power-user complaints and "hack" threads |
| LinkedIn posts | Professional framing; useful if B2B | Search pain + your domain keywords |
| Blog posts & tutorials | Authors often describe the problem they're solving in the intro | Look for "I struggled with X until..." patterns |
| Substack newsletters | Long-form frustration essays; often very quotable | Search Substack for your domain |
| Product reviews (G2, Capterra, App Store) | Users describe what they wish was different | Sort by 3-star reviews — they contain the most nuanced pain |
| Customer support tickets | Verbatim customer language under frustration | Work with your support team to identify recurring themes |
| Customer interviews | Gold standard, but requires scheduling | Use JTBD interview format; ask "tell me about the last time you..." |

---

## Research Questions to Answer

Work through these questions using your sources. Aim to collect at least 15–20 distinct customer quotes before synthesizing.

### Primary Questions

1. **What exact words do customers use to describe the problem?**
   - Collect verbatim quotes. Do not paraphrase yet.
   - Look for recurring vocabulary — specific words that appear across multiple sources are signals.

2. **What metaphors do customers reach for?**
   - Metaphors reveal the mental model. "It's like having a new employee every day" tells you more than "context doesn't persist."
   - Note: metaphors are often more emotionally true than literal descriptions.

3. **What do customers say they want?** (even if you suspect they're wrong about the solution)
   - Document stated desires separately from the underlying need.
   - Example: "I want a search bar" may mean "I can't find what I need."

4. **What frustration language appears?**
   - Words like "annoying," "broken," "finally," "why can't it just" — these signal unmet expectations.
   - Frustration language often points to where expectation and reality diverge.

5. **What is conspicuously absent from customer language?**
   - If customers never mention a capability you thought was central, that absence is data.

### Secondary Questions

6. **How do different customer segments describe the same problem differently?**
   - A beginner and an expert will use different language for the same pain. Capture both.

7. **What journey stage are customers at when they express this problem?**
   - First encounter? After months of use? Post-abandonment?
   - Stage context changes the interpretation of the pain.

8. **Are there recurring trigger events?**
   - "Every time I..." or "when I need to..." — these identify the specific moments the problem surfaces.

---

## Synthesis Prompts

After collecting your raw quotes and sources, use these to structure your Layer 1 synthesis document:

1. **What is the single most common customer-voiced problem?** (Use their language, not yours.)
2. **What are the top 3 recurring phrases or metaphors?**
3. **What is the emotional register?** (Frustrated? Resigned? Curious? Confused?)
4. **What does the customer think the solution should be?** (Even if you disagree.)
5. **What did you expect to find that wasn't there?**
6. **What surprised you most in the raw data?**

---

## Common Mistakes in Layer 1

**Interpreting too early**: Resist categorizing or synthesizing while collecting. Spend at least a full pass in pure listening mode.

**Selecting confirming quotes**: If all your quotes support your existing hypothesis, you've introduced bias. Actively seek disconfirming voices.

**Ignoring the lurkers**: On Reddit and Hacker News, sort by "top" to find what resonated with the silent majority — not just the loudest posters.

**Treating interview data as representative**: One interview is a story, not a pattern. Layer 1 needs sufficient breadth before synthesis.

---

## Output

Produce two documents:

1. **Raw research document** (e.g., `layer-1-reddit-research.md`, `layer-1-interview-notes.md`) — verbatim quotes, sources, links. No interpretation.
2. **Layer 1 synthesis** (use `templates/layer-synthesis-template.md`) — consolidated findings, key insight, strategic implication.

When writing files, the default output path is `docs/research/` in your current project. Claude will confirm the location with you before writing.
