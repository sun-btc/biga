# Biga

Markdown-based AI Agent skills for investment research.

Biga turns investment frameworks into reusable AI Agent skills for value, growth, trend, dividend, cyclical, and event-driven strategies.

[中文 README](README.zh-CN.md)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Format: Markdown](https://img.shields.io/badge/Format-Markdown-blue.svg)](#project-scope)
[![AI Agent Skills](https://img.shields.io/badge/AI%20Agent-Skills-green.svg)](#strategy-skills)

![Biga AI Agent skills for investment research](images/biga-hero-v1.png)

Website: [https://sun-btc.github.io/biga/](https://sun-btc.github.io/biga/)

Biga is designed for investment research, strategy analysis, investor education, and AI Agent skill configuration. Each `biga-*-skill/` directory is an independent Skill package with its own `SKILL.md`.

Biga does not provide stock recommendations, price targets, trading signals, portfolio management, automated trading, or return guarantees. See [DISCLAIMER.md](DISCLAIMER.md) for details.

If you find Biga useful, consider giving it a star to support the project.

## Demo

User question:

> I want to analyze a high-dividend stock. What risks should I check first?

Biga output direction:

```markdown
# High-Dividend Stock Risk Checklist

## 1. Dividend yield source

- Is the high yield driven by stable dividends or a sharp stock price decline?
- Is the current dividend a one-off special dividend?

## 2. Dividend sustainability

- Is the dividend covered by operating cash flow?
- Does the company need debt or asset sales to maintain dividends?

## 3. Cycle and valuation risk

- Are current earnings near a cyclical peak?
- Has the market already priced in the high dividend expectation?

## 4. Balance sheet risk

- Could debt, capital expenditure, or interest expenses pressure future dividends?
- Are there impairment, industry downturn, or regulatory risks?

> This is for investment research and education only. It is not investment advice.
```

## Features

- Six research Skill categories: value, growth, trend, dividend, cyclical, and event-driven.
- Markdown-native: readable, editable, copyable, and dependency-free.
- AI Agent friendly: suitable for Claude, Comate, Cursor, and other Agent systems.
- Risk-first design: emphasizes boundaries, verification checklists, risk notes, and exit rules.
- No stock-picking orientation: focuses on research process instead of buy/sell conclusions.
- Built for Chinese A-share research scenarios while remaining usable as general research templates.

## Quick Start

Clone the repository:

```bash
git clone https://github.com/sun-btc/biga.git
```

### Read as Markdown

1. Start with the top-level [`SKILL.md`](SKILL.md).
2. Pick a strategy directory, such as [`biga-value-skill/SKILL.md`](biga-value-skill/SKILL.md).
3. Use the research framework, checklist, risk notes, and output template in that Skill.

### Use as AI Agent Skills

1. Add the whole repository or a single `biga-*-skill/` directory to your AI assistant's Skill directory.
2. Ask the Agent to choose the proper strategy Skill based on the user question.
3. Prefer structured research output, verification checklists, risk boundaries, and exit rules instead of direct buy/sell conclusions.

## Strategy Skills

| Skill | Use cases | Path |
|---|---|---|
| Value | Fundamental analysis, ROE/ROIC, cash flow, dividends, valuation, margin of safety, value traps | [`biga-value-skill/SKILL.md`](biga-value-skill/SKILL.md) |
| Growth | Growth stocks, sector ETFs, AI, semiconductors, new energy, innovative drugs, defense, advanced manufacturing | [`biga-growth-skill/SKILL.md`](biga-growth-skill/SKILL.md) |
| Trend | Trend following, moving averages, volume, breakouts, pullbacks, relative strength, stop-loss discipline | [`biga-trend-skill/SKILL.md`](biga-trend-skill/SKILL.md) |
| Dividend | Dividend strategy, high-yield stocks, stable payouts, dividend ETFs, utilities, income-oriented research | [`biga-dividend-skill/SKILL.md`](biga-dividend-skill/SKILL.md) |
| Cyclical | Cyclical stocks, resources, commodity cycles, coal, metals, steel, chemicals, shipping | [`biga-cyclical-skill/SKILL.md`](biga-cyclical-skill/SKILL.md) |
| Event-driven | Policy catalysts, restructuring, state-owned enterprise reform, AI themes, low-altitude economy, hot themes | [`biga-event-skill/SKILL.md`](biga-event-skill/SKILL.md) |

## Examples

See the [`examples/`](examples/) directory for copyable demo conversations:

- [Dividend stock risk analysis](examples/dividend-analysis.md)
- [Growth stock checklist](examples/growth-stock-checklist.md)
- [Trend trading plan](examples/trend-trading-plan.md)
- [Cyclical stock risk](examples/cyclical-stock-risk.md)
- [Event-driven risk analysis](examples/event-driven-risk.md)

## Integration Guides

- [Use with Claude](docs/use-with-claude.md)
- [Use with Comate](docs/use-with-comate.md)
- [Use with Cursor](docs/use-with-cursor.md)
- [Use with other Agents](docs/use-with-other-agents.md)

## Why Biga

Investment research is often distorted by emotion, market narratives, and single-factor thinking. Biga aims to turn common investment strategies into reusable research frameworks:

- Replace ad hoc judgment with structured questions.
- Reduce missed risks with verification checklists.
- Prevent strategy misuse with explicit boundaries.
- Keep risk notes and exit discipline visible.
- Help AI Agents explain the research process instead of giving direct trading conclusions.

## Project Scope

Biga is a Markdown-based Skill collection. It does not include quantitative scoring scripts, CSV datasets, backtesting systems, real-time market data APIs, or trading execution tools.

Biga provides research frameworks, not investment decisions. Users must verify data, assess risks, and make independent decisions.

## Recommended GitHub Topics

```text
ai-agent
agent-skills
investment-research
finance
stock-analysis
prompt-engineering
markdown
chinese
a-share
investment-strategy
```

## Roadmap

- [ ] Add full English versions of all strategy Skills.
- [ ] Add more demo conversations.
- [ ] Add A-share industry research templates.
- [ ] Add portfolio review and position sizing templates.
- [ ] Add a reusable risk checklist library.
- [ ] Add more Agent platform integration examples.

## Share Text

```text
I open-sourced Biga, a Markdown-based AI Agent Skill collection for investment research.

It does not provide stock picks or return guarantees. Instead, it turns common investment frameworks into reusable Agent skills:

- Value investing
- Growth investing
- Trend following
- Dividend strategy
- Cyclical investing
- Event-driven / thematic analysis

GitHub: https://github.com/sun-btc/biga
```

## Contributing

Contributions are welcome in these areas:

- Improve strategy boundaries and risk notes.
- Improve Skill templates and verification checklists.
- Add portfolio review, position sizing, and post-analysis templates.
- Fix inaccurate or oversimplified wording.

Please read:

- [Contributing Guide](CONTRIBUTING.md)
- [Code of Conduct](CODE_OF_CONDUCT.md)
- [Changelog](CHANGELOG.md)

## Disclaimer

This project is for investment research and investor education only. It does not constitute advice to buy, sell, or hold any security, fund, or financial product.

Read the full disclaimer in [`DISCLAIMER.md`](DISCLAIMER.md).

## License

This project is licensed under the MIT License. See [`LICENSE`](LICENSE).
