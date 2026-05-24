# Biga

AI Agent 投资研究策略 Skill 集合。

> 把价值投资、成长投资、趋势投资、股息策略、周期投资、事件驱动等研究框架，整理成可直接接入 AI Agent 的 Markdown Skill。

[English README](README.md)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Format: Markdown](https://img.shields.io/badge/Format-Markdown-blue.svg)](#项目定位)
[![AI Agent Skills](https://img.shields.io/badge/AI%20Agent-Skills-green.svg)](#策略-skill)

![Biga AI Agent 投资研究策略 Skill 集合](images/biga-hero-v1.png)

项目主页：[https://sun-btc.github.io/biga/](https://sun-btc.github.io/biga/)

Biga 面向 A 股投资研究、策略分析、投资者教育和 AI Agent 能力配置场景。项目中的每个 `biga-*-skill/` 目录都是一个独立 Skill 包，包含对应策略的 `SKILL.md`，用于输出研究框架、核验清单、风险提示和分析模板。

Biga 不提供荐股、喊单、目标价、收益承诺或自动交易能力。完整边界请阅读 [免责声明](DISCLAIMER.md)。

如果你觉得 Biga 有用，欢迎 Star 支持项目。

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

## 快速开始

克隆仓库：

```bash
git clone https://github.com/sun-btc/biga.git
```

### 作为文档阅读

1. 先阅读顶层 [`SKILL.md`](SKILL.md)，判断问题属于哪类策略场景。
2. 进入对应策略目录，例如 [`biga-value-skill/SKILL.md`](biga-value-skill/SKILL.md)。
3. 按 Skill 文档中的研究框架、核验清单和风险提示进行分析。

### 作为 AI Agent / Skill 使用

1. 将整个仓库或单个 `biga-*-skill/` 目录加入 AI 编程助手或 Agent 的 Skill 目录。
2. 让 Agent 根据用户问题选择对应策略 Skill。
3. 输出时优先使用研究框架、核验清单、风险提示和退出纪律，而不是直接给买卖结论。

### 示例

查看 [`examples/`](examples/) 目录中的可复制示例：

- [高股息风险分析](examples/dividend-analysis.md)
- [成长股筛选清单](examples/growth-stock-checklist.md)
- [趋势交易计划](examples/trend-trading-plan.md)
- [周期股风险分析](examples/cyclical-stock-risk.md)
- [事件驱动风险分析](examples/event-driven-risk.md)

### 接入指南

- [Claude 使用指南](docs/use-with-claude.md)
- [Comate 使用指南](docs/use-with-comate.md)
- [Cursor 使用指南](docs/use-with-cursor.md)
- [通用 Agent 使用指南](docs/use-with-other-agents.md)

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

## 项目定位

本项目当前定位为 Markdown 文档型 Skill 集合，不包含量化评分脚本、CSV 数据产物、回测系统、实时行情接口或运行环境依赖。

Biga 提供的是投资研究框架，不是投资决策系统。涉及具体资产时，应由使用者自行核验数据、评估风险并独立决策。

## Roadmap

- [ ] 增加英文版 Skill 文档。
- [ ] 增加更多 Demo 对话。
- [ ] 增加 A 股行业研究模板。
- [ ] 增加组合复盘和仓位管理模板。
- [ ] 增加风险清单库。
- [ ] 增加不同 Agent 平台的接入示例。

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

完整说明见 [`DISCLAIMER.md`](DISCLAIMER.md)。

## License

本项目使用 MIT License，详见 [`LICENSE`](LICENSE)。
