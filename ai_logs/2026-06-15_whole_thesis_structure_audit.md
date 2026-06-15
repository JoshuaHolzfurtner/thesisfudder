# Whole-Thesis Structure Audit

Date: 2026-06-15

Task: whole-repository structural review of the current thesis draft, with emphasis on argument flow, repeated material, missing bridges, contribution balance, and cleanup targets.

Boundary: this is a structural audit, not thesis prose and not thesis evidence. It does not add results, participant numbers, implementation facts, citations, or interpretations. Suggestions that depend on data or author-only details are marked as such.

## Executive Verdict

The thesis has a strong central idea and a surprisingly disciplined caution structure: it repeatedly frames the project as a comparison between movement-congruent ergometer representation and sport-faithful boat/oar representation, without assuming one is superior. That spine is good and worth preserving.

The current manuscript is also heavily front-loaded. Chapter 1, Chapter 2, and Chapter 4 contain substantial scaffold prose, while the declared primary contribution, the system/prototype, is still almost empty. Results, discussion, and conclusion are also placeholders. In its current state, the thesis reads more like a carefully prepared framing and method plan than a system-and-evaluation thesis.

The main structural task is not to add more theory. It is to move the manuscript's center of gravity toward the built XR rowing mechanism, the two concrete mappings, and the evaluation pipeline.

## Current State Snapshot

- `main.tex` includes seven chapters plus appendices.
- Active prose exists mainly in:
  - `chapters/01_introduction/*`
  - `chapters/02_theoretical_background/*`
  - `chapters/04_study_design/*`
  - questionnaire and study-material appendices
- Placeholder chapters:
  - `chapters/03_system_prototype.tex`
  - `chapters/05_results.tex`
  - `chapters/06_discussion.tex`
  - `chapters/07_conclusion.tex`
- Frontmatter placeholders remain in:
  - `frontmatter/abstract.tex`
  - `frontmatter/acknowledgements.tex`
  - `frontmatter/title_page.tex` is not active, but still placeholder
- Existing evidence/audit packs are strongest for:
  - Chapter 1 motivation and core design tension
  - Chapter 4 questionnaire and method rationale
- The project already has a useful second-opinion outline in `New_Outline.md`, which recommends moving rowing basics earlier, compressing embodiment genealogy, demoting long related-work lists, and naming alignment/IK as system contributions.

## What Is Working

### 1. The core tension is clear

The thesis has a genuinely good central contrast:

- ergometer-congruent representation: preserve the user's actual physical action loop
- boat-realistic representation: preserve the recognizable boat/oar sport depiction

This is stated cleanly in the global notes and appears throughout the introduction, background, and method.

### 2. The overclaim guardrails are unusually good

The draft repeatedly avoids saying:

- the ergometer mode is automatically better
- the boat mode is automatically more embodied
- realistic visuals equal realistic action
- the thesis resolves embodiment theory generally

That caution should stay.

### 3. The method logic is coherent

Chapter 4 already does a good job keeping validated embodiment measures separate from thesis-specific rowing/interface items. It also avoids collapsing realism, preference, comfort, ownership, agency, and self-location into one vague score.

### 4. The citation-audit culture is strong

The existing `SOURCE-CHECK` comments and dossiers are useful during drafting. They make it much harder to accidentally turn adjacent source support into invented findings.

## Main Structural Problems

### Problem 1: The primary contribution is missing from the manuscript body

The contribution hierarchy says the primary contribution is the developed XR rowing mechanism. But `chapters/03_system_prototype.tex` contains only a TODO scaffold.

This creates a structural mismatch:

- Chapter 1 promises a prototype and comparison.
- Chapter 2 explains why the comparison matters.
- Chapter 4 explains how the comparison will be evaluated.
- But Chapter 3 does not yet show the actual system that makes the comparison possible.

This should be the first major writing priority. Without Chapter 3, the thesis risks feeling like a theory/method proposal rather than a completed design-and-evaluation thesis.

Recommended Chapter 3 spine:

