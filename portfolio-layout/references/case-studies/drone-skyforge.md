# Case Study: SkyForge (Drone XR Training) — "final (locked)" Version

Text-only reconstruction of an excellent portfolio project. It is written so a reader who never sees the images can rebuild every page in their head. Quoted copy is verbatim from the Figma layers, typos included (marked *[sic]*). Proportions are approximate and come from reading the screenshots.

## Contents
- 0. Format and global visual system
- 1. Page-by-page description (01–08)
- 2. Detailed logic chain with linking sentences
- 3. Block-writing formulas (with examples)
- 4. Strengths, weaknesses, transferable lessons

---

## 0. Format and Global Visual System

- **Format**: 8 landscape spreads, each 2522 × 1073 (Figma frames). Very wide, about 2.35:1. Reading runs left → right, usually in three columns.
- **Project type**: XR / HCI / game-like training simulator (VR headset + real drone remote controller), built in Unity.
- **Narrative voice**: "We".
- **Background**: dark charcoal page with light-grey rounded panels as content cards. Some panels and conclusion bars are black.
- **Accent**: neon lime green. It marks the "FORGE" half of the logo, conclusion bars, opportunity cards, arrows and highlighted chart series.
- **Section labels (level 1)**: all-caps bold text in a black pill with a white "switch" dot. Labels used: BACKGROUND, RESEARCH, COMPETITIVE ANALYSIS, USER RESEARCH, CONCEPT, GAMEFLOW, SCENE DESIGN, ITERATION PROCESS, MAKING, EXPERIENCE FLOW, CODING, FINAL, USER TESTING.
- **Sub-headlines (level 2)**: all-caps heavy display sans, written as claims, e.g. "INDUSTRY GIANTS DRIVE PILOT DEMAND", "WHERE TRAINING BREAKS DOWN".
- **Body**: small sans, often justified.
- **Recurring components**: conclusion bars (black or lime, bold, centred, one sentence); numbered cards; role-labelled quote cards; ✗/✓ comparison; flowchart with a legend.
- **Colour roles**: lime = opportunity / conclusion / positive. Black card = conclusion or person. Blue sky background = power-line track. Green field background = crop track.

---

## 1. Page-by-Page Description

### Page 01 — Cover
- **Label**: none (cover).
- **Grid**: a full-bleed render fills the spread. A frosted-glass text card covers about the left 45%; the right ~55% is left to the hero image, which shows a crop-spraying drone and a transmission tower, so both use scenarios appear in one picture.
- **Reading order inside the card**:
  1. Logo "sky" (white) + "forge" (lime), very large.
  2. Subtitle: "Cross-Reality Simulation Platform for Drone-Based Industrial Operations".
  3. Thin divider.
  4. Body: "This XR-based mixed reality drone training system integrates VR headsets with real remote controllers for immersive training across two standardized workflows: Power Inspection Module: Simulates 220kV tension towers, wine-glass towers, and cat-head towers in winter and summer conditions. Users operate drones to inspect 14–16 key nodes per tower. Agricultural Plant Protection Module: Replicates farmland boundary mapping and automated pesticide spraying. Users mark spraying zones based on terrain and execute pre-planned flight paths."
  5. Video link: "https://youtu.be/lIF95ye7LO0".
  6. Three pill tags at the bottom: "Mixed-reality", "Drone Simulation", "High realism".
- **Strengths**: the cover states the product, the two modules and concrete parameters (220kV, 14–16 nodes), and links a demo video.
- **Weaknesses**: the long justified paragraph stretches word spacing.
- **Transition**: none explicit. Page 02 opens with market context.

### Page 02 — Background + Research + Competitive Analysis (densest page)
- **Labels**: BACKGROUND (left), RESEARCH (centre), COMPETITIVE ANALYSIS (right-bottom). That is three level-1 labels on one page.
- **Grid**: three columns of roughly equal width. Right column split into top (frictions) and bottom (competitors).

