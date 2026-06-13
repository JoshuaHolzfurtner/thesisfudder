# Pitch Dossier for Chat Pro 5.5: Chapter 4 Questionnaire Section

Date: 2026-06-13  
Target writer: Chat Pro 5.5  
Target location: Chapter 4, especially `chapters/04_study_design/05_measures_embodiment.tex`, `06_measures_rowing_specific.tex`, `07_data_handling_scoring.tex`, and Appendix A questionnaire files.

## Handoff Purpose

Write or revise the Chapter 4 questionnaire/measures section and, if asked, refine the questionnaire itself. The section should explain why these measures fit the thesis, not merely list survey items.

The questionnaire is the empirical translation of the thesis' central design tension:

- The ergometer-congruent mode prioritizes direct correspondence between the real ergometer movement and the virtual body/handle.
- The boat-realistic mode prioritizes recognizable rowing-on-water depiction with oars and boat context, even where the real handle path and virtual oar/hand path cannot fully match.

The questionnaire must therefore separate:

- reported ownership of the virtual body,
- reported agency/control over the virtual movement,
- exploratory body-location/alignment experience,
- rowing-specific action congruence and handle/oar mismatch,
- rowing-on-water plausibility,
- preference and comfort.

Do not collapse these into one "embodiment" score unless the author explicitly decides to do that. The thesis is interesting precisely because these dimensions may diverge.

## Current State in the Thesis

The current Chapter 4 already has a good architecture:

- `05_measures_embodiment.tex`: VEQ Ownership/Acceptance and Control/Agency are primary; body-location items are exploratory; no single undifferentiated embodiment score.
- `06_measures_rowing_specific.tex`: custom rowing-specific items cover embodied action congruence, real handle anchoring, virtual hand/oar mapping, sport-action plausibility, and perceived mismatch.
- `07_data_handling_scoring.tex`: VEQ scores are means of selected VEQ items; custom items and preference are reported separately.
- Appendix A has English and German draft questionnaires, plus a post-comparison block.

The writer's job is not to invent a new study. The job is to make the rationale crisp, source-backed, and methodologically cautious.

## Recommended Section Pitch

The Chapter 4 questionnaire section should read as a measurement argument:

1. Start from the research question: the study compares two representation strategies for the same real rowing action.
2. Explain that embodiment is measured through explicit self-report because the first evaluation focuses on subjective experience of the virtual body and movement.
3. Use VEQ Ownership/Acceptance and Control/Agency as the primary outcomes.
4. Explain why VEQ Change is not primary: the study does not mainly manipulate perceived body size, shape, or body-schema change.
5. Add exploratory body-location items because self-location is conceptually relevant but not preserved as a final VEQ factor.
6. Add custom rowing-specific items because VEQ does not measure whether the real handle, virtual hands/oars, and rowing depiction make sense as rowing.
7. Keep safety/comfort and preference separate from embodiment scoring.
8. Close by saying that the questionnaire design allows divergent profiles: one mode may feel more controllable, another may look more like rowing, and user preference may not follow ownership or agency.

Suggested section logic in prose:

> The questionnaire was designed to keep established embodiment measures separate from thesis-specific rowing interface questions. VEQ ownership and agency items capture whether the virtual rowing body and its movements are experienced as one's own and under one's control. Additional exploratory items capture body-location, real-handle anchoring, hand/oar mapping, sport-action plausibility, and perceived mismatch, because these are the concrete dimensions on which the two rowing representations differ. This structure avoids interpreting a preference for the boat-like scene as stronger embodiment, or a stronger sense of control in the ergometer-congruent mode as general superiority.

## Recommended Questionnaire Architecture

Use a short within-subject questionnaire after each condition, followed by a comparison questionnaire after both conditions.

### Per-Condition Block

Use one 7-point agreement scale for all per-condition items unless the author changes it:

`1 = strongly disagree` through `7 = strongly agree`.

Participant-facing labels can be neutral. The appendix may group items by construct for auditability, but the actual form should avoid over-explaining the constructs to participants if possible.

Recommended order:

1. VEQ Ownership/Acceptance, four items.
2. VEQ Control/Agency, four items.
3. Exploratory body-location, two items.
4. Rowing-specific exploratory items, ideally 6-8 items.
5. Safety/comfort check, not scored with embodiment.
6. Open comment about convincing or mismatched aspects.

### Primary VEQ Items

Keep VEQ wording as close as possible to the source if treating the subscales as VEQ-derived. Current Appendix A wording matches the English VEQ sheet closely.

Ownership/Acceptance:

- It felt like the virtual body was my body.
- It felt like the virtual body parts were my body parts.
- The virtual body felt like a human body.
- It felt like the virtual body belonged to me.

Control/Agency:

- The movements of the virtual body felt like they were my movements.
- I felt like I was controlling the movements of the virtual body.
- I felt like I was causing the movements of the virtual body.
- The movements of the virtual body were in sync with my own movements.

Scoring:

- Ownership/Acceptance = mean of the four ownership items.
- Control/Agency = mean of the four agency items.
- Do not mix exploratory rowing items into these scores.

### Exploratory Body-Location Items

Keep these separate from VEQ:

- I felt as if my body was located where I saw the virtual rowing body.
- I felt as if my hands were located where I saw the virtual hands.

Rationale:

- Kilteni treats self-location as one component of SoE.
- VEQ discusses self-location but does not retain it as a final VEQ factor.
- Gonzalez-Franco and Peck include body-location/co-location as an embodiment questionnaire category.

### Rowing-Specific Exploratory Items

The current Appendix A item list is directionally good. The construct set should stay:

- embodied action congruence,
- real handle as haptic/proprioceptive anchor,
- virtual hand/oar mapping acceptability,
- controllable extension/tool-like action,
- sport-action plausibility,
- perceived mismatch/conflict.

Current items worth keeping:

- The virtual rowing body felt connected to the movement I performed on the real ergometer.
- The real handle I was holding fit with the virtual hands, handle, or oars I saw.
- The real handle I was holding made the virtual rowing action feel physically grounded.
- The virtual hand and arm movement made sense in relation to my real handle movement.
- The virtual oar or rowing motion felt like a controllable extension of my own action.
- The representation felt believable as rowing on water.
- The visible hand, handle, or oar path made sense for the rowing representation I saw.
- I noticed a conflict between the real handle movement and the virtual hand or oar movement.

Potential tightening:

- If the questionnaire feels too long, keep six custom items: connected movement, handle fit, hand/arm mapping, controllable extension, rowing-on-water plausibility, conflict/mismatch.
- Keep the negative mismatch item separate or reverse-code only if a final scoring scheme is explicitly documented.
- Do not call these validated scales. Call them custom exploratory thesis-specific items.

### Safety and Comfort

Keep safety and comfort separate:

- dizziness,
- nausea,
- pain,
- unsafe discomfort,
- distress,
- headset/erg fit issue.

Do not interpret comfort as embodiment. It is feasibility/safety/limitation material.

Avoid adding a full cybersickness questionnaire unless the author wants the extra burden. The current first-data-collection version is intentionally lightweight.

### Post-Comparison Block

Administer only after both conditions:

- Which representation did you prefer overall?
- Which representation felt more directly connected to your real ergometer movement?
- Which representation looked more like rowing on water?
- In which representation did the relation between the real handle and the virtual hands or oars feel more convincing?
- Which representation would you rather use again?
- Open comment: main difference noticed between the two rowing representations.

Open decision:

- Forced choice is simple and fits a small study.
- A 7-point comparative scale gives more nuance.
- Using both may be possible but increases burden. Decide before pilot testing and document it.

## How Section and Questionnaire Are Interwoven

The section should explicitly state that the questionnaire is not generic. Each block corresponds to one layer of the design tension:

| Design issue | Questionnaire layer | Interpretation |
| --- | --- | --- |
| Does the virtual body feel like mine? | VEQ Ownership/Acceptance | Body ownership outcome |
| Do I feel I control/cause the movement? | VEQ Control/Agency | Agency outcome |
| Do I feel spatially aligned with the avatar/hands? | Exploratory body-location items | Self-location/body-location cue, not VEQ |
| Does the real handle anchor the virtual action? | Custom handle/grounding items | Haptic/proprioceptive bridge |
| Does the hand/oar mapping make sense? | Custom mapping items | Where boat mode may gain or lose |
| Does it look like rowing on water? | Custom sport-action plausibility item | Boat-realistic strength, not embodiment by itself |
| Do I notice conflict/mismatch? | Custom mismatch item | Direct probe of the tradeoff |
| Which mode would I choose? | Post-comparison preference | Design-facing outcome, not proof of embodiment |

