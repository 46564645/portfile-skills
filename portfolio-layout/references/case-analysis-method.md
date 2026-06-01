# Case Analysis Method

Use when the user provides优秀案例, 小红书 screenshots, scraped folders, image-only portfolio examples, or folders that contain images plus txt notes. The goal is to extract reusable layout patterns, not to copy visual style or treat social-media captions as rules.

## Evidence Rules

- Treat images as primary evidence for layout.
- Treat txt as weak context: title, possible project type, keywords, page labels, or author-provided notes.
- Ignore or down-rank marketing language, tags, generic praise, posting metadata, and unrelated captions.
- Do not infer project story, school result, author identity, or design intention unless visible in the image or clearly stated in txt.
- Do not invent numeric rules from cases. If a case shows "large title" or "wide margin", record qualitative traits unless the file explicitly provides measurements.
- Do not store source images inside this skill. Summarize patterns in text.

## Per-Case Reading Order

1. **Inventory**: Count images and read txt filenames/content if present.
2. **Context Guess**: Identify only safe context: likely project type, page type, theme keywords, language, and whether pages seem sequential.
3. **Visual Pass**: Observe structure before content: grid, columns, image scale, margins, density, color, typography roles, and page rhythm.
4. **Information Pass**: Identify title, key statement, body, caption, chart, process evidence, final output, and whether hierarchy is clear.
5. **Pattern Extraction**: Name the reusable layout move without tying it to the specific author.
6. **Applicability**: State which user page type it could help: research page, concept page, process page, system page, UI page, final page, cover, chapter page, or other works.
7. **Risks**: Note when the pattern would fail, such as insufficient image quality, too much text, weak project logic, or over-decorative copying.

## Output Template

Use this compact format when analyzing a case folder:

```markdown
### Case: <folder name or safe title>

- Evidence used: <image count; txt present/absent; txt reliability>
- Likely page/project type: <only observable or stated context>
- Observable layout structure: <columns/grid/focus/path>
- Hierarchy strategy: <how attention is guided>
- Image/text relationship: <integration, separation, annotation, overlay, etc.>
- Color/material strategy: <qualitative, no invented numbers>
- Reusable pattern: <short pattern name>
- Why it works: <reading/logic benefit>
- Use for: <page types>
- Do not copy: <style-only or risky parts>
```

## Pattern Naming Rules

Name patterns by structure and reading function, not by social-media title or author. Good names:

- 中央主视觉 + 两侧解释
- 灰度素材 + 单色重点
- 大图场景 + 局部标注
- 流程链路 + 证据卡片
- 系统图核心 + 周边节点
- 左侧叙事栏 + 右侧成果展示

Avoid names such as "高级感排版", "爆款风格", or "某某作者同款".

## Using Cases in User Diagnosis

When applying case patterns to a user's page:

- Say "可以借用某种结构" rather than "照着这个案例做".
- Explain the fit: what problem in the user's page the pattern solves.
- Keep all recommendations tied to observable user-page problems.
- Combine case patterns with source rules from the other references when possible.

Example:

`你这页的问题不是内容不够，而是所有信息平均铺开。可以借用“中央主视觉 + 两侧解释”的结构：把最能说明研究结论的图放到视觉中心，左侧放背景/问题，右侧放证据或注释。这里不需要复制案例风格，重点是建立阅读路径。`