1. Design goals and experimental constraints
2. Hardware and software setup
3. Real-virtual alignment and calibration
4. Tracking inputs and inferred body state
5. IK/avatar motion pipeline
6. Shared elements across both modes
7. Ergometer-congruent mode
8. Boat-realistic mode
9. Mode comparison table
10. Implementation limitations relevant to evaluation

Do not make Chapter 3 merely an apparatus inventory. It should explain how the prototype operationalizes the thesis tension.

### Problem 2: The thesis repeats the same mode contrast too many times

The repetition is understandable because the contrast is the thesis spine, but right now many sections restate the same explanation with only small changes.

Core repeated claim:

> The ergometer mode preserves physical/visuomotor congruence with the real ergometer, while the boat mode preserves recognizable rowing-on-water depiction but transforms the felt handle path.

Places where this is repeated:

- `chapters/01_introduction/01_motivation.tex:89-152`
- `chapters/01_introduction/02_core_design_tension.tex:39-145`
- `chapters/01_introduction/03_embodiment_and_experiential_evaluation.tex:7-16`
- `chapters/01_introduction/05_research_objectives_and_questions.tex:4-30`
- `chapters/01_introduction/06_contributions.tex:6-14`
- `chapters/02_theoretical_background/03_visuomotor_congruence_and_synchrony.tex:12-28`
- `chapters/02_theoretical_background/06_rowing_biomechanics_and_ergometer_rowing.tex:12-18`
- `chapters/02_theoretical_background/08_synthesis_for_this_thesis.tex:4-14`
- `chapters/04_study_design/01_design_overview.tex:4-14`

Recommendation:

- Keep the full version in Chapter 1.2.
- Keep a concise theory-facing version in Chapter 2 synthesis.
- Keep a concrete implementation-facing version in Chapter 3.
- Keep a method-facing one-paragraph operationalization in Chapter 4.
- Compress the rest into cross-references or one-sentence reminders.

The thesis should feel like it is moving forward through different layers of the same problem, not circling the same hill from almost identical angles.

### Problem 3: Terminology drifts across the draft

The global framing prefers:

- `ergometer-congruent mode`
- `boat-realistic mode`

The active prose also uses:

- `erg-centered`
- `ergometer-centred`
- `ergometer-based`
- `boat-centric`
- `boat-centered`
- `boat-centred`
- `boat-based`
- `sport-depiction representation`
- `sport-action depiction`

Examples:

- `chapters/01_introduction/02_core_design_tension.tex:40` uses `erg-centered` and `boat-centered`.
- `chapters/01_introduction/05_research_objectives_and_questions.tex:4` uses `boat-centric`.
- `chapters/02_theoretical_background/05_presence_vection_and_stationary_self_motion.tex:8` uses `boat-centred`.
- `chapters/04_study_design/01_design_overview.tex:8` uses `boat-realistic`.
- `notes/01_introduction/02_core_design_tension_evidence_pack_verification.md:113` already flags this.

Recommendation:

- Use `ergometer-congruent` and `boat-realistic` as the official condition names.
- Use `erg-centered` and `boat-centered` only if they are introduced as informal shorthand, and then use that shorthand consistently.
- Avoid mixing US and UK spelling in technical labels. Pick `centered` or `centred`; the global notes lean US-style in some places but not uniformly.
- In methods/results, condition labels should exactly match participant materials and analysis tables.

Possible official naming scheme:

- Full first mention: `ergometer-congruent representation`
- Short label: `ergometer-congruent mode`
- Full first mention: `boat-realistic representation`
- Short label: `boat-realistic mode`

### Problem 4: The research gap needs a more auditable support structure

Chapter 1 currently says the exact comparison "appears to be missing" from the reviewed literature:

- `chapters/01_introduction/04_research_gap.tex:15-18`

This is cautious wording, but the claim still needs an explicit literature-map basis. Existing notes already flag this:

- `notes/01_introduction/dossier_section_1.md:442`
- `notes/01_introduction/dossier_section_1_verification.md:848`

