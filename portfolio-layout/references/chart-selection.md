# Chart Selection Atlas for English-Language Portfolios

Use this when advising on quantitative charts. The entries are a broad working vocabulary, not a claim that a finite list can contain every invented or domain-specific chart. Recommend a form only after identifying the question, data structure, and comparison the reader must make. Explain *why this form fits* and give an English title, axis/legend label, or annotation example when useful. Advise on form and page placement; do not prescribe palettes or create a finished chart unless separately requested.

## Decision path

1. State the intended takeaway as a sentence, not a chart name.
2. Identify whether the source contains counts, rates, proportions, ordered categories, time, locations, pairs of measurements, ranges, or qualitative observations. Preserve units, denominator, sample, and source.
3. Pick the family matching the reading task below. Prefer a familiar form if it communicates the same result with less effort. Treat novelty as a reason to test, not a reason to recommend.
4. Check whether the form supports the exact comparison: absolute values versus share, individual values versus distribution, sequence versus duration, association versus causation, and location versus magnitude.
5. Tell the student how to integrate the result into the English portfolio page: an insight-led heading, chart, direct labels or a short annotation, source/method note, and a visible link to the design decision.

## 1. Magnitude, comparison, and ranking

| Form | Best use in a portfolio | Watch for |
|---|---|---|
| Horizontal bar | Compare category values, especially with long names | Start the quantitative axis at zero; sort by value or meaningful order. |
| Vertical column | Compare short categories or discrete time periods | Start at zero; avoid crowded labels. |
| Grouped bar / column | Compare a small number of series within the same categories | Too many groups make scanning hard. |
| Diverging bar | Compare positive and negative values against a meaningful baseline | Mark the baseline and explain the sign. |
| Spine chart | Show how a whole splits into two opposing components | Explain the shared total and where the split occurs. |
| Paired / back-to-back bar | Compare two populations on the same ordered categories | Keep scales symmetric and labels aligned. |
| Ordered bar / column | Show ranking with values | Distinguish a change in rank from a change in magnitude. |
| Lollipop | Rank values when a lighter visual footprint helps | Use a bar if precise magnitude comparison is the main task. |
| Dot plot / Cleveland dot plot | Compare category values on one aligned scale | Label sparse or important values directly. |
| Dumbbell / connected dot | Show a before/after gap for each category | Keep paired endpoints and direction unambiguous. |
| Range plot / floating bar | Show minimum–maximum or an interval per category | Define what the interval represents. |
| Bullet chart | Compare an observed value with a target or benchmark | Name the target and avoid unexplained bands. |
| Slope chart | Compare changes between two time points or conditions | Use when endpoints matter more than the path between them. |
| Bump chart | Track rank changes across several time points | Use only when rank, rather than the underlying value, is the message. |
| Pictogram / icon array | Make whole-number counts or a part of a count tangible | Do not imply fractions with cut-up icons. |
| Proportional symbols | Show large magnitude differences where exact reading is secondary | Size by area, not radius; label values if precision matters. |
| Ordered proportional symbols | Show rank when differences are large and approximate comparison is sufficient | Use a bar when close values must be compared. |
| Radar / spider | Give a compact overview of several comparable dimensions | Shared scales and variable order matter; prefer aligned bars for close comparison. |
| Parallel coordinates | Compare multivariate profiles across observations | Needs clear axis order and a manageable number of lines. |

## 2. Change over time and schedules

