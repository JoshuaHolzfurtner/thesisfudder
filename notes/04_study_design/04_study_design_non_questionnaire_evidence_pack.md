# Chapter 4 Non-Questionnaire Method Evidence Pack

Status: companion evidence pack for the parts of Chapter 4 that are not primarily about questionnaire item wording. This file is meant to complement the questionnaire-focused evidence work, not replace it. It does not rewrite `.tex`, does not add citations to the thesis, and does not invent study details.

Target chapter: `chapters/04_study_design.tex`

Main target sections:

- `chapters/04_study_design/01_design_overview.tex`
- `chapters/04_study_design/02_participants_recruitment.tex`
- `chapters/04_study_design/03_apparatus_setting.tex`
- `chapters/04_study_design/04_procedure.tex`
- `chapters/04_study_design/07_data_handling_scoring.tex`
- `chapters/04_study_design/08_analysis_plan.tex`
- `chapters/04_study_design/09_ethics_safety_limitations.tex`

Boundary sections touched only at method level:

- `chapters/04_study_design/05_measures_embodiment.tex`
- `chapters/04_study_design/06_measures_rowing_specific.tex`

Reason for boundary: those sections contain the questionnaire constructs and custom item rationale. They need their own item-level evidence pack. This file covers how those measures fit into the study design, scoring, procedure, analysis, and limitations.

## Files Read

Instruction and framing files:

- `AGENTS.md`
- `notes/global/thesis_spine.md`
- `notes/global/claims_register.md`
- `notes/global/terminology.md`
- `notes/global/contribution_hierarchy.md`
- `notes/chapters/03_system_prototype_back_of_mind.md`
- `notes/chapters/04_study_design_back_of_mind.md`
- `literature/AGENT-thesis_literature_map_first_pitch.md`
- `literature/First_Wave_thesis_master_paper_inventory_37_bundles.md`
- `literature/concept_source_map.md`
- `references.bib`

Chapter and appendix files:

- `chapters/03_system_prototype.tex`
- `chapters/02_theoretical_background/03_visuomotor_congruence_and_synchrony.tex`
- `chapters/02_theoretical_background/04_virtual_hands_tools_and_body_mapping.tex`
- `chapters/04_study_design.tex`
- `chapters/04_study_design/01_design_overview.tex`
- `chapters/04_study_design/02_participants_recruitment.tex`
- `chapters/04_study_design/03_apparatus_setting.tex`
- `chapters/04_study_design/04_procedure.tex`
- `chapters/04_study_design/05_measures_embodiment.tex`
- `chapters/04_study_design/06_measures_rowing_specific.tex`
- `chapters/04_study_design/07_data_handling_scoring.tex`
- `chapters/04_study_design/08_analysis_plan.tex`
- `chapters/04_study_design/09_ethics_safety_limitations.tex`
- `appendices/appendix_b_study_materials/01_materials_overview.tex`
- `appendices/appendix_b_study_materials/02_participant_information_english.tex`
- `appendices/appendix_b_study_materials/04_session_script_english.tex`
- `appendices/appendix_b_study_materials/06_safety_checklist.tex`

Paper markdown consulted directly for this pass:

- `MD Papers/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_markdown_bundle/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_raw_page_marked.md`
- `MD Papers/soper_hume_2004_ideal_rowing_technique_biomechanics_markdown_bundle/soper_hume_2004_ideal_rowing_technique_biomechanics_raw_page_marked.md`
- `MD Papers/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_markdown_bundle/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_raw_page_marked.md`
- `MD Papers/neumann_2018_interactive_virtual_reality_sport_systematic_review_markdown_bundle/neumann_2018_interactive_virtual_reality_sport_systematic_review_raw_page_marked.md`
- `MD Papers/arndt_2018_vr_hmd_rowing_workouts_markdown_bundle/arndt_2018_vr_hmd_rowing_workouts_raw_page_marked.md`
- `MD Papers/murray_2016_presence_of_others_vr_rowing_exercise_markdown_bundle/murray_2016_presence_of_others_vr_rowing_exercise_raw_page_marked.md`
- `MD Papers/kilteni_2012_sense_of_embodiment_markdown_bundle/kilteni_2012_sense_of_embodiment_raw_page_marked.md`
- `MD Papers/kalckert_ehrsson_2012_moving_rubber_hand_dissociation_ownership_agency_markdown_bundle/kalckert_ehrsson_2012_moving_rubber_hand_dissociation_ownership_agency_raw_page_marked.md`
- `MD Papers/waltemate_2016_latency_perceptual_judgments_motor_performance_vr_markdown_bundle/waltemate_2016_latency_perceptual_judgments_motor_performance_vr_raw_page_marked.md`
- `MD Papers/roth_latoschik_2020_virtual_embodiment_questionnaire_veq_markdown_bundle/roth_latoschik_2020_virtual_embodiment_questionnaire_veq_raw_page_marked.md`
- `MD Papers/kalckert_ehrsson_2017_moving_rubber_hand_ownership_onset_time_markdown_bundle/kalckert_ehrsson_2017_moving_rubber_hand_ownership_onset_time_raw_page_marked.md`
- `MD Papers/mottelson_2023_body_ownership_illusions_vr_markdown_bundle/mottelson_2023_body_ownership_illusions_vr_raw_page_marked.md`
- `MD Papers/seinfeld_mueller_2020_visuomotor_feedback_detached_virtual_hands_markdown_bundle/seinfeld_mueller_2020_visuomotor_feedback_detached_virtual_hands_raw_page_marked.md`
- `MD Papers/colombo_2025_vr_cycling_immersion_interaction_effort_markdown_bundle/colombo_2025_vr_cycling_immersion_interaction_effort_raw_page_marked.md`
- `MD Papers/richlan_2023_virtual_training_real_effects_vr_sports_review_markdown_bundle/richlan_2023_virtual_training_real_effects_vr_sports_review_raw_page_marked.md`

Broad searches were also run across `MD Papers/` for method terms such as `within-subject`, `counterbalanced`, `familiarization`, `latency`, `sickness`, `fatigue`, `paired t`, `Wilcoxon`, `descriptive statistics`, and `sample size`.

## Chapter 4 Method Argument Summary

Chapter 4 currently sets up a short exploratory within-subject XR rowing study. The core methodological idea is that every participant rows on the same physical ergometer setup in both conditions, while the virtual representation changes between an ergometer-congruent mapping and a boat-realistic mapping. This makes the study a comparison of representation strategies rather than a comparison of different exercise tasks.

The non-questionnaire method logic has five load-bearing parts:

1. Keep the physical task and study setting stable across conditions so differences are more plausibly tied to representation mode.
2. Use a within-subject design because embodiment ratings are subjective and person-specific; each participant can compare both mappings.
3. Counterbalance or otherwise document condition order because order, learning, adaptation, fatigue, and sickness can affect ratings.
4. Treat calibration, tracking, and latency as part of the experimental apparatus, because they can influence the exact embodiment experiences being measured.
5. Keep interpretation cautious because this is an early prototype evaluation, likely with a small/convenience sample and mostly self-report data.

The source base supports this structure, but not every method detail is externally sourced. Several details are thesis/project decisions that must be confirmed before data collection.

## Stable Method Source Spine

