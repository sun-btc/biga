# Use Biga with Claude

## Who this is for

Use this guide if you want Claude to apply Biga's investment research frameworks as reusable Markdown instructions.

## Setup

Clone the repository:

```bash
git clone https://github.com/sun-btc/biga.git
```

Then make the repository or a selected `biga-*-skill/` directory available to Claude as project context or a reusable skill directory, depending on your Claude environment.

## Recommended usage

1. Add the top-level `SKILL.md` so Claude can route questions to the correct strategy.
2. Add one or more strategy directories, such as `biga-dividend-skill/` or `biga-growth-skill/`.
3. Ask Claude to follow the selected Skill and output structured research, verification steps, and risk boundaries.

## Example prompts

```text
Use Biga to analyze the risks of a high-dividend stock. Do not recommend whether to buy or sell.
```

```text
Use Biga's growth investing skill to build a checklist for evaluating an AI-related A-share company.
```

```text
Use Biga's cyclical investing skill to explain why low PE can be a trap in commodity stocks.
```

## Output expectations

Claude should provide:

- A research framework.
- Verification questions.
- Risk factors.
- Boundary conditions.
- Follow-up data to check.

Claude should not provide:

- Stock recommendations.
- Target prices.
- Buy or sell instructions.
- Return guarantees.
- Automated trading decisions.

## Boundary note

Biga is for investment research and investor education only. It is not investment advice.