| Form | Best use in a portfolio | Watch for |
|---|---|---|
| Line | Show a continuous trend or repeated measurements through time | Mark gaps and irregular observations. |
| Multi-series line | Compare a few trajectories | Use small multiples when lines obscure one another. |
| Step line | Show values that change in discrete jumps, such as policy or state | Do not smooth abrupt changes. |
| Area | Emphasize a total evolving over time | Area needs a meaningful zero baseline. |
| Surplus/deficit filled line | Show positive and negative deviation from a baseline across time | Label the baseline and signed difference. |
| Stacked area | Show changing total and its components | Middle bands are hard to compare precisely. |
| 100% stacked area | Show changes in composition, independent of changing total | State that the vertical scale is share, not volume. |
| Streamgraph | Show broad composition rhythm over time | Use for pattern, not precise component comparison. |
| Time columns | Show separated intervals or event counts by period | Appropriate when discrete periods matter more than continuity. |
| Calendar heatmap | Show daily or weekly periodicity across a calendar | Useful for pattern; exact values need labels or table support. |
| Cycle plot / seasonal subseries | Compare repeating time cycles across periods | Keep the cycle units and period boundaries clear. |
| Circular timeline / clock plot | Show a genuinely repeating day or cycle | Do not force a one-way chronology into a circle. |
| Gantt / interval timeline | Show start, finish, overlap, and duration of activities | Distinguish planned from observed durations. |
| Priestley timeline | Show many historically dated intervals along a shared chronology | Use when duration and overlap both matter. |
| Event timeline / annotated timeline | Sequence milestones, images, and explanations | Space dates accurately if elapsed time matters. |
| Barcode / event rug | Show many individual event times | Add summary when events are too dense. |
| Seismogram / radial event plot | Show event magnitude across a recurring or long time span | The radial scale needs a clear key; use a line if precision matters. |
| Sparkline | Give a compact trend beside a metric in a table | It is context, not a substitute for a fully labelled main chart. |
| Horizon chart | Compare many long time series in limited space | Use only when the audience can decode its folded scale. |
| Fan chart | Show a forecast with a widening uncertainty range | Separate observed history from projection. |
| OHLC / candlestick | Show open, high, low, and close for each trading period | Use only when the four measures are relevant. |

## 3. Composition, shares, and contribution to a total

| Form | Best use in a portfolio | Watch for |
|---|---|---|
| Stacked bar / column | Show total plus a few parts across categories | Components without a common baseline are hard to compare. |
| 100% stacked bar | Compare composition across categories | Total magnitude disappears; provide it separately if relevant. |
| Diverging stacked bar | Show opposing survey responses around a neutral point | Explain the centre and response order. |
| Pie | Show a simple part-to-whole message with few slices | Avoid when close slice comparison is required. |
| Donut | Same as pie, with room for a central total | The hole does not solve difficult slice comparisons. |
| Waffle / unit grid | Show a proportion as countable units | Match grid units to the underlying denominator. |
| Treemap | Show hierarchical share using nested rectangles | Small areas need labels or a focused subset. |
| Sunburst | Show hierarchy and share across levels in radial bands | Hard to compare small arcs; use a tree if structure is primary. |
| Icicle / partition | Show nested hierarchy with aligned rectangular bands | Explain parent–child levels and keep labels readable. |
| Circle packing | Show nested groups and approximate relative sizes | Use for structure and overview, not fine value comparison. |
| Marimekko / mosaic | Show two categorical dimensions and their joint shares | Requires explanation of both width and height. |
| Stacked pictogram | Show components through repeated units | Use real counts or a clearly defined unit. |
| Parliament / hemicycle | Show seats or fixed membership by group | Suitable for counts of members, not generic percentages. |
| Waterfall | Show sequential additions and subtractions to a total | Label starting value, signed steps, and final value. |
| Funnel | Show attrition through ordered stages | Stage widths must use a consistent denominator and actual counts. |
| Gridplot / unit square | Show an integer percentage or part of a fixed set | Each cell must represent a defined unit. |
| Venn / Euler diagram | Show overlap among sets | Treat areas as schematic unless overlap is quantitatively encoded. |

## 4. Distribution and spread

| Form | Best use in a portfolio | Watch for |
|---|---|---|
| Histogram | Show how many observations fall in numerical intervals | Bin size affects the visible pattern. |
| Density curve | Show a smoothed distribution | Smoothing can hide small samples or multiple peaks. |
| Dot strip / strip plot | Show each observation along a value axis | Overlap may hide repeated values. |
| Jitter plot | Reveal overlapping observations with small offsets | Offsets are display aids, not data values. |
| Beeswarm | Show individual observations while avoiding overlap | Dense groups may need summarization. |
| Box plot | Compare median, quartiles, spread, and outliers | Do not present it as showing every data point. |
| Violin | Compare the shape of several distributions | Pair with sample size and median if needed. |
| Raincloud | Show density, summary, and raw points together | Complex form needs enough room and a clear reading order. |
| Ridgeline | Compare several related distributions or their changes | Vertical overlap can obscure scale. |
| Population pyramid | Compare two distributions across ordered bands | Use matched scales. |
| Cumulative distribution / ECDF | Read percentiles and compare distributions | Explain the cumulative vertical axis. |
| Lorenz curve | Show inequality or concentration | State the cumulative share definitions. |
| Q–Q plot | Check whether data fit a reference distribution | Mainly for technical research pages. |
| Stem-and-leaf | Preserve individual values while showing a small distribution | Best for small datasets. |
| 2D histogram / hexbin | Summarize dense pairs of values | Bin settings affect apparent clusters. |

