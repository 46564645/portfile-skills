# Narrative Logic Chains (Cross-Case Synthesis)

Use this file when a user's portfolio has a weak or broken argument: pages that don't follow from one another, research that never reaches a design decision, a concept without justification, or validation that doesn't close the loop. Also use it when writing or rewriting headlines, intro lines, conclusion bars or captions, and before a portfolio ships.

It distils three reviewed cases, each of which has a full text description:
- **[D]** SkyForge (drone XR training), `case-studies/drone-skyforge.md`
- **[R]** RescuePod (flood-rescue wearable), `case-studies/rescuepod.md`
- **[C]** CHITOLOOP (chitosan pond modules + circular service), `case-studies/chitoloop.md`

These are observed patterns, not mandatory templates. Recommend them as directions that fit the user's problem (see `case-analysis-method.md`). `logic-framework.md` covers the macro skeleton (WHY → HOW → WHAT, Inspiration → Research → Development → Final). This file covers the sentence-level and page-level links inside that skeleton.

## Contents
- 1. Glossary
- 2. The core idea: a chain of verdicts
- 3. Logic-chain patterns (A–L)
- 4. Block-writing formula library
- 5. Page archetypes: what each must contain
- 6. Pre-ship checklist
- 7. Common chain breaks (diagnosis cues)

---

## 1. Glossary

Use these terms consistently in advice.

- **Logic chain**: the ordered causal steps of a project, each justified by the step before it.
- **Conclusion bar**: one emphasised sentence (a tinted or dark strip) that ends a block and states its verdict.
- **Intro line**: one sentence under a heading saying what was done and why ("We/I + action + purpose").
- **Back-reference**: an explicit pointer to earlier evidence ("per our Background analysis").
- **Closure**: the ending returns to the opening problem, people or variables.
- **Page archetype**: a page's job (cover, research, interview, insight, concept, system, making, iteration, testing, field test, final, roadmap).

## 2. The Core Idea: A Chain of Verdicts

In all three cases, a reviewer can skip every chart and still follow the project by reading only the headlines, intro lines and conclusion bars. Each verdict sets up the next block.
- [D]: "SkyForge focuses on two of these…" → "…all four channels still rely on the same physical process…" → "…none combines real-controller immersion, industry-specific scenarios, and low-cost deployment…" → "What's missing isn't more flight hours — it's…"
- [C]: "Overproduction swamps the market…" → "Farmers produce what markets don't want…" → "The death of Elodea in high temperatures is the primary cause…" → "Core risk window = Jun–Aug…"

**Diagnostic test**: list only the user's headings and bold sentences in order. If that list does not tell the story, the problem is the logic, not the layout.

---

## 3. Logic-Chain Patterns

### A. Problem Funnel (macro → group → place → measurable variables) — [R], [D], [C]
Narrow one level at a time, and hand over each level with a conclusion bar.
- [R]: flood trend ("rebounded to 26 in 2024") → responders ("…systematic protection of their safety has been overlooked.") → place ("the last 100 meters is where mobility support ends and exposure begins.") → variables ("Risk Trio — Drop. Flow. Obstacles.").
- [D]: market → two verticals → training process → five frictions.
- **Use when** the topic starts broad (climate, industry, society).
- **Fails when** the funnel stops at "people suffer" and never reaches something designable or measurable.

### B. Reframing (the problem is not X, it is Y) — [C], [D]
Turn the obvious framing into a sharper one, with an evidence chart for each turn.
- [C]: "oversupply" → "Farmers produce what markets don't want (60% small) and can't produce enough of what markets demand (10% large)." (Sankey + two ring charts.)
- [D]: "What's missing isn't more flight hours — it's physical feedback, reproducible scenes, and real job transfer in one system."
- **Formula**: "What's missing isn't X — it's A, B, and C." / "X produce what … don't want and can't produce enough of what … demand."

### C. Root-Cause Drill-Down — [C], [R]
Ask successive questions until one causal sentence remains.
- [C]: Q1 (other size factors?) → Q2 (how does die-off affect crayfish?) → Q3 (tried solutions?) → "The Critical Discovery: The death of Elodea in high temperatures is the primary cause of poor crayfish quality."
- [R]: "Where exactly is it most dangerous in a rescue?" → three Insights → one bar.

