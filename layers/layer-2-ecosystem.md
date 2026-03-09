# Layer 2: Ecosystem View

**Framework**: Teresa Torres 6-Layer Problem Definition Framework — Layer 2
**Core Question**: "How do other actors interpret or feel the impact of this problem?"

---

## What This Layer Is For

Layer 1 captured your direct customer's voice. Layer 2 expands the frame to everyone else who is affected by — or has a stake in — the problem. This includes:

- Adjacent roles (not your primary user, but affected by them)
- Supply-side actors (people who create things your users consume)
- Intermediaries (platforms, marketplaces, distributors)
- Regulators, standards bodies, professional communities
- Competitors and alternatives (as ecosystem actors, not threats)

The purpose is to surface perspectives and power dynamics invisible from the customer's vantage point. Solutions that ignore ecosystem actors often fail — not because they're wrong about the customer, but because they misread the ecosystem.

> "Customers are not the only ones who feel the impact of a problem. Mapping the full ecosystem often reveals leverage points — and landmines — your direct customer interviews won't surface."
>
> — Teresa Torres, *Continuous Discovery Habits*

---

## Research Sources for This Layer

| Source | Who you'll find | What to look for |
|--------|----------------|-----------------|
| GitHub repository authors | Creators of tools your users use | Their pain points distributing and maintaining work |
| Developer forums (Dev.to, Hashnode) | Practitioners who write for peers | How they frame problems for their audience |
| Professional community newsletters | Industry observers | How the problem is framed at the ecosystem level |
| Marketplace/platform documentation | Platform operators | What problems they chose to solve (and didn't) |
| Conference talks (YouTube) | Thought leaders, practitioners | Ecosystem narratives; how they position the problem |
| LinkedIn influencer posts | Champions who advocate for solutions | Who evangelizes; what language drives adoption |
| Analyst reports (Gartner, Forrester) | Institutional interpretation | How the problem is categorized and sized |
| Competitor post-mortems | Failed alternatives | What ecosystem dynamics they misjudged |
| Job postings | Hiring organizations | What problems companies are paying to solve |

---

## Research Questions to Answer

### Actor Mapping

1. **Who are the actors in this ecosystem beyond your direct customer?**
   - List every category of person who creates, distributes, consumes, or regulates the thing your customer uses.
   - Include people your customer never interacts with directly.

2. **How does each actor *describe* the same problem?**
   - A creator describes the same problem differently than a consumer.
   - Document each actor's vocabulary and framing separately before synthesizing.

3. **Which actors benefit from the current problem persisting?**
   - Every problem has incumbents who profit from the status quo.
   - Identifying them is essential for understanding resistance later in Layer 6.

### Ecosystem Dynamics

4. **Where is fragmentation occurring?**
   - Are there multiple disconnected communities, platforms, or standards where there could be one?
   - Fragmentation is often the problem wearing a disguise.

5. **What are the biggest actor pain points that don't show up in customer interviews?**
   - Supply-side pain (e.g., creators who can't reach their audience) rarely surfaces in consumer research.
   - Ecosystem solutions often require solving supply-side problems first.

6. **Which actors have influence over your customer's behavior?**
   - Champions (people who advocate for tools to peers), gatekeepers (people who approve adoption), and influencers (people whose usage signals quality to others) all shape customer behavior without being the customer.

7. **What ecosystem norms govern acceptable solutions?**
   - Open source vs. commercial? Self-hosted vs. cloud? Community trust requirements?
   - Violating ecosystem norms can doom an otherwise valid solution.

### Power Dynamics

8. **Who has distribution power?**
   - Distribution is often more valuable than the product. Who controls discoverability in this ecosystem?

9. **What dependencies exist between actors?**
   - If your customer depends on a creator, and the creator depends on a platform, the platform has leverage over both.
   - Map these chains — they determine where influence is actually concentrated.

---

## Synthesis Prompts

After collecting ecosystem research, use these to structure your Layer 2 synthesis:

1. **Draw an actor map**: List every ecosystem actor and how they relate to the problem.
2. **What is the #1 pain for each major actor category?**
3. **Which actor's pain is most underserved by existing solutions?**
4. **What ecosystem dynamic is most likely to make a solution fail if ignored?**
5. **Who are the champions?** — the people who actively advocate for good solutions.
6. **What does ecosystem fragmentation look like, concretely?**

---

## Common Mistakes in Layer 2

**Stopping at direct users**: The ecosystem view requires deliberately going outside your usual research scope. If you're only talking to your existing customers, you're doing Layer 1 research with Layer 2 labels.

**Treating competitors as enemies rather than ecosystem actors**: Competitors reveal what the ecosystem was willing to pay for and what it rejected. Their failures are data.

**Missing supply-side pain**: Consumer-focused teams systematically underestimate creator/author/supply-side problems. These often unlock distribution solutions the demand side never would have reached.

**Ignoring champions**: The person who installs your product is often not the person who champions it internally. If you don't understand the champion persona, you'll optimize for the wrong adoption moment.

---

## Output

Produce two documents:

1. **Raw research document(s)** — one per actor category (e.g., `layer-2-creator-research.md`, `layer-2-platform-research.md`). Verbatim findings, links.
2. **Layer 2 synthesis** (use `templates/layer-synthesis-template.md`) — actor map, consolidated findings, key insight, strategic implication.

When writing files, the default output path is `docs/research/` in your current project. Claude will confirm the location with you before writing.
