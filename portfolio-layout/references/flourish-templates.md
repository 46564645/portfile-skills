# Flourish template reference

A working catalog for English design-portfolio visualizations. Charts are built in [Flourish](https://flourish.studio/). When recommending a visualization, name the **Flourish template** (as it appears in the template chooser) in one sentence, then add data-shape and limit notes as needed.

**Researched:** 10 November 2026 (Asia/Shanghai), from public pages only (no login). Primary sources: the public template chooser at [app.flourish.studio/templates](https://app.flourish.studio/templates), the [Flourish help center](https://helpcenter.flourish.studio/hc/en-us) (Charts, Maps, Tables and heatmaps, Content based templates, Stories and scrollies, Data, Exporting), and selected [visualisations](https://flourish.studio/visualisations/) / blog pages listed at the end. Nothing in this file is invented; gaps are marked **unverified**.

**How to read names.** Template names below match the headings in the public template chooser. Many chooser “starting points” (Arrow plot, Waffle chart, Streamgraph, Treemap, and so on) are modes of a parent template, not separate templates. Those are listed under the parent, not as their own rows.

---

## Decision shortcuts

Map the portfolio situation to a Flourish template. Prefer the parent template name in any one-sentence recommendation.

| Situation | Use this Flourish template | Why / how |
| --- | --- | --- |
| Predicted vs actual, before/after, or a dumbbell / connected-dot comparison | **Scatter** | There is no separate Dumbbell or Arrow plot template. The chooser’s **Connected dot plot**, **Cleveland dot plot**, and **Arrow plot** starting points all belong to Scatter. An official 2019 blog post, [(Ar)row row row your plot](https://flourish.studio/blog/make-arrow-plots/), says: bind a “Series (connect with line)” column, enable lines in **Lines & arrows**, and optionally turn on arrowheads. Point order in the sheet is the line direction (arrow on the final point). Line, bar and pie charts can show two values as grouped or diverging bars, but it does not have a documented dumbbell / arrow-plot mode. |
| Equal-weight relationships (every link should look the same) | **Network graph** | Links sheet: Source, Target, Value. Set every Value to 1 so widths stay equal. Optional Points sheet: Id, group (color), size. Choose classic, directed (arrows), or radial layout in Chart type. |
| Weighted flows, user-journey stages, or how a set regroups | **Sankey diagram** | Classic Sankey or Alluvial starting points. Source, Target, optional Values; alluvial also needs Step from / Step to. If Values is empty, link width is the **number of rows**. Node and band size encode quantity — do not use this when heights must stay equal. |
| Mutual or directional volume between a closed set of entities | **Chord diagram** | Source, Target, Value. Directional chords need two rows per pair (missing reverse flow is treated as 0). Non-directional chords should repeat the same value in both directions. Circular layout; chord thickness encodes Value. |
| Survey Likert / question-by-question results | **Survey** if you have **one row per respondent**; **Line, bar and pie charts** if you only have aggregated percentages | Survey: one row per person, one column per question; views include groups, bars, a grid, and (with place names) a map. The Line, bar and pie chooser includes **Column chart (Likert scale)**, **Diverging stacked bar chart**, and **Survey bars** starting points for already-summarized scales. |
| Proportions, waffle, or icon unit charts | **Pictogram** (waffle); or **Line, bar and pie charts** (pie, donut, stacked / proportional bars) | Pictogram has **Waffle chart** and **Waffle chart (people)** starting points. Enable filler icons and use **Fill final row** when making a waffle ([help](https://helpcenter.flourish.studio/hc/en-us/articles/8761575173263-How-to-enable-filler-icons-in-your-pictogram-visualization)). |
| Ranking over time (race) | **Bar chart race** or **Line chart race** | Bar chart race: one row per competitor, later columns are cumulative stages. Line chart race has **Scores** (raw values) and **Ranks** (bump chart) modes. |
| Simple ranking of categories (static) | **Line, bar and pie charts** (sorted bar/column) or **Hierarchy** (Ranking wheel starting point) | Hierarchy’s Ranking wheel is a starting point, not a separate template. |
| Change over time (trends) | **Line, bar and pie charts** | Line, area, streamgraph, bump, combo, and small-multiples are all Chart type options in this one template. Dashed lines for projections are documented here ([How to create dashed lines](https://helpcenter.flourish.studio/hc/en-us/articles/8761539818639-How-to-create-dashed-lines)). |
| Two moments, many categories (before → after slopes) | **Slope chart** | Wide data: one label column plus a value column per period. Also has a Parallel coordinates starting point. |
| Timeline of events | **Timeline**; use **Gantt chart** for tasks with start and end; use **Calendar** for dates on a calendar grid | Timeline needs long-format rows with at least a start time (end time optional). |
| Distribution of one numeric variable | **Scatter** | Starting points: Dot plot, Beeswarm, Box plot, Violin plot. These are modes of Scatter, not separate templates ([box / violin / beeswarm help](https://helpcenter.flourish.studio/hc/en-us/articles/9859136207759-How-to-make-box-violin-and-beeswarm-scatter-plots)). |
| Correlation of two numeric variables | **Scatter** | X and Y columns; optional size, color, shape, time slider, trend lines, WebGL for large data. |
| Nested proportions (treemap, packed circles, sunburst) | **Hierarchy** | Long data; nest by categorical columns, size by numeric columns. Starting points include Treemap, Packed circles, Sunburst, Hierarchical bars, Radial tree. |
| Parts of a whole with a second dimension (variable bar width) | **Marimekko** | Classic (both axes as %) or Bar mekko (absolute secondary axis). Bindings: Name, Primary metric, Secondary metric (stackable). |
| Photo before/after | **Photo slider** | Starting point: Before and after. Upload two images (optional mobile alternatives). Not for numeric before/after data. |
| Process or annotated custom diagram | **Interactive SVG** | Upload an SVG whose groups have ID attributes; Data tab: one row per clickable ID, plus heading/content columns. |
| Scrollytelling page | **Flourish stories** in **Scrolly** mode (story editor, not a chart template) | Documented as Enterprise and Publisher only. Works with script embeds and HTML downloads, not iframe embeds. |
| Maps of regions or points | See the Maps table; start with **Projection map** unless you need WebGL, 3D, or a locator-style marker map | Projection map can download as SVG and does not require WebGL. 3D map supports larger data, heatmaps, and animated points. Marker map is for points of interest (icons, emoji, images). |

---

## 1. Template catalog

**44 featured visualization templates** are listed in the public chooser. Each row is one template. Help URLs are articles whose text was retrieved for this guide.

### Comparison

| Template name | Best for | Data shape | Known limits (design-relevant) | Source |
| --- | --- | --- | --- | --- |
| Line, bar and pie charts | Everyday comparison, trends, parts of a whole, combo and small-multiples charts | Typically **wide** data: a Labels/time column plus one or more Values columns. Long format is needed for Charts grid or Row filter (can unpivot inside Flourish). | One template, many Chart types — not separate templates. Documented or chooser starting points include line, area (stacked/unstacked), streamgraph, area bump, line bump, bar, column, stacked, grouped, proportional, diverging bar, diverging stacked bar, waterfall, pie, donut, combo (column + line, line + area), histogram, population pyramid, Likert / survey bars, grids, and more. Dashed lines are a Line, bar and pie feature (name the series in **Dashed lines**). Waterfall is a Chart type in this template, not its own template. Dual-axis and streamgraph marketing pages also point back to this family. | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761567940495-Line-bar-and-pie-charts-an-overview); [dashed lines](https://helpcenter.flourish.studio/hc/en-us/articles/8761539818639-How-to-create-dashed-lines); [waterfall](https://helpcenter.flourish.studio/hc/en-us/articles/8761539591567-How-to-make-a-waterfall-chart); [combo](https://helpcenter.flourish.studio/hc/en-us/articles/8761574478735-How-to-make-combo-charts-in-our-Line-bar-pie-template); [area bump](https://helpcenter.flourish.studio/hc/en-us/articles/9951629626383-How-to-create-an-area-bump-chart); [visualisations page](https://flourish.studio/visualisations/line-bar-pie-charts/) |
| Slope chart | Change between a few time points across many categories | **Wide** data: labels/series in one column, a value column per period, all bound to Values | Help-center section title is “Slope”. Chooser also has Grid of slopes, Inline labels, Parallel coordinates, and With filter starting points. | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761582577551-Slope-an-overview) |
| Radar chart | Comparing several attributes of entities on a shared scale | A names column plus **at least three numeric columns on the same scale** (e.g. scores out of 10). Optional category column to filter. | Help-center section title is “Radar”. Starting points include radial bar and polar with time slider. Values must be comparable; mixed units will mislead. | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761575550351-Radar-an-overview) |
| Marimekko | Market maps or two metrics at once (bar width and segment height) | **Long** format. Bindings: Name, Primary metric (bar baseline, not stacked), Secondary metric (one or more stackable columns), optional Grid / Color category / Filter | Two modes: Classic (both axes as percentages) and Bar mekko (secondary axis is absolute). | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761553749007-Marimekko-charts-an-overview) |
| Gauge | One or more single-value metrics | One row per gauge. Binding two or more columns to Value adds a filter. | Three modes: single, grid, or filter. Custom min/max applies to all gauges in the view. | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761567109135-Gauge-an-overview) |
| Bubble chart | Sized or packed circles, optionally placed on an X axis, with images | **Wide** data, one row per bubble. Only **Label** is required; optional size, axis values, color, images, popups | This is a separate template from Scatter’s “Bubble chart” starting point. **Does not support date formats** for axis placement (a workaround is documented). Auto-resizes bubbles to fit the screen. | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761547086735-Bubble-chart-An-overview); [axis placement](https://helpcenter.flourish.studio/hc/en-us/articles/8761552648591-Positioning-bubbles-along-an-axis-in-the-Bubble-chart-template) |
| Pictogram | Isotype / icon unit charts and waffles | Two sheets: **Data** (Main category, Sub category, Value, optional Icon id, Color) and optional **Icons** (Icon id plus icon assets). | Less precise than bars. Icon value is auto-calculated (about 100 icons per bar) unless overridden. Waffle: enable filler icons and Fill final row. Custom icons are supported. | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761540123407-Pictogram-an-overview); [filler / waffle](https://helpcenter.flourish.studio/hc/en-us/articles/8761575173263-How-to-enable-filler-icons-in-your-pictogram-visualization) |
| Table | Searchable, filterable tables, optionally with mini bar or line charts in cells | One binding: bind all columns to **Table values** | Mobile can be Blocks or a scrollable table. Search modes: Anywhere, Start, Whole. | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761554867983-Table-an-overview) |

### Change over time

| Template name | Best for | Data shape | Known limits (design-relevant) | Source |
| --- | --- | --- | --- | --- |
| Bar chart race | Animated ranking of competitors over stages | One **row per participant**; first column is the name; later columns are stages. Data should be **cumulative**. | About 1,000 rows (Flourish’s published limits table). Captions, images next to bars, and axis highlights (including dashed highlight lines) are documented. | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761566757647-Bar-chart-race-an-overview) |
| Line chart race | Animated lines of scores, or a bump chart of ranks | Same wide “one row per participant, columns as stages” shape as bar chart race | Two modes: **Scores** (raw values) and **Ranks** (bump chart). | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761547629711-Line-chart-race-an-overview) |
| Timeline | Event timelines, past/present/future | **Long** format; recommended columns include Start time (required), End time, Category, Title, Text, Image | Auto-set columns are supported. | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761582943759-Timeline-an-overview) |
| Calendar | Events on a year / month / week / continuous calendar | A dates column and an event name; optional color, icon, filter, popup columns | Can highlight today and open on today’s date if that date is in the data. Written month names are recognized in English only in Flourish’s general date typing (see Import tips). | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/10242475125007-Calendar-an-overview) |
| Gantt chart | Project schedules or event spans | **Long** format, one event per row, with start and end date/time plus a main category; optional assignee, progress, etc. | Also usable as a timeline of events, but it is a Gantt, not the Timeline template. | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761546639375-Gantt-chart-an-overview) |
| Countdown | Count down (or up) to a date and time | A target date; optional custom format with `{{d}}`, `{{h}}`, etc.; optional end text in countdown mode | Minimal data; more of a content widget than a dataset chart. | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761561446543-Countdown-an-overview) |
| Number ticker | An animated number, optionally inside a sentence | Simple mode: Tick from / Tick to. Custom mode: text with `{{1000}}` or `{{-5000/4000}}` (markdown supported) | Not a dataset chart. | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761548263823-Number-ticker-an-overview) |
| Draw the line chart | Let viewers guess a time series before revealing the real line | Same structure as a line chart: a time column and a column per line. Gaps for the guessable segment are created in settings, not in the sheet. | Engagement / quiz-style, not a standard explanatory line chart. | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761560393487-Draw-the-line-chart-an-overview) |