### D. Naming the Problem — [R], [C]
Give the core problem a memorable name and a visual code, then reuse both to the last page.
- [R]: "Dark Water" → "Risk Trio" with red/blue/yellow icons, reused on pages 03–11.
- [C]: the project name "CHITOLOOP" is the concept (a material loop), delivered on pages 05 and 09.

### E. Time-Window Targeting — [C]
Plot supply and demand on one time axis and mark the gap. The gap becomes the period the design has to work in.
- [C]: "Core risk window = Jun–Aug: habitat demand peaks while supply bottoms." Add a user rule of thumb as a numeric target: "Around 50–60% coverage keeps shelter, food, and oxygen in balance."

### F. Opportunity Mapping (pain ↔ opportunity, 1:1) — [D]
Each pain gets exactly one opportunity with parallel wording. Reuse the set as concept principles and as Future work.
- [D]: "No physical fidelity" → "Real physics in simulation"; "Scenes can't be reproduced" → "Any scenario, on demand"; "Feedback has no data" → "Every flight becomes data". Future work then names "stronger physical feedback, clearer training evaluation, and better scalability".

### G. Concept Justification — [D], [R]
Derive the concept; don't just announce it. Two forms appear:
- **Counter-examples + compromise** [D]: "A pure PC sim has no physical feel; a real aircraft is costly and risky. Pairing a VR headset with a real flight controller keeps…"
- **Derivation by elimination** [R]: "Facing the current" / "Torso already loaded" / "Hands are occupied" / "Risk appears underfoot" → "The anterior shin is the device's primary sensing placement…"
- Always add **back-references**: [D] "(per our Background analysis)", "our trainees said can't be reproduced".

### H. Variable → Module → Feedback → Test → Final Mapping — [R] (also [D])
Each problem variable owns one technical module, one output pattern, one test and one final-page element.
- [R]: Drop → ultrasonic → red + continuous vibration → Drop Test → "Drop Alarm"; Flow → differential pressure → blue + rhythmic → Flow Test → "Flow Alarm"; Obstacles → inductive → yellow + pulse → Obstacles Test → "Obstacles Alarm". Then add an interaction test: "Multi-factor Priority Test".
- [D]: three opportunities → scenes (reproducible), Plan 2 (real feel), coverage scoring and replay (data).

### I. Co-Creation Funnel — [C]
Recruitment + agenda → each role's quote → one design instruction per role → at most three parameterised attributes → concept options.
- [C]: chemist / farmer / ecologist → "Use bio-based chitosan…" / "Provide a vertical shelter…" / "Replicating with pleated textures…" → Chitosan / Structure ("18–30 cm… 1–2 cm gaps") / Texture → "Chitosan Disks" vs "Chitosan Reeds".

### J. Iteration Bands — [R], [D], [C]
Show versions as rows: what changed → Issue → (last row) Conclusion. Compare options on the same dimensions.
- [R]: Ver.001 → 002 → 003 with "Issue:" lines and a final "Conclusion:"; V1 → V2 with mirrored names ("Too Narrow" ↔ "Wider").
- [D]: ✗ Plan1 vs ✓ Plan2 on Immersion / Readability / Realism / Training Transfer.
- [C]: failed / failed / success material tests, each with a mechanism; the losing structure gets "secondary/adjacent habitat".

### K. Layered Validation — [R], [C], [D]
Build credibility step by step: single-factor lab test → combined/controlled test → real context → scored or behavioural evidence.
- [R]: four "To verify…" tank tests → river test → six-dimension scores (lowest highlighted → next iteration).
- [C]: structure comparison (72% vs 48%) → 4-week control (77% vs 27%) → one-day pond observation → farmer "decided to keep the modules".
- [D]: qualitative quotes only. This is a gap; add a metric.

### L. Closure — [D], [C] (missed in [R])
The ending brings back the opening people, variables or problem.
- [D]: "We invited the original interview participants…"; each role's quote answers its page 03 concern.
- [C]: the trial returns to the Qianjiang farmer; the roadmap ends on "- 20% Unsold crayfish" and "+ 8–12% Household revenue".
- [R] miss: the final page does not return to "the last 100 meters", and the tester was not an interviewee.

