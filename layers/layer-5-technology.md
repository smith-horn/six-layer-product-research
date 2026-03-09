# Layer 5: Technology Enablers

**Framework**: Teresa Torres 6-Layer Problem Definition Framework — Layer 5
**Core Question**: "Where does product or technology create new possibilities?"

---

## What This Layer Is For

Layers 1–4 described the problem from the human side — customer voice, ecosystem dynamics, behavioral forces, and the graveyard of prior attempts. Layer 5 asks a different question: **what has changed technically that makes a new class of solution possible now?**

This is not a technology exploration exercise. It is a constraint-calibration exercise. The goal is to identify:
- What is technically feasible today that wasn't 2–3 years ago
- Which technical capabilities align with the user needs surfaced in Layers 1–3
- Which technical capabilities could eliminate the failure modes found in Layer 4

Layer 5 answers the question: *Why might this problem be solvable now, when it wasn't before?*

---

## Why Layer 5 Comes After the Human Layers

Teams that start with technology often build solutions in search of problems. By running Layers 1–4 first, you have:
- A clear problem in customer language (Layer 1)
- A map of ecosystem actors and their pain (Layer 2)
- A behavioral model of why the problem persists (Layer 3)
- A catalog of what has already been tried and why it failed (Layer 4)

Layer 5 research is then filtered through this lens: *Does this technical capability address the specific blockers we found?* If a technology is impressive but doesn't address a documented human need, it doesn't belong in this layer.

---

## Categories of Technology Enablers to Investigate

### Infrastructure Shifts

New infrastructure that reduces the cost of building or delivering a solution:

- What has become dramatically cheaper or faster in the last 2–3 years?
- What infrastructure previously required significant engineering investment that is now commodity?
- What developer platforms or protocols have emerged that enable new integration patterns?

Examples to investigate for your domain:
- New API standards (e.g., MCP for AI tools, OpenAPI adoption, etc.)
- Edge computing and reduced latency for previously server-only operations
- Serverless and reduced operational overhead
- New embedding and vector search capabilities
- Protocol-level changes (new authentication standards, webhook standards)

### UX/Interaction Paradigm Shifts

New interaction patterns that reduce friction in ways previously impossible:

- What interaction patterns have been normalized by high-adoption products that you can leverage?
- Where has the bar for "zero-friction onboarding" shifted?
- What do users now expect to work without configuration that previously required setup?

### Quality Signal Technologies

Technical capabilities that address trust or quality verification problems:

- Automated quality scoring systems
- Reputation and provenance tracking
- Sandboxed execution for safe trials
- Versioning and diff capabilities

### Discovery and Recommendation Technologies

Technical capabilities that address invisibility or discoverability problems:

- Semantic search vs. keyword search
- Contextual recommendation (based on current task, not just history)
- Ambient/passive discovery vs. active search
- Federated index aggregation from multiple sources

---

## Research Questions to Answer

### Feasibility Assessment

1. **What technical capabilities exist today that directly address the behavioral blockers from Layer 3?**
   - Be specific. "AI" is not an answer. "Contextual recommendation that triggers at the right workflow moment without user initiation" is an answer.

2. **What technical capabilities existed when the abandoned solutions in Layer 4 were built — but don't exist now?**
   - Some prior failures weren't failures of idea; they were failures of timing. Technology catches up.

3. **What capabilities are emerging (not yet production-ready) that might be ready in 12–18 months?**
   - Note these separately from production-ready capabilities. They inform the roadmap, not the MVP.

### Alignment with Human Layers

4. **Which technical capability most directly reduces the friction identified in Layer 3?**
   - Map each significant technical capability to a specific friction.
   - Discard technical capabilities that don't map to a documented friction.

5. **Which technical capability could eliminate a repeated failure mode from Layer 4?**
   - Example: if curation burnout killed prior solutions, automated quality scoring is the technical answer.
   - If cold start killed them, federated aggregation across existing sources is the answer.

### Ecosystem Technical Assessment

6. **What technical standards are forming in the ecosystem?**
   - Standards that form early become locked in. Positioning relative to an emerging standard is strategic.
   - Is there a protocol or format that all actors in Layer 2 are converging on?

7. **What technical integrations would existing ecosystem actors want most?**
   - From Layer 2, you know who the ecosystem actors are and what they want.
   - Which technical integrations address their pain directly?

8. **What technical capabilities would violate ecosystem norms if used?**
   - Not all technically feasible approaches are acceptable to the ecosystem.
   - Identify approaches that are possible but would create trust problems.

### Build vs. Integrate Assessment

9. **For each key technical capability: build, integrate, or rely on platform?**
   - Building: required only when off-the-shelf doesn't exist or when the capability is core differentiation
   - Integrating: most technical enablers should be integration, not build
   - Platform reliance: acceptable when the platform is stable and aligned with your interests

10. **What is the minimum viable technical stack that enables the core value proposition?**
    - Start minimal. Document what can be deferred.

---

## Synthesis Prompts

1. **What is the single most important technical capability that makes a solution possible now that wasn't before?** (One sentence.)
2. **Map each Layer 3 behavioral blocker to a technical enabler.** If a blocker has no technical answer, flag it as requiring a non-technical intervention.
3. **Which Layer 4 failure mode does technology now make avoidable?** (And which failure modes remain structural?)
4. **What technical standards are forming that you must align with?** (Falling outside an emerging standard = ecosystem exclusion.)
5. **What is the smallest technical footprint that proves the core thesis?**

---

## Common Mistakes in Layer 5

**Technology-first framing**: If you find yourself excited about a technology and then looking for a problem it solves, you've inverted the framework. Layer 5 research is filtered through Layers 1–4 needs, not the other way around.

**Over-weighting emerging capabilities**: Distinguish production-ready from emerging. Roadmaps built on emerging capabilities frequently slip 12–24 months.

**Ignoring ecosystem standards**: A technically superior approach that violates forming standards will lose to a technically inferior approach that aligns with them. Standards have network effects.

**Building what should be integrated**: The instinct to build everything is especially strong in technical teams. Most technical enablers should be integrations.

---

## Output

Produce two documents:

1. **Raw research document** (`layer-5-technical-capabilities.md`) — each technical capability, sources, feasibility assessment, alignment to Layers 1–4.
2. **Layer 5 synthesis** (use `templates/layer-synthesis-template.md`) — capability map, Layer 3 friction → technical answer alignment table, strategic technical bets.

When writing files, the default output path is `docs/research/` in your current project. Claude will confirm the location with you before writing.