| Source key | Best role in Chapter 4 method | Confidence | Caution |
|---|---|---|---|
| `neumannEtAl2018interactiveVrSport` | VR sport framing; exertion interface; ergometer transformed into virtual boat; VR environment changes in response to athlete. | verified | Does not justify embodiment measures by itself. |
| `lamb1989kinematicComparison` | Ergometer and on-water rowing are related but not identical; supports why the two modes are a meaningful comparison. | verified | Do not use as VR or methods source. |
| `soperHume2004rowingTechnique` | Ergometer use and limitations relative to on-water rowing body patterns. | verified | Keep narrow; does not support study design or embodiment outcomes. |
| `rauterEtAl2013rowingTransfer` | Rowing as rower/boat/oar/water interaction; ordinary ergometer limitations; realistic simulator contrast. | verified | Their simulator is not this prototype; avoid transfer/training claims. |
| `kilteniEtAl2012senseEmbodiment` | SoE, agency, ownership, self-location, and visuomotor congruence rationale for why mapping quality matters. | verified | Not a rowing or method-protocol source. |
| `kalckertEhrsson2012movingRubberHand` | Ownership/agency dissociation and example of Wilcoxon use for non-normal questionnaire data in moving RHI. | verified | Hand paradigm; not a stats authority or rowing source. |
| `waltemateEtAl2016latency` | Latency/feedback delay can affect motor performance, agency, ownership, and simultaneity; supports documenting latency. | verified | Do not import exact latency thresholds as requirements for this prototype. |
| `rothLatoschik2020veq` | VEQ measurement instrument; ownership, agency, change factors; latency/jitter validation context. | verified | Item-level wording belongs in the questionnaire evidence pack. |
| `kalckertEhrsson2017ownershipOnset` | Moving RHI ownership onset and most participants experiencing illusion within first minute; supports familiarization rationale cautiously. | verified | Hand illusion, not rowing; use only as exposure-timing rationale. |
| `mottelsonEtAl2023bodyOwnershipVr` | Review/meta-analysis context for within-subject body ownership designs, modest power, repeated-measures practice. | verified | Not a general statistics textbook; use as field-context, not method law. |
| `seinfeldMueller2020detachedVirtualHands` | Example of fully counterbalanced within-group VR embodiment study, order/learning controls, power analysis, inclusion/ethics wording. | verified | Detached virtual hands task, not rowing; use as methodological analogy. |
| `arndtEtAl2018vrRowingWorkouts` | Concrete HMD indoor-rowing study with sensors, warm-up/baseline, randomized order, paired tests, motion-sickness reporting. | verified | Pilot study; do not generalize its results. |
| `colomboEtAl2025vrCyclingEffort` | Adjacent VR cycling/exercise method analogy: randomized condition order, screening, cybersickness check, descriptive/inferential statistics. | verified | Cycling, not rowing; use cautiously as adjacent exercise-VR practice. |
| `richlanEtAl2023vrSportsReview` | VR sport review caution about short sessions/breaks to avoid cybersickness; HMD vs non-HMD caution; sample-size context. | verified | Narrative review; use for broad safety/method framing, not exact protocol. |

## Section-by-Section Claim Audit

### 4.1 Study Design

Target file: `chapters/04_study_design/01_design_overview.tex`

Current function: establish that the study compares two representation modes for the same physical rowing action, with a within-subject design and counterbalanced condition order where possible.

Key claims:

- Claim: The study compares two representation modes for the same physical rowing action.
  - Classification: thesis/internal project framing.
  - Source support: internal thesis spine and contribution hierarchy; external support from `neumannEtAl2018interactiveVrSport` that sport VR can map physical ergometer exertion to virtual sport action.
  - Status: verified for framing; implementation details still need final confirmation.
  - Narrowing: keep "compares" and "designed to"; do not claim results yet.

- Claim: In both conditions participants row on the same ergometer setup; the representation changes.
  - Classification: internal project method detail.
  - Source support: no literature source needed for the study's own design, but should be confirmed against final procedure and apparatus.
  - Status: TODO:CONFIRM.
  - Narrowing: say "planned" until study is finalized.

- Claim: Ergometer-congruent mode prioritizes close spatial and temporal correspondence between real ergometer interaction and virtual body.
  - Classification: internal project framing with literature-backed rationale.
  - Source support: `kilteniEtAl2012senseEmbodiment` and `waltemateEtAl2016latency` for why visuomotor/temporal congruence matters; `neumannEtAl2018interactiveVrSport` for physical action to virtual sport performance.
  - Status: verified for rationale; TODO:CONFIRM for exact implementation.
  - Narrowing: do not state it actually achieved high congruence unless measured or technically documented.

- Claim: Boat-realistic mode prioritizes sport-action depiction while virtual oar path cannot literally copy real handle path.
  - Classification: thesis design rationale.
  - Source support: `lamb1989kinematicComparison`, `soperHume2004rowingTechnique`, `rauterEtAl2013rowingTransfer`, and `neumannEtAl2018interactiveVrSport`.
  - Status: verified as rationale.
  - Narrowing: do not claim boat-realistic mode is objectively "more realistic" in all senses; specify sport-action depiction.

- Claim: Within-subject design is appropriate because each participant serves as their own control.
  - Classification: method rationale.
  - Source support: `mottelsonEtAl2023bodyOwnershipVr` shows within-subject factors are common in BOI studies and found larger embodiment effects for within-subject designs; `seinfeldMueller2020detachedVirtualHands` is a VR embodiment example with both conditions experienced by each participant; `colomboEtAl2025vrCyclingEffort` and `arndtEtAl2018vrRowingWorkouts` are adjacent VR exercise/rowing examples using repeated conditions.
  - Status: likely.
  - Narrowing: good method rationale, but if the thesis wants a formal design-method citation, add a statistics/experimental-design source. Current corpus supports field practice, not universal methodology.

- Claim: Counterbalancing reduces order, learning, adaptation, and fatigue effects.
  - Classification: method rationale.
  - Source support: `seinfeldMueller2020detachedVirtualHands` explicitly counterbalanced order and controlled for learning/training effects; `colomboEtAl2025vrCyclingEffort` explicitly randomizes condition exposure to minimize order effects such as learning, fatigue, or familiarity; `arndtEtAl2018vrRowingWorkouts` randomized condition order.
  - Status: verified as method analogy.
  - Narrowing: say "reduce" or "minimize risk," not "eliminate."

- Claim: First data-collection version excludes threat, heart-rate, and hand-offset probes.
  - Classification: internal project scope decision.
  - Source support: no source needed; must match actual protocol.
  - Status: TODO:CONFIRM.
  - Narrowing: keep as scope decision and not as a literature recommendation.

Best citation use:

- Use rowing sources near the description of why boat-realistic mode cannot literally copy ergometer mechanics.
- Use method-analogy citations sparingly in a source note or dossier, not as a heavy citation group in main prose.
- Do not cite every methods example in the final text. The dossier can hold the detailed support.

Evidence anchors:

- `neumannEtAl2018interactiveVrSport`: `MD Papers/neumann_2018_interactive_virtual_reality_sport_systematic_review_markdown_bundle/neumann_2018_interactive_virtual_reality_sport_systematic_review_raw_page_marked.md`, lines 105-123, PDF page 4; lines 404-419, PDF page 12.
- `mottelsonEtAl2023bodyOwnershipVr`: `MD Papers/mottelson_2023_body_ownership_illusions_vr_markdown_bundle/mottelson_2023_body_ownership_illusions_vr_raw_page_marked.md`, lines 1117-1125, PDF page 22 / 42; lines 1513-1520, PDF page 29 / 42.
- `seinfeldMueller2020detachedVirtualHands`: `MD Papers/seinfeld_mueller_2020_visuomotor_feedback_detached_virtual_hands_markdown_bundle/seinfeld_mueller_2020_visuomotor_feedback_detached_virtual_hands_raw_page_marked.md`, lines 119-132, PDF page 2; lines 297-323, PDF page 5.
- `colomboEtAl2025vrCyclingEffort`: `MD Papers/colombo_2025_vr_cycling_immersion_interaction_effort_markdown_bundle/colombo_2025_vr_cycling_immersion_interaction_effort_raw_page_marked.md`, lines 307-323, PDF page 3.
- `arndtEtAl2018vrRowingWorkouts`: `MD Papers/arndt_2018_vr_hmd_rowing_workouts_markdown_bundle/arndt_2018_vr_hmd_rowing_workouts_raw_page_marked.md`, lines 219-253, PDF page 2; lines 265-274, PDF page 3.

Verdict: sourceable, but condition order and exact protocol remain `TODO:CONFIRM`.

### 4.2 Participants and Recruitment

Target file: `chapters/04_study_design/02_participants_recruitment.tex`

Current function: define recruitment as exploratory, list background variables, and ensure neutral instructions.

Key claims:

- Claim: Recruitment is exploratory and not representative of all rowers, VR users, or exercise users.
  - Classification: thesis scope control.
  - Source support: internal thesis spine; optional context from `richlanEtAl2023vrSportsReview` that VR sport studies vary widely in samples and from `mottelsonEtAl2023bodyOwnershipVr` that body ownership studies have modest power.
  - Status: verified as cautious thesis framing.
  - Narrowing: keep it. This is method honesty.