**Left column — BACKGROUND (dark rounded card)**, three stacked blocks:
1. "A GROWING MARKET": a line chart titled "Global drone market size, 2017–2025" (y-axis 💲10B–💲40B, rising line).
2. "GROWTH LANDS IN INDUSTRY". Intro: "Commercial drone activity is uneven. Construction, energy, and agriculture rank as the top three verticals, together accounting for over half the market — each further splitting by asset type." Below it a segmented horizontal bar chart titled "Where drones actually fly — by industry vertical". Rows and shares:
   - Construction: Surveying 40%, Inspection 25%, Progress 20%, Mapping 15%
   - Energy: Pipelines 35%, Power lines 30%, Wind turbines 20%, Solar 15%
   - Agriculture: Crop spraying 40%, Monitoring 30%, Mapping 20%, Other 10%
   - Entertainment: Photography 50%, Film / video 30%, Real estate 20%
   - Row totals 22%, 19%, 16%, 14%
3. "THE WORK DEMANDS COMPOUND SKILL". Intro: "China's drone industry faces a 1 million-pilot talent gap, concentrated in industrial scenarios — power-line inspection, crop spraying, mapping, and emergency response.Among *[sic, missing space]* these four, mapping is largely software-automated; the real flight-skill challenge lies in power-line inspection and crop spraying." Two charts:
   - Bar chart "How fast new pilots are entering the field" (4.5w → 10w → 20w → 22.5w across 2018–2024).
   - Sankey "Where new pilots actually go after certification", with sources AOPA training schools 75%, College programs 20%, In-house corporate 5%, and destination shares 22/19/14/14/12/10/9%.
- **Lime conclusion bar**: "SkyForge focuses on two of these — power-line inspection and crop spraying — where compound skill matters most."

**Centre column — RESEARCH**
1. "INDUSTRY GIANTS DRIVE PILOT DEMAND". Intro: "We mapped the buyer side of power-line inspection and crop spraying to see where pilot demand actually concentrates." Then a Venn diagram: left circle labelled "power-line inspection" (SGCC, China Southern Power Grid (CSG), Other Generation and Grid Utilities, Third-party Power Inspection Service Company, Renewable Energy Plant, Power-focused vocational colleges & training centers); right circle "crop spraying" (Supply and Marketing Cooperative (SMC) System, Rural Agricultural Service Cooperatives, Leading Agribusinesses, OEM-operated service networks (e.g., DJI Agriculture), Agrochemical Companies, Digital Agriculture Platform by Non-agri Conglomerates). Overlap: UAV OEMs and their distribution networks, Full-service UAS operators, training institutions/vocational colleges, Government Departments & Public Institutions.
2. "Training institutions for pilots": four numbered rows, each with a logo (CAAC, DJI and others):
   - "01 — CAAC-Certified Flight Schools: The main pipeline for licensed pilots. All UAV license exams are channeled through CAAC- or AOPA-approved schools — individuals cannot register directly with the regulator."
   - "02 — Employer In-House Training: Public-safety, utility, and municipal units increasingly train existing staff in-house — cost-effective, and employees already know the operational context."
   - "03 — Manufacturer-Run Academies: Product makers training their own operators. Leading OEMs leverage their hardware and field scenarios to run proprietary training systems."
   - "04 — Higher Education (Undergraduate + Vocational): The fastest-growing degree-based channel. A new undergraduate major — "Low-Altitude Technology & Engineering" — has been added, alongside the established vocational track in UAV Application Technology."
- **Black conclusion bar**: "However different their scope, depth, and standards, all four channels still rely on the same physical process — a real aircraft, cleared airspace, and a live instructor, all at once."

**Right column top — "WHERE TRAINING BREAKS DOWN"**
- Intro: "Across every institution type surveyed above, real-world pilot training runs into the same five frictions."
- Five numbered frictions. The numbers are large and staggered in height like a staircase, and there is a cut-out photo of a person with a drone:
  1. "Low throughput — Each trainee needs a real aircraft, an instructor, and a cleared field at the same time — the process scales poorly against the growing pilot shortfall."
  2. "Weather-dependent — Wind, rain, fog, and low visibility regularly cancel training days, especially for outdoor verticals like power-line inspection and crop spraying"
  3. "High cost of real-world mistakes — A miscalculation in live flight can mean a damaged drone, a damaged asset, or an injury — pushing instructors to keep trainees inside a narrow safety envelope."
  4. "Hard to rehearse complex tasks — Industrial scenarios — a specific tower under a specific wind, or a specific field at a specific crop stage — are nearly impossible to reproduce on demand…"
  5. "Restricted airspace and limited training sites— now tighter under the 2026 low-altitude regulations." (with a detail line on no-fly zones, time windows and pre-flight clearance)