### Distribution and exploration

| Template name | Best for | Data shape | Known limits (design-relevant) | Source |
| --- | --- | --- | --- | --- |
| Scatter | Relationships between two variables; also dot plots, arrow plots, box / violin / beeswarm, and Hans Rosling-style animated scatters | Two numeric columns (X, Y) for a basic scatter, one row per dot. Optional color, size, shape, time + name columns for animation, filter, popup info. For connected / arrow plots, bind **Series (connect with line)**. | Help-center title is “Scatter plot”. Chooser starting points include Basic scatter plot, Bubble chart, Beeswarm, Box plot, Connected dot plot, Dot plot, Arrow plot, Cleveland dot plot, Violin plot, and others. Beeswarm is for one numeric metric across categories (dots “swarm” so they do not overlap as they might in a dot plot). WebGL renderer is available for large data (limits table: up to 200,000 rows in WebGL mode). | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761582471439-Scatter-plot-an-overview); [box / violin / beeswarm](https://helpcenter.flourish.studio/hc/en-us/articles/9859136207759-How-to-make-box-violin-and-beeswarm-scatter-plots); [arrow plots blog](https://flourish.studio/blog/make-arrow-plots/); [dot vs scatter blog](https://flourish.studio/blog/scatter-vs-dot-plot/) |
| Data explorer | Interactive exploration: packed circles, beeswarm, scatter, or a map view | One **row per entity**; columns tagged categorical (color, aggregation, filter) or numeric (position, size). Optional Geo Regions and Geo Points sheets, joined by key IDs. | Up to about 1,000 rows (limits table). Layouts depend on which columns are bound. | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761567730575-Data-explorer-an-overview) |
| Heatmap | A matrix of magnitude by color, categorical or numeric | One sheet: **X axis**, **Y axis**, **Values**, optional Filter and popup columns | Can use categorical or numeric color palettes. Change the data type of an axis if the chart looks wrong. 3D map also has a heatmap mode — that is a different template. | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761546958479-Heatmap-an-overview) |
| Survey | Individual-level survey answers; dots that animate into groups, bars, a comparison grid, or a map | One **row per respondent**, one **column per question**. Bind categorical columns to Values (Group by / Shade by / Compare); continuous columns to Size by; optional Geographic (must match names in the Places sheet), Label, Slider/menu, Unique name/ID. | Ideal up to about 10,000 rows (20,000 with a filter, per the limits table); larger sets work but more slowly. Default view is a circle; **create a story** to set other default views. Labels are not recommended for more than a few hundred dots. | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761569396879-Survey-an-overview); [default view / stories](https://helpcenter.flourish.studio/hc/en-us/articles/8761563099663-How-to-change-the-default-view-of-your-Survey-visualization) |

### Relationships, networks, and flow

| Template name | Best for | Data shape | Known limits (design-relevant) | Source |
| --- | --- | --- | --- | --- |
| Network graph | Connections between entities; equal-weight or weighted links | Two sheets. **Links** (minimum): Source, Target, optional Value (sets **link width**). **Points** (optional but useful): Id, group (color), size. The Points sheet, if used, defines the complete set of nodes. | Layouts: classic network, directed (arrows on links), radial / packed radial. Link width encodes Value — use 1 for equal weight. **Dashed links: not documented.** Label modes: Auto, All, selected and neighbours, hover, or None; long labels truncate. Forces (repulsion, collision) control layout; animation of the simulation is optional. Popup opacity can be reduced when the chart is busy. Limits table: up to 10,000 rows. Whether two rows with the same Source–Target draw as two links is **unverified**. | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761553784719-Network-graph-an-overview); [network charts page](https://flourish.studio/visualisations/network-charts/) |
| Chord diagram | Weighted relationships or flows among a closed set, in a circle | At least three columns: Source, Target, Value. For **directional** chords, two rows per pair (one each way; a missing reverse flow is 0). For **non-directional**, two rows with the **same** value. | Help-center section title is “Chord”. Chord thickness encodes Value. Highlight syntax: an arc name, or `Arc 1 >> Arc 2`. Directional vs non-directional also affects popups. Not a two-column node-link layout. | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761539049743-Chord-An-overview); [chord page](https://flourish.studio/visualisations/chord-diagrams/) |
| Sankey diagram | Directed flows; alluvial diagrams of how items regroup across steps | **Long** format, one row per record. Bind Source and Target; optional Values; for alluvial, numeric **Step from** and **Step to**. If Values is empty, widths are based on **row counts**. Duplicate source–target rows are aggregated. | Band width (and node size) encode value or row count — nodes with more incident flow grow larger. Alluvials are more rigid (a band at every horizontal step). Names in the no-Values model are compared case-insensitively with non-alphanumeric characters stripped. | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761554356879-Sankey-diagram-an-overview); [data format](https://helpcenter.flourish.studio/hc/en-us/articles/8761554327183-How-to-format-your-data-to-build-classic-and-alluvial-Sankeys); [sankey page](https://flourish.studio/visualisations/sankey-charts/) |

### Hierarchy

| Template name | Best for | Data shape | Known limits (design-relevant) | Source |
| --- | --- | --- | --- | --- |
| Hierarchy | Nested part-to-whole structure | **Long** format, one row per entity. Nest by **categorical** columns; size by **numeric** columns. Click to zoom when nesting two or more columns. | Five types (switch in settings / starting points): treemap, circles / packed circles, radial partition (**Sunburst** starting point), stacked / hierarchical bars, radial tree (also Radial dendrogram, Ranking wheel). Depth setting controls visible levels. | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761561023375-Hierarchy-an-overview); [treemaps page](https://flourish.studio/visualisations/treemaps/) |

### Maps

Core guidance: [When to use which map template](https://helpcenter.flourish.studio/hc/en-us/articles/8827922341519-When-to-use-which-map-template). GeoJSON files in the limits table: up to 5MB.

| Template name | Best for | Data shape | Known limits (design-relevant) | Source |
| --- | --- | --- | --- | --- |
| Projection map | Shaded regions and/or points, spikes, or arrows on a projected map | **Regions geometry** (boundaries) joined to **Regions** by a unique **ID** (must match exactly). Region bindings: ID, Name, Label, Color by, optional Grouped, popup metadata. **Points**: one row per point, longitude and latitude (decimal degrees); optional shade/size. **Lines**: custom GeoJSON. | Does not require WebGL. **Can download as SVG.** 40+ projections. Points can be drawn as spikes or arrows. Best default unless you need larger data, 3D, or a locator marker map. | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761562464911-Projection-map-an-overview); [which map](https://helpcenter.flourish.studio/hc/en-us/articles/8827922341519-When-to-use-which-map-template) |
| Marker map | Points of interest with markers, emoji, icons, or images | **Locations** table: place names and coordinates; marker appearance via upload, URL, emoji, or icons | Optional inset map. Vector, raster, or projection base. | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761553766799-Marker-map-an-overview) |
| 3D map | Large geographic datasets, animated points, region extrusion, map heatmaps | Points with latitude/longitude; optional timestamps; optional GeoJSON regions and polylines | Uses WebGL; supports larger data (limits table: up to 500,000 rows). Heatmaps, inset map, animated timeline. SVG download is not listed among its advantages (WebGL templates may have no image download — see Export tips). | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761538116879-3D-map-an-overview) |
| 3D globe | Global point data, optionally over time, on a globe | Minimum: latitude and longitude columns | Timeline, camera, and globe-surface styling (including satellite) are documented. WebGL. | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761538098191-3D-globe-template-an-overview) |
| Arc map | Geographic relationships drawn as arcs between two places | Two datasets: **Data** (origin/target IDs, optional category, value for arc thickness) and **Locations** (name, unique ID, longitude, latitude). Bind Source location and Destination location to **IDs**, not display names. | Arc thickness encodes the value column. Color: basic source–destination gradient or categorical. This is a **map**, not an Arc diagram. | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761566736015-Arc-map-an-overview) |
| Connections globe | Connections between places on a 3D globe | **Locations** (names, coordinates, codes) and **Values** (source and destination **codes**, optional amounts and categories) | Codes, not names, join values to locations. Globe skins include satellite. WebGL. | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761574167439-Connections-globe-An-overview) |