- Claim: Participant number, recruitment route, inclusion/exclusion criteria, and approval route must be fixed before reporting.
  - Classification: method requirement / TODO.
  - Source support: internal project management; examples from `seinfeldMueller2020detachedVirtualHands` and `colomboEtAl2025vrCyclingEffort` show studies report participant counts, inclusion criteria, ethics approval, and consent.
  - Status: TODO:CONFIRM for this thesis.
  - Narrowing: do not invent participant count or approval status.

- Claim: Background variables include prior VR experience, prior rowing/ergometer experience, sickness susceptibility, and health/comfort restrictions.
  - Classification: method rationale.
  - Source support: `neumannEtAl2018interactiveVrSport` notes athlete, VR environment, task, and non-VR environment factors influence outcomes; `colomboEtAl2025vrCyclingEffort` screens for ability to engage in mild/moderate physical activity and excludes significant motion sickness/epilepsy; `arndtEtAl2018vrRowingWorkouts` uses demographics and reports motion-sickness/QoE.
  - Status: likely to verified depending final variable list.
  - Narrowing: keep as context variables, not grouping variables unless analysis plan changes.

- Claim: Instructions should avoid suggesting one mode is expected to be better.
  - Classification: internal anti-bias procedure.
  - Source support: no direct source in current corpus; aligns with thesis non-superiority framing.
  - Status: verified as internal scope rule; `TODO:CITE` only if a demand-characteristics/source-bias argument is made.
  - Narrowing: good as procedural instruction; no need to cite in final text unless developed.

Evidence anchors:

- `seinfeldMueller2020detachedVirtualHands`: lines 119-132, PDF page 2. Evidence: reports within-group design, counterbalanced order, participant count, inclusion criteria, ethics approval, written informed consent.
- `colomboEtAl2025vrCyclingEffort`: lines 328-335, PDF page 3. Evidence: confirms physical-activity ability, excludes sitting problems, severe visual impairment, significant motion sickness, epilepsy, and reports ethics approval.
- `neumannEtAl2018interactiveVrSport`: lines 73-88, PDF page 3. Evidence: VR sport outcomes are influenced by athlete, VR system, task, and non-VR environment factors.
- `richlanEtAl2023vrSportsReview`: lines 389-411, PDF page 4. Evidence: VR sports studies vary in device type, intervention duration, sample size, and should treat HMD and non-HMD studies cautiously.

Verdict: needs final human confirmation for all concrete participant details.

### 4.3 Apparatus and Study Setting

Target file: `chapters/04_study_design/03_apparatus_setting.tex`

Current function: define the apparatus, make calibration/tracking methodologically visible, and explain why latency/responsiveness should be documented.

Key claims:

- Claim: Apparatus consists of ergometer, headset, tracking/calibration setup, and Unity prototype.
  - Classification: internal project detail.
  - Source support: Chapter 3 should eventually verify this; current `chapters/03_system_prototype.tex` is still a scaffold.
  - Status: TODO:CONFIRM.
  - Narrowing: keep future/planned wording until Chapter 3 is filled.

- Claim: Same physical task/basic environment is used in both conditions to reduce confounding.
  - Classification: method rationale.
  - Source support: internal design; `seinfeldMueller2020detachedVirtualHands` provides an analogy where conditions differed only by virtual hand model while other virtual hand models were otherwise the same; `colomboEtAl2025vrCyclingEffort` tries to isolate condition effects by randomizing order.
  - Status: likely.
  - Narrowing: "reduce the risk" is safe; do not say "ensures."

- Claim: Handle relation is tracked through hands; remaining rowing-body motion is inferred from aligned machine, setup geometry, and body measurements.
  - Classification: implementation-specific.
  - Source support: internal prototype documentation needed.
  - Status: TODO:CONFIRM.
  - Narrowing: do not cite papers for this unless they describe this prototype.

- Claim: Calibration is part of the experimental apparatus because poor alignment can affect ratings.
  - Classification: thesis-method inference.
  - Source support: `waltemateEtAl2016latency` and `rothLatoschik2020veq` support that feedback delay/latency affects embodiment measures; `kilteniEtAl2012senseEmbodiment` supports agency dependence on predicted vs actual sensory consequences, but exact calibration/alignment source is still light.
  - Status: likely.
  - Narrowing: say "may reflect setup error" rather than "will reflect."

- Claim: Latency/responsiveness should be documented because delayed closed-loop avatar feedback can influence agency, ownership, simultaneity, and motor performance.
  - Classification: directly source-backed.
  - Source support: `waltemateEtAl2016latency`; supporting `rothLatoschik2020veq` validation study.
  - Status: verified.
  - Narrowing: do not import thresholds directly; report if known.

Evidence anchors:

- `waltemateEtAl2016latency`: `MD Papers/waltemate_2016_latency_perceptual_judgments_motor_performance_vr_markdown_bundle/waltemate_2016_latency_perceptual_judgments_motor_performance_vr_raw_page_marked.md`, lines 37-60, PDF page 1; lines 70-84, PDF page 1; lines 221-229, PDF page 2; lines 520-540, PDF page 5; lines 847-855, PDF page 7.
- `rothLatoschik2020veq`: `MD Papers/roth_latoschik_2020_virtual_embodiment_questionnaire_veq_markdown_bundle/roth_latoschik_2020_virtual_embodiment_questionnaire_veq_raw_page_marked.md`, lines 636-650, PDF page 6; lines 678-697, PDF page 6; lines 834-845, PDF page 7; lines 974-979, PDF page 8; lines 1783-1788, appendix PDF page 3.
- `arndtEtAl2018vrRowingWorkouts`: lines 175-190, PDF page 2; lines 219-253, PDF page 2. Evidence: HMD rowing prototype, sensors capturing sledge and handlebars, controllers locating the ergometer, virtual lake/scull, force-dependent movement.

Verdict: good conceptual support, but many apparatus details remain `TODO:CONFIRM`.

### 4.4 Procedure

Target file: `chapters/04_study_design/04_procedure.tex`

Current function: specify session flow: information/consent/safety check, neutral setup introduction, calibration, familiarization, standardized rowing period, questionnaire, rest, post-comparison, open comments, and stop criteria.

Key claims:

- Claim: Session begins with participant information, consent, and health/comfort check.
  - Classification: ethical/procedural method detail.
  - Source support: appendix materials; examples from `seinfeldMueller2020detachedVirtualHands` and `colomboEtAl2025vrCyclingEffort` report informed consent, ethics approval, and exclusion/screening criteria.
  - Status: verified as method expectation, TODO:CONFIRM for final wording/approval.
  - Narrowing: do not state formal ethics approval unless true.

- Claim: Participants should be introduced neutrally and told to report their experience rather than identify the "correct" mode.
  - Classification: internal anti-bias script.
  - Source support: no direct source in checked corpus; aligned with thesis framing.
  - Status: internal project framing.
  - Narrowing: keep in script and method; no citation needed unless discussing demand characteristics.

- Claim: Familiarization period is included because movement-based ownership may take time to emerge and very short exposures can capture confusion.
  - Classification: method rationale.
  - Source support: `kalckertEhrsson2017ownershipOnset`; supporting method analogy from `arndtEtAl2018vrRowingWorkouts` warm-up/baseline and `seinfeldMueller2020detachedVirtualHands` familiarization/training.
  - Status: verified as rationale.
  - Narrowing: hand-illusion onset is not rowing. Use it to justify "at least brief familiarization," not exact rowing duration.

- Claim: After each condition, participants complete per-condition questionnaires; after both, comparative preferences and open comments.
  - Classification: internal method design.
  - Source support: `seinfeldMueller2020detachedVirtualHands` uses questionnaire after experience and repeats procedure for second condition; `arndtEtAl2018vrRowingWorkouts` asks participants to fill questionnaires after each session.
  - Status: likely.
  - Narrowing: final exact forms and language remain Appendix A/B work.