---

## 4. Block-Writing Formula Library

Write portfolio copy in English. One formula per block type; examples are verbatim.

| Block | Formula | Example (case) |
|---|---|---|
| Sub-headline | A claim or a question, not a bare noun | "WHERE TRAINING BREAKS DOWN" [D]; "What makes the "last 100 meters" so dangerous?" [R] |
| Intro line | We/I + action + purpose | "We benchmarked the four simulators most cited, scoring each across six dimensions." [D]; "To identify a workable forming route…, I ran a series of chitosan substrate tests." [C] |
| Conclusion bar (concession) | However different X…, all still Y | "However different their scope, depth, and standards, all four channels still rely on…" [D] |
| Conclusion bar (gap) | Each leads on…, but none combines A, B, C | [D] competitor bar |
| Conclusion bar (reframe) | What's missing isn't X — it's A, B, C | [D] |
| Key-term emphasis | Bold or tint the term that the next page picks up | "**last 100 meters**" [R] |
| Chart title | Question-like phrase about what to read | "Where new pilots actually go after certification" [D] |
| Quote card | ROLE · credential → concrete quote → Insight | "TRAINEE · 2–3 months in…" [D] |
| Journey step | PAIN: symptom — consequence | "PAIN: Everything revolves around the license; passing the test ≠ doing the job" [D] |
| Pain ↔ opportunity | Pain — cause / Opportunity — how | [D] |
| Rationale | Bold verdict — evidence (back-reference) | "Highest pilot demand — … (per our Background analysis)." [D] |
| Elimination | Constraint: fact, so … | "Hands are occupied — …so interaction must be fully hands-free." [R] |
| Scope set | Scope set: X; two reasons; one exclusion + why | [C] |
| Tech spec | Method + threshold + output (+ source of threshold) | "Kalman-filtered ultrasonic range; alert if distance > 50 cm…" [R] |
| Tech module | Module title + responsibility list | "Builds the shared control foundation… including…" [D] |
| Transition | With X verified…, the next step is Y | [R] page 05 |
| Version row | Ver.N name — change — Issue / Conclusion | [R] page 06 |
| Mirrored fix | Problem name ↔ antonym fix name | "PLA Not Durable Enough" ↔ "Carbon-Nylon Shell" [R] |
| ✗/✓ comparison | Same dimensions, short phrases | "Feels like watching a monitor" vs "Feels closer to real operation" [D] |
| Failed test | Test N – method (failed) + one-line mechanism | "no crosslinking; the acidic film rehydrates" [C] |
| Test block | To verify… → 3 frames → conclusion | [R] page 09 |
| Controlled test summary | Condition, duration: treated n/N (%) vs control n/N (%) | "77% (23/30) vs 27% (8/30)" [C] |
| Score card | Dimension + big score + evidence; lowest in alert colour | "Weight Balance 3.5" [R] |
| Flow caption | User action + system rule/feedback | "If a collision occurs, the mission restarts after 3 seconds." [D] |
| Scene card | Scene N · name — condition; difficulty role; skill trained | "Scene 2 · Cat-head Tower — Cloudy, strong wind. The hardest scene…" [D] |
| Roadmap | Short / Mid / Long; KPIs, or Partnerships – Actions – Outcomes | [C] page 09 |

---

## 5. Page Archetypes: What Each Must Contain