**Right column bottom — COMPETITIVE ANALYSIS**
- Intro: "We benchmarked the four simulators most cited, scoring each across six dimensions."
- Four identical cards, each with a screenshot, name, company · country, a one-line positioning, and a six-axis radar (Physics / Scenario / Immersion / license / Devices / Access):
  - SIMUUAV (SESP-U1 / STS-H1), Wuhan Aoreier · China: "The CAAC-native challenger — scenes built around the official exam."
  - DJI Flight Simulator, DJI · China: "The default in Chinese training centers — bundled with DJI's industrial fleet."
  - ZEPHYR Drone Simulator, Little Arms Studios · USA: "The global standard — FAA-certified, used most widely."
  - SIMLAT C-STAR / INTER, SIMLAT · Israel: "The high-end professional rig — 80+ deployments across 30+ countries."
- **Conclusion bar**: "Each leads on a different axis, but none combines real-controller immersion, industry-specific scenarios, and low-cost deployment in one product."
- **Strengths**: every column ends with a one-sentence verdict. Reading only the three bars gives the whole argument: focus → common bottleneck → market gap.
- **Weaknesses**: text and chart labels are very small; three level-1 labels on one page cause overload.
- **Transition**: the gap is stated; page 03 goes on-site to find root causes.

### Page 03 — User Research
- **Label**: USER RESEARCH. Sub-blocks: On-site research, User journey map, interview Keywords, PERSONA, PAIN POINTS AND OPPORTUNITIES.
- **Grid**: left column ~1/3 (on-site research + keywords + conclusion); centre-top wide band (journey map); centre-bottom (three personas); right column (pain → opportunity).
- **Left column**:
  - Intro (place credential): "We visited TianJiHui UAV Training Center, a CAAC-authorized drone-training institution and one of Hefei's well-known training bases. It runs real-aircraft training for both certification students and working pilots — around [400–500] *[sic, leftover brackets]* trainees a year. We sat down with trainees and the institution's head to hear where real-world training actually breaks down."
  - Three role cards (label + credential + quote + photo):
    - TRAINEE, "2–3 months in · heading into power-line inspection": "The sim has no inertia — push the stick and it goes. The real aircraft lags and drifts, and weather never gets into the computer's math."
    - INSTRUCTOR, "front-line flight coach": "One trainee ties up one real drone, one instructor, and one cleared field — a specific tower under a specific wind is almost impossible to reproduce on demand."
    - INSTITUTION HEAD, "runs a school training 400–500 pilots/year": "What I care about is cost-performance and a real experience; what I worry about is whether the training actually transfers and gets students on the job faster."
  - "interview Keywords" bubble cloud: Cost of mistakes, Unreal stick feel, The impact of weather, Job-transfer gap, Repeated training that can be done anytime, Compound-skill gap, Can't reproduce scenes.
  - Black bar with lime text: "What's missing isn't more flight hours — it's physical feedback, reproducible scenes, and real job transfer in one system."
- **Centre — User journey map**:
  - Intro: "I went through the complete drone-pilot training pipeline myself — from classroom theory to real-aircraft flight — and mapped where the experience breaks down for a new trainee." (Here the voice switches to "I".)
  - Ten numbered steps laid out in a U: top row 1→5 left to right (Classroom theory, Tutored question, Drone components, PC simulator practice, Route & mission study), bottom row 6→10 right to left (Pre-flight check, First real flight, Logging more reps, Review the process, Instructor flight review). A "User sentiment curve" runs between the rows. Each step has a real photo and a "PAIN:" line, e.g.:
    - "PAIN: Knowledge stays on paper — you memorize the rules but never see what flying actually looks like"
    - "PAIN: Everything revolves around the license; passing the test ≠ doing the job"
    - "PAIN: componentsMany *[sic]* trainees share one unit…"
    - "PAIN: Push the stick and it flies — no inertia, no drift, no wind; skills don't transfer to a real aircraft"
    - "PAIN: One aircraft, one instructor, one field — no parallel practice, so real flight time is heavily diluted"
    - "PAIN: Logging is manual with no objective replay, so progress is hard to quantify"