Recommendation:

- In Chapter 1, keep the gap short and cautious.
- In Chapter 2 related work, add a compact table showing what prior rowing/VR sport systems varied or evaluated.
- Add a note or dossier entry documenting the search boundary: which papers/systems were reviewed, what variables they studied, and why they do not constitute the same head-to-head mapping comparison.

Do not claim "no one has studied this" unless that absence claim has a maintained audit trail. Safer wording:

> The reviewed literature offers adjacent VR rowing, rowing simulator, and VR sport systems, but the specific comparison between an ergometer-congruent mapping and a boat-realistic mapping under the same physical rowing task appears to have received limited direct attention.

### Problem 5: Chapter 2 is concise, but it may be ordered backwards for this thesis

Current Chapter 2 starts with virtual embodiment, then moves through agency/ownership/self-location, congruence, tools, presence/vection, rowing biomechanics, related work, and synthesis.

That is defensible. But the thesis hook depends on the reader understanding why ergometer rowing and boat/oar rowing cannot simply be the same mapping. The alternative outline in `New_Outline.md` recommends putting a minimal rowing domain baseline earlier.

Two viable structures:

Option A, current theory-first structure:

1. Virtual embodiment
2. Agency, ownership, self-location
3. Visuomotor congruence
4. Tools and body mapping
5. Presence and vection
6. Rowing biomechanics
7. VR sport/rowing related work
8. Synthesis

Option B, problem-first structure:

1. Rowing and ergometer/on-water mismatch
2. VR/XR embodied interaction baseline
3. Sense of embodiment and subcomponents
4. Visuomotor/spatial/temporal congruence
5. Tools, hands, handle, and body mapping
6. Presence, plausibility, vection as secondary constructs
7. Related XR rowing/sport systems
8. Synthesis

Recommendation:

Option B may serve this thesis better because the project is not a general embodiment thesis. It is a rowing-system thesis using embodiment theory as a lens. Put the rowing constraint early enough that the theory is always being read through the actual design problem.

### Problem 6: Chapter 2 currently applies the mode contrast inside almost every section

This is pedagogically useful in draft form, but the final version may feel repetitive. Examples:

- `chapters/02_theoretical_background/01_virtual_embodiment.tex:18-22`
- `chapters/02_theoretical_background/02_agency_ownership_and_self_location.tex:11-26`
- `chapters/02_theoretical_background/03_visuomotor_congruence_and_synchrony.tex:12-28`
- `chapters/02_theoretical_background/04_virtual_hands_tools_and_body_mapping.tex:11-20`
- `chapters/02_theoretical_background/05_presence_vection_and_stationary_self_motion.tex:8-20`
- `chapters/02_theoretical_background/06_rowing_biomechanics_and_ergometer_rowing.tex:12-18`
- `chapters/02_theoretical_background/08_synthesis_for_this_thesis.tex:4-14`

Recommendation:

- Keep short thesis-facing bridges inside each theory section only where needed.
- Move the full "what this means for the two modes" integration into `08_synthesis_for_this_thesis.tex`.
- Consider a small table in the synthesis:

| Cue/design dimension | Ergometer-congruent mode | Boat-realistic mode |
|---|---|---|
| Temporal synchrony | intended high | intended high |
| Spatial hand/handle congruence | intended high | transformed |
| Tool depiction | real handle/virtual handle | real handle/virtual oars |
| Sport-action plausibility | lower or limited | higher or intended higher |
| Expected pressure on SoA | direct control | predictable transformation |
| Expected pressure on SoO | body/handle alignment | body/oar plausibility vs mismatch |

This would reduce repeated prose while clarifying the design logic.

### Problem 7: "Overall sense of embodiment" is promised more strongly than it is measured

The global notes and research objectives mention broader SoE/overall embodiment. Chapter 4 wisely treats ownership and agency as primary, body-location/self-location as exploratory, and custom rowing items as separate.

Potential tension:

