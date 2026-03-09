# Six-Layer Product Research

A Claude Code skill that guides you through Teresa Torres' 6-Layer Problem Definition Framework for rigorous product research.

![6-Layer Problem Definition Framework](https://res.cloudinary.com/diqcbcmaq/image/upload/f_auto,q_auto,w_1200/blog/six-layer-product-research/framework-layers)

## What It Does

Executes a structured, six-layer research process that produces a multi-perspective problem definition before any solution work begins. Each layer examines the problem through a different lens:

1. **Customer Mental Models** - What customers say in their own words
2. **Ecosystem View** - How other actors interpret the problem
3. **Behavioral Dynamics** - Frictions, incentives, and habits blocking change
4. **Status Quo Attempts** - What has been tried and why it failed
5. **Technology Enablers** - What new capabilities make solutions possible
6. **Feasible Influence** - What you can realistically change

The framework deliberately separates these perspectives. Running all six before considering solutions produces a problem definition robust enough to survive contact with reality.

## Install

### Via Skillsmith (recommended)

```bash
skillsmith install smith-horn/six-layer-product-research
```

### Via Git (no dependencies)

```bash
git clone https://github.com/smith-horn/six-layer-product-research.git ~/.claude/skills/six-layer-product-research
```

### Manual Download

Download the [latest release](https://github.com/smith-horn/six-layer-product-research/releases/latest) and extract to `~/.claude/skills/six-layer-product-research/`.

After installing by any method, restart Claude Code. The skill will be available as `/six-layer-product-research`.

## Usage

### Quick Start

```
/six-layer-product-research AI-powered code review tools
/six-layer-product-research developer onboarding --quick
```

Or use natural language: "run product research on [your domain]"

### First-Time Walkthrough

If this is your first time running the framework, here's what to expect:

1. **Setup prompt** — Claude will ask you three things:
   - What product or problem domain you're researching
   - Whether you want Quick mode (desk research, 5-10 sources/layer) or Full mode (primary research, 25-40+ sources/layer)
   - Where to save output files (defaults to `docs/research/` in your project)

2. **Layer-by-layer execution** — Claude works through each layer in order, using WebSearch and WebFetch to gather evidence. After each layer, you'll see key findings and a synthesis before moving to the next. You can pause between layers, ask follow-up questions, or redirect the research.

3. **Cross-layer synthesis** — After all six layers are complete, Claude produces a unified problem statement, a solution direction, and a convergence analysis showing patterns that appeared across multiple layers.

4. **Review** — Claude presents the final output and asks whether the findings match your intuition, what surprised you, and whether you'd adjust scope boundaries.

**A realistic first run takes 2-4 hours in Quick mode** (one session or split across days). Full mode is substantially longer and typically runs across multiple sessions.

### Choosing a Depth Mode

| | Quick Mode | Full Mode |
|---|---|---|
| **Sources per layer** | 5-10 | 25-40+ |
| **Research type** | Desk research (web, forums, existing data) | Primary research (interviews, academic lit, deep analysis) |
| **Time per layer** | 1-2 days | 3-5 days |
| **Best for** | Repositioning, layer updates, time-boxed exploration | New product from scratch, major strategic pivot |
| **Output depth** | Consolidated findings with key quotes | Detailed research docs with comprehensive evidence |

**Recommendation**: Start with Quick mode. If the findings surface questions that need deeper investigation, you can re-run specific layers in Full mode without redoing the entire framework.

### Running Individual Layers

You don't always need all six layers. The skill supports selective execution:

- **Layers 1-3 are fresh, but the market shifted** — Re-run Layer 4 (Status Quo) and Layer 5 (Technology Enablers) to update your competitive and technical landscape.
- **Strategy is drifting from reality** — Re-run Layer 6 (Feasible Influence) to recalibrate scope.
- **New technology emerged** — Re-run Layer 5 to assess whether it changes your technical thesis, then Layer 6 to re-scope.

Ask Claude: "run layer 5 only for [domain]" or "update the technology enablers analysis."

### Tips for Better Results

**Provide context upfront.** The more Claude knows about your product, customers, and market position before starting, the more targeted the research will be. Share existing docs, personas, or hypotheses.

**Push back on Layer 1.** The most common mistake is confirming your existing hypothesis instead of listening for what customers actually say. If all the findings align perfectly with what you already believed, tell Claude to look harder for disconfirming evidence.

**Don't skip Layer 4.** Teams consistently undervalue the graveyard of prior attempts. Understanding why previous solutions failed is often more valuable than understanding the problem itself. Every domain has abandoned tools, burned-out maintainers, and workarounds that reveal the shape of what users actually need.

**Layer 3 is the hardest.** Behavioral dynamics require going beyond what people say and examining invisible forces — cognitive load, social norms, status quo bias. If Claude's Layer 3 output reads like a communication problem ("users need better docs"), push for deeper behavioral analysis using the Fogg, TAM, and Rogers frameworks included in the skill.

**Save output incrementally.** Each layer produces standalone documents. If your session is interrupted, completed layers are preserved and you can resume from where you left off.

## Output Artifacts

For each layer, the skill produces two documents:

| Document | Contents |
|----------|----------|
| Raw research | Verbatim quotes, data points, source URLs — no interpretation |
| Layer synthesis | Consolidated findings, key insight, strategic implication (uses structured template) |

After all six layers:

| Document | Contents |
|----------|----------|
| Cross-layer synthesis | Convergences across 3+ layers, tensions between layers, unified barriers |
| Problem statement | One paragraph grounded in all six lenses |
| Solution direction | What the research points toward (a direction, not a spec) |
| Source index | All sources cited, organized by layer |

Total output: 14-20 documents depending on depth mode.

### What Comes After

The 6-Layer framework produces the *opportunity* side of Teresa Torres' Opportunity Solution Tree. After completing it you have a rigorous problem definition, a map of behavioral barriers, an understanding of what has been tried, and a scoped view of what's feasibly changeable.

The next step (outside this skill's scope) is building the Opportunity Solution Tree — mapping opportunities to potential solutions, then assumption-mapping and running structured experiments.

## Behavioral Science Frameworks

Layer 3 (Behavioral Dynamics) draws on three established frameworks, all documented with application guidance in `resources/references.md`:

| Framework | Author | Key Concept |
|-----------|--------|-------------|
| **Behavior Model (B=MAP)** | BJ Fogg | Behavior requires Motivation + Ability + Prompt simultaneously |
| **Technology Acceptance Model** | Fred Davis | Perceived Usefulness and Perceived Ease of Use drive adoption |
| **Diffusion of Innovations** | Everett Rogers | Five attributes predict adoption speed; the "chasm" between early adopters and early majority |

These aren't academic decoration — each framework provides a specific diagnostic lens. If adoption is failing, the Fogg model identifies *which* component is missing. TAM distinguishes value perception problems from friction problems. Rogers identifies where you are on the adoption curve and which attribute is the bottleneck.

## Project Structure

```
six-layer-product-research/
├── SKILL.md                                  # Skill entry point
├── README.md                                 # This file
├── CHANGELOG.md                              # Version history
├── LICENSE                                   # MIT
├── layers/                                   # Per-layer research guides
│   ├── layer-1-mental-models.md
│   ├── layer-2-ecosystem.md
│   ├── layer-3-behavioral.md
│   ├── layer-4-status-quo.md
│   ├── layer-5-technology.md
│   └── layer-6-feasibility.md
├── templates/                                # Output templates
│   ├── layer-synthesis-template.md
│   └── cross-layer-synthesis-template.md
└── resources/                                # Framework docs & references
    ├── framework.md
    ├── references.md
    └── framework-layers.png
```

## Attribution

Framework by [Teresa Torres](https://www.producttalk.org/) (*Continuous Discovery Habits*, 2021). Behavioral frameworks include BJ Fogg (B=MAP), Fred Davis (TAM), and Everett Rogers (Diffusion of Innovations).

## License

MIT
