# Six-Layer Product Research

A Claude Code skill that guides you through Teresa Torres' 6-Layer Problem Definition Framework for rigorous product research.

## What It Does

Executes a structured, six-layer research process that produces a multi-perspective problem definition before any solution work begins. Each layer examines the problem through a different lens:

1. **Customer Mental Models** - What customers say in their own words
2. **Ecosystem View** - How other actors interpret the problem
3. **Behavioral Dynamics** - Frictions, incentives, and habits blocking change
4. **Status Quo Attempts** - What has been tried and why it failed
5. **Technology Enablers** - What new capabilities make solutions possible
6. **Feasible Influence** - What you can realistically change

## Install

```bash
skillsmith install smith-horn/six-layer-product-research
```

Or copy to `~/.claude/skills/six-layer-product-research/`.

## Usage

```
/six-layer-product-research AI-powered code review tools
/six-layer-product-research developer onboarding --quick
```

Or use natural language: "run product research on [your domain]"

## Depth Modes

- **Quick** (~1-2 days/layer): 5-10 sources per layer, desk research only
- **Full** (~3-5 days/layer): 25-40+ sources per layer, primary research included

## Output

Per layer: raw research documents + structured synthesis.
After all layers: cross-layer convergence analysis, unified problem statement, solution direction.

## Project Structure

```
six-layer-product-research/
├── SKILL.md                                  # Skill entry point
├── README.md                                 # This file
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
    └── references.md
```

## Attribution

Framework by [Teresa Torres](https://www.producttalk.org/) (*Continuous Discovery Habits*, 2021). Behavioral frameworks include BJ Fogg (B=MAP), Fred Davis (TAM), and Everett Rogers (Diffusion of Innovations).

## License

MIT