- `notes/global/thesis_spine.md` says empirical focus includes SoO, SoA, and broader SoE.
- `chapters/01_introduction/05_research_objectives_and_questions.tex:10` includes "overall sense of embodiment."
- `chapters/04_study_design/05_measures_embodiment.tex:14` says embodiment will not be a single undifferentiated score.

Recommendation:

- Keep SoE as the conceptual umbrella.
- Do not promise a single overall SoE score unless one is actually defined.
- Phrase the empirical claim as:

> The study evaluates embodiment-related experience through ownership, agency, exploratory body-location items, and thesis-specific movement-mapping measures.

This preserves the theory while matching the method.

### Problem 8: Comfort appears as both outcome and safety observation

Chapter 1 and the RQs include comfort:

- `chapters/01_introduction/05_research_objectives_and_questions.tex:10`
- `chapters/01_introduction/05_research_objectives_and_questions.tex:25`

Chapter 4 says comfort/sickness symptoms are safety and debriefing observations, not embodiment outcomes:

- `chapters/04_study_design/01_design_overview.tex:14`
- `chapters/04_study_design/06_measures_rowing_specific.tex:18`

Recommendation:

- Decide whether comfort is an exploratory outcome or only a safety/feasibility observation.
- If comfort remains in an RQ, add a light reporting plan in Results.
- If not, remove it from the RQ and say safety/comfort is monitored for feasibility and ethical handling.

## Chapter-by-Chapter Notes

### Frontmatter

The abstract is still placeholder text:

- `frontmatter/abstract.tex:6-8`

The acknowledgements contain placeholder names:

- `frontmatter/acknowledgements.tex:8`

The inactive title page contains placeholders:

- `frontmatter/title_page.tex:7-14`

The active title page is a PDF include:

- `main.tex:98`

Recommendation:

- Leave abstract until results/discussion exist.
- Before any review export, replace or remove placeholder acknowledgements.
- Confirm whether the PDF title page is final and whether `frontmatter/title_page.tex` should stay as a template or be archived.

### Chapter 1: Introduction

Strengths:

- Strong motivation from rowing mechanics into VR representation.
- Good caution that the comparison is not real rowing vs fake rowing.
- Research question is aligned with the global thesis spine.

Structural pressure:

- Motivation and core design tension are both long and both explain the same fundamental conflict.
- Citation audit footnotes are extremely long and currently visible through `\showsourcenotestrue`.
- The introduction may feel like it is already doing part of Chapter 2's literature review and part of Chapter 3's design explanation.

Suggestions:

- Keep `01_motivation.tex` focused on why the problem matters.
- Let `02_core_design_tension.tex` define the two representation strategies once.
- Shorten `03_embodiment_and_experiential_evaluation.tex` so it only introduces why embodiment and preference/realism are measured.
- In `04_research_gap.tex`, avoid listing commercial apps unless they are sourced or clearly framed as non-academic context.
- In `05_research_objectives_and_questions.tex`, align "comfort" and "overall SoE" with the actual method.

Specific double taps:

- Ergometer vs on-water mismatch:
  - `01_motivation.tex:4-7`
  - `01_motivation.tex:89-92`
  - `02_core_design_tension.tex:4-7`
  - `02_core_design_tension.tex:104-108`
- Same "both strategies are compromises" point:
  - `02_core_design_tension.tex:104-108`
  - `06_contributions.tex:12`
  - `02_theoretical_background/08_synthesis_for_this_thesis.tex:12`
- Same "preference is exploratory, embodiment is primary" point:
  - `03_embodiment_and_experiential_evaluation.tex:14-16`
  - `04_study_design/06_measures_rowing_specific.tex:16-20`
  - `04_study_design/08_analysis_plan.tex:6`

### Chapter 2: Theoretical Background and Related Work

Strengths:

- The chapter is concise and structurally sensible.
- It separates embodiment, agency/ownership/self-location, congruence, tool mediation, presence/vection, rowing biomechanics, and related work.
- It correctly treats presence/vection as secondary concepts.

Weaknesses:

- Nearly every section contains TODO citations.
- The chapter is more like a conceptual scaffold than a source-integrated literature review.
- Related work is too high-level to support the research gap yet.
- Rowing biomechanics arrives late despite being essential to the core design tension.

Suggestions:

- Consider moving rowing biomechanics earlier, or at least adding a short "domain constraint" section before the embodiment theory.
- Add citations from the existing paper inventory rather than expanding the theory scope.
- Make the related-work section more concrete with a compact table:
  - system/source
  - physical setup
  - virtual representation
  - manipulated variable
  - measured outcome
  - relevance to this thesis
- Move detailed VR rowing project summaries to an appendix or dossier.
- Keep vection/presence short unless measured.

Do not let Chapter 2 become:

- a full RHI genealogy chapter
- a rowing biomechanics chapter
- a VR sport training-transfer chapter
- a motor-learning chapter

### Chapter 3: System and Prototype

Current state:

- Placeholder only.

This is the biggest structural gap.

Recommended purpose:

Chapter 3 should make the reader believe that the thesis actually built the comparison promised in Chapters 1 and 2. It should answer:

- What physical system did the participant use?
- What is tracked directly?
- What is inferred?
- How is the ergometer aligned with the virtual world?
- What does the avatar do?
- What is identical across modes?
- What changes between modes?
- Where exactly is congruence preserved or sacrificed?
- What implementation limitations could affect interpretation?

Suggested section plan:

1. `Design Goals and Constraints`
   - Same physical rowing action.
   - Two representation mappings.
   - Control of obvious visual/task confounds where possible.

2. `Hardware and Physical Setup`
   - Ergometer model.
   - HMD.
   - Tracking devices.
   - Computer/standalone/network setup.
   - Safety-relevant spatial setup.

3. `Software Architecture`
   - Unity version and major packages.
   - Avatar/IK solution.
   - Input pipeline.
   - Scene/environment pipeline.

4. `Calibration and Alignment`
   - How real erg, user, seat/handle reference, and virtual scene are aligned.
   - What is measured vs estimated.
   - How long it takes if known.
   - Failure modes.

5. `Tracking and Body-State Estimation`
   - Hands/head/seat/handle/body measurement details.
   - What IK solves.
   - What is not tracked.

6. `Shared Rowing Environment`
   - What remains constant across both conditions.
   - Lighting/avatar/environment/locomotion/feedback equivalence.

7. `Ergometer-Congruent Mode`
   - Actual mapping.
   - Which cues are intended to be congruent.
   - Which cues are less sport-realistic.

8. `Boat-Realistic Mode`
   - Actual retargeting.
   - Oar/oarlock/blade/hand path logic.
   - Which cues are intended to be sport-realistic.
   - Where mismatch may appear.

9. `Comparison of the Two Modes`
   - A table is better than another long paragraph.

10. `Prototype Limitations`
   - Latency, tracking quality, calibration, visual fidelity, missing haptics, avatar constraints.

Important: do not invent implementation details. Use TODOs where the author must supply exact values.

### Chapter 4: Study Design and Method

Strengths:

- Method scope is clear.
- Within-subject rationale is appropriate.
- The measure separation is strong.
- Safety and ethics are present.

Weaknesses:

- Many final protocol facts remain TODOs.
- It currently depends on Chapter 3 for apparatus details, but Chapter 3 is empty.
- Some claims are future tense and must later be converted to past tense if the study has been conducted.
- The method promises comparability, but the exact controlled/shared elements need to be backed by the system chapter.

High-priority author facts to fill:

- final participant count
- recruitment route
- inclusion/exclusion criteria
- condition labels
- condition order/counterbalancing
- exact exposure/familiarization duration
- standardized rowing duration
- rest duration
- final questionnaire item wording
- response scale
- final analysis tests and effect sizes
- exact data handling/anonymization
- ethics/supervisor approval wording
- apparatus and latency details

Potential structure improvement:

Move `Participants and Recruitment` after `Study Design` is fine. But `Apparatus and Study Setting` may be shorter once Chapter 3 exists, because it should not repeat the full system description.

