# Use Biga with Cursor

## Who this is for

Use this guide if you want Cursor to reference Biga's Markdown files while drafting research templates, checklists, or Agent instructions.

## Setup

Clone the repository:

```bash
git clone https://github.com/sun-btc/biga.git
```

Open the cloned repository in Cursor, or add the relevant Markdown files to your working context.

## Recommended usage

1. Open `SKILL.md` to understand strategy routing.
2. Open a specific strategy file, such as `biga-trend-skill/SKILL.md`.
3. Ask Cursor to generate structured research output based on that file.
4. Use the `examples/` directory as reference output style.

## Example prompts

```text
Based on biga-trend-skill/SKILL.md, draft a trend trading plan template with risk controls.
```

```text
Based on biga-growth-skill/SKILL.md, create a checklist for evaluating growth quality.
```

```text
Based on examples/cyclical-stock-risk.md, explain why low PE may be misleading in cyclical stocks.
```

## Output expectations

Cursor should preserve Biga's risk-first structure:

- Research context.
- Verification checklist.
- Failure conditions.
- Risk controls.
- Disclaimer.

## Boundary note

Do not use Biga to generate direct buy, sell, hold, target price, or return-guarantee statements.
