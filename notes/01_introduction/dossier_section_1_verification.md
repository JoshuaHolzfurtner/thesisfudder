# Chapter 1 Citation Dossier Verification

Status: source-support audit for `notes/01_introduction/dossier_section_1.md`. This file checks whether the dossier's citation suggestions are supported by the cited sources. It does not rewrite thesis prose, edit `.tex` files, or add citations to the thesis.

All external citation keys checked below are present in `references.bib`. Source verification used the cited markdown files, with raw page-marked markdown used for all external literature anchors checked here.

## Entry 1.1.1 - Indoor rowing is whole-body, technically structured, and ergometer-based

### Verdict
too broad

### Claim checked
Indoor rowing is whole-body, technically structured, and ergometer-based.

### Source checked
`soperHume2004rowingTechnique`: `MD Papers/soper_hume_2004_ideal_rowing_technique_biomechanics_markdown_bundle/soper_hume_2004_ideal_rowing_technique_biomechanics_raw_page_marked.md`, lines 79-85.

`lamb1989kinematicComparison`: `MD Papers/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_markdown_bundle/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_raw_page_marked.md`, lines 86-98.

### Evidence check
Soper and Hume support that rowing ergometers are commonly used for performance testing, technique coaching, crew selection, and poor-weather training. Lamb supports that the rowing stroke is a cyclic sequence with catch, drive, finish, and recovery. The listed anchors do not fully support the "whole-body" part; that is better supported by Lamb's abstract lines 42-60 or Rauter's lines 283-302 on sequential movement of legs, trunk, and arms.

### Anchor check
- MD path: valid
- Line range: valid
- PDF page: valid

### Source role
supporting

### Required action
- narrow the claim
- replace source with `rauterEtAl2013rowingTransfer` for the whole-body/coordinated movement wording, or add the stronger Lamb abstract anchor

## Entry 1.1.2 - Ergometer rowing approximates training aspects but differs from on-water rowing

### Verdict
verified

### Claim checked
Ergometer rowing approximates important rowing-training aspects but differs from on-water rowing.

### Source checked
`lamb1989kinematicComparison`: raw page-marked markdown lines 20-63 and 419-483.

`soperHume2004rowingTechnique`: raw page-marked markdown lines 109-123.

### Evidence check
The Lamb abstract and discussion directly support the "related but not identical" claim: most drive-phase variables were similar, especially legs and trunk, while upper arm and forearm differed at the beginning and end of the drive. Soper and Hume support that ergometers reproduce parts of the body action but not trunk and upper-limb patterns well compared with on-water rowing.

### Anchor check
- MD path: valid
- Line range: valid
- PDF page: valid; the Lamb 419-483 range plausibly spans pages 6-7

### Source role
best

### Required action
- keep as verified

## Entry 1.1.3 - VR can reintroduce rowing context, environments, avatars, and social context

### Verdict
verified

### Claim checked
VR can reintroduce visual rowing context, virtual environments, avatars, and social context.

### Source checked
`murrayEtAl2016vrRowingPresence`: raw page-marked markdown lines 42-55 and 266-283.

`arndtEtAl2018vrRowingWorkouts`: raw page-marked markdown lines 47-57 and 219-253.

`neumannEtAl2018interactiveVrSport`: raw page-marked markdown lines 228-239.

### Evidence check
Murray supports ergometer rowing in VR, including individual and companion VR and an avatar whose stroke timing matched the ergometer. Arndt supports an HMD rowing-machine prototype using sensors, a virtual lake, and a scull. Neumann supports the broader definition of VR sport as computer-simulated sport environments with interactivity and presence aims.

### Anchor check
- MD path: valid
- Line range: valid
- PDF page: valid

### Source role
best for concrete VR rowing examples; background for the general VR sport definition

### Required action
- keep as verified
- mark TODO:CITE for "spatial sound" if that phrase remains in the thesis prose; these anchors do not support it

## Entry 1.1.4 - Exertion on stationary equipment can drive movement through a virtual environment

### Verdict
verified

### Claim checked
Physical exertion on stationary exercise equipment can drive movement through a virtual environment.

### Source checked
`murrayEtAl2016vrRowingPresence`: raw page-marked markdown lines 76-99.

`neumannEtAl2018interactiveVrSport`: raw page-marked markdown lines 405-416.