### Chapter 5: Results

Current state:

- Placeholder only.

Recommended pre-data shell:

1. Participants and data completeness
2. Condition order and exclusions, if any
3. Ownership results
4. Agency results
5. Exploratory body-location/self-location results
6. Rowing-specific movement/congruence/mismatch items
7. Sport-action plausibility / rowing realism
8. Preference and comparative questions
9. Open comments
10. Safety/comfort observations

Even before data, section headings can prevent later drift. Do not pre-write outcomes.

### Chapter 6: Discussion

Current state:

- Placeholder only.

Recommended discussion architecture:

1. Short answer to the research question
2. Embodiment profile of the two modes
3. Agency vs ownership divergence, if observed
4. Sport realism vs sensorimotor congruence
5. What the findings imply for XR rowing design
6. What the findings imply, cautiously, for embodied XR sport systems
7. Prototype limitations
8. Study limitations
9. Future work

Important distinction:

- Prototype limitations: tracking, calibration, avatar fidelity, latency, missing oar haptics.
- Study limitations: sample, order/fatigue, self-report, exposure duration, participant background.

Do not let the discussion become a second literature review. It should interpret the observed patterns once results exist.

### Chapter 7: Conclusion

Current state:

- Placeholder only.

Recommended shape:

1. What was built
2. What was compared
3. What was found
4. What the thesis contributes
5. What should happen next

Keep it short. Avoid adding new literature or new claims here.

## Double-Tap Register

These are places where the manuscript currently repeats itself enough that a later compression pass would help.

### DT1: Ergometer/on-water rowing mismatch

Appears in:

- `chapters/01_introduction/01_motivation.tex:4-7`
- `chapters/01_introduction/01_motivation.tex:89-92`
- `chapters/01_introduction/02_core_design_tension.tex:4-7`
- `chapters/02_theoretical_background/06_rowing_biomechanics_and_ergometer_rowing.tex:4-18`
- `chapters/04_study_design/01_design_overview.tex:8`
- `chapters/04_study_design/06_measures_rowing_specific.tex:4`

Keep full explanation once in intro or background. Elsewhere, refer back briefly.

### DT2: Two-mode definitions

Appears in:

- `chapters/01_introduction/02_core_design_tension.tex:39-63`
- `chapters/01_introduction/03_embodiment_and_experiential_evaluation.tex:7-14`
- `chapters/01_introduction/05_research_objectives_and_questions.tex:4-10`
- `chapters/01_introduction/06_contributions.tex:6-12`
- `chapters/02_theoretical_background/08_synthesis_for_this_thesis.tex:8-12`
- `chapters/04_study_design/01_design_overview.tex:4-8`

Keep definitions in Chapter 1.2 and concrete implementation in Chapter 3. Shorten the rest.

### DT3: "Neither mode is universally better"

Appears in:

- `notes/global/thesis_spine.md`
- `notes/global/claims_register.md`
- `chapters/01_introduction/05_research_objectives_and_questions.tex:30`
- `chapters/01_introduction/06_contributions.tex:12`
- `chapters/02_theoretical_background/08_synthesis_for_this_thesis.tex:12`
- `chapters/04_study_design/08_analysis_plan.tex:14`

This is a useful guardrail, but it can be stated less often in final prose.

### DT4: Preference/realism are separate from embodiment

Appears in:

- `chapters/01_introduction/03_embodiment_and_experiential_evaluation.tex:14-16`
- `chapters/04_study_design/06_measures_rowing_specific.tex:16-20`
- `chapters/04_study_design/08_analysis_plan.tex:6`
- `appendices/appendix_a_questionnaires/01_questionnaire_overview.tex:16-20`

This is methodologically important. Keep it in Chapter 4 and the appendix; shorten in Chapter 1.

### DT5: Presence/vection as secondary

Appears in:

- `chapters/01_introduction/01_motivation.tex:41-48`
- `chapters/02_theoretical_background/05_presence_vection_and_stationary_self_motion.tex:1-20`
- `notes/global/thesis_spine.md` under optional presence/realism ratings