| Archetype | Must contain | Seen in |
|---|---|---|
| **Cover** | Name; a one-line positioning ("turning invisible risks into clear visual–haptic alerts"); 2–3 tags; a hero image that *demonstrates* the use; optional demo link | [D] 01, [R] 01, [C] 01 |
| **Background / research** | A macro chart with a labelled key point; a narrowing step; a conclusion bar that states the focus | [D] 02, [R] 02, [C] 01–02 |
| **Competitive / existing solutions** | Same-dimension cards (name / maker / one-line positioning / same axes) + a gap sentence | [D] 02 (missing in [R], [C]) |
| **Interview** | Place/credential; role + credential + concrete quote; Insight per quote; one synthesis sentence | [D] 03, [R] 02–03, [C] 02 |
| **Insight / root cause** | A named problem or reframe; a visual of the gap (time axis, annotated scene); ≤ 3 variables or opportunities | [R] 03, [C] 03, [D] 03 right |
| **Concept** | Back-referenced justification (counter-examples or elimination); a visual equation or placement figure; scope rationale | [D] 04, [R] 04 |
| **System** | Input → core → output diagram, or a service loop with sources and recovery; a legend for flows | [D] 04, [R] 04–05, [C] 05 |
| **Making** | Ordered, numbered steps with photos; exploded view with labels; process tied to decisions | [R] 07, [C] 06, [D] 05 |
| **Iteration** | Version rows or ✗/✓ on the same dimensions; Issue → Conclusion; mirrored names | [R] 06, 08; [D] 05; [C] 05 |
| **Testing (lab)** | "To verify…"; props/controls; frames; per-test conclusion; one combined or controlled test with numbers | [R] 09, [C] 06–07 |
| **Field test** | Real user and context (ideally an original interviewee); numbered tasks; informative feedback; scores with scale and n | [R] 10, [C] 08, [D] 08 |
| **Experience flow** | Shared entry → tracks (colour-coded) → shared exit; one action + feedback caption per frame | [D] 06 |
| **Final** | A hero in real context; final features that repeat the problem variables; real-use or exhibition proof | [D] 08, [R] 11, [C] 08 |
| **Roadmap / future** | Future work that mirrors the opportunities; phases with named partners; projections visibly marked as projections | [C] 09, [D] 08 |

**Density note (observed)**: the pages flagged as overloaded in every case are the research pages that stack several level-1 labels ([D] 02 has three; [R] 02 has three) or many sub-blocks ([D] 04 has six). Recommend splitting those pages rather than shrinking the type.

---

## 6. Pre-Ship Checklist

Copy this, check each item, fix, and re-check until every item passes.

```
Logic
- [ ] Reading only headings + intro lines + conclusion bars tells the whole story.
- [ ] Every research block ends with a conclusion bar that the next block picks up.
- [ ] The core problem has one name, used identically on every page.
- [ ] Pains and opportunities pair 1:1, and they reappear in concept, tests and future work.
- [ ] The concept page points back to specific earlier evidence.
- [ ] Each problem variable has a module, a feedback pattern, a test and a final-page element.
- [ ] Validation includes at least one number (score, rate, time, count) with its scale and n.
- [ ] Field testing uses the original interviewees or context, or the page says why not.
- [ ] The last page answers the opening question.
Evidence integrity
- [ ] Every statistic has a source or data-collection note; every threshold has a reason.
- [ ] Percentages match their fractions (e.g. 24/30 = 80%, not 83%).
- [ ] Projections are styled differently from measured results and give their basis.
- [ ] Claims match the sample (no plural "users" for n = 1; no "successfully" for one tank).
Copy hygiene
- [ ] Product and component names are identical everywhere (no RescuePod/Eddyline/EddyLine).
- [ ] No typos, placeholder brackets ("[400–500]"), hidden "Text" layers, or leftover labels.
- [ ] No duplicated paragraphs across versions or pages.
- [ ] Headings contrast enough with the background to be read.
- [ ] Body text is not stretched by justification.
```

---

## 7. Common Chain Breaks (Diagnosis Cues)

| Symptom on the user's page | Likely break | Fix pattern |
|---|---|---|
| Lots of charts, no stated takeaway | No verdicts | Add conclusion bars (§2, §4) |
| Research ends at "users suffer" | Funnel stops early | A. Problem funnel to measurable variables |
| Concept appears out of nowhere | No justification | G. Counter-examples or elimination + back-references |
| Personas or journey maps that change nothing | Orphan method | Tie each method to a pain or opportunity, or cut it ([D] personas) |
| Process photos without decisions | Effort, not reasoning | J. Iteration bands with Issue → Conclusion |
| Tests only say "it works" | Flat validation | K. Layered validation + numbers |
| Final page lists features unrelated to the research | No closure | H mapping + L closure |
| Code screenshots nobody can read | Wrong evidence form | Module title + responsibility line, or an algorithm diagram ([D] 07, [R] 05) |