- **Centre-bottom — PERSONA**: three dark cards. Chen "Power-line pilot · 28", Lin Fei "Crop-spray pilot · 34", Teacher Lin "Sim-training lead · 36". Each has four slider scales (Cautious–Bold, Low tech–High tech, Theory–Hands-on, Low risk–High risk) and three goals, e.g. "Master complex-terrain hover, crash-free", "Regain feel fast after off-season", "Cut beginner crash rate, save budget".
- **Right — PAIN POINTS AND OPPORTUNITIES**: three pain cards in black, each paired with a lime opportunity card:
  - "No physical fidelity — the sim has no inertia, drift, or wind, so skills never transfer to the real aircraft." → "Real physics in simulation — a real controller plus a physics model makes practice transfer to the aircraft."
  - "Scenes can't be reproduced or scaled — training is locked to flat, open ground with one aircraft and one trainee at a time." → "Any scenario, on demand — VR generates confined, job-specific scenes anytime, for multiple trainees in parallel."
  - "Feedback has no data — logging is manual, progress is hard to quantify, and the same scenario can't be replayed." → "Every flight becomes data — objective tracks and replay make feedback measurable and scenarios re-runnable."
- **Strengths**: the evidence moves from institution to roles to the author's own experience. The three pains map one-to-one onto three opportunities.
- **Weaknesses**: the personas sit after the synthesis and add little to the argument; the typo and the placeholder brackets were not cleaned up.
- **Transition**: the three opportunities become the design principles on page 04.

### Page 04 — Concept
- **Labels**: CONCEPT, GAMEFLOW. Sub-blocks: WHY VR + REAL CONTROLLER, WHY these two drone domains, product introduce, Interaction mode selection, system design.
- **Grid**: three columns, each split top and bottom (six sub-blocks).
- **Left-top — WHY VR + REAL CONTROLLER**:
  - Quote card INSTRUCTOR: ""I need to see where the drone really is in the air — judging position and distance by eye is the whole skill." —on-site interview".
  - "From the above" card: "A pure PC sim has no physical feel; a real aircraft is costly and risky. Pairing a VR headset with a real flight controller keeps the true stick-and-physics feel while making the scene reproducible, safe, and cheap."
  - A lime down-arrow leads to a visual equation of icons: "VR deceive *[sic: device]* + drone controller = XR".
- **Left-bottom — WHY these two drone domains** (overlaid on a tower photo). Lead: "As our market research established, two verticals drive the pilot gap — so we standardize on them:"
  - "Highest pilot demand — power-line inspection + crop spraying lead the 1M-pilot gap (per our Background analysis)."
  - "Hardest to rehearse — exactly the compound-skill scenarios our trainees said can't be reproduced on a real field."
  - "Both standardizable — inspection (14–16 nodes/tower) and spraying (boundary mapping + planned paths) model cleanly as XR tasks."
- **Centre-top — product introduce**: "SkyForge uses a VR headset as the visual terminal and a real flight controller for actual flight control, merging true stick-feel with reproducible scenarios. It targets two vertical engineering domains." Two scene cards:
  - Power-line inspection: "…modeled on transmission lines, with wine-glass, tension, and cat-head towers across summer and winter lighting; trainees fly to 14–16 task nodes and photo-log each, scored by camera coverage."
  - Crop protection: "…reproduces two stages — boundary mapping and spraying execution: trainees mark the spray zone, then one-tap plan the route and trigger automated spraying, scored by coverage progress."
- **Centre-bottom — Interaction mode selection**: "The trainee wears a VR headset connected through SteamVR, while the project runs on the PC. A real drone controller is connected to the computer and used as the main input device." Line drawing of a person in a headset, plus front and back views of the controller with callouts: Left joystick, Right joystick, Wheel ("Adjust the angle of the drone gimbal"), "Confirm button/photo button", "Supports mainstream remote controls that can connect to computers", "Supports two scenarios: power inspection and agricultural plant protection".
- **Right-top — system design**: "Built on Unity 2023 , using the OpenXR standard and input system for headset and interaction support. with a real flight controller integrated for actual flight control." The architecture diagram reads: Trainee (VR headset on / Real controller, Stick input) → input → Simulation engine {Task simulation: Flight physics, nodes · XR scene: Power/agri render · Environment: Season, light, wind · Feedback system: Coverage, replay} → VR view / Feedback. Unity and OpenXR logos are shown.
- **Right-bottom — GAMEFLOW**: two swim-lane flowcharts with a legend (Process / Decision / Start / end / Input / Retry path).
  - Shared start: Start → Bind controller ("First: 8-step calibration / Else: load profile") → Select scene (Power / Crop).
  - Power inspection: Select tower (3 types · unlock) → Fly to node (14–16 in order) → "Collision? hit?" (Yes → reset & unlock) → "Coverage? ≥ threshold" (No → adjust position) → Shutter (capture node; more nodes → next) → Results (time/collisions).
  - Crop protection: Unlock flight (gesture trigger) → Mark zone (confirm vertices) → "Collision?" → "≥ 3 points? area % shown" (No / reselect → re-mark) → Plan & spray (auto route) → Results (time/area %).