- Claim: Rest offered between conditions and session stops on nausea, dizziness, pain, distress, or unsafe discomfort.
  - Classification: safety procedure.
  - Source support: `richlanEtAl2023vrSportsReview` advises short sessions and breaks to avoid VR sickness; `colomboEtAl2025vrCyclingEffort` notes lack of rest can leave residual sickness/fatigue and uses sickness screening/checks; appendix safety checklist.
  - Status: verified as safety rationale; TODO:CONFIRM exact stop wording.
  - Narrowing: do not cite adjacent VR cycling as if it defines rowing safety rules.

Evidence anchors:

- `kalckertEhrsson2017ownershipOnset`: `MD Papers/kalckert_ehrsson_2017_moving_rubber_hand_ownership_onset_time_markdown_bundle/kalckert_ehrsson_2017_moving_rubber_hand_ownership_onset_time_raw_page_marked.md`, lines 58-70, PDF page 1; lines 244-266, PDF page 3; lines 389-407, PDF page 5.
- `arndtEtAl2018vrRowingWorkouts`: lines 236-253, PDF page 2; lines 265-274, PDF page 3.
- `seinfeldMueller2020detachedVirtualHands`: lines 297-323, PDF page 5; lines 638-684, PDF pages 7-8.
- `richlanEtAl2023vrSportsReview`: `MD Papers/richlan_2023_virtual_training_real_effects_vr_sports_review_markdown_bundle/richlan_2023_virtual_training_real_effects_vr_sports_review_raw_page_marked.md`, lines 126-134, PDF page 2.
- `colomboEtAl2025vrCyclingEffort`: lines 307-323, PDF page 3; lines 601-622, PDF page 6.

Verdict: strong enough for procedure rationale; exact durations remain `TODO:CONFIRM`.

### 4.5 and 4.6 Measures Boundary

Target files:

- `chapters/04_study_design/05_measures_embodiment.tex`
- `chapters/04_study_design/06_measures_rowing_specific.tex`

Current function in this pack: not item-level questionnaire validation; only how measures fit methodologically into the study.

Key non-questionnaire claims:

- Claim: Primary embodiment outcomes are ownership and agency, with body-location exploratory.
  - Classification: measurement design; questionnaire-focused.
  - Source support: `rothLatoschik2020veq`, `gonzalezFrancoPeck2018avatarEmbodiment`, `kilteniEtAl2012senseEmbodiment`.
  - Status: should be handled in item-level questionnaire pack.
  - This pack note: use method file only to preserve separation between primary validated subscales and exploratory/custom items.

- Claim: Custom rowing-specific items should not be mixed into VEQ scores.
  - Classification: scoring/method decision.
  - Source support: `rothLatoschik2020veq` supports VEQ factors; custom items are thesis-specific and should remain separate unless validated.
  - Status: verified as conservative scoring logic.
  - Narrowing: custom items are exploratory; do not call them validated subscales.

- Claim: Safety/comfort symptoms are recorded separately from embodiment outcomes.
  - Classification: method distinction.
  - Source support: `colomboEtAl2025vrCyclingEffort` separates cybersickness/discomfort check; `arndtEtAl2018vrRowingWorkouts` reports motion sickness/QoE; thesis logic.
  - Status: likely.
  - Narrowing: comfort can contextualize ratings but is not an embodiment score.

Evidence anchors:

- `rothLatoschik2020veq`: lines 37-48, PDF page 1. Evidence: VEQ constructed as validated instrument with factors ownership, agency, body-schema change.
- `colomboEtAl2025vrCyclingEffort`: lines 601-622, PDF page 6. Evidence: discomfort/cybersickness check kept short due protocol burden; symptoms traced to SSQ subscales if reported.
- `arndtEtAl2018vrRowingWorkouts`: lines 352-354, PDF page 3. Evidence: VR rowing pilot reported slightly elevated motion sickness but no participant quit and it was not reported as uncomfortable.

Verdict: item-level sources should live in the questionnaire dossier; this method pack supports separation and reporting.

### 4.7 Data Handling and Scoring

Target file: `chapters/04_study_design/07_data_handling_scoring.tex`

Current function: specify table structure, pseudonymization, scoring separation, open comment use, and TODOs for file format/anonymization/missing data.

Key claims:

- Claim: Analysis table includes participant code, condition order, background variables, per-condition ratings, comparative preference, and open comments.
  - Classification: internal data structure.
  - Source support: no external source required; must match final data collection.
  - Status: TODO:CONFIRM final file format.
  - Narrowing: keep as "will include" only after final forms are set.

- Claim: Condition order must be retained because order, learning, and fatigue are possible interpretive factors.
  - Classification: directly supported method rationale.
  - Source support: `seinfeldMueller2020detachedVirtualHands` explicitly includes order despite counterbalancing to control habituation/training effects; `colomboEtAl2025vrCyclingEffort` discusses random order minimizing learning/fatigue/familiarity effects but residual effects cannot be excluded.
  - Status: verified.
  - Narrowing: retain order as a covariate/context, not necessarily a primary analysis factor unless sample allows.

- Claim: Direct identifiers should not be stored in the analysis table.
  - Classification: data protection/ethics procedure.
  - Source support: local ethics/data protection policy needed; not covered by current paper corpus.
  - Status: TODO:CONFIRM.
  - Narrowing: do not claim compliance until exact process is set.

- Claim: VEQ Ownership/Acceptance and Control/Agency scores are means of selected items; custom items remain separate.
  - Classification: scoring rule.
  - Source support: `rothLatoschik2020veq` for VEQ factors; exact item scoring must be checked against questionnaire source and Appendix A.
  - Status: TODO:VERIFY for final item list.
  - Narrowing: if items are adapted, document adaptation.

- Claim: Open comments contextualize questionnaire patterns.
  - Classification: internal exploratory analysis plan.
  - Source support: no direct source needed if framed as qualitative context.
  - Status: likely.
  - Narrowing: do not overstate comments as systematic qualitative analysis unless a coding scheme is defined.

Evidence anchors:

- `seinfeldMueller2020detachedVirtualHands`: lines 297-323, PDF page 5.
- `colomboEtAl2025vrCyclingEffort`: lines 307-323, PDF page 3.
- `rothLatoschik2020veq`: lines 37-48, PDF page 1; lines 678-697, PDF page 6; lines 1783-1788, appendix PDF page 3.

Verdict: methodologically sensible; final data protection, file format, and missing-data handling need human confirmation.

### 4.8 Analysis Plan

Target file: `chapters/04_study_design/08_analysis_plan.tex`

Current function: specify within-participant comparisons, primary outcomes, exploratory outcomes, descriptive statistics, conditional inferential tests, and cautious interpretation.

Key claims:

- Claim: Analysis compares ergometer-congruent and boat-realistic conditions within participants.
  - Classification: internal design; method consequence.
  - Source support: same as design section; within-subject method analogies from `mottelsonEtAl2023bodyOwnershipVr`, `seinfeldMueller2020detachedVirtualHands`, `arndtEtAl2018vrRowingWorkouts`, `colomboEtAl2025vrCyclingEffort`.
  - Status: verified as plan if final design remains within-subject.
  - Narrowing: if counterbalancing or order is incomplete, state it.

- Claim: Primary comparisons are VEQ Ownership/Acceptance and VEQ Control/Agency.
  - Classification: measurement design.
  - Source support: `rothLatoschik2020veq`.
  - Status: verified, pending final item selection.
  - Narrowing: do not include Change as primary unless explicitly measured and justified.

- Claim: Exploratory outcomes are not validated embodiment subscales.
  - Classification: conservative scoring/interpretation.
  - Source support: `rothLatoschik2020veq` factor structure; custom-item logic.
  - Status: verified as cautious interpretation.
  - Narrowing: custom item patterns can inform interpretation, not replace validated scales.

- Claim: Descriptive statistics include mean, median, SD/IQR, and within-participant difference where appropriate.
  - Classification: statistical reporting plan.
  - Source support: `colomboEtAl2025vrCyclingEffort` is an adjacent method analogy using mean/SD for normal variables and median/IQR for non-normal variables; `seinfeldMueller2020detachedVirtualHands` displays medians/IQRs in VR questionnaire boxplots.
  - Status: likely.
  - Narrowing: for final thesis, use a formal stats source or supervisor-approved analysis plan if this becomes a methodological claim.

