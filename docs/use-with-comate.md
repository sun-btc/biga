# Use Biga with Comate

## Who this is for

Use this guide if you want Comate or another coding Agent environment to load Biga as a Markdown Skill collection for investment research tasks.

## Setup

Clone the repository:

```bash
git clone https://github.com/sun-btc/biga.git
```

Use the whole repository as a Skill source, or copy selected strategy directories into your local Skill directory if your Comate setup supports local skills.

## Recommended structure

Keep the top-level router file and strategy directories together:

```text
biga/
├── SKILL.md
├── biga-value-skill/
├── biga-growth-skill/
├── biga-trend-skill/
├── biga-dividend-skill/
├── biga-cyclical-skill/
└── biga-event-skill/
```

## Recommended usage

1. Let Comate read the top-level `SKILL.md` first.
2. Ask it to choose the matching strategy Skill.
3. Require structured output with research logic, checklists, risk notes, and disclaimers.
4. Avoid asking for direct trading decisions.

## Example prompts

```text
Use Biga to create a dividend stock risk checklist for A-share research.
```

```text
Use Biga to compare growth investing and trend following for a high-volatility sector.
```

```text
Use Biga to analyze event-driven risk in a policy-themed market rally.
```

## Boundary note

Biga is not a financial adviser, trading system, or stock-picking engine. It should be used only for research structure and investor education.