### Ranking, race, elections, and sports

| Template name | Best for | Data shape | Known limits (design-relevant) | Source |
| --- | --- | --- | --- | --- |
| Sports race | Athletes racing a fixed distance (sprint, swim, etc.) | One row per participant; name plus time columns (finish, laps, or checkpoints). Required time format is specified in the overview (check the article when preparing data). | Built for course-style races, not general bar ranking (use Bar chart race for that). | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761554645263-Sports-race-an-overview) |
| Sports | Lineups and tactics boards on a pitch or court | Player data; bindings depend on sport. Positions are filled in sheet order (e.g. goalkeeper first). | Starting points cover football, basketball, American football, cricket, ice hockey, rugby, tennis, shot charts, and more. | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761554628367-Sports-an-overview) |
| Tournament | Single-elimination brackets | A round column, columns for the two competitors, optional Winner (blank = upcoming), optional scores | Only documented for single-elimination tournaments. | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761555017743-Tournament-an-overview) |
| Parliament chart | Seat totals in a circular or semi-circular chamber, with a results table | One column of party names, plus a column per election to include in the filter | Can show several elections and change over time in one visualization. | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761553852559-Parliament-chart-an-overview) |
| Election results chart | Results against a majority threshold | **Wide** format (a column per party or candidate). Optional **Historical data** sheet to compute percent change. | One overall result, or a dropdown for specific results. | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761523017487-Election-results-chart-an-overview) |