- Claim: Paired t-test may be used for approximately symmetric interval-style differences; Wilcoxon signed-rank as fallback.
  - Classification: statistical analysis plan.
  - Source support: current corpus has examples, not formal authority. `arndtEtAl2018vrRowingWorkouts` uses paired t-test for VR/non-VR rowing; `kalckertEhrsson2012movingRubberHand` and `kalckertEhrsson2017ownershipOnset` use Wilcoxon for Likert/ownership comparisons; `colomboEtAl2025vrCyclingEffort` uses repeated-measures ANOVA/Friedman depending distribution.
  - Status: needs manual check.
  - Narrowing: keep as planned options until final sample/distributions/supervisor advice decide. Add formal statistics citation if required.

- Claim: Interpretation remains cautious and prototype-specific.
  - Classification: thesis scope control.
  - Source support: internal thesis spine; `mottelsonEtAl2023bodyOwnershipVr` notes modest power in BOI studies; `richlanEtAl2023vrSportsReview` shows VR sport studies vary widely in sample size/device/intervention.
  - Status: verified as caution.
  - Narrowing: avoid universal superiority claims.

Evidence anchors:

- `rothLatoschik2020veq`: lines 37-48, PDF page 1; lines 678-697, PDF page 6; lines 1783-1788, appendix PDF page 3. Evidence: VEQ factor structure and mean-score formulas for ownership/agency, including the Acceptance/Ownership and Control/Agency appendix naming.
- `arndtEtAl2018vrRowingWorkouts`: lines 318-323, PDF page 3. Evidence: paired t-test comparing VR and non-VR rowing conditions.
- `kalckertEhrsson2017ownershipOnset`: lines 244-266, PDF page 3; lines 389-407, PDF page 5. Evidence: Likert ownership items, repeated onset measures, breaks between trials, median onset times.
- `mottelsonEtAl2023bodyOwnershipVr`: lines 1117-1125, PDF page 22 / 42; lines 1513-1520, PDF page 29 / 42; lines 1630-1636, PDF page 32 / 42.
- `colomboEtAl2025vrCyclingEffort`: lines 647-656, PDF page 6; lines 908-916, PDF page 9. Evidence: mean/SD for normal variables, median/IQR for non-normal variables, repeated-measures ANOVA/Friedman, effect size reporting.
- `seinfeldMueller2020detachedVirtualHands`: lines 297-323, PDF page 5; lines 958-963, PDF page 10.

Verdict: good draft plan, but formal statistical finalization remains `TODO:CONFIRM`.

### 4.9 Ethics, Safety, and Method Limitations

Target file: `chapters/04_study_design/09_ethics_safety_limitations.tex`

Current function: define safety/withdrawal/stop criteria and bound interpretation.

Key claims:

- Claim: Study involves physical exertion on an ergometer while wearing a VR headset, so safety screening and stop criteria are needed.
  - Classification: method/safety rationale.
  - Source support: `richlanEtAl2023vrSportsReview` recommends short sessions and breaks to avoid VR sickness; `colomboEtAl2025vrCyclingEffort` screens physical activity ability, motion sickness, epilepsy, and asks about discomfort/cybersickness; `arndtEtAl2018vrRowingWorkouts` reports avoiding rapid fatigue and motion-sickness observations.
  - Status: verified as safety rationale.
  - Narrowing: exact medical/exclusion wording must be approved locally.

- Claim: Participants may experience fatigue, discomfort, dizziness, or VR-related sickness symptoms.
  - Classification: source-backed safety caution.
  - Source support: `richlanEtAl2023vrSportsReview`, `colomboEtAl2025vrCyclingEffort`, `arndtEtAl2018vrRowingWorkouts`.
  - Status: verified.
  - Narrowing: do not imply high risk; say may experience.

- Claim: Participant may stop at any time.
  - Classification: ethical procedure.
  - Source support: appendix materials; local ethics/consent process needed. The paper corpus has examples of consent, but not your local policy.
  - Status: TODO:CONFIRM exact wording.
  - Narrowing: do not state formal rights/process details beyond what consent form confirms.

- Claim: First study version avoids threat, physiological response measures, and hand-offset probes to reduce complexity and stay focused.
  - Classification: internal scope decision.
  - Source support: no citation needed.
  - Status: TODO:CONFIRM.
  - Narrowing: do not make this sound like a literature requirement.

- Claim: Limitations include self-report, prototype-specific implementation, small/convenience sample, and ambiguity between representation concept vs calibration/tracking quality.
  - Classification: thesis limitation.
  - Source support: internal thesis scope; `mottelsonEtAl2023bodyOwnershipVr` for modest power/body-ownership study context; `waltemateEtAl2016latency` for technical feedback affecting ratings; `richlanEtAl2023vrSportsReview` for sample/device variability in VR sports.
  - Status: verified as cautious limitation.
  - Narrowing: distinguish study-design limitations from prototype limitations.

Evidence anchors:

- `richlanEtAl2023vrSportsReview`: lines 126-134, PDF page 2; lines 389-411, PDF page 4.
- `colomboEtAl2025vrCyclingEffort`: lines 328-335, PDF page 3; lines 601-622, PDF page 6.
- `arndtEtAl2018vrRowingWorkouts`: lines 219-253, PDF page 2; lines 352-354, PDF page 3.
- `waltemateEtAl2016latency`: lines 847-855, PDF page 7.

Verdict: safety rationale is supported, but consent, approval, data protection, and exact exclusion criteria remain human/local decisions.

## Source Cards

### Source: `lamb1989kinematicComparison`

- Source role: best rowing biomechanics source for ergometer versus on-water similarity and mismatch.
- What it says that matters here: ergometer and on-water rowing share many leg/trunk drive-phase variables, but upper arm and forearm kinematics differ, especially around catch and finish because on-water rowing involves oar-water and oar-lift/feathering mechanics not reproduced in the same way on an ergometer.
- Supports: why a boat-realistic representation cannot simply copy the ergometer handle path and still be fully on-water-realistic.
- Does not support: study design, embodiment outcomes, or questionnaire choices.
- Evidence type: direct rowing-domain premise.
- Confidence: verified.
- Anchors:
  - MD: `MD Papers/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_markdown_bundle/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_raw_page_marked.md`, lines 20-63, PDF page 1.
  - MD: same file, lines 419-500, PDF pages 6-7.

### Source: `soperHume2004rowingTechnique`

- Source role: supporting rowing biomechanics source for ergometer legitimacy and limitations.
- What it says that matters here: rowing ergometers are commonly used for testing, technique coaching, selection, and poor-weather training; common ergometers can simulate some physiological and lower-limb aspects but do not reproduce trunk and upper-limb patterns well compared with on-water rowing/sculling because of the central pulley system.
- Supports: Chapter 4's claim that the boat-realistic condition is motivated by real ergometer/on-water differences, not a purely aesthetic choice.
- Does not support: VR embodiment, procedure, or analysis.
- Evidence type: direct rowing-domain premise.
- Confidence: verified.
- Anchors:
  - MD: `MD Papers/soper_hume_2004_ideal_rowing_technique_biomechanics_markdown_bundle/soper_hume_2004_ideal_rowing_technique_biomechanics_raw_page_marked.md`, lines 79-85, PDF page 1.
  - MD: same file, lines 109-123, PDF page 2.

### Source: `rauterEtAl2013rowingTransfer`

- Source role: best source for rower/boat/oar/water interaction and ordinary ergometer limitation relative to oar handling.
- What it says that matters here: rowing involves continuous haptic interaction among rower, boat, oar, and water; ordinary ergometers render resistance through a cable-driven windmill and do not train oar immersion height or oar handling in the same way; realistic simulation may involve visual, auditory, and haptic rendering of oar-water interactions.
- Supports: why boat/oar/water depiction is sport-specific and why the two modes compare different action-representation priorities.
- Does not support: this prototype's effectiveness, transfer learning, or user-study results.
- Evidence type: direct rowing/simulator premise.
- Confidence: verified.
- Anchors:
  - MD: `MD Papers/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_markdown_bundle/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_raw_page_marked.md`, lines 149-199, PDF page 2.
  - MD: same file, lines 283-320, PDF page 3.

### Source: `neumannEtAl2018interactiveVrSport`

