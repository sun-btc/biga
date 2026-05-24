# Biga

Markdown-based AI Agent skills for investment research.

Biga turns investment frameworks into reusable AI Agent skills for value, growth, trend, dividend, cyclical, and event-driven strategies.

中文：Biga 是一个 AI Agent 投资研究策略 Skill 集合，把价值投资、成长投资、趋势投资、股息策略、周期投资、事件驱动等研究框架，整理成可直接接入 AI Agent 的 Markdown Skill。

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Format: Markdown](https://img.shields.io/badge/Format-Markdown-blue.svg)](#项目定位)
[![AI Agent Skills](https://img.shields.io/badge/AI%20Agent-Skills-green.svg)](#策略-skill)

Biga is designed for investment research, strategy analysis, investor education, and AI Agent skill configuration. Each `biga-*-skill/` directory is an independent Skill package with its own `SKILL.md`.

Biga 不提供荐股、喊单、目标价、收益承诺或自动交易能力。

If you find Biga useful, consider giving it a star to support the project.

## Demo

用户输入：

> 我想分析一只高股息股票，应该看哪些风险？

Biga 输出方向：

```markdown
# 高股息股票风险核验

## 1. 股息率来源

- 股息率是来自稳定分红，还是来自股价大幅下跌。
- 当前分红是否属于一次性高分红。

## 2. 分红可持续性

- 分红是否被经营现金流覆盖。
- 公司是否需要依靠举债或出售资产维持分红。

## 3. 周期和估值风险

- 当前利润是否处于周期高景气阶段。
- 高股息是否已经被市场充分定价。

## 4. 资产负债表风险

- 负债、资本开支和利息支出是否挤压未来分红。
- 是否存在减值、行业下行或监管变化风险。

> 以上内容仅用于投资研究和教育，不构成投资建议。
```

## Features

- 六类投资研究 Skill：价值、成长、趋势、股息、周期、事件驱动。
- Markdown 原生：可读、可改、可复制，不依赖运行环境。
- AI Agent 友好：适合接入 Comate、Claude、Cursor 或其他 Agent。
- 风险优先：默认输出适用边界、风险提示、核验清单和退出条件。
- 非荐股导向：强调研究过程，不直接给买卖结论或收益承诺。
- 面向中文投资研究：覆盖 A 股常见策略、行业主题和投资者教育场景。

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

### Examples

See the [`examples/`](examples/) directory for copyable demo conversations:

- [Dividend stock risk analysis](examples/dividend-analysis.md)
- [Growth stock checklist](examples/growth-stock-checklist.md)
- [Trend trading plan](examples/trend-trading-plan.md)
- [Cyclical stock risk](examples/cyclical-stock-risk.md)
- [Event-driven risk analysis](examples/event-driven-risk.md)

## 策略 Skill

| Skill | 适用场景 | 路径 |
|---|---|---|
| Value | 价值投资、公司基本面、ROE/ROIC、现金流、分红、估值、安全边际、价值陷阱 | [`biga-value-skill/SKILL.md`](biga-value-skill/SKILL.md) |
| Growth | 成长投资、成长股、行业 ETF、AI、半导体、新能源、创新药、军工、高端制造 | [`biga-growth-skill/SKILL.md`](biga-growth-skill/SKILL.md) |
| Trend | 趋势投资、趋势交易、均线、成交量、突破、回踩、相对强弱、止损纪律 | [`biga-trend-skill/SKILL.md`](biga-trend-skill/SKILL.md) |
| Dividend | 股息策略、红利、高股息、稳定分红、收息、红利 ETF、公用事业分红 | [`biga-dividend-skill/SKILL.md`](biga-dividend-skill/SKILL.md) |
| Cyclical | 周期投资、周期股、资源股、商品周期、煤炭、有色、钢铁、化工、航运 | [`biga-cyclical-skill/SKILL.md`](biga-cyclical-skill/SKILL.md) |
| Event-driven | 事件驱动、主题投资、政策利好、并购重组、国企改革、AI 概念、低空经济 | [`biga-event-skill/SKILL.md`](biga-event-skill/SKILL.md) |

## 为什么需要 Biga

投资研究容易受到情绪、热点和单一指标影响。Biga 的目标不是给出确定性结论，而是把常见投资策略沉淀为可复用的分析框架：

- 用结构化问题替代临时判断。
- 用核验清单降低遗漏关键风险的概率。
- 用适用边界约束策略误用。
- 用风险提示和退出纪律避免只看收益、不看回撤。
- 让 AI Agent 输出研究过程，而不是直接给买卖结论。

## 适合谁使用

- 希望用结构化框架分析 A 股投资策略的人。
- 希望为 AI Agent、Comate、Claude、Cursor 或其他助手配置投资研究 Skill 的用户。
- 希望沉淀价值、成长、趋势、股息、周期、事件主题等策略分析模板的人。
- 希望用清单化方式做投资研究、复盘和风险核验的人。

## 不适合什么场景

- 不适合用作股票推荐、荐股、喊单或自动交易工具。
- 不适合直接替代财务审计、投顾服务或专业投资决策。
- 不适合输出“必涨”“稳赚”“满仓”等确定性结论。
- 不适合在缺少数据核验和风险评估的情况下直接做买卖决策。

## 目录结构

```text
biga/
├── SKILL.md
├── LICENSE
├── README.md
├── CONTRIBUTING.md
├── CODE_OF_CONDUCT.md
├── CHANGELOG.md
├── biga-value-skill/
│   └── SKILL.md
├── biga-growth-skill/
│   └── SKILL.md
├── biga-trend-skill/
│   └── SKILL.md
├── biga-dividend-skill/
│   └── SKILL.md
├── biga-cyclical-skill/
│   └── SKILL.md
└── biga-event-skill/
    └── SKILL.md
```

## 项目定位

本项目当前定位为 Markdown 文档型 Skill 集合，不包含量化评分脚本、CSV 数据产物、回测系统、实时行情接口或运行环境依赖。

Biga 提供的是投资研究框架，不是投资决策系统。涉及具体资产时，应由使用者自行核验数据、评估风险并独立决策。

## English Summary

Biga is a collection of Markdown-based AI Agent Skills for investment research.

It provides reusable frameworks for value investing, growth investing, trend following, dividend strategy, cyclical investing, and event-driven analysis, with a focus on Chinese A-share research scenarios.

Biga does not provide stock recommendations, price targets, trading signals, portfolio management, or return guarantees.

## 推荐 GitHub Topics

如果你 fork 或维护类似项目，可以在 GitHub 仓库右侧 About 区域添加这些 topics：

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

- [ ] 增加英文版 Skill 文档。
- [ ] 增加更多 Demo 对话。
- [ ] 增加 A 股行业研究模板。
- [ ] 增加组合复盘和仓位管理模板。
- [ ] 增加风险清单库。
- [ ] 增加不同 Agent 平台的接入示例。

## 分享文案

```text
我开源了一个 AI Agent 投资研究策略 Skill 集合：Biga。

它不是荐股工具，也不承诺收益，而是把常见投资研究方法整理成可复用的 Markdown Skill：

- 价值投资
- 成长投资
- 趋势投资
- 股息策略
- 周期投资
- 事件驱动 / 主题投资

适合接入 Claude、Comate、Cursor 或其他 Agent，用来输出结构化分析框架、核验清单、风险提示和复盘模板。

GitHub: https://github.com/sun-btc/biga
```

## 贡献方式

欢迎围绕以下方向改进：

- 补充策略适用边界和风险提示。
- 优化各策略 Skill 的分析模板和核验清单。
- 增加组合研究、复盘框架和仓位管理模板。
- 修正文档中的不准确表述或过度简化内容。

提交贡献前请阅读：

- [贡献指南](CONTRIBUTING.md)
- [社区行为准则](CODE_OF_CONDUCT.md)
- [版本变更记录](CHANGELOG.md)

## 免责声明

本项目内容仅用于投资研究和投资者教育，不构成任何证券、基金或其他金融产品的买入、卖出或持有建议。本项目不提供荐股、喊单、代客理财、自动交易或任何形式的收益承诺。

任何投资决策都应由使用者基于自身风险承受能力、资金情况、投资期限和独立判断审慎做出。项目维护者不保证内容的准确性、完整性、及时性或适用于任何特定投资目标，也不承担因使用本项目内容产生的投资损失或其他后果。

## License

本项目使用 MIT License，详见 [`LICENSE`](LICENSE)。