### Evidence check
Murray explicitly states that in VR exercise applications, physical exertion on exercise equipment allows movement through a virtual environment. Neumann gives the rowing-ergometer example where handle pulls become virtual oar movement and higher exertion changes virtual movement through water/scenery.

### Anchor check
- MD path: valid
- Line range: valid
- PDF page: valid

### Source role
best

### Required action
- keep as verified

## Entry 1.1.5 - Optic flow and visual motion may support an impression of self-motion

### Verdict
verified

### Claim checked
Optic flow and visual motion may support an impression of self-motion while the body remains stationary.

### Source checked
`niehorster2021opticFlowHistory`: raw page-marked markdown lines 28-34 and 75-79.

`kooijmanEtAl2024measuringVection`: raw page-marked markdown lines 45-53.

`palmisanoEtAl2015vectionChallenges`: raw page-marked markdown lines 46-54 and 899-904.

### Evidence check
Niehorster supports optic flow as a global visual-motion pattern caused by and signaling self-motion, and notes that observers can perceive direction of self-motion from optic flow. Kooijman and Palmisano support vection/self-motion as subjective self-motion in the absence of actual physical motion, commonly in stationary observers. The wording must remain cautious and should not imply that vection was measured.

### Anchor check
- MD path: valid
- Line range: valid
- PDF page: valid

### Source role
best for self-motion/vection definitions when Kooijman or Palmisano are included; Niehorster is best for optic flow definition only

### Required action
- keep as verified
- narrow the claim if it drifts toward measured vection, presence, ownership, or agency

## Entry 1.1.6 - VR rowing creates a design problem because visual restoration does not remove the ergometer

### Verdict
likely

### Claim checked
VR indoor rowing creates a design problem because the boat/oars can be visually restored, but the user remains on an ergometer.

### Source checked
`soperHume2004rowingTechnique`: raw page-marked markdown lines 109-123.

`lamb1989kinematicComparison`: raw page-marked markdown lines 453-483.

`rauterEtAl2013rowingTransfer`: raw page-marked markdown lines 149-199.

### Evidence check
The sources support the premises: ergometers are biomechanically incomplete relative to on-water rowing, Lamb documents arm/oar differences around catch/finish, and Rauter describes continuous haptic rower-boat-oar-water interaction plus ordinary ergometer limitations. The broader "design problem" is a thesis synthesis, not a claim directly made by the cited sources.

### Anchor check
- MD path: valid
- Line range: valid
- PDF page: valid

### Source role
supporting

### Required action
- downgrade to likely
- narrow the claim by making clear it is the thesis' design interpretation of the source-backed rowing-interface mismatch

## Entry 1.2.1 - Ergometer and boat do not provide the same movement interface

### Verdict
verified

### Claim checked
A rowing ergometer and a rowing boat do not provide the same movement interface.

### Source checked
`lamb1989kinematicComparison`: raw page-marked markdown lines 419-483.

`soperHume2004rowingTechnique`: raw page-marked markdown lines 109-123.

`rauterEtAl2013rowingTransfer`: raw page-marked markdown lines 149-199.

### Evidence check
The cited sources directly support a descriptive interface difference: ergometer and on-water rowing share some leg/trunk drive characteristics but differ in arm/oar mechanics, central-pulley ergometers do not reproduce trunk and upper-limb patterns well, and ordinary ergometers do not train oar handling or oar height in water.

### Anchor check
- MD path: valid
- Line range: valid
- PDF page: valid

### Source role
best

### Required action
- keep as verified

## Entry 1.2.2 - The two representation strategies are thesis-defined modes

### Verdict
verified

### Claim checked
The two representation strategies are thesis-defined modes rather than literature categories.

### Source checked
Internal: `notes/global/thesis_spine.md`, lines 5-17; `notes/chapters/01_introduction_back_of_mind.md`, lines 5-19.

External support: `harrisEtAl2019visionForAction`, raw page-marked markdown lines 34-45 and 257-286.

### Evidence check
The internal notes define the thesis comparison. Harris supports the caution that visually convincing VR action can differ from real-world action because of altered depth cues and limited haptic information. Harris does not name the two modes, and the dossier correctly warns against citing it as if it did.

### Anchor check
- MD path: valid
- Line range: valid
- PDF page: valid for Harris; not applicable for internal notes

### Source role
best for internal framing; supporting for Harris

### Required action
- keep as verified

## Entry 1.2.3 - Visuomotor congruence and sport depiction can come apart in indoor rowing

### Verdict
too broad