This table is a good hidden blueprint for the section. It does not need to appear in the thesis unless useful.

## Suggested Chapter 4 Wording Skeleton

Use this as a scaffold, not final prose:

> The questionnaire was designed around the distinction between established embodiment constructs and rowing-specific interface experience. The primary embodiment outcomes were ownership and agency, measured with the Ownership/Acceptance and Control/Agency subscales of the Virtual Embodiment Questionnaire. These subscales correspond directly to the study question: whether the virtual rowing body and its movement are experienced as belonging to the participant and as being caused or controlled by the participant's own rowing action. The VEQ Change subscale was not used as a primary outcome because the study does not primarily manipulate avatar body size, shape, or body-schema change.

> Because self-location remains conceptually relevant to sense of embodiment, but is not retained as a final VEQ factor, the questionnaire included exploratory body-location items adapted from avatar embodiment questionnaire practice. These items were analyzed separately from the VEQ subscales.

> The study also included custom rowing-specific items. These were necessary because the main manipulation is not an abstract avatar manipulation but a representational choice in a sport-specific, equipment-mediated task. The custom items therefore asked whether the virtual rowing body felt connected to the real ergometer movement, whether the real handle fitted the virtual hand/handle/oar representation, whether the visible hand and oar path made sense, whether the action appeared believable as rowing on water, and whether participants noticed conflict between the felt handle path and the seen virtual movement.

> Custom rowing-specific items were treated as exploratory and were not combined with VEQ scores. This separation allows the analysis to report cases where a condition feels more controllable but less rowing-realistic, or more rowing-realistic but less directly connected to the physical ergometer action.

## Source Map for the Writer

Use only citation keys that already exist in `references.bib`.

### Core Measurement Sources

`rothLatoschik2020veq`

- Use for VEQ as validated self-report instrument.
- Supports final factors Ownership/Acceptance, Control/Agency, and Change.
- Supports four items per factor and mean scoring.
- Anchors:
  - `MD Papers/roth_latoschik_2020_virtual_embodiment_questionnaire_veq_markdown_bundle/roth_latoschik_2020_virtual_embodiment_questionnaire_veq_thesis_notes.md`, lines 21-34, 46-67, 170-179, 207-229.
  - `MD Papers/roth_latoschik_2020_virtual_embodiment_questionnaire_veq_markdown_bundle/roth_latoschik_2020_virtual_embodiment_questionnaire_veq_clean_reading.md`, lines 603-622 and 1457-1666.
- Caution: VEQ does not directly preserve self-location as a final factor. Do not present Change as primary unless body-schema change is actually studied.

`gonzalezFrancoPeck2018avatarEmbodiment`

- Use for avatar embodiment questionnaire categories and body-location items.
- Useful categories: ownership, agency/motor control, tactile sensation, location of the body, appearance, response to stimuli.
- Anchors:
  - `MD Papers/gonzalez_franco_peck_2018_avatar_embodiment_questionnaire_markdown_bundle/gonzalez_franco_peck_2018_avatar_embodiment_questionnaire_thesis_notes.md`, lines 17-41, 53-60, 62-76, 188-198, 249-258.
  - `MD Papers/gonzalez_franco_peck_2018_avatar_embodiment_questionnaire_markdown_bundle/gonzalez_franco_peck_2018_avatar_embodiment_questionnaire_clean_reading.md`, lines 434-582.
- Caution: questionnaire proposal, not a fully validated gold standard. Do not overstate.

### Conceptual Embodiment Sources

`kilteniEtAl2012senseEmbodiment`