- Source role: best for VR sport/exertion-interface framing.
- What it says that matters here: VR sport uses sport-relevant computer-generated content and interactivity; physical effort on an ergometer can be mapped to virtual race-course speed; the rowing example explicitly says an ergometer can be transformed into a virtual boat where handle pulls become virtual oar movements.
- Supports: study design rationale, same physical action plus altered representation, VR sport framing.
- Does not support: embodiment outcomes, the exact two thesis modes, or the specific questionnaire design.
- Evidence type: direct context and thesis-synthesis premise.
- Confidence: verified.
- Anchors:
  - MD: `MD Papers/neumann_2018_interactive_virtual_reality_sport_systematic_review_markdown_bundle/neumann_2018_interactive_virtual_reality_sport_systematic_review_raw_page_marked.md`, lines 105-123, PDF page 4.
  - MD: same file, lines 228-241, PDF page 7.
  - MD: same file, lines 404-419, PDF page 12.

### Source: `kilteniEtAl2012senseEmbodiment`

- Source role: best conceptual source for why agency/ownership/self-location are relevant to the mapping comparison.
- What it says that matters here: SoE is associated with self-location, agency, and body ownership; agency is linked to the match between predicted and actual sensory consequences, including synchronous visuomotor correlations, and discrepancies between seen action feedback and actual movement can reduce agency.
- Supports: rationale that mapping, latency, and calibration quality can affect embodiment-relevant ratings.
- Does not support: rowing-specific method details or exact analysis plan.
- Evidence type: conceptual/theoretical premise.
- Confidence: verified.
- Anchors:
  - MD: `MD Papers/kilteni_2012_sense_of_embodiment_markdown_bundle/kilteni_2012_sense_of_embodiment_raw_page_marked.md`, lines 190-226, PDF page 3.
  - MD: same file, lines 338-377, PDF pages 4-5.
  - MD: same file, lines 436-444, PDF page 5.
  - MD: same file, lines 922-926, PDF page 11.

### Source: `kalckertEhrsson2012movingRubberHand`

- Source role: ownership/agency dissociation source and analysis-method example for non-normal questionnaire data.
- What it says that matters here: active movement can elicit ownership and agency over a model hand, but the two can dissociate; asynchrony eliminated both ownership and agency, passive movement abolished agency but left ownership intact, and questionnaire data that were not normally distributed were analyzed with Wilcoxon signed-rank tests.
- Supports: reporting ownership and agency separately; cautious use of non-parametric paired tests when questionnaire data are not normally distributed.
- Does not support: final statistical plan as a formal rule; does not determine rowing results.
- Evidence type: theoretical premise plus methodological analogy.
- Confidence: verified.
- Anchors:
  - MD: `MD Papers/kalckert_ehrsson_2012_moving_rubber_hand_dissociation_ownership_agency_markdown_bundle/kalckert_ehrsson_2012_moving_rubber_hand_dissociation_ownership_agency_raw_page_marked.md`, lines 50-72, PDF page 1.
  - MD: same file, lines 570-580, PDF page 5.
  - MD: same file, lines 640-648, PDF page 6.

### Source: `waltemateEtAl2016latency`

- Source role: best for latency/responsiveness documentation and interpretation.
- What it says that matters here: feedback delay in full-body VR affects motor performance, simultaneity perception, agency, and ownership; latency should be reported and considered.
- Supports: apparatus section, calibration/latency relevance, limitations around tracking/mapping/feedback quality.
- Does not support: exact latency thresholds for HMD rowing or exact prototype adequacy.
- Evidence type: direct evidence for latency relevance; methodological analogy for full-body avatar feedback.
- Confidence: verified.
- Anchors:
  - MD: `MD Papers/waltemate_2016_latency_perceptual_judgments_motor_performance_vr_markdown_bundle/waltemate_2016_latency_perceptual_judgments_motor_performance_vr_raw_page_marked.md`, lines 37-60, PDF page 1.
  - MD: same file, lines 70-84, PDF page 1.
  - MD: same file, lines 520-540, PDF page 5.
  - MD: same file, lines 847-855, PDF page 7.

### Source: `kalckertEhrsson2017ownershipOnset`

- Source role: best for familiarization/exposure-timing rationale.
- What it says that matters here: in a moving rubber hand setup, ownership took around 23 seconds on average to emerge, and 90 percent of participants experienced it within about the first minute; the protocol used repeated onset measurements and breaks.
- Supports: giving participants at least a short familiarization period before measured ratings.
- Does not support: exact duration required for rowing embodiment, or claim that one minute is sufficient for all participants in XR rowing.
- Evidence type: methodological analogy.
- Confidence: verified.
- Anchors:
  - MD: `MD Papers/kalckert_ehrsson_2017_moving_rubber_hand_ownership_onset_time_markdown_bundle/kalckert_ehrsson_2017_moving_rubber_hand_ownership_onset_time_raw_page_marked.md`, lines 58-70, PDF page 1.
  - MD: same file, lines 244-266, PDF page 3.
  - MD: same file, lines 389-407, PDF page 5.

### Source: `mottelsonEtAl2023bodyOwnershipVr`

- Source role: field-context source for body ownership study design and analysis practice.
- What it says that matters here: body ownership studies commonly include within-subject and/or between-subject factors; within-subject designs showed larger embodiment effects in the review; power was modest; the review also contains an example of repeated-measures Likert responses analyzed with Friedman and Wilcoxon tests.
- Supports: within-subject rationale and cautious interpretation around sample/power.
- Does not support: a formal proof that this thesis must use within-subject design, or exact sample size.
- Evidence type: review context / methodological analogy.
- Confidence: verified.
- Anchors:
  - MD: `MD Papers/mottelson_2023_body_ownership_illusions_vr_markdown_bundle/mottelson_2023_body_ownership_illusions_vr_raw_page_marked.md`, lines 1117-1125, PDF page 22 / 42.
  - MD: same file, lines 1513-1520, PDF page 29 / 42.
  - MD: same file, lines 1630-1636, PDF page 32 / 42.

### Source: `seinfeldMueller2020detachedVirtualHands`

- Source role: strong methodological analogy for a counterbalanced within-group VR embodiment study.
- What it says that matters here: participants experienced both virtual hand conditions; order was fully counterbalanced; inclusion criteria, ethics approval, consent, repeated-measures analysis, and order/learning controls are reported.
- Supports: counterbalancing, order retention, neutral repeated-condition method logic, final analysis including order/learning concerns.
- Does not support: rowing-specific procedure.
- Evidence type: methodological analogy.
- Confidence: verified.
- Anchors:
  - MD: `MD Papers/seinfeld_mueller_2020_visuomotor_feedback_detached_virtual_hands_markdown_bundle/seinfeld_mueller_2020_visuomotor_feedback_detached_virtual_hands_raw_page_marked.md`, lines 119-132, PDF page 2.
  - MD: same file, lines 297-323, PDF page 5.
  - MD: same file, lines 638-684, PDF pages 7-8.
  - MD: same file, lines 958-963, PDF page 10.

### Source: `arndtEtAl2018vrRowingWorkouts`

- Source role: concrete HMD indoor rowing method example.
- What it says that matters here: stationary rowing machine data are used in VR; sensors capture sledge and handlebar movement; HTC Vive HMD is used; participants complete warm-up/baseline and two test conditions; order is randomized; participants fill questionnaires after sessions; motion sickness was slightly elevated in VR but no one quit.
- Supports: HMD rowing feasibility, warm-up/familiarization, condition procedure, optional motion-sickness reporting, paired comparison analogy.
- Does not support: embodiment claims, thesis two-mode trade-off, or validated questionnaire choice.
- Evidence type: direct related-work example / methodological analogy.
- Confidence: verified.
- Anchors:
  - MD: `MD Papers/arndt_2018_vr_hmd_rowing_workouts_markdown_bundle/arndt_2018_vr_hmd_rowing_workouts_raw_page_marked.md`, lines 47-57, PDF page 1.
  - MD: same file, lines 175-190, PDF page 2.
  - MD: same file, lines 219-253, PDF page 2.
  - MD: same file, lines 265-274, PDF page 3.
  - MD: same file, lines 318-323, PDF page 3.
  - MD: same file, lines 352-354, PDF page 3.