## 5. Correlation, multivariate patterns, and matrices

| Form | Best use in a portfolio | Watch for |
|---|---|---|
| Scatterplot | Show association between two numeric variables | Correlation alone does not show causation. |
| Bubble scatterplot | Add a third numeric variable through area | Too many large marks overlap; compare exact values in labels or table. |
| Connected scatterplot | Show how a two-variable relationship evolves in sequence | Direction and order need visible cues. |
| Line + column | Show a count and a related rate over the same periods | Different units need unmistakable scale labels; consider aligned panels. |
| Quadrant plot | Classify observations against two meaningful thresholds | Explain why the cutoffs matter. |
| Pair plot / scatterplot matrix | Explore pairwise relations among several variables | Too dense for a final portfolio page unless focused. |
| Correlogram | Summarize pairwise correlations across many variables | The statistic and sign must be stated. |
| Heatmap / matrix chart | Reveal a pattern across two categorical axes | Use when pattern matters more than exact values. |
| Contour / density contour | Show regions of equal value or bivariate concentration | Indicate what each contour level means. |
| Parallel sets | Follow categories across several dimensions | Distinguish counts from proportions. |
| Radar | Compare a compact profile of shared measures | Avoid mixing unrelated units without normalization. |
| Parallel coordinates | Compare individual multivariate profiles | Usually works better with a highlighted subset. |
| Ternary plot | Show three components that sum to one whole | Explain the three-axis reading convention. |
| Table with in-cell marks | Preserve exact values while exposing a pattern | Use when precise lookup is the reader's task. |

## 6. Flow and change between states

| Form | Best use in a portfolio | Watch for |
|---|---|---|
| Sankey | Show quantities flowing through stages | Band widths must represent the same quantity throughout. |
| Alluvial | Show how group membership changes across dimensions or time | Requires trackable groups or shares. |
| Chord | Show many-to-many exchange among groups | Dense arcs are hard to trace; use a matrix for precise comparison. |
| Flow map | Show movement between actual locations | Use a map only when geography is necessary to the argument. |
| Origin–destination matrix | Compare many flows between places or groups | Better than a tangled map when exact pairs matter. |
| Waterfall | Show signed steps from a start value to an end value | It is an arithmetic bridge, not a generic process diagram. |
| Funnel | Show stage-by-stage conversion or loss | Do not infer causes of drop-off from the chart alone. |
| Cumulative flow diagram | Show work-item states and bottlenecks over time | Needs consistent state definitions. |
| Chord / circular flow | Show reciprocal exchange or redistribution | Favor a simpler diagram for a small number of connections. |

## 7. Hierarchy and network structure

| Form | Best use in a portfolio | Watch for |
|---|---|---|
| Tree / dendrogram | Show parent–child hierarchy or clustering | In a dendrogram, branch length may carry distance. |
| Indented tree | Show many levels with readable labels | Strong for exact names, weak for overall proportions. |
| Radial tree | Show a broad hierarchy with a central root | Labels can become hard to scan. |
| Treemap | Show hierarchical proportions | Area comparisons are approximate. |
| Sunburst / icicle | Show hierarchy plus composition across levels | Pick radial or rectangular form for the available space. |
| Node–link network | Show entities and their connections | Use only when link structure is the question. |
| Force-directed network | Reveal clusters or hubs in a network | Spatial proximity is layout-derived, not measured geography. |
| Adjacency matrix | Show connections in a dense network | Better than crossed lines for many nodes. |
| Arc diagram | Show links among ordered nodes | Order determines the apparent pattern. |
| Bipartite network | Show relationships between two distinct sets | Keep the two sets visually separable. |
| Edge-bundled network | Reduce clutter in a large structured network | Bundling can obscure individual edges. |

## 8. Geographic and spatial data

| Form | Best use in a portfolio | Watch for |
|---|---|---|
| Locator map | Show where an intervention or observation happened | Context and orientation matter more than statistics. |
| Choropleth | Show a rate or proportion across geographic units | Avoid raw totals when region sizes/populations differ. |
| Proportional symbol map | Show counts or magnitudes at locations | Size symbols by area and watch overlap. |
| Dot-density map | Show the spatial pattern of many instances | Explain what one dot represents. |
| Point map | Show exact sampled sites or events | May need clustering when points overlap. |
| Heat / density map | Show concentration over a continuous area | A smoothed surface is not an exact event location. |
| Hexbin map | Aggregate dense spatial points into equal cells | Cell size can change the pattern. |
| Contour / isarithmic map | Show continuous surfaces such as elevation or exposure | Explain contour intervals. |
| Cartogram, area-scaled | Make geographic area proportional to a quantity | Distorted boundaries need careful orientation cues. |
| Tile-grid map | Compare equal-sized regions while retaining rough geography | Exact shapes and distances are lost. |
| Dorling / circle cartogram | Replace regions with sized circles to show geographic magnitude | Preserve geographic context with labels or orientation cues. |
| Dasymetric map | Refine an area-based map using ancillary spatial information | Explain the modeling assumptions. |
| Flow / connection map | Show origin–destination movement | Use only if the route or geography matters. |
| Voronoi / service-area map | Show nearest facility or catchment assignment | It assumes distance or travel metric chosen for the model. |