- Use for SoE subcomponents: self-location, agency, body ownership.
- Use for measuring SoE through subcomponents rather than one direct global measure.
- Use for agency dependence on visuomotor synchrony and ownership dependence on sensory/morphological/spatial cues.
- Anchors:
  - `MD Papers/kilteni_2012_sense_of_embodiment_markdown_bundle/kilteni_2012_sense_of_embodiment_thesis_notes.md`, lines 15-30, 47-80, 83-100.
  - `MD Papers/kilteni_2012_sense_of_embodiment_markdown_bundle/kilteni_2012_sense_of_embodiment_raw_page_marked.md`, lines 214-229, 338-376, 377-426, 673-688, 719-770, 808-840, 921-957.
- Caution: self-location is not presence. Do not claim the three components are independent in a strong sense.

`kalckertEhrsson2012movingRubberHand`

- Use to justify separate reporting of ownership and agency.
- Supports that ownership and agency can be dissociated and that synchrony matters.
- Anchors:
  - `MD Papers/kalckert_ehrsson_2012_moving_rubber_hand_dissociation_ownership_agency_markdown_bundle/kalckert_ehrsson_2012_moving_rubber_hand_dissociation_ownership_agency_thesis_notes.md`, lines 20-45, 47-65.
  - `MD Papers/kalckert_ehrsson_2012_moving_rubber_hand_dissociation_ownership_agency_markdown_bundle/kalckert_ehrsson_2012_moving_rubber_hand_dissociation_ownership_agency_raw_page_marked.md`, lines 52-65, 590-704, 1213-1218.
- Caution: finger/rubber-hand paradigm, not rowing. Use as construct rationale, not direct rowing evidence.

`kalckertEhrsson2017ownershipOnset`

- Use for familiarization/questionnaire timing.
- Supports not asking ownership questions immediately after a few seconds of exposure.
- Anchors:
  - `MD Papers/kalckert_ehrsson_2017_moving_rubber_hand_ownership_onset_time_markdown_bundle/kalckert_ehrsson_2017_moving_rubber_hand_ownership_onset_time_thesis_notes.md`, lines 37-58, 60-72, 130-148, 192-211.
  - `MD Papers/kalckert_ehrsson_2017_moving_rubber_hand_ownership_onset_time_markdown_bundle/kalckert_ehrsson_2017_moving_rubber_hand_ownership_onset_time_raw_page_marked.md`, lines 52-69, 276-302, 316-340.
- Caution: does not prove a one-minute rowing exposure guarantees ownership. It only supports a short stable familiarization period.

`mottelsonEtAl2023bodyOwnershipVr`

- Optional supporting review for VR body ownership research, measurement heterogeneity, and strong role of visuomotor synchrony.
- Anchor: `MD Papers/mottelson_2023_body_ownership_illusions_vr_markdown_bundle/mottelson_2023_body_ownership_illusions_vr_thesis_notes.md`, lines 11-34, 43-59, 60-65.
- Caution: high-level review; do not use as the sole definition of embodiment.

`girondiniEtAl2025humanBodiesVirtualWorlds`

- Optional modern review for explicit vs implicit measures and SoA/SoO separation.
- Anchor: `MD Papers/girondini_2025_human_bodies_virtual_worlds_markdown_bundle/girondini_2025_human_bodies_virtual_worlds_thesis_notes.md`, lines 18-27, 42-50, 57-91, 105-123.
- Caution: review of immersive VR implicit measures, not rowing.

### Rowing-Specific Sources for Custom Items

`lamb1989kinematicComparison`

- Use to justify that ergometer and on-water rowing are related but not identical, especially around arm/oar/finish mechanics.
- Anchors:
  - `MD Papers/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_markdown_bundle/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_thesis_notes.md`, lines 17-31, 80-135, 137-164, 198-208.
  - `MD Papers/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_markdown_bundle/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_raw_page_marked.md`, lines 20-65, 419-500.
- Caution: rowing biomechanics source, not embodiment or questionnaire source.

`soperHume2004rowingTechnique`

- Use for rowing stroke structure and ergometer vs on-water distinction.
- Anchor: `MD Papers/soper_hume_2004_ideal_rowing_technique_biomechanics_markdown_bundle/soper_hume_2004_ideal_rowing_technique_biomechanics_thesis_notes.md`, lines 13-24, 46-65, 88-125, 127-162, 163-172.
- Caution: not VR, not embodiment, not proof of a best representation.

