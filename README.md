# Biga 投资研究策略 Skill 集合

> 把投资分析框架，变成 AI Agent 可复用的 Skill。
>
> Turn investment frameworks into reusable AI Agent skills.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Format: Markdown](https://img.shields.io/badge/Format-Markdown-blue.svg)](#项目定位)
[![AI Agent Skills](https://img.shields.io/badge/AI%20Agent-Skills-green.svg)](#策略-skill)

Biga 是一个按策略维度组织的投资研究 Skill 文档集合，面向 A 股投资研究、策略分析、投资者教育和 AI Agent 能力配置场景。

项目中的每个 `biga-*-skill/` 目录都是一个独立 Skill 包，包含对应策略的 `SKILL.md`，用于输出研究框架、核验清单、风险提示和分析模板。Biga 不提供荐股、收益承诺或自动交易能力。

## 快速开始

1. 先阅读顶层 [`SKILL.md`](SKILL.md)，判断问题属于哪类策略场景。
2. 进入对应策略目录，例如 [`biga-value-skill/SKILL.md`](biga-value-skill/SKILL.md)。
3. 按 Skill 文档中的研究框架、核验清单和风险提示进行分析。
4. 如作为 AI Agent Skill 使用，将整个仓库或单个 `biga-*-skill/` 目录加入助手的 Skill 目录。

## 为什么需要 Biga

投资研究容易受到情绪、热点和单一指标影响。Biga 的目标不是给出确定性结论，而是把常见投资策略沉淀为可复用的分析框架：

- 用结构化问题替代临时判断。
- 用核验清单降低遗漏关键风险的概率。
- 用适用边界约束策略误用。
- 用风险提示和退出纪律避免只看收益、不看回撤。
- 让 AI Agent 输出研究过程，而不是直接给买卖结论。

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

## 策略 Skill

| Skill | 适用场景 | 路径 |
|---|---|---|
| Value | 价值投资、公司基本面、ROE/ROIC、现金流、分红、估值、安全边际、价值陷阱 | [`biga-value-skill/SKILL.md`](biga-value-skill/SKILL.md) |
| Growth | 成长投资、成长股、行业 ETF、AI、半导体、新能源、创新药、军工、高端制造 | [`biga-growth-skill/SKILL.md`](biga-growth-skill/SKILL.md) |
| Trend | 趋势投资、趋势交易、均线、成交量、突破、回踩、相对强弱、止损纪律 | [`biga-trend-skill/SKILL.md`](biga-trend-skill/SKILL.md) |
| Dividend | 股息策略、红利、高股息、稳定分红、收息、红利 ETF、公用事业分红 | [`biga-dividend-skill/SKILL.md`](biga-dividend-skill/SKILL.md) |
| Cyclical | 周期投资、周期股、资源股、商品周期、煤炭、有色、钢铁、化工、航运 | [`biga-cyclical-skill/SKILL.md`](biga-cyclical-skill/SKILL.md) |
| Event-driven | 事件驱动、主题投资、政策利好、并购重组、国企改革、AI 概念、低空经济 | [`biga-event-skill/SKILL.md`](biga-event-skill/SKILL.md) |

## 适合谁使用

- 希望用结构化框架分析 A 股投资策略的人。
- 希望为 AI Agent、Comate、Claude 或其他助手配置投资研究 Skill 的用户。
- 希望沉淀价值、成长、趋势、股息、周期、事件主题等策略分析模板的人。
- 希望用清单化方式做投资研究、复盘和风险核验的人。

## 不适合什么场景

- 不适合用作股票推荐、荐股、喊单或自动交易工具。
- 不适合直接替代财务审计、投顾服务或专业投资决策。
- 不适合输出“必涨”“稳赚”“满仓”等确定性结论。
- 不适合在缺少数据核验和风险评估的情况下直接做买卖决策。

## 使用方式

### 作为文档阅读

1. 先阅读顶层 [`SKILL.md`](SKILL.md)，判断问题属于哪类策略场景。
2. 进入对应的 `biga-*-skill/SKILL.md`。
3. 按该策略文档中的框架进行分析、核验和复盘。

### 作为 AI Agent / Skill 使用

1. 将整个仓库或单个 `biga-*-skill/` 目录加入 AI 编程助手或 Agent 的 Skill 目录。
2. 让 Agent 根据用户问题选择对应策略 Skill。
3. 输出时优先使用研究框架、核验清单、风险提示和退出纪律，而不是直接给买卖结论。

## 设计原则

- 研究框架优先：输出可复用分析路径，而不是一次性结论。
- 风险提示优先：任何策略都需要说明适用边界、失效条件和回撤风险。
- 证据核验优先：避免基于传闻、单一指标或未经核验数据做判断。
- 非荐股导向：不提供具体买卖建议、收益承诺或仓位指令。
- 文档简单优先：当前保持 Markdown Skill 集合定位，不引入不必要的运行环境依赖。

## 项目定位

本项目当前定位为 Markdown 文档型 Skill 集合，不包含量化评分脚本、CSV 数据产物、回测系统、实时行情接口或运行环境依赖。

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