### Source: `colomboEtAl2025vrCyclingEffort`

- Source role: adjacent VR exercise method and safety/statistics analogy.
- What it says that matters here: all participants performed multiple conditions in randomized order to reduce order effects; screening covered physical activity ability, sitting, visual impairment, motion sickness, and epilepsy; discomfort/cybersickness was checked; descriptive and repeated-measures/non-parametric analyses were used depending distributions.
- Supports: order randomization/counterbalancing logic, safety screening rationale, short cybersickness check, descriptive statistics and non-parametric fallback as analogy.
- Does not support: rowing or embodiment directly.
- Evidence type: methodological analogy.
- Confidence: verified.
- Anchors:
  - MD: `MD Papers/colombo_2025_vr_cycling_immersion_interaction_effort_markdown_bundle/colombo_2025_vr_cycling_immersion_interaction_effort_raw_page_marked.md`, lines 307-323, PDF page 3.
  - MD: same file, lines 328-335, PDF page 3.
  - MD: same file, lines 601-622, PDF page 6.
  - MD: same file, lines 647-656, PDF page 6.
  - MD: same file, lines 908-916, PDF page 9.

### Source: `richlanEtAl2023vrSportsReview`

- Source role: broad VR sport safety and variability context.
- What it says that matters here: VR sport can be safe and repeatable when used properly, including keeping sessions short and taking breaks to avoid cybersickness; VR sports studies vary in HMD/screen/projection setup, intervention duration, and sample size.
- Supports: keeping sessions short, breaks/rest, safety limitations, cautious generalization.
- Does not support: exact rowing session duration or embodiment measures.
- Evidence type: background/context.
- Confidence: verified.
- Anchors:
  - MD: `MD Papers/richlan_2023_virtual_training_real_effects_vr_sports_review_markdown_bundle/richlan_2023_virtual_training_real_effects_vr_sports_review_raw_page_marked.md`, lines 126-134, PDF page 2.
  - MD: same file, lines 389-411, PDF page 4.

### Source: `rothLatoschik2020veq`

- Source role: questionnaire/scoring boundary source.
- What it says that matters here: VEQ was built to measure virtual embodiment and confirmed three factors: ownership, agency, and change. The article table gives mean-score formulas for VEQ Ownership, Agency, and Change; the appendix labels the corresponding questionnaire sections as Acceptance/Body Ownership, Control/Agency, and Change. A validation study tested latency/latency jitter effects on VEQ factors.
- Supports: primary outcome selection and keeping VEQ scores separate from custom exploratory items.
- Does not support: rowing-specific custom items.
- Evidence type: direct measurement source.
- Confidence: verified.
- Anchors:
  - MD: `MD Papers/roth_latoschik_2020_virtual_embodiment_questionnaire_veq_markdown_bundle/roth_latoschik_2020_virtual_embodiment_questionnaire_veq_raw_page_marked.md`, lines 37-48, PDF page 1.
  - MD: same file, lines 636-650, PDF page 6.
  - MD: same file, lines 678-697, PDF page 6.
  - MD: same file, lines 834-845, PDF page 7.
  - MD: same file, lines 974-979, PDF page 8.
  - MD: same file, lines 1783-1788, appendix PDF page 3.

## Missing / Human-Confirmation List

- TODO:CONFIRM final participant count, recruitment route, inclusion criteria, exclusion criteria, age range, compensation if any, and approval route.
- TODO:CONFIRM exact ergometer model, HMD, tracking devices, software version, room setup, calibration steps, and whether Chapter 3 will document them.
- TODO:CONFIRM exact condition labels and whether final terminology is `ergometer-congruent` / `boat-realistic`.
- TODO:CONFIRM condition order assignment: randomized, alternating, blocked, manually balanced, or fully counterbalanced.
- TODO:CONFIRM familiarization duration, standardized rowing duration, and rest duration.
- TODO:CONFIRM whether end-to-end latency can be measured, estimated, or only qualitatively discussed.
- TODO:CONFIRM final file format, pseudonymization/anonymization process, missing-data handling, and storage separation between consent/contact and analysis data.
- TODO:VERIFY final VEQ item wording, custom item wording, response scale, and all German translations before data collection.
- TODO:CONFIRM final analysis tests, alpha level, effect-size reporting, and whether analysis is primarily descriptive due to sample size.
- TODO:CITE or supervisor-confirm if a formal statistics source is required for paired t-test / Wilcoxon / repeated-measures wording.
- TODO:CONFIRM consent form, data protection wording, right-to-withdraw wording, safety checklist, and local ethics/supervisor approval requirements.

## Overclaim Boundaries

- Do not claim the study proves one representation is universally superior.
- Do not claim within-subject design eliminates order effects; it only helps control participant-level variability and requires order management.
- Do not claim counterbalancing removes fatigue, learning, or cybersickness; it reduces systematic bias.
- Do not claim the apparatus achieves close alignment or low latency unless Chapter 3 or measurements verify it.
- Do not cite Waltemate latency thresholds as direct design thresholds for the rowing prototype.
- Do not treat Arndt or Colombo as evidence for embodiment outcomes in this thesis.
- Do not treat custom rowing-specific items as validated subscales.
- Do not treat discomfort/cybersickness observations as embodiment outcomes.
- Do not state formal ethics approval, data protection compliance, or participant count until confirmed.
- Do not interpret low ratings as necessarily caused by the representation concept; tracking, calibration, latency, and prototype polish can also affect ratings.

## Recommended Citation Strategy for Chapter 4 Rest

Main text should stay citation-light and method-focused. The detailed evidence can remain in this pack.

Suggested main-text citation placement:

- Study design / VR sport representation context: cite `neumannEtAl2018interactiveVrSport` and the rowing sources only where the mode rationale is explained.
- Ergometer/on-water mismatch: cite `lamb1989kinematicComparison`, `soperHume2004rowingTechnique`, and `rauterEtAl2013rowingTransfer` near the boat-realistic rationale.
- Latency/responsiveness documentation: cite `waltemateEtAl2016latency`; optionally `rothLatoschik2020veq` if discussing VEQ latency validation.
- Familiarization rationale: cite `kalckertEhrsson2017ownershipOnset` cautiously.
- Safety/rest/cybersickness rationale: cite `richlanEtAl2023vrSportsReview` or `colomboEtAl2025vrCyclingEffort` only if the final prose explicitly discusses this literature-level rationale. Otherwise keep safety wording as procedural.
- Analysis plan: do not over-cite examples. If the final thesis needs formal statistics support, add or identify a real stats source rather than relying on adjacent VR papers.

## Suggested Chat Handoff Brief

Use this pack to draft the non-questionnaire parts of Chapter 4. Keep the prose methodical and cautious. Treat the thesis' own study design as project-authored, not as something papers prove. Cite papers only for the premises they actually support: why the two modes are a meaningful comparison, why within-subject and counterbalancing logic is reasonable in embodiment/VR exercise contexts, why latency/calibration matter, why familiarization is included, and why safety/rest/stop criteria are needed. Leave exact participant counts, durations, apparatus details, item wording, and statistics as TODOs until confirmed by the author.

## Final Source-Check Blocks for Later Use

These are not inserted into `.tex`; they are ready-to-copy blocks if the author wants audit comments later.

```tex
% SOURCE-CHECK:
%   key: lamb1989kinematicComparison; soperHume2004rowingTechnique; rauterEtAl2013rowingTransfer
%   md: MD Papers/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_markdown_bundle/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_raw_page_marked.md, lines 20-63 and 419-500; MD Papers/soper_hume_2004_ideal_rowing_technique_biomechanics_markdown_bundle/soper_hume_2004_ideal_rowing_technique_biomechanics_raw_page_marked.md, lines 79-85 and 109-123; MD Papers/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_markdown_bundle/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_raw_page_marked.md, lines 149-199 and 283-320
%   pdf: Lamb p. 1 and pp. 6-7; Soper/Hume p. 1 and p. 2; Rauter p. 2 and p. 3
%   evidence: Ergometer and on-water rowing are related but not identical; common ergometers reproduce some rowing aspects but not all trunk/upper-limb/oar mechanics; rowing on water involves rower-boat-oar-water interaction and oar/blade mechanics.
%   confidence: verified
%   caution: Supports the mode rationale and rowing mismatch, not embodiment outcomes or study results.
```

