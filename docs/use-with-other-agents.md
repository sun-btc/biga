# Use Biga with Other Agents

## Overview

Biga is plain Markdown. Any Agent that can read Markdown files can use it as a research instruction library.

## Setup

Clone the repository:

```bash
git clone https://github.com/sun-btc/biga.git
```

Provide the Agent with:

1. The top-level `SKILL.md` router.
2. The relevant strategy `SKILL.md` file.
3. Optional example files from `examples/`.

## Suggested routing logic

Use this mapping when your Agent needs to choose a strategy:

| User intent | Recommended Skill |
|---|---|
| Fundamental quality, valuation, cash flow, value traps | `biga-value-skill/SKILL.md` |
| Growth stocks, AI, semiconductors, new energy, innovation themes | `biga-growth-skill/SKILL.md` |
| Moving averages, breakouts, pullbacks, stop-loss discipline | `biga-trend-skill/SKILL.md` |
| Dividends, high-yield stocks, income strategy | `biga-dividend-skill/SKILL.md` |
| Commodity cycles, low PE traps, resource stocks | `biga-cyclical-skill/SKILL.md` |
| Policy themes, restructuring, hot concepts, event catalysts | `biga-event-skill/SKILL.md` |

## Agent instruction template

```text
Use Biga as an investment research framework.

Select the most relevant strategy Skill, then produce:
- research logic
- verification checklist
- risk factors
- failure conditions
- data to check next

Do not provide stock recommendations, trading signals, target prices, or return guarantees.
```

## Boundary note

Biga is intended for research structure and education. Users remain responsible for independent verification and decisions.