### Claim checked
Visuomotor congruence and realistic sport depiction can support different design goals and come apart in indoor rowing.

### Source checked
`harrisEtAl2019visionForAction`: raw page-marked markdown lines 34-45.

`kilteniEtAl2012senseEmbodiment`: raw page-marked markdown lines 338-377.

`waltemateEtAl2016latency`: raw page-marked markdown lines 37-60 and 70-84.

### Evidence check
The sources support narrower premises: Harris supports the distinction between visual realism and action-relevant sensory/haptic fidelity; Kilteni supports agency as related to matching predicted and actual sensory consequences and synchronous visuomotor correlations; Waltemate supports latency effects on performance, agency, ownership, and simultaneity. These sources alone do not establish the rowing-specific "come apart" premise. That part needs the rowing mechanics sources already used elsewhere, especially `lamb1989kinematicComparison` and `rauterEtAl2013rowingTransfer`.

### Anchor check
- MD path: valid
- Line range: valid
- PDF page: valid; Kilteni 338-377 plausibly spans pages 4-5

### Source role
supporting

### Required action
- downgrade to likely
- narrow the claim, or add `lamb1989kinematicComparison` and `rauterEtAl2013rowingTransfer` for the indoor-rowing-specific split

## Entry 1.3.1 - Sense of embodiment includes self-location, agency, and body ownership

### Verdict
verified

### Claim checked
Sense of embodiment commonly includes self-location, agency, and body ownership.

### Source checked
`kilteniEtAl2012senseEmbodiment`: raw page-marked markdown lines 35-49, 190-226, and 436-444.

### Evidence check
Kilteni et al. directly define SoE and state that it consists of self-location, agency, and body ownership. The source also defines SoE toward a body as processing that body's properties as if they were one's biological body.

### Anchor check
- MD path: valid
- Line range: valid
- PDF page: valid

### Source role
best

### Required action
- keep as verified

## Entry 1.3.2 - Spatial and temporal alignment can influence ownership and agency

### Verdict
verified

### Claim checked
Spatial and temporal alignment of seen and felt signals can influence ownership and agency.

### Source checked
`botvinickCohen1998rubberHand`: raw page-marked markdown lines 45-55 and 116-162.

`kalckertEhrsson2012movingRubberHand`: raw page-marked markdown lines 50-72 and 109-156.

`kilteniEtAl2012senseEmbodiment`: raw page-marked markdown lines 338-377.

### Evidence check
Botvinick and Cohen support the classic synchronous rubber-hand setup and show reduced illusion prevalence under asynchrony. Kalckert and Ehrsson support multisensory matching for ownership and report that asynchrony eliminated both ownership and agency in their moving rubber-hand paradigm. Kilteni supports agency as linked to synchronous visuomotor correlations and negatively affected by visual-feedback discrepancies.

### Anchor check
- MD path: valid
- Line range: valid
- PDF page: valid; Kalckert/Ehrsson 109-156 plausibly spans pages 1-2 and Kilteni 338-377 plausibly spans pages 4-5

### Source role
best

### Required action
- keep as verified

## Entry 1.3.3 - Rowing differs from classic hand-ownership paradigms

### Verdict
likely

### Claim checked
Rowing differs from classic hand-ownership paradigms because it is active, rhythmic, tool-mediated, and whole-body.

### Source checked
`rauterEtAl2013rowingTransfer`: raw page-marked markdown lines 149-165 and 283-302.

`martelEtAl2016toolUseBodyRepresentation`: raw page-marked markdown lines 31-41 and 1574-1596.

### Evidence check
Rauter supports the rowing-action description: continuous haptic interaction among rower, boat, oar, and water; periodic strokes; and a sequential movement of legs, trunk, and arms. Martel supports the general claim that tool use can affect body representation/body schema, but it is conceptual background rather than rowing evidence. The contrast with classic hand-ownership paradigms is a thesis synthesis.

### Anchor check
- MD path: valid
- Line range: valid
- PDF page: valid

### Source role
best for Rauter; background for Martel

### Required action
- keep as likely

## Entry 1.3.4 - Boat-centric depiction may support sport realism and plausibility

### Verdict
likely

### Claim checked
A boat-centric depiction may support sport realism and plausibility even when bodily/device congruence is weaker.

### Source checked
`slater2009placePlausibility`: raw page-marked markdown lines 29-41 and 571-580.

`rauterEtAl2013rowingTransfer`: raw page-marked markdown lines 283-320.