Keep if presence/vection helps explain boat-realistic plausibility, but do not let it become a parallel thesis.

## Citation and Evidence Pressure Points

High-priority citation gaps:

- Chapter 2 general embodiment framework:
  - `chapters/02_theoretical_background/01_virtual_embodiment.tex:5-16`
  - `chapters/02_theoretical_background/02_agency_ownership_and_self_location.tex:7-22`
  - `chapters/02_theoretical_background/03_visuomotor_congruence_and_synchrony.tex:5-26`
- Chapter 2 presence/vection:
  - `chapters/02_theoretical_background/05_presence_vection_and_stationary_self_motion.tex:5-18`
- Chapter 2 rowing biomechanics:
  - `chapters/02_theoretical_background/06_rowing_biomechanics_and_ergometer_rowing.tex:5-10`
- Chapter 2 VR sport/related work:
  - `chapters/02_theoretical_background/07_vr_sport_and_rowing_related_work.tex:5-18`
- Chapter 1 research gap:
  - `chapters/01_introduction/04_research_gap.tex:15-18`

Useful existing source map:

- `literature/First_Wave_thesis_master_paper_inventory_37_bundles.md`

It already identifies the likely core sources. Use it to avoid uncontrolled source expansion.

Citation-key sanity check:

- Active citation commands were checked against `references.bib` during this audit.
- All active keys found in `main.tex`, `chapters/`, `appendices/`, and `frontmatter/` currently exist in `references.bib`.
- The issue is therefore not missing BibTeX keys at this stage. The issue is unfinished citation placement, verification, and deciding which TODO claims should become cited prose.

## Figures and Tables That Would Help

The current thesis has no substantive figures or tables in the active prose. This is a missed opportunity because the central problem is spatial and visual.

Recommended figures/tables:

1. Intro figure: ergometer handle path vs boat/oar path
2. Chapter 2 cue table: congruence/realism variables mapped to the two modes
3. Chapter 3 system architecture diagram: sensors/input -> calibration -> mapping -> IK/avatar/environment
4. Chapter 3 mode comparison figure or side-by-side screenshots
5. Chapter 3 calibration/alignment diagram
6. Chapter 4 study timeline: consent -> calibration -> condition 1 -> questionnaire -> rest -> condition 2 -> questionnaire -> comparison/debrief
7. Chapter 4 measures table: construct, source, items, timing, primary/exploratory status
8. Chapter 5 result plots: paired within-participant lines or dot plots for primary measures

Do not overload the introduction with many visuals. One decisive "why you cannot match both" figure may do more work than several paragraphs.

## Mechanical and Repository Cleanup

These are not intellectual structure issues, but they will save confusion.

### Cleanup 1: Duplicate package loading

`main.tex` loads `hyperref` and `cleveref` twice:

- first around `main.tex:21-22`
- again around `main.tex:43-45`

The existing `main.log` reports:

- `Package hyperref Warning: Option 'pdftex' has already been used`

Clean this up before final formatting.

### Cleanup 2: Visible source notes

`main.tex:48-60` sets `\showsourcenotestrue`, so `\sourcechecknote{...}` becomes visible footnotes.

This is useful for audit drafts, but not for a clean reader-facing thesis. Before final export, either:

- set source notes false,
- use hover-only draft mode if desired,
- or move source-check information into dossiers and leave only normal citations in text.

### Cleanup 3: Dormant wrapper files

The repository contains:

- `chapters/01_introduction/00_chapter.tex`
- `chapters/02_theoretical_background/00_chapter.tex`

The active files are:

- `chapters/01_introduction.tex`
- `chapters/02_theoretical_background.tex`

Dormant wrappers are not inherently bad, but they can confuse future editing passes because they contain overlapping labels and stale TODO/include comments.

### Cleanup 4: Duplicate/copy file

`chapters/01_introduction/02_core_design_tension copy.tex` is not included, but it duplicates the active section label:

- `sec:introduction_core_design_tension`

This should be archived, renamed clearly as backup, or removed once no longer needed. Do not leave it where future tools may accidentally process it.

### Cleanup 5: Label aliases

Some chapters have duplicate labels for convenience:

- `chapters/02_theoretical_background.tex:2-3`
- `chapters/03_system_prototype.tex:5-6`

This is not necessarily wrong, but choose one canonical label in prose and notes. The system chapter currently has both `chap:system` and `chap:system_prototype`; Chapter 4 references `chap:system` while Chapter 1 references `chap:system_prototype`.

### Cleanup 6: Placeholder frontmatter

Before a supervisor-facing build, remove or replace:

- abstract placeholder
- acknowledgements placeholder
- inactive title page placeholders, if still visible in repo review

### Cleanup 7: German ASCII transliteration drafts

The German appendices intentionally use ASCII transliteration and include `TODO:VERIFY-DE`. This is fine during drafting, but not final participant-facing material.

## Suggested Rework Order

### Pass 1: Stabilize condition terminology

Decide once:

- `ergometer-congruent`
- `boat-realistic`

Then apply consistently to:

- Chapter 1
- Chapter 2
- Chapter 4
- appendices
- notes where they drive future edits

### Pass 2: Write Chapter 3

This is the most important missing body of work. Do not over-polish Chapter 1/2 before the system chapter exists, because Chapter 3 will reveal what claims are actually safe.

### Pass 3: Add minimal Results/Discussion/Conclusion shells

Even if data are not ready, create section headings that mirror the RQs and measures. This keeps later analysis from drifting.

### Pass 4: Compress repeated framing

After Chapter 3 exists, return to Chapters 1 and 2 and remove repeated mode descriptions. The reader should encounter:

- motivation in Chapter 1
- theory in Chapter 2
- concrete implementation in Chapter 3
- operational method in Chapter 4

### Pass 5: Build the related-work table

Use the existing paper inventory and evidence packs. The purpose is to support the gap, not to summarize every VR rowing project.

### Pass 6: Citation cleanup

Replace TODO citation comments with existing `references.bib` keys where verified. Leave `TODO:CITE` or `TODO:VERIFY` where support is missing.

### Pass 7: Clean LaTeX and final draft helpers

Disable source notes, remove stale wrappers/backups from active search paths, clean duplicate package loads, and remove placeholder frontmatter.

## Suggested Final Chapter Logic

One possible final architecture:

1. Introduction
   - motivation
   - core design tension
   - research gap
   - research questions
   - contributions
   - thesis structure

2. Background and Related Work
   - rowing/ergometer mismatch
   - virtual embodiment and SoE subcomponents
   - visuomotor congruence and synchrony
   - tools, hands, and body mapping
   - presence/plausibility/vection as secondary concepts
   - VR sport and rowing related work
   - synthesis and hypotheses/expectations

3. System and Prototype
   - design goals
   - hardware/software
   - tracking/calibration/alignment
   - avatar/IK pipeline
   - shared environment
   - ergometer-congruent mode
   - boat-realistic mode
   - implementation limitations

4. Study Design and Method
   - design
   - participants
   - apparatus reference to Chapter 3
   - procedure
   - measures
   - scoring/data handling
   - analysis
   - ethics/safety

5. Results
   - sample/data completeness
   - primary embodiment outcomes
   - exploratory body-location and rowing-specific outcomes
   - preference/open comments
   - safety/comfort observations

6. Discussion
   - answer RQs
   - interpret mode profiles
   - design implications
   - limitations
   - future work

7. Conclusion
   - built, compared, learned, contribution

## Most Important Takeaway

The draft's argument is good. The draft's weight distribution is not yet good.

Right now the thesis explains the tension many times, but has not yet shown the artifact strongly enough. The next major gain will come from writing the system chapter and making the two modes concrete. Once that is done, the introduction and background can become leaner, because Chapter 3 will carry the specific design burden that Chapters 1 and 2 are currently trying to carry in advance.
