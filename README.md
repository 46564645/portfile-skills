# Portfolio Layout Coach | 作品集排版辅导 Skill

`portfolio-layout` is a Codex skill for portfolio layout critique and teaching, built for design students preparing study-abroad, postgraduate, or interview portfolios.

It focuses on industrial design, interaction design/UX, HCI, service design, game design, digital media, and other cross-disciplinary design portfolios.

这个仓库公开保存一个 Codex skill：`portfolio-layout`。它用于帮助设计专业学生分析作品集页面、学习排版方法，并从优秀案例中提炼可复用的版式模式。

## What It Does

- Diagnoses uploaded portfolio pages and gives page-specific layout feedback.
- Teaches portfolio layout principles such as 信息层级, 留白, 版心, 叙事逻辑, 可视化, and project sequencing.
- Helps translate strong visual examples into reusable layout patterns without copying the original cases.
- Supports project-specific guidance for UX, HCI, industrial design, service design, social issue projects, technical prototypes, and game/interactive installations.

## 适合谁使用

- 正在准备留学、保研、考研复试作品集的设计学生
- 想系统学习作品集排版、信息层级和项目叙事的人
- 需要批量分析优秀作品集案例并沉淀排版模式的人
- 想诊断调研页、交互页、技术页、成果页、游戏/装置页面的人

## Skill Structure

```text
portfolio-layout/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── basic-rules.md
    ├── logic-framework.md
    ├── visual-principles.md
    ├── visualization.md
    ├── project-types.md
    ├── common-problems.md
    ├── case-analysis-method.md
    └── case-patterns.md
```

## Key Principles

This skill is intentionally conservative about evidence:

- It does not invent exact numbers. Numeric advice is only allowed when the source material contains that number, such as `4/8` spacing multiples, `15mm` margins, `1920 x 1080`, `1/3` and `2/3` layout division, or `60%` Development/Deliver weight.
- It treats external portfolio screenshots as visual examples, not authoritative rules.
- It does not store source case images.
- It does not invent project background, author intention, school result, or design concept from screenshots.
- It uses scraped text only as weak context because titles, tags, and marketing copy may be unreliable.

## How To Install

Clone this repository and copy the skill folder into your Codex skills directory:

```bash
git clone https://github.com/46564645/portfile-skills.git
mkdir -p ~/.codex/skills
cp -R portfile-skills/portfolio-layout ~/.codex/skills/
```

Restart Codex or reload skills if needed.

## Example Prompts

```text
Use $portfolio-layout to diagnose this interaction portfolio page.
```

```text
Use $portfolio-layout to explain how to layout a research-heavy UX project page.
```

```text
Use $portfolio-layout to extract reusable layout patterns from these portfolio examples.
```

## Suggested GitHub Description

```text
Codex skill for design portfolio layout critique, teaching, and visual case-pattern extraction.
```

## Notes

The current knowledge base was distilled from portfolio-layout teaching notes and a first batch of visual case-pattern observations. The case-pattern registry records only reusable layout structures and does not include original social-media screenshots.