`harrisEtAl2019visionForAction`: raw page-marked markdown lines 34-45.

### Evidence check
Slater supports plausibility illusion as the illusion that what appears to be happening is really happening. Rauter supports the rowing-specific oar/boat/water action structure. Harris supports caution that visual realism and action-relevant sensorimotor fidelity are not the same. Together these support a cautious design rationale, not a measured claim that a boat-centric depiction increases sport realism or preference.

### Anchor check
- MD path: valid
- Line range: valid
- PDF page: valid

### Source role
supporting

### Required action
- keep as likely
- narrow the claim if it is used as evidence of measured sport realism

## Entry 1.3.5 - Preference is an exploratory complement

### Verdict
likely

### Claim checked
Preference is an exploratory complement, not the main theoretical construct.

### Source checked
Internal: `notes/global/thesis_spine.md`, lines 11-17; `notes/chapters/01_introduction_back_of_mind.md`, lines 21-29.

External support: `neumannEtAl2018interactiveVrSport`, raw page-marked markdown lines 73-88; `murrayEtAl2016vrRowingPresence`, raw page-marked markdown lines 42-55.

### Evidence check
The internal notes support the study framing. Neumann supports that interactive VR sport outcomes include psychological and performance outcomes influenced by athlete, task, environment, and system factors. Murray supports enjoyment, motivation/affect, and performance in VR rowing. These sources do not make preference a theoretical embodiment construct, which matches the dossier's caution.

### Anchor check
- MD path: valid
- Line range: valid
- PDF page: valid for external sources; not applicable for internal notes

### Source role
supporting

### Required action
- keep as likely
- mark TODO:VERIFY or add a UX/preference source if the thesis makes a broader claim about desirability or practical system evaluation

## Entry 1.4.1 - Embodiment research shows congruence, synchrony, and avatar representation matter

### Verdict
verified

### Claim checked
Virtual embodiment research shows that multisensory congruence, visuomotor synchrony, and avatar representation influence virtual-body/action experience.

### Source checked
`kilteniEtAl2012senseEmbodiment`: raw page-marked markdown lines 338-377 and 397-411.

`kalckertEhrsson2012movingRubberHand`: raw page-marked markdown lines 262-292.

`gonzalezFrancoPeck2018avatarEmbodiment`: raw page-marked markdown lines 107-130.

### Evidence check
Kilteni supports visuomotor and visuotactile correlations in agency/ownership. Kalckert and Ehrsson support timing, movement-mode, and posture manipulations affecting agency/ownership. Gonzalez-Franco and Peck support avatar location/collocation and visual sensorimotor correlations as factors in embodiment illusions. If "avatar representation" is intended to include avatar appearance or user control, the Gonzalez-Franco and Peck anchor should extend beyond line 130; lines 148-181 cover agency/control, external appearance, and the summary that appearance and control enhance the embodiment illusion.

### Anchor check
- MD path: valid
- Line range: valid
- PDF page: valid

### Source role
best for embodiment/congruence; supporting for avatar-specific framing

### Required action
- keep as verified
- extend the `gonzalezFrancoPeck2018avatarEmbodiment` anchor through lines 148-181 if the dossier uses "avatar representation" to mean appearance or control, not only collocation/sensorimotor correlation

## Entry 1.4.2 - VR sport/exercise work has explored training, motivation, feedback, presence, and rowing

### Verdict
verified

### Claim checked
VR sport/exercise work has explored training, motivation, feedback, presence, and rowing-related systems.

### Source checked
`neumannEtAl2018interactiveVrSport`: raw page-marked markdown lines 73-88 and 304-337.

`murrayEtAl2016vrRowingPresence`: raw page-marked markdown lines 188-216.

`arndtEtAl2018vrRowingWorkouts`: raw page-marked markdown lines 175-190.

`rauterEtAl2013rowingTransfer`: raw page-marked markdown lines 28-43.

### Evidence check
Neumann supports interactive VR sport/exercise research and notes endurance sports including rowing. Murray supports VR rowing focused on performance, motivation, and enjoyment. Arndt supports an HMD indoor-rowing prototype focused on performance and experience. Rauter supports rowing simulator/skill-transfer work. The dossier's distinction that Rauter is not a consumer VR exercise example is correct.

### Anchor check
- MD path: valid
- Line range: valid
- PDF page: valid; Neumann 304-337 plausibly spans pages 9-10

