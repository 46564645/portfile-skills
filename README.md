# Portfolio Layout Coach | 作品集排版辅导 Skill

`portfolio-layout` is a Codex skill for advising on English-language design portfolio layout, built for students preparing study-abroad, postgraduate, or interview portfolios.

It focuses on industrial design, interaction design/UX, HCI, service design, game design, digital media, and other cross-disciplinary design portfolios.

这个仓库公开保存一个 Codex skill：`portfolio-layout`。它用于帮助设计专业学生分析英文作品集页面、学习排版方法、选择适合数据和关系的图表或图解，并从优秀案例中提炼可复用的版式模式。

## What It Does

- Diagnoses uploaded portfolio pages and gives page-specific layout feedback.
- Starts with the relationships and data a page needs to communicate, including relationships within a single module.
- Recommends suitable charts, diagrams, tables, sequences, or spatial arrangements for the evidence at hand, with chart-specific use cases and cautions.
- Teaches portfolio layout principles such as information hierarchy, spacing, narrative, visualization, and project sequencing.
- Helps translate strong visual examples into reusable layout patterns without copying the original cases.
- Supports project-specific guidance for UX, HCI, industrial design, service design, social issue projects, technical prototypes, and game/interactive installations.
- Gives advice and sample portfolio wording in English; palette and colour-matching recommendations are outside its scope.

## 适合谁使用

- 正在准备留学、保研、考研复试作品集的设计学生
- 想系统学习作品集排版、信息层级和项目叙事的人
- 需要批量分析优秀作品集案例并沉淀排版模式的人
- 想诊断调研页、交互页、技术页、成果页、游戏/装置页面的人

## Skill Structure

```text
dist/
├── portfolio-layout-skill.zip
└── portfolio-layout.skill

portfolio-layout/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── basic-rules.md
    ├── logic-framework.md
    ├── narrative-logic-chains.md
    ├── visual-principles.md
    ├── visualization.md
    ├── relationship-layout.md
    ├── chart-selection.md
    ├── visualization-case-studies.md
    ├── project-types.md
    ├── common-problems.md
    ├── case-analysis-method.md
    ├── case-patterns.md
    └── case-studies/
        ├── drone-skyforge.md
        ├── rescuepod.md
        └── chitoloop.md
```

## Key Principles

This skill is intentionally conservative about evidence:

- It checks whether a relationship or data comparison should be made visible before refining type and spacing.
- It recommends a chart only when the data and reading task suit that chart; a short sentence or simple arrangement can be clearer.
- It does not invent exact numbers. Numeric advice is only allowed when the source material contains that number, such as `4/8` spacing multiples, `15mm` margins, `1920 x 1080`, `1/3` and `2/3` layout division, or `60%` Development/Deliver weight.
- It treats external portfolio screenshots as visual examples, not authoritative rules.
- It does not store source case images.
- It does not invent project background, author intention, school result, or design concept from screenshots.
- It uses scraped text only as weak context because titles, tags, and marketing copy may be unreliable.

## Quick Use

### Claude Upload

If you are using Claude's skill upload page, do not upload the `portfolio-layout/` folder directly. Claude expects a `.skill`, `.zip`, or `.md` file.

Use one of these files instead:

- `dist/portfolio-layout-skill.zip`
- `dist/portfolio-layout.skill`

The archive root contains `SKILL.md`, `references/`, and `agents/`, so it can be uploaded directly.

### Codex Local Install

Clone this repository and copy the skill folder into your Codex skills directory:

```bash
git clone https://github.com/46564645/portfile-skills.git
mkdir -p ~/.codex/skills
cp -R portfile-skills/portfolio-layout ~/.codex/skills/
```

Restart Codex or reload skills if needed.

### Install From GitHub Zip

You can also download this repository as a ZIP from GitHub, then upload `dist/portfolio-layout-skill.zip` to a skill uploader that accepts `.zip` files.

## Example Prompts

```text
Use $portfolio-layout to diagnose this interaction portfolio page.
```

```text
Use $portfolio-layout to explain how to layout a research-heavy UX project page.
```

```text
Use $portfolio-layout to choose a chart for these observations and explain how to place it in my portfolio page.
```

```text
Use $portfolio-layout to extract reusable layout patterns from these portfolio examples.
```

## Suggested GitHub Description

```text
English design portfolio layout advice with relationship-first page critique, chart selection, research visualization, and visual case studies.
```

## Notes

The knowledge base combines portfolio-layout teaching notes, a chart-selection reference, and text-only observations of visual tutorials and case patterns. It does not include original social-media screenshots.