### Text, storytelling, and interactive content

| Template name | Best for | Data shape | Known limits (design-relevant) | Source |
| --- | --- | --- | --- | --- |
| Cards | Grid or carousel of mixed content (images, text, hover/click, audio) | Bind text, images, and other content columns in the Data tab (example in the overview is a set of profiles) | Views: grid or carousel (scrollbar or buttons, optional autoplay). Layouts: Portrait, Landscape, Image overlay; several image/text structures. Custom card HTML is available. Up to about 2,000 rows (limits table). | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761573940879-Cards-an-overview) |
| Quiz | Multiple-choice or slider quizzes with feedback and finish cards | Three sheets: **Questions** (question text, input type, correct answer; multiple-choice options separated by `::`), **Feedback** (question name must match exactly; at least two rows per question, **incorrect first**; slider ranges use `-`, `*` for all; ranges are inclusive of the start and exclusive of the end), **End result** (one row per final-score band) | Feedback order matters; a wrong order shows the incorrect message for a correct answer. | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761554288783-Quiz-an-overview) |
| Photo slider | Compare two images (slide, fade, or spotlight) | Two images in Photos settings; optional mobile alternatives | Starting point **Before and after** is for photos, not numeric before/after data. | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761553867535-Photo-slider-an-overview) |
| Text annotator | Highlight passages and attach interactive notes | Paste the full text in Text settings. Data tab: Text snippets + Annotations, one row per note. For repeated phrases, wrap `[text]{identifier}` and use the identifier in the sheet. | Identifiers are the way to reuse one annotation or to disambiguate repeats. HTML/CSS can be added to the text. | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761569636879-Text-annotator-an-overview) |
| Word cloud | Frequent words in a text | Either paste raw text, or a Data sheet of word frequencies (required if you want to color by category) | Pasting raw text can be slow for large amounts of text. Category coloring is only available via the Data sheet. | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761569717647-Word-cloud-an-overview) |
| Interactive SVG | Make a custom SVG diagram clickable | An SVG whose groups have ID attributes, uploaded under Graphic. Data tab: one row per group ID, plus Heading 1, Heading 2, Content (HTML allowed, including images). | Mobile modes: Interactive, Show all, or Accordion. Illustrator compatibility is covered in a separate article. A **Process flow chart** starting point exists, but this is still the Interactive SVG template, not a flow template like Sankey. | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761539216911-Interactive-SVG-An-overview) |
| Calculator | A custom question-and-formula calculator | One row per question, with question type, answer options, and related metadata; formulas/variables are configured in the template | Results can be saved to a Google Sheet (details in the overview). Not a statistical chart. | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761547152783-Calculator-an-overview) |
| Audio | Embedded audio (single or multiple tracks) | **Unverified** in the help center — no overview article was found. The chooser lists starting points **Multiple tracks** and **Single track**. | Featured in the public chooser. Do not invent bindings; inspect the starting-point Data tab in Flourish, or treat format as unverified until documented. | Confirmed in [template chooser](https://app.flourish.studio/templates) only |

**Story editor modes** (not visualization templates in the chooser, but official Flourish storytelling formats):

| Name | Best for | Data shape | Known limits (design-relevant) | Source |
| --- | --- | --- | --- | --- |
| Flourish stories | Multi-step explainers that step through one or more visualizations with captions | A story is a sequence of slides; each slide can hold a visualization and caption | Stories can autoplay, include video or audio, or be a single slide (used to lock a Survey default view). Downloading a story as an image exports only the selected slide. Video download of stories is listed under Premium features. | [Stories category](https://helpcenter.flourish.studio/hc/en-us/categories/12984335680911-Stories-and-scrollies) |
| Scrolly (story editor) | Scroll-driven storytelling | Same as a story; set navigation to Scrolly so captions sit in the center and slide buttons are removed | Documented for **Enterprise and Publisher** customers. No-code scrolly works with **script embeds and HTML downloads**, not iframe embeds. Scrolly captions are **not shown in preview**; publish to review scrolling. | [How to create a scrolly](https://helpcenter.flourish.studio/hc/en-us/articles/8761522702991-How-to-create-a-scrolly-using-the-story-editor) |

### 3D (non-map)

| Template name | Best for | Data shape | Known limits (design-relevant) | Source |
| --- | --- | --- | --- | --- |
| 3D Viewer | Displaying a 3D model (product, architecture, scientific scene), including inside a story | A 3D file: **.glb (binary glTF) recommended**; also glTF, OBJ, FBX. Additional texture files as required by the format. | WebGL. Help-center title is “3D viewer”. Image download may be unavailable for WebGL templates (see Export tips). | [Overview](https://helpcenter.flourish.studio/hc/en-us/articles/8761538217615-3D-viewer-an-overview) |

### Also in the chooser, not featured (limited documentation)

These appear on the public templates page, tagged as Flourish, but they are **not** in the featured list and most have **no help-center overview**. Treat them cautiously; several look like older duplicates of featured templates.

| Name in the chooser | What is confirmed | What is unverified |
| --- | --- | --- |
| **Arc diagram** | Present in the chooser (`data-external-id="arc-diagram"`). A 22 October 2025 entry in the public Flourish Charts changelog adds `@flourish/arc-diagram` at version **0.0.0**. A typical arc diagram places nodes along **one axis** and draws arcs for links — not a two-column layout. | No help-center article was found. Data bindings, dashed-line support, and whether it can pin nodes into two columns are **unverified**. Do not recommend it unless you open a starting point and confirm the layout yourself. |
| Progress chart; Growth comparison; Vega-Lite | Visible in the chooser | No help-center overviews found; data formats **unverified**. Vega-Lite is categorized as `chart,technical`. |
| Region map (3D); Time map: London / New York / San Francisco / USA / the world | Visible; names and older IDs suggest earlier 3D / time-map variants | Likely superseded by **3D map** / **Marker map**, but that relationship is **unverified**. |
| SVG annotator (two entries); older Bubble chart, Gauge, Sports race, Timeline | Visible; names overlap featured templates | Probably legacy versions; prefer the featured templates. |
| Advanced theme editor; Simple theme editor | Visible | These are theme tools, not chart templates. |
| Owned premium standalone security canary; Zky M2 | Visible, **not** tagged `flourish` | Ignore; not product templates. |

---

## 2. Import tips

Source: [Adding data to a template](https://helpcenter.flourish.studio/hc/en-us/articles/8761545383183-Adding-data-to-a-template), [How to auto-set your columns](https://helpcenter.flourish.studio/hc/en-us/articles/8761559290255-How-to-auto-set-your-columns), [How to unpivot your data](https://helpcenter.flourish.studio/hc/en-us/articles/8761537001103-How-to-unpivot-your-data), [How much data Flourish templates can handle](https://helpcenter.flourish.studio/hc/en-us/articles/8827938638991-How-much-data-Flourish-templates-can-handle).

1. **Start from a starting point, then look at its default data.** The default sheet shows the shape the template expects. For Network graph, that means a **Links** sheet and a **Points** sheet at the top left of the Data tab.
2. **Upload or paste CSV or Excel.** Flourish also describes a “Start with data” workflow that recommends templates from a file. You can paste into the datasheet; the help article walks through upload options in an embedded story.
3. **Bind columns on the right of the datasheet.** Single-column bindings (for example Labels/time in Line, bar and pie) take one column. Multi-column bindings (for example Values) accept ranges and lists: `A-E,G` means A, B, C, D, E, and G.
4. **Auto-set columns** can assign bindings after import. As of the 20 February 2026 help article, this exists in: Line, Bar, Pie; Slope; Cards; Hierarchy; Scatter; Radar; Timeline; Sankey; Table; Bar chart race; Line chart race; Marimekko; 3D map; Heatmap; Gauge; and Projection Map. **Network graph is not on that list** — bind Source, Target, Value, and Points Id/group yourself. When re-uploading, untick “Automatically choose column to be visualized after import” if you want to keep existing bindings.
5. **Wide vs long.** Many comparison templates want wide data. Survey, Hierarchy, Gantt, Timeline, Sankey, Marimekko, and Network links want long data (one row per record or link). Flourish can **unpivot** wide columns into a category column plus a value column inside the Data tab.
6. **Dates.** Auto date typing currently recognizes **written months in English only** (a date like `21 février 1967` is treated as text).
7. **Live data from Google Sheets** is documented as a **Premium** feature.
8. **Published data-size estimates** (from the Flourish table embedded in the limits article; figures are approximate and depend on device and page context):

| Template | Published estimate |
| --- | --- |
| Line, Bar, Pie | Around 5,000 rows (10,000 with a filter) |
| Bar chart race | Around 1,000 rows |
| Survey | Around 10,000 rows (20,000 with a filter) |
| Scatter (WebGL mode) | Up to 200,000 rows |
| Network graph | Up to 10,000 rows |
| 3D map | Up to 500,000 rows |
| GeoJSON files | Up to 5MB |
| Data explorer | Up to 1,000 rows |
| Cards | Up to 2,000 rows |

---

## 3. Export tips (SVG, PNG, embed, plans)

Sources: [Understanding image download options](https://helpcenter.flourish.studio/hc/en-us/articles/8761545595791-Understanding-image-download-options), [Exporting, publishing, embedding and sharing](https://helpcenter.flourish.studio/hc/en-us/articles/8761565550607-Exporting-publishing-embedding-and-sharing), [Free accounts vs paid accounts](https://helpcenter.flourish.studio/hc/en-us/articles/8761536676111-Free-accounts-vs-paid-accounts).

- **Free accounts** can use the full template library, create unlimited visualizations and stories, and publish or embed **with Flourish attribution**. Projects are private until published. Once published they appear on a public `public.flourish.studio` page (search-indexed) and in Flourish’s “Latest” feed. Paid plans can prevent projects from being duplicable by default.
- **Image download (PNG and similar) is a paid-plan feature.** The help center states: “Image downloads are offered as part of our paid plans.” Paid-account features also include publishing without attribution, password-protected publish, PowerPoint embeds, logo support, HTML download, email support, and more. Some plans add live data, custom fonts, and scrollytelling.
- **SVG download** is only available for **SVG-based** templates. Canvas-rendered templates (used because they are faster with many items) do not offer SVG. The SVG export is a **vector of the graphic only** — headers and legends are omitted, which is intentional if you will finish the chart in Figma or Illustrator. For print, Flourish recommends SVG when it is available.
- **Some templates have no image download at all**, mainly those that use **WebGL** (interactive 2D/3D). The documented workaround is a screenshot. Projection map is explicitly listed as able to download as SVG and as not requiring WebGL. Whether Network graph is SVG-based is **unverified**.
- **Download HTML** (self-host the project) is only on **Business and Enterprise** plans, plus **legacy Personal** plans.
- **Embed options:** the default is a responsive script embed (height adjusts). Basic iframe and AMP iframe embeds have a **fixed height**, which does not suit some templates. Terms require a Flourish credit and link under iframe embeds. Except on **Presenter, Business, and Enterprise** plans, a link back to Flourish is also required wherever you publish or embed an **image** of a Flourish graphic.
- **Stories:** image download is of the currently selected slide only. Scrolly constraints are in the storytelling table above.

---

## 4. How to recommend a chart from now on

In any visualization recommendation, lead with one sentence that names the Flourish template, for example:

> For equal-weight links between two groups of nodes, use Flourish’s **Network graph** template and set every link Value to 1.

Then add only the data-shape and limit notes the user needs. Prefer parent template names (Scatter, not “the Arrow plot template”; Pictogram, not “the Waffle template”; Hierarchy, not “the Treemap template”).

---

## Sources opened for this guide

- Template chooser: https://app.flourish.studio/templates
- Chart guides hub: https://flourish.studio/visualisations/
- Examples hub: https://flourish.studio/examples/
- Help center home and category indexes, including [Charts](https://helpcenter.flourish.studio/hc/en-us/categories/8636109131791-Charts), [Maps](https://helpcenter.flourish.studio/hc/en-us/categories/8825239695759-Maps), [Tables and heatmaps](https://helpcenter.flourish.studio/hc/en-us/categories/12984386242703-Tables-and-heatmaps), [Content based templates](https://helpcenter.flourish.studio/hc/en-us/categories/12984403849615-Content-based-templates), [Stories and scrollies](https://helpcenter.flourish.studio/hc/en-us/categories/12984335680911-Stories-and-scrollies)
- Overview and how-to articles linked in the tables above (retrieved from the Flourish help-center API, same URLs)
- Marketing pages used to confirm that streamgraph, treemap, box plot, dual-axis, network, Sankey, chord, and heatmap pages map to parent templates: https://flourish.studio/visualisations/streamgraph-maker/, https://flourish.studio/visualisations/treemaps/, https://flourish.studio/visualisations/box-plots/, https://flourish.studio/visualisations/dual-axis-charts/, https://flourish.studio/visualisations/network-charts/, https://flourish.studio/visualisations/sankey-charts/, https://flourish.studio/visualisations/chord-diagrams/, https://flourish.studio/visualisations/heatmaps/
- Blogs: https://flourish.studio/blog/make-arrow-plots/, https://flourish.studio/blog/scatter-vs-dot-plot/
- Data-limits table published as Flourish visualization 7210398 (embedded in the limits help article)
- Flourish sitemap (https://flourish.studio/sitemap.xml) used only to discover public `/visualisations/` URLs
- Flourish Charts changelog (public, used only to confirm that `@flourish/arc-diagram` was added at version 0.0.0): https://github.com/canva-public/flourishcharts/blob/main/changelog.md