## 9. Uncertainty, estimates, and technical research

| Form | Best use in a portfolio | Watch for |
|---|---|---|
| Error-bar / interval plot | Show an estimate with a measured or modeled range | Define the interval: standard deviation, confidence, or range. |
| Dot-and-whisker / forest plot | Compare several estimates and their intervals | Include the reference value and what each row represents. |
| Fan chart | Show a forecast widening into future uncertainty | Do not display projections as observed values. |
| Prediction band | Show likely range around a fitted line | Distinguish it from a confidence interval for the mean. |
| Control chart | Show variation against process limits over time | Limits should be calculated, not invented as decorative guides. |
| Pareto chart | Rank contributors and show cumulative share | Use when prioritization by contribution is the question. |
| ROC / precision–recall curve | Compare model trade-offs across thresholds | State the task and relevant baseline. |
| Calibration plot | Compare predicted probability with observed frequency | Useful only when predictions are probabilistic. |
| Residual plot | Diagnose a model's errors across fitted values or time | Technical evidence, not a substitute for a main finding. |
| Bland–Altman plot | Compare agreement between two measurement methods | Interpret differences and limits, not correlation alone. |
| Volcano plot | Show effect size against statistical significance in high-volume studies | State thresholds and avoid implying significance equals practical importance. |
| Manhattan plot | Show many statistical tests across ordered genomic positions | Specialized scientific form; explain threshold and position axis. |

## 10. Text, categorical patterns, and qualitative evidence

| Form | Best use in a portfolio | Watch for |
|---|---|---|
| Frequency bar | Rank coded themes or terms with documented counts | Do not imply population prevalence from a small qualitative sample. |
| Theme-by-participant matrix | Show which themes appeared in which interviews or observations | Presence is not severity or agreement. |
| Co-occurrence matrix | Show which codes or topics appear together | Explain counting method and overlap. |
| Word cloud | Show a loose sense of prominent words | Poor for precise comparison; avoid as the sole research result. |
| Quote-and-theme board | Pair representative quotations with synthesized themes | Preserve the connection to source evidence. |
| Affinity map | Cluster individual observations into themes | Show the synthesis, not an unreadable wall of sticky notes. |

## Composition devices that work across families

| Device | Best use in a portfolio | Watch for |
|---|---|---|
| Small multiples / faceting | Compare the same chart across groups, places, or periods | Use aligned scales for magnitude comparisons; explain any independent scale. |
| Aligned chart-and-table | Pair a visual pattern with exact values readers may need | Keep category order and units consistent. |
| Annotated chart sequence | Lead readers through a complex finding in a few static frames | Each frame should add one clear point rather than repeat the entire chart. |

## Source anchors and boundaries

- [Financial Times Visual Vocabulary](https://github.com/Financial-Times/chart-doctor/blob/main/visual-vocabulary/README.md): task-based families, including deviation, ranking, distribution, time, part-to-whole, magnitude, spatial, flow, and correlation.
- [From Data to Viz](https://www.data-to-viz.com/): chart selection by input data type; its authors explicitly say chart types are open-ended and context affects choice.
- [Datawrapper chart-type guide](https://www.datawrapper.de/blog/chart-types-guide): accessible examples organized by the message to communicate.
- [Office for National Statistics chart guidance](https://service-manual.ons.gov.uk/data-visualisation/chart-types): use cases and conventions for common statistical charts.
- [ONS axes and gridlines](https://service-manual.ons.gov.uk/data-visualisation/guidance/axes-and-gridlines): zero baselines for filled bar/area forms and comparable scales across panels.

This atlas synthesizes and extends those source taxonomies into portfolio advice. It does not copy their images or treat one publication's categories as a universal law. When a specialized field introduces a form not listed here, identify its data and reading task, then assess it by the same decision path.