### Source role
best for related-work examples

### Required action
- keep as verified

## Entry 1.4.3 - Existing rowing-related work has relevant ingredients but not necessarily this comparison

### Verdict
too broad

### Claim checked
Existing rowing-related VR/simulation work contains many relevant ingredients, but not necessarily this exact mapping comparison.

### Source checked
`murrayEtAl2016vrRowingPresence`: raw page-marked markdown lines 266-283.

`arndtEtAl2018vrRowingWorkouts`: raw page-marked markdown lines 175-190 and 219-253.

`rauterEtAl2013rowingTransfer`: raw page-marked markdown lines 305-320.

`neumannEtAl2018interactiveVrSport`: raw page-marked markdown lines 405-416.

### Evidence check
The cited sources support the "ingredients" part: projected VR rowing with avatar timing, HMD rowing with sensors and virtual lake/scull, a CAVE scull simulator with oars and sound/visual oar-water interaction, and an ergometer-as-virtual-boat example. They do not by themselves verify the absence of the exact mapping comparison. The chapter prose also mentions commercial/consumer-facing applications, which are not supported by these academic anchors.

### Anchor check
- MD path: valid
- Line range: valid
- PDF page: valid

### Source role
supporting

### Required action
- downgrade to likely
- mark TODO:CITE for commercial/consumer-facing application examples, or remove that suggestion from the dossier
- narrow the claim so the absence of the exact comparison is not treated as verified by adjacent examples alone

## Entry 1.4.4 - The exact head-to-head comparison appears missing

### Verdict
needs manual check

### Claim checked
The exact head-to-head comparison appears missing from the reviewed literature.

### Source checked
Internal: `literature/AGENT-thesis_literature_map_first_pitch.md`, lines 65-99 and 349-354.

Adjacent sources: `murrayEtAl2016vrRowingPresence`, `arndtEtAl2018vrRowingWorkouts`, and `rauterEtAl2013rowingTransfer` at the dossier's cited ranges.

### Evidence check
The internal literature map frames the comparison as underexplored and the adjacent sources show that related systems focused on VR/non-VR rowing, social/motivational effects, HMD feedback, and simulator transfer. This is not enough to verify a literature-absence claim. A search log, inclusion criteria, or maintained evidence-review table is needed before treating the gap as checked.

### Anchor check
- MD path: valid
- Line range: valid
- PDF page: valid for external sources; missing for internal literature map

### Source role
weak for absence claim

### Required action
- keep as needs manual check
- mark TODO:VERIFY until a formal search/audit note supports the absence claim

## Entry 1.4.5 - Mapping choice may influence embodiment, realism, and preference

### Verdict
likely

### Claim checked
Mapping choice may influence agency, ownership, self-location, realism, and preference.

### Source checked
`kilteniEtAl2012senseEmbodiment`: raw page-marked markdown lines 190-226 and 338-377.

`kalckertEhrsson2012movingRubberHand`: raw page-marked markdown lines 50-72 and 262-292.

`slater2009placePlausibility`: raw page-marked markdown lines 29-41.

`neumannEtAl2018interactiveVrSport`: raw page-marked markdown lines 73-88.

### Evidence check
The sources support the rationale for studying these outcomes: SoE components, agency/ownership effects of timing/movement/posture, plausibility/presence framing, and VR sport outcome factors. They do not directly show that the present rowing mapping choice influences all listed outcomes, especially realism and preference. The dossier's caution is appropriate.

### Anchor check
- MD path: valid
- Line range: valid
- PDF page: valid; Kilteni 338-377 plausibly spans pages 4-5

### Source role
supporting

### Required action
- keep as likely
- narrow the claim to rationale wording such as "may influence" or "motivates measuring"

## Entry 1.5.1 - The objective and research questions compare the two representation strategies

### Verdict
verified

### Claim checked
The thesis objective and research questions compare the two representation strategies.

### Source checked
Internal: `notes/global/thesis_spine.md`, lines 5-23; `notes/global/contribution_hierarchy.md`, lines 5-23; `notes/chapters/01_introduction_back_of_mind.md`, lines 21-29.

### Evidence check
The internal notes support the prototype, two-mode comparison, empirical focus, and exploratory framing. No external citation is needed for the thesis' own objective.

### Anchor check
- MD path: valid
- Line range: valid
- PDF page: not checked

### Source role
best for internal framing

### Required action
- keep as verified

## Entry 1.5.2 - The research questions are comparative and exploratory