`rauterEtAl2013rowingTransfer`

- Use to justify that oar-water interaction, oar handling, blade depth/angle, and rowing simulators are meaningful in rowing-system design.
- Anchor: `MD Papers/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_markdown_bundle/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_thesis_notes.md`, lines 26-38, 48-62, 63-106, 117-150, 152-163.
- Caution: high-fidelity rowing simulator/skill transfer, not embodiment. Do not cite as proof that this thesis prototype teaches technique.

### VR Sport / Realism Cleanup Sources

`neumannEtAl2018interactiveVrSport`

- Use only for situating the system as interactive VR sport / exertion interface.
- Anchor: `MD Papers/neumann_2018_interactive_virtual_reality_sport_systematic_review_markdown_bundle/neumann_2018_interactive_virtual_reality_sport_systematic_review_thesis_notes.md`, lines 23-40, 41-58, 73-105, 147-155.
- Caution: not questionnaire or embodiment evidence.

`harrisEtAl2019visionForAction`

- Use to warn that visual sport realism does not equal action realism.
- Anchor: `MD Papers/harris_2019_virtually_the_same_vr_vision_for_action_markdown_bundle/harris_2019_virtually_the_same_vr_vision_for_action_thesis_notes.md`, lines 10-27, 43-52, 111-148, 149-166, 198-207.
- Caution: not rowing-specific and not a questionnaire source.

`slater2009placePlausibility`

- Use if presence/plausibility must be distinguished from embodiment.
- Anchor: `MD Papers/slater_2009_place_illusion_plausibility_realistic_behaviour_vr_markdown_bundle/slater_2009_place_illusion_plausibility_realistic_behaviour_vr_thesis_notes.md`, lines 50-77, 78-92, 139-172, 173-183.
- Caution: do not claim place illusion equals ownership.

`skarbezEtAl2017presenceSurvey`

- Use for terminology cleanup: presence, immersion, fidelity, coherence, embodiment.
- Anchor: `MD Papers/skarbez_2017_survey_presence_related_concepts_markdown_bundle/skarbez_2017_survey_presence_related_concepts_thesis_notes.md`, lines 44-68, 78-118, 130-138, 203-211, 233-242.
- Caution: not primary embodiment mechanism evidence.

### Paper Coverage / Boundary Check

The repository contains more useful papers than this questionnaire section should cite. For Chapter 4 measures, keep the citation stack lean: core measurement sources, the embodiment construct sources needed to justify separate ownership/agency/body-location measures, and rowing-specific sources needed for custom items.

Use these adjacent sources only if the section expands into their specific topic:

- `botvinickCohen1998rubberHand`: classic rubber-hand ownership background; useful for Chapter 2, not necessary for the questionnaire architecture unless briefly tracing why ownership is measured.
- `iontaEtAl2011bodilySelfConsciousness`: self-location and multisensory bodily self-consciousness; optional if strengthening the exploratory body-location rationale.
- `waltemateEtAl2016latency`: latency/temporal congruence and motor-performance judgments in VR; useful for system limitations or timing rationale, not item wording.
- `lokEtAl2002realObjectsSelfAvatar`: real objects and self-avatar fidelity in virtual environments; optional if the real ergometer handle is discussed as a physical anchor, but do not claim the handle is embodied unless measured.
- `diPinoEtAl2014augmentationBrainPlasticity`, `martelEtAl2016toolUseBodyRepresentation`, `millerEtAl2017visualToolUse`: tool/body-representation background; optional for virtual oars as tool-mediated action, not core questionnaire evidence.
- `seinfeldMueller2020detachedVirtualHands` and `odermattEtAl2021congruencyOwnershipPerformance`: optional VR hand/congruency sources; cite only if the writer adds a short bridge from visuomotor congruence to virtual hand ownership/control.
- `kocurEtAl2022rubberHandVrRealWorld`, `kocurEtAl2025customizedAvatarsExercise`, `pilacinskiEtAl2023phantomTouch`: adjacent avatar/RHI/VR-exercise sources; not needed unless Chapter 4 adds avatar appearance, real-world transfer, or phantom-touch claims.
- `maHommel2013virtualHandIllusion`: threat/impact and affective response; do not cite in the questionnaire section unless a threat or physiological probe is actually included.
- `arndtEtAl2018vrRowingWorkouts`, `murrayEtAl2016vrRowingPresence`, `richlanEtAl2023vrSportsReview`, `colomboEtAl2025vrCyclingEffort`, `hibbsEtAl2024vrImmersionCycling`: related-work and VR-sport framing; useful elsewhere, but not evidence that the current questionnaire measures embodiment.
- `ashidaFujimoto2022opticFlowBodySway`, `niehorster2021opticFlowHistory`, `palmisanoEtAl2015vectionChallenges`, `kooijmanEtAl2024measuringVection`: optic-flow/vection sources; only use if vection is measured or carefully framed as future work. Do not let vection become an implicit embodiment score.
- `bacaEtAl2006footStretcherForceProfiles`, `floodSimpsonCompleteGuideIndoorRowing`: rowing mechanics/history/context; optional support for ergometer/on-water differences, but Lamb, Soper/Hume, and Rauter are usually enough for the custom-item rationale.