```tex
% SOURCE-CHECK:
%   key: kilteniEtAl2012senseEmbodiment
%   md: MD Papers/kilteni_2012_sense_of_embodiment_markdown_bundle/kilteni_2012_sense_of_embodiment_raw_page_marked.md, lines 190-226, 338-377, 436-444, and 922-926
%   pdf: p. 3, pp. 4-5, p. 5, and p. 11
%   evidence: SoE is associated with self-location, agency, and ownership; agency depends on predicted versus actual sensory consequences and synchronous visuomotor correlations; temporal discrepancies can affect agency.
%   confidence: verified
%   caution: Conceptual embodiment source, not rowing or protocol evidence.
```

```tex
% SOURCE-CHECK:
%   key: mottelsonEtAl2023bodyOwnershipVr
%   md: MD Papers/mottelson_2023_body_ownership_illusions_vr_markdown_bundle/mottelson_2023_body_ownership_illusions_vr_raw_page_marked.md, lines 1117-1125, 1513-1520, and 1630-1636
%   pdf: pp. 22/42, 29/42, and 32/42
%   evidence: The review notes common within-subject and between-subject factors in body ownership illusion studies, modest mean power for body-ownership manipulations, larger embodiment effects for within-subject designs, and an example of repeated-measures Likert data analyzed with Friedman/Wilcoxon tests.
%   confidence: verified
%   caution: Field-context and methodological analogy only; not a formal sample-size or statistics authority for this thesis.
```

```tex
% SOURCE-CHECK:
%   key: kalckertEhrsson2012movingRubberHand
%   md: MD Papers/kalckert_ehrsson_2012_moving_rubber_hand_dissociation_ownership_agency_markdown_bundle/kalckert_ehrsson_2012_moving_rubber_hand_dissociation_ownership_agency_raw_page_marked.md, lines 50-72, 570-580, and 640-648
%   pdf: p. 1, p. 5, and p. 6
%   evidence: Moving rubber hand study separates ownership and agency and uses Wilcoxon signed-rank tests for non-normally distributed questionnaire data.
%   confidence: verified
%   caution: Hand paradigm and method analogy only; not a final statistics authority for this thesis.
```

```tex
% SOURCE-CHECK:
%   key: neumannEtAl2018interactiveVrSport
%   md: MD Papers/neumann_2018_interactive_virtual_reality_sport_systematic_review_markdown_bundle/neumann_2018_interactive_virtual_reality_sport_systematic_review_raw_page_marked.md, lines 105-123, 228-241, and 404-419
%   pdf: p. 4, p. 7, and p. 12
%   evidence: VR sport can use exertion interfaces; physical effort on an ergometer can translate into virtual sport performance; sport VR involves computer-generated sport-relevant content and interactivity; rowing ergometer input can be transformed into virtual boat/oar movement through water.
%   confidence: verified
%   caution: Supports VR sport/exertion-interface mapping, not embodiment outcomes or this thesis' exact two-mode categories.
```

```tex
% SOURCE-CHECK:
%   key: waltemateEtAl2016latency
%   md: MD Papers/waltemate_2016_latency_perceptual_judgments_motor_performance_vr_markdown_bundle/waltemate_2016_latency_perceptual_judgments_motor_performance_vr_raw_page_marked.md, lines 37-60, 70-84, 221-229, 520-540, and 847-855
%   pdf: p. 1, p. 2, p. 5, and p. 7
%   evidence: Visual feedback latency in full-body VR affected motor performance, simultaneity, agency, and ownership; agency is discussed as a comparison between predicted and actual feedback; authors argue latency should be reported and considered.
%   confidence: verified
%   caution: Do not import exact latency thresholds as requirements for the rowing prototype.
```

```tex
% SOURCE-CHECK:
%   key: kalckertEhrsson2017ownershipOnset
%   md: MD Papers/kalckert_ehrsson_2017_moving_rubber_hand_ownership_onset_time_markdown_bundle/kalckert_ehrsson_2017_moving_rubber_hand_ownership_onset_time_raw_page_marked.md, lines 58-70, 244-266, and 389-407
%   pdf: p. 1, p. 3, and p. 5
%   evidence: Moving RHI ownership onset averaged around 23 s, and 90 percent onset occurred within about the first minute; protocol used repeated onset measurements and breaks.
%   confidence: verified
%   caution: Hand-illusion timing supports familiarization rationale only; it does not define required rowing exposure duration.
```

```tex
% SOURCE-CHECK:
%   key: seinfeldMueller2020detachedVirtualHands
%   md: MD Papers/seinfeld_mueller_2020_visuomotor_feedback_detached_virtual_hands_markdown_bundle/seinfeld_mueller_2020_visuomotor_feedback_detached_virtual_hands_raw_page_marked.md, lines 119-132, 297-323, and 638-684
%   pdf: p. 2, p. 5, and pp. 7-8
%   evidence: VR embodiment study used a within-group design, both conditions per participant, full counterbalancing, consent/ethics reporting, repeated procedure, and analysis controls for order/learning.
%   confidence: verified
%   caution: Methodological analogy only; detached virtual hands are not rowing.
```

```tex
% SOURCE-CHECK:
%   key: rothLatoschik2020veq
%   md: MD Papers/roth_latoschik_2020_virtual_embodiment_questionnaire_veq_markdown_bundle/roth_latoschik_2020_virtual_embodiment_questionnaire_veq_raw_page_marked.md, lines 37-48, 678-697, 974-979, and 1783-1788
%   pdf: p. 1, p. 6, p. 8, and appendix p. 3
%   evidence: VEQ was constructed as a virtual embodiment questionnaire with confirmed Ownership, Agency, and Change factors; the article gives mean-score formulas for VEQ Ownership and Agency items, the appendix labels scoring as Acceptance (Ownership) and Control (Agency), and latency/jitter significantly affected ownership and agency.
%   confidence: verified
%   caution: Supports VEQ ownership/agency scoring and latency sensitivity; custom rowing-specific items remain exploratory and separate.
```

```tex
% SOURCE-CHECK:
%   key: colomboEtAl2025vrCyclingEffort
%   md: MD Papers/colombo_2025_vr_cycling_immersion_interaction_effort_markdown_bundle/colombo_2025_vr_cycling_immersion_interaction_effort_raw_page_marked.md, lines 307-323, 328-335, 601-622, 647-656, and 908-916
%   pdf: p. 3, p. 6, and p. 9
%   evidence: Adjacent VR cycling study randomized exposure order to reduce order effects, screened for physical activity ability/motion sickness/epilepsy, checked discomfort/cybersickness, and used descriptive and repeated-measures/non-parametric statistics with effect-size reporting depending distribution.
%   confidence: verified
%   caution: Cycling/exercise analogy only; not rowing or embodiment-specific.
```

```tex
% SOURCE-CHECK:
%   key: richlanEtAl2023vrSportsReview
%   md: MD Papers/richlan_2023_virtual_training_real_effects_vr_sports_review_markdown_bundle/richlan_2023_virtual_training_real_effects_vr_sports_review_raw_page_marked.md, lines 126-134 and 389-411
%   pdf: p. 2 and p. 4
%   evidence: VR sport review notes that short sessions and breaks can help avoid cybersickness, and that VR sport studies vary in HMD/screen setup, intervention duration, and sample size.
%   confidence: verified
%   caution: Broad VR sport safety/context source, not a protocol for this rowing study.
```

```tex
% SOURCE-CHECK:
%   key: arndtEtAl2018vrRowingWorkouts
%   md: MD Papers/arndt_2018_vr_hmd_rowing_workouts_markdown_bundle/arndt_2018_vr_hmd_rowing_workouts_raw_page_marked.md, lines 47-57, 219-253, 265-274, 318-323, and 352-354
%   pdf: p. 1, p. 2, and p. 3
%   evidence: HMD indoor-rowing pilot used rowing-machine sensor data, virtual lake/scull, warm-up/baseline, randomized condition order, questionnaires after sessions, paired comparisons, and motion-sickness reporting.
%   confidence: verified
%   caution: Pilot/related-work evidence only; do not generalize its performance or sickness findings.
```