### Verdict
verified

### Claim checked
The research questions are intentionally comparative and exploratory.

### Source checked
Internal: `notes/chapters/01_introduction_back_of_mind.md`, lines 21-29; `notes/global/thesis_spine.md`, lines 19-23.

### Evidence check
The back-of-mind file directly supports exploratory framing and warns against implying known results or superiority. The thesis-spine anchor is valid but incomplete for the "not universally superior" sentence, which appears at line 24 rather than within lines 19-23.

### Anchor check
- MD path: valid
- Line range: valid but incomplete for the thesis-spine "universally superior" support
- PDF page: not checked

### Source role
best for internal framing

### Required action
- keep as verified
- correct the thesis-spine anchor to lines 19-24 if this support is retained

## Entry 1.6.1 - The three contributions are prototype, comparison, and design implications

### Verdict
verified

### Claim checked
The three contributions are prototype, embodiment-oriented comparison, and design implications.

### Source checked
Internal: `notes/global/contribution_hierarchy.md`, lines 5-23; `notes/global/thesis_spine.md`, lines 7-23.

### Evidence check
The contribution hierarchy directly supports the developed XR rowing mechanism, prototype with two modes, user evaluation, interpretation/design implications, and academic positioning. No external citation is needed.

### Anchor check
- MD path: valid
- Line range: valid
- PDF page: not checked

### Source role
best for internal framing

### Required action
- keep as verified

## Entry 1.6.2 - The contribution is not a universal superiority claim

### Verdict
verified

### Claim checked
The contribution is not a universal claim that one representation is superior.

### Source checked
Internal: `notes/global/thesis_spine.md`, lines 19-23; `notes/chapters/01_introduction_back_of_mind.md`, lines 21-29.

### Evidence check
The back-of-mind file supports this restraint. The thesis-spine range cited in the dossier is incomplete: line 24 contains the direct statement that the thesis does not claim one representation is universally superior.

### Anchor check
- MD path: valid
- Line range: valid but incomplete for the thesis-spine universal-superiority sentence
- PDF page: not checked

### Source role
best for internal framing

### Required action
- keep as verified
- correct the thesis-spine anchor to lines 19-24 if this support is retained

## Entry 1.7.1 - Chapter previews describe the thesis layout

### Verdict
verified

### Claim checked
Chapter previews describe the thesis layout.

### Source checked
Internal: Chapter 1 structure files and the chapter preview in `chapters/01_introduction/07_thesis_structure.tex`; supporting internal notes `notes/global/thesis_spine.md`, lines 5-23 and `notes/global/contribution_hierarchy.md`, lines 5-23.

### Evidence check
This is navigational text, not a literature claim. It should track final chapter contents. The dossier is correct that no external citation is required.

### Anchor check
- MD path: valid
- Line range: valid
- PDF page: not checked

### Source role
background

### Required action
- keep as verified

## Entry M1 - Missing-source item: spatial sound

### Verdict
verified

### Claim checked
"Spatial sound" needs either a verified rowing simulator/VR audio source or removal from the broad list.

### Source checked
`rauterEtAl2013rowingTransfer`: raw page-marked markdown lines 305-320.

### Evidence check
Rauter supports a CAVE scull simulator with a sound wave field synthesis system used to render a realistic soundscape and visible/audible oar-water interaction. It does not support a generic claim that VR rowing systems add spatial sound.

### Anchor check
- MD path: valid
- Line range: valid
- PDF page: valid

### Source role
supporting

### Required action
- mark TODO:CITE for the generic "spatial sound" wording, or narrow it to the Rauter simulator example

## Entry M2 - Missing-source item: commercial/consumer-facing applications

### Verdict
needs manual check

### Claim checked
Commercial/consumer-facing applications such as Holofit/EXR illustrate representational choices.

### Source checked
No verified academic source anchor in the dossier supports this claim.

### Evidence check
The adjacent academic sources support prior VR rowing and simulation systems, but not Holofit/EXR-style commercial comparisons.

### Anchor check
- MD path: missing
- Line range: missing
- PDF page: missing

### Source role
weak

### Required action
- mark TODO:CITE
- remove citation suggestion unless a source is added or the text is clearly labeled as a non-academic market example

## Entry M3 - Missing-source item: no direct head-to-head mapping comparison

### Verdict
needs manual check

### Claim checked
The "no direct head-to-head mapping comparison found" gap needs evidence-review support.