- **Strengths**: the concept is derived from two counter-examples plus a compromise; the rationale points back to earlier pages ("per our Background analysis", "our trainees said"); the decision nodes make the scoring rules readable.
- **Weaknesses**: "VR deceive" typo; six sub-blocks on one page.
- **Transition**: the principles are set; page 05 shows the scenes and interaction being designed and built.

### Page 05 — Scene Design + Iteration Process + Making
- **Labels**: SCENE DESIGN (left), ITERATION PROCESS (right-top), MAKING (right-bottom).
- **Grid**: left ~1/3 column; right ~2/3 split top and bottom.
- **SCENE DESIGN**: intro "Four training scenes were built, each pairing a specific tower type or task with a distinct season and wind condition — so trainees rehearse the same skills across the real range of weather and difficulty they'll face on the job." Four line-art cards, each with a lime vertical bar on the left:
  - "Scene 1 · Tension Tower — Summer, light breeze. The baseline inspection scene: clear conditions and stable air."
  - "Scene 2 · Cat-head Tower — Cloudy, strong wind. The hardest scene: low light, and heavy wind that test precise hover and drift control."
  - "Scene 3 · Wine-glass Tower — Winter, moderate wind. Flatter light and gusts that force constant attitude correction during inspection."
  - "Scene 4 · Farmland — Wheat field. The crop-protection scene: boundary mapping and automated spraying over open terrain."
  - Black "Visual style" card: "A stylized, realistic rendering — clean enough that task targets and depth cues stay clear inside the headset, while season, lighting, and weather still make each scene feel like a real engineering site."
- **ITERATION PROCESS**: intro "We iterated the interaction display to make the training experience closer to real drone operation. The goal was to reduce the gap between watching a simulation and actually controlling a drone." Two panels side by side:
  - Red ✗ "PLan1 — Floating Screen View": process "Enter the VR scene / Hold the real drone controller / View a large virtual screen / Control the drone with the real controller / Read camera view and mission data on the screen". Ratings: Immersion "Feels like watching a monitor", Readability "Large screen is easy to read", Realism "Controller is separate from view", Training Transfer "Limited body-control connection".
  - Green ✓ "PLan2 —Controller-based View": the process text is identical to Plan 1 *[weakness]*. Ratings: Immersion "Feels closer to real operation", Readability "Controller screen stays in view", Realism "Hands, sticks are connected", Training Transfer "Close to reality".
- **MAKING**: a timeline with four phases (Environment Foundation → Training System Development → System Assemble → Expand) and six numbered cards (1 Scene Building, 2 Mission Design, 3 Feedback System, 4 Controller Integration, 5 VR Setup, 6 Scene expansion). Each card has small process screenshots captioned Creating terrain, Vegetation design, Modeling, Coding, Reference textbook, Component fabrication, Making UI Canvas, Editing unity input system, Remote control testing, Cat-head Tower/Cloudy, Wine-glass Tower/Winter, Farmland.
- **Strengths**: the scene cards follow "condition + difficulty role + skill trained"; ✗/✓ is compared on the same four dimensions.
- **Weaknesses**: duplicated process text; the MAKING screenshots are tiny and mostly show effort rather than decisions.

