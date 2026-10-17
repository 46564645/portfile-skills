# Relationship-First Layout Advice

Read this whenever a portfolio page contains data **or a relationship the reader must understand**. Relationship means more than a link between modules. It can exist among items inside one block, between image and caption, among research observations, between a claim and its evidence, between evidence and design decision, across time, across space, among actors, or between a whole and its parts.

## First layout principle

Before recommending margins, type treatment, or decoration, ask: **What relationship or comparison must become visible on this page?** Recommend an appropriate chart, diagram, table, annotated sequence, or deliberate spatial arrangement when it would make that relationship easier to grasp. Do not force a diagram when a short sentence or a simple side-by-side layout is clearer. If there is no meaningful relation to encode, continue with ordinary visual-hierarchy advice.

Give advice, not a completed visualization, unless the user asks to make one. For an English-language portfolio, write sample headings, labels, legends, and captions in English; explanations to the user may follow the user's language. Avoid palette and colour-matching advice in this workflow.

## Relationship-to-form atlas

| Relationship the page needs to show | Useful forms | When this helps |
|---|---|---|
| Chronology | Linear timeline, annotated timeline, before/after sequence | Show how events or design iterations unfolded. |
| Repeating time | Circular timeline, cycle diagram | Show a true daily, seasonal, or repeated loop. |
| Duration and overlap | Gantt / interval timeline | Show activities running in parallel and their lengths. |
| Order of actions | Flowchart, task flow, storyboard | Show how a user or mechanism moves from one step to the next. |
| Decisions and branches | Decision tree, state diagram | Show alternatives, conditions, and outcomes. |
| Responsibility across steps | Swimlane diagram | Show which actor or team owns each action. |
| User experience across stages | User journey / experience map | Align actions, touchpoints, observations, and pain points over time. |
| Frontstage and backstage dependencies | Service blueprint | Explain how service components support visible touchpoints. |
| Screen-to-screen interaction | User flow, wireflow | Link actions and decision points to specific interface states. |
| Story in context | Storyboard, annotated scenario sequence | Show people, environment, trigger, action, and result. |
| Parent–child grouping | Tree, indented hierarchy, site map, information architecture | Show nested structure or navigation. |
| Whole–part assembly | Exploded view, layered breakdown, labelled sectional view | Show how components fit and what each part does. |
| Spatial placement | Plan, map, site diagram, annotated photograph | Show where observations or interventions occur. |
| Proximity / zones | Hub-and-spoke, concentric ecosystem map | Show central and peripheral actors or touchpoints; define what distance means. |
| One-to-one correspondence | Aligned pairs, matched columns, trace lines | Match an observation to a feature, quote, prototype change, or outcome. |
| Many-to-many correspondence | Matrix, adjacency matrix, crosswalk table | Avoid tangled connecting lines among many items. |
| Similarities and differences | Comparison table, paired panels, small multiples | Keep corresponding fields aligned on the same scale or frame. |
| Categories and intersections | Venn / Euler diagram, overlap matrix | Show conceptual set overlap; do not imply quantitative area unless measured. |
| Cause hypotheses | Causal chain, fishbone / Ishikawa, problem tree | State hypothesized mechanisms and distinguish them from observed evidence. |
| Feedback and reinforcement | Causal-loop / feedback-loop diagram | Show a recurring influence with marked direction. |
| Dependencies | Dependency graph, system architecture | Show what relies on what; label the link meaning. |
| Exchange among actors | Network diagram, stakeholder map, ecosystem map | Show interaction, influence, or resource exchange. |
| Position along two criteria | Two-axis matrix / quadrant | Show classification by explicit criteria, not arbitrary placement. |
| Qualitative synthesis | Affinity map, theme matrix, evidence board | Show how observations form themes and insights. |
| Evidence to action | Evidence → insight → opportunity → design decision chain | Make the argument behind a design move reviewable. |
| Alternative concepts | Option matrix, concept comparison | Explain tradeoffs using the same criteria for each option. |
| Evolution of a design | Iteration sequence, before/after with callouts | Show what changed because of testing. |
| Input–transformation–output | Process diagram, mechanism schematic | Show how a system produces an outcome. |
| Scale or magnitude | Quantitative chart from `chart-selection.md` | Use measured data rather than making size decorative. |
| Distribution | Histogram, dot strip, box plot, density plot | Show variation rather than only a mean. |
| Flow of quantity | Sankey, alluvial, flow map | Use only when widths correspond to actual quantities. |

## Page-level recommendation pattern

Use concise, actionable wording, for example:

> “The page asks readers to connect three interview findings with three prototype changes. Place findings and changes in aligned columns, draw only the three necessary correspondences, and add a one-line English insight above each pair. This makes the evidence behind each design choice visible.”

Or:

> “The research combines observations from different times of day. First align them on one shared time axis; then use separate bands for activity, foot traffic, and field photographs. Keep the explanatory notes near the moments they describe.”

Do not suggest a format solely because it is visually distinctive. A form is successful when readers can answer the intended question with less effort and without misunderstanding the evidence.

## Source anchors

- [NN/g UX Maps Glossary](https://www.nngroup.com/articles/ux-maps-glossary/) distinguishes mapping forms and their purposes.
- [NN/g UX Mapping Methods visual-design guide](https://www.nngroup.com/articles/ux-mapping-methods-visual-design-guide/) addresses layout and reading order in UX maps.
- [NN/g Service Blueprints](https://www.nngroup.com/articles/service-blueprints-definition/) defines the relations among touchpoints, people, processes, and evidence.
- [NN/g Mapping in Discovery](https://www.nngroup.com/articles/mapping-in-discovery/) describes ecosystem maps, journey maps, and blueprints as different views of a problem space.
- [Financial Times Visual Vocabulary](https://github.com/Financial-Times/chart-doctor/blob/main/visual-vocabulary/README.md) supplies the quantitative relationship families.