Bottom line: if a source does not support a measurement choice, a custom item category, or a scoring/interpretation rule, leave it out of the Chapter 4 questionnaire section.

## Existing Project Anchors

Use these files before writing:

- `AGENTS.md`: no invented thesis content, no invented citations, no overclaims.
- `notes/global/thesis_spine.md`: one-sentence thesis and contribution hierarchy.
- `notes/global/claims_register.md`: allowed and forbidden wording.
- `notes/global/terminology.md`: official terminology.
- `notes/global/contribution_hierarchy.md`: system/prototype first, theory as lens.
- `notes/chapters/04_study_design_back_of_mind.md`: Chapter 4 purpose and TODOs.
- `New_Outline.md`, lines 152-179: Chapter 4 should keep measures lean and participant-friendly.
- `thesis_notes_from_chat_marked_points.md`, lines 222-306: questionnaire/evaluation notes and recommended order.
- `rowing_project_agent_context_Thesis.md`, lines 38-48 and 112-123: condition control and measurement cautions.

## Guardrails

Do not invent:

- participant count,
- final sample size,
- final item order,
- final German wording,
- exact exposure duration,
- exact counterbalancing scheme,
- statistical significance,
- results,
- apparatus details not already supplied,
- new sources or BibTeX entries.

Use `TODO:CITE` if a claim needs evidence and no existing key supports it. Use `TODO:VERIFY` if the likely source must still be checked.

Safe wording:

- "primary self-report outcomes"
- "exploratory thesis-specific items"
- "participant-reported ownership/agency"
- "may support"
- "is intended to capture"
- "reported separately"
- "not combined with VEQ scores"

Avoid:

- "proves embodiment"
- "objective embodiment"
- "validated rowing embodiment scale"
- "boat mode is more realistic" without specifying "sport-action depiction"
- "erg mode is better"
- "presence equals embodiment"
- "the real handle becomes embodied" unless measured directly.

## Open Decisions for the Author

These should stay TODOs until the author decides:

- Final English item wording against VEQ source sheet.
- Final German item wording by a human German speaker.
- Whether participant-facing questionnaire shows construct headings or only neutral item blocks.
- Whether item order is grouped or randomized.
- Whether post-comparison questions are forced choice, 7-point comparative ratings, or both.
- Exact familiarization duration and rowing duration per condition.
- Exact data table format and missing-data handling.
- Whether open comments are translated, paraphrased, or quoted.
- Whether the study remains lightweight on sickness/comfort or adds a fuller cybersickness scale.

## Best Final Shape

The best version of this section is modest, rigorous, and useful:

- It names VEQ as the primary validated questionnaire basis.
- It explains why only Ownership/Acceptance and Control/Agency are primary.
- It keeps body-location exploratory.
- It defends custom rowing-specific items as necessary because the thesis compares two rowing representations, not a generic avatar.
- It states scoring rules clearly.
- It keeps preference, realism, comfort, and comments analytically separate.
- It leaves TODOs where the author still needs to decide the final protocol.

In short: the questionnaire should not ask "Which mode is more embodied?" It should let the data show whether ownership, agency, body-location, rowing realism, mismatch, comfort, and preference move together or apart.