### Page 06 — Experience Flow
- **Label**: EXPERIENCE FLOW.
- **Grid**: a narrow left column for onboarding; two wide horizontal bands in the middle (top: POWER-LINE INSPECTION on a blue-sky background; bottom: CROP PROTECTION on a green-field background); a narrow right column for results. Huge translucent words (START / STEP4:PRACTICE / STEP5:REVIEW) sit in the background as navigation.
- **Left**: "STEP1:Wear VR headset and real controller" → lime arrow → "STEP2 : first time of bind real controller" → "STEP3 : select mission".
- **Inspection band** (five in-game screenshots, one caption each): "Arm the drone with the inward or outward stick gesture." / "Unlock successful. The drone is ready for operation." / "Follow the guide line and fly to each target point." / "Capture is only allowed when the target coverage reaches the required value." / "If a collision occurs, the mission restarts after 3 seconds."
- **Crop band**: "Arm and take off the drone, then confirm the target farmland area on the map." / "Fly to the guide point to confirm the selected operation area." / "The system calculates the farmland coverage percentage for area-selection evaluation." / "Confirm the area and generate an automatic flight route within the selected boundary." / "Start the automatic operation and monitor the drone status in real time."
- **Right (step5:review)**: two result screens, "TRAINING COMPLETED" ("View training time, number of attempts, and completed capture points.") and "MISSION ACCOMPLISHED" ("View training time, number of attempts, and farmland coverage rate.").
- **Strengths**: a U-shaped flow (shared entry → two tracks → shared exit); background colour encodes the track; each caption is one user action plus the system rule or feedback.

### Page 07 — Coding
- **Label**: coding.
- **Grid**: three strictly equal columns, each with a module title, a responsibility paragraph, two code cards with icon titles, and the footer "Selected Implementation Code Snippets".
  - "Universal XR Drone Control System": "Builds the shared control foundation for both training scenarios, including real-controller calibration, input normalization, flight control, arming logic, and responsive drone movement." Cards: "Real Controller Calibration and Input Mapping", "Drone Flight Control and Attitude System".
  - "Power-Line Inspection Training Workflow": "Supports tower and line inspection tasks through 3D route planning, task-zone detection, camera coverage scoring, and threshold-based photo capture." Cards: "3D A* Obstacle-Aware Path Planning", "Power-Line Inspection Capture and Coverage Scoring".
  - "Crop Autonomous Spraying Workflow": "Covers farmland boundary mapping, coverage evaluation, and autonomous spraying. The 3D A* planner is embedded inside the sweep-route generation step to convert scan lines into safe flight paths." Cards: "Agricultural Area Mapping and Coverage Evaluation", "Automatic Sweep Route Generation and Execution".
- **Strengths**: the architecture is legible from the titles alone (one shared base + two workflows).
- **Weaknesses**: the code itself is unreadable; an algorithm diagram (A* path, coverage map) would carry more information.

### Page 08 — User Testing + Final + Future Work
- **Labels**: final, USER TESTING, FUTURE WORK.
- **Grid**: a narrow white card on the left (testing); the right ~3/4 is a FINAL image collage: one large hero render, three smaller renders (tower close-up, tower from below, spraying) and three exhibition photos of real visitors wearing the headset.
- **USER TESTING**: intro "We invited the original interview participants — including a trainee, an instructor, and a training-center manager — to test the early SkyForge prototype." Three photo + black speech-bubble pairs:
  - "This simulator's drone handling feels identical to real flight training. —TRAINEE"
  - "the repeatable scenarios useful for teaching specific flight mistakes. However, they also need a wider range of scenarios to cover different real-world situations. —INSTRUCTOR" (sentence is missing its subject)
  - "The manager saw potential in reducing weather dependence, field cost, and one-to-one training pressure. —INSTITUTION HEAD"
- **FUTURE WORK** (black card; the heading is nearly invisible): "Future development will focus on three directions: stronger physical feedback, clearer training evaluation, and better scalability. Wind, drift, and collision warnings will be improved to make the simulation closer to real flight. Replay, scoring, and flight-path records will be added to help instructors review trainee performance."
- **Strengths**: closure. The same three roles from page 03 return; each quote answers that role's original concern; the future directions mirror the three opportunities; the exhibition photos prove the system ran.
- **Weaknesses**: there are no quantitative results (completion time, crash rate, before/after coverage).

---

## 2. Detailed Logic Chain

One line: **market gap → the training process itself is the bottleneck → frontline users confirm three root causes → "VR + real controller" answers all three → scenes, interaction and code build it → the original interviewees validate it.**