### Source checked
Internal literature map and adjacent academic sources listed under Entry 1.4.4.

### Evidence check
The adjacent sources show related work but do not prove absence. The dossier's warning is correct.

### Anchor check
- MD path: valid for listed internal and adjacent sources
- Line range: valid
- PDF page: valid for external sources; missing for internal literature map

### Source role
weak for absence claim

### Required action
- keep as TODO:VERIFY

## Entry M4 - Missing-source item: preference and desirability

### Verdict
likely

### Claim checked
"Preference" and "desirable for the activity" are design-facing and plausible, but should not be made theoretical without a source.

### Source checked
Internal design framing plus `neumannEtAl2018interactiveVrSport` and `murrayEtAl2016vrRowingPresence` as checked under Entry 1.3.5.

### Evidence check
The sources support motivation, enjoyment, affect, performance, and broader VR sport outcome factors. They do not validate preference as an embodiment construct or support broad UX/desirability claims.

### Anchor check
- MD path: valid for already listed anchors
- Line range: valid
- PDF page: valid for external sources

### Source role
supporting

### Required action
- keep as TODO:VERIFY if the claim becomes broader than study-specific design rationale

## Entry M5 - Missing-source item: popularity, market growth, health effects, adoption

### Verdict
unsupported

### Claim checked
Future claims about indoor rowing popularity, market growth, health effects, or broad adoption need sources.

### Source checked
No source anchor is provided in the dossier for these future claims.

### Evidence check
No support checked. The dossier correctly warns not to add these claims without citation.

### Anchor check
- MD path: missing
- Line range: missing
- PDF page: missing

### Source role
wrong source

### Required action
- mark TODO:CITE for any such future claim

## Entry M6 - Missing-source item: boat-centric terminology

### Verdict
needs manual check

### Claim checked
If "boat-centric" remains the label, check terminology consistency against global notes.

### Source checked
Internal terminology/framing files: `notes/global/thesis_spine.md`, `notes/global/terminology.md`, and `notes/chapters/01_introduction_back_of_mind.md`.

### Evidence check
The global spine uses "boat-realistic representation"; terminology also uses "boat-centered mode" in the cyborg's dilemma entry. Chapter 1 currently uses "boat-centric representation." This is not a citation problem, but the dossier is right to flag consistency.

### Anchor check
- MD path: valid
- Line range: not checked for a single final terminology decision
- PDF page: not checked

### Source role
background

### Required action
- narrow the claim by standardizing the mode label before final citation cleanup

# Summary

## Keep
Entries safe as verified or already appropriately cautious: 1.1.2, 1.1.3 except spatial sound, 1.1.4, 1.1.5, 1.2.1, 1.2.2, 1.3.1, 1.3.2, 1.3.3 as likely, 1.3.4 as likely, 1.3.5 as likely, 1.4.1, 1.4.2, 1.4.5 as likely, 1.5.1, 1.5.2 with anchor correction, 1.6.1, 1.6.2 with anchor correction, 1.7.1.

## Downgrade
1.1.1 should not remain verified with the current anchors because "whole-body" is under-supported. 1.1.6 should be likely because the design-problem claim is thesis synthesis. 1.2.3 should be downgraded or narrowed because the cited embodiment/action sources do not by themselves establish the rowing-specific trade-off. 1.4.3 should be downgraded because the sources verify related ingredients, not the absence of the exact comparison.

## Replace
For 1.1.1, add or replace with `rauterEtAl2013rowingTransfer` for sequential legs/trunk/arms and whole-body rowing wording, or add the stronger Lamb abstract anchor. For 1.2.3, add `lamb1989kinematicComparison` and `rauterEtAl2013rowingTransfer` if the sentence claims the trade-off comes apart specifically in indoor rowing. For 1.4.1, extend the `gonzalezFrancoPeck2018avatarEmbodiment` anchor through lines 148-181 if "avatar representation" includes appearance or control.

## Remove or TODO
Keep TODO:CITE for generic "spatial sound" unless narrowed to Rauter. Keep TODO:CITE/TODO:VERIFY for commercial applications such as Holofit/EXR. Keep TODO:VERIFY for the absence of a direct head-to-head mapping comparison until a search table or evidence-review note exists. Keep TODO:VERIFY for broad preference/desirability claims. Keep TODO:CITE for any future popularity, market, health-effect, or adoption claims.

## Dossier quality rating
usable with fixes