| Step | From → To | Linking sentence (verbatim) |
|---|---|---|
| 1 | Market → scope | "SkyForge focuses on two of these — power-line inspection and crop spraying — where compound skill matters most." |
| 2 | Institutions → shared bottleneck | "However different their scope, depth, and standards, all four channels still rely on the same physical process — a real aircraft, cleared airspace, and a live instructor, all at once." |
| 3 | Bottleneck → frictions | "Across every institution type surveyed above, real-world pilot training runs into the same five frictions." |
| 4 | Competitors → gap (three selling points) | "Each leads on a different axis, but none combines real-controller immersion, industry-specific scenarios, and low-cost deployment in one product." |
| 5 | Field research → root causes | "What's missing isn't more flight hours — it's physical feedback, reproducible scenes, and real job transfer in one system." |
| 6 | Root causes → opportunities (1:1) | No physical fidelity → Real physics in simulation; Scenes can't be reproduced → Any scenario, on demand; Feedback has no data → Every flight becomes data |
| 7 | Opportunities → concept | "From the above … Pairing a VR headset with a real flight controller keeps the true stick-and-physics feel while making the scene reproducible, safe, and cheap." |
| 8 | Concept → scope justification (back-reference) | "As our market research established…", "(per our Background analysis)", "our trainees said can't be reproduced" |
| 9 | Concept → build | Scenes deliver "reproducible scenes", Plan 2 delivers "real feel / transfer", coverage scoring and replay deliver "every flight becomes data" |
| 10 | Build → validation (closure) | "We invited the original interview participants…"; Future work = the three opportunities |

---

## 3. Block-Writing Formulas

| Block | Formula | Example |
|---|---|---|
| Sub-headline | Claim, not a noun | "WHERE TRAINING BREAKS DOWN" |
| Intro line | We + action + purpose | "We benchmarked the four simulators most cited, scoring each across six dimensions." |
| Conclusion bar | Contrast / concession | "However different X… all still Y" · "Each leads on…, but none combines A, B, and C" · "What's missing isn't X — it's A, B, and C" |
| Chart title | A question-like phrase | "Where new pilots actually go after certification" |
| Pain → opportunity | "Pain — cause" paired with "Opportunity — how" | "Feedback has no data — logging is manual…" → "Every flight becomes data — objective tracks and replay…" |
| Quote card | ROLE + credential + concrete quote | "TRAINEE · 2–3 months in · heading into power-line inspection" |
| Journey step | "PAIN: symptom — consequence" | "PAIN: Everything revolves around the license; passing the test ≠ doing the job" |
| Rationale list | Bold verdict — evidence (back-reference) | "Highest pilot demand — … (per our Background analysis)." |
| Competitor card | Name / maker · country / "The ___ — positioning" / same-axis radar | "The global standard — FAA-certified, used most widely." |
| Scene card | Scene N · name — condition. Difficulty role: skill tested | "Scene 2 · Cat-head Tower — Cloudy, strong wind. The hardest scene…" |
| ✗/✓ comparison | Same dimensions, ≤ 5 words each | Immersion: "Feels like watching a monitor" vs "Feels closer to real operation" |
| Flow caption | User action + system rule/feedback | "If a collision occurs, the mission restarts after 3 seconds." |
| Flow decision | "Condition?" + branch outcomes | "Coverage? ≥ threshold" → "No → adjust position" |
| Tech module | Module title + responsibility list | "Builds the shared control foundation… including…" |

---

## 4. Strengths, Weaknesses, Transferable Lessons

**Why it works**
1. Every research block lands on a sentence, so the argument still holds if the charts are skipped.
2. It points back explicitly ("per our Background analysis") and closes the loop with the same interviewees.
3. The evidence ladder climbs from macro data to institutions, competitors, an on-site credential, role quotes, first-person journey, and finally the original participants.
4. A rhythm of three: pains, opportunities, roles, code modules, future directions.
5. Stable visual coding: lime = opportunity/verdict; blue/green = track; ✗/✓ for options; one pill label style throughout.
6. Visible technical depth: architecture, GAMEFLOW logic, A* planning and coverage scoring.

**Weaknesses to avoid**: overloaded pages 02–04; no quantitative validation; typos and placeholders ("VR deceive", "componentsMany", "[400–500]"); duplicated Plan text; unreadable code; justified cover text; a near-invisible "Future work" heading.

**Transferable lessons**
- Close every research block with a contrast conclusion bar.
- Write sub-headlines as claims and put a "We/I + action + purpose" line under each.
- Map pains to opportunities one-to-one (≤ 3) and reuse them as concept principles and future work.
- Justify the concept with two counter-examples plus a compromise, and point back to the earlier evidence.
- Validate with the original interviewees and add at least one quantitative measure.
- Encode parallel tracks with background colour; draw flows as shared entry → branches → shared exit.
- On tech pages, let module titles and responsibility lines carry the meaning; prefer algorithm diagrams to code screenshots.
