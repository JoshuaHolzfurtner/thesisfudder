# Core Design Tension Evidence Pack Verification

Status: second-pass verification of `notes/01_introduction/02_core_design_tension_evidence_pack.md` against raw page-marked markdown evidence. This file is a verification note only. It does not rewrite thesis prose, does not edit `.tex`, and does not add or remove citations.

Date: 2026-06-13

Target subsection: `chapters/01_introduction/02_core_design_tension.tex`

Evidence pack checked: `notes/01_introduction/02_core_design_tension_evidence_pack.md`

## Overall Verdict

The evidence pack is usable for handoff to ChatGPT / Pro as a source-grounding layer. I did not find a citation failure in the stable citation spine. The main sources support the premises the pack assigns to them:

- `lamb1989kinematicComparison`, `soperHume2004rowingTechnique`, and `rauterEtAl2013rowingTransfer` support the ergometer/on-water mismatch and rowing action-interface claims.
- `neumannEtAl2018interactiveVrSport` supports the VR sport/exertion-interface mapping claim, including the specific example of an ergometer being transformed into a virtual boat with handle pulls shown as virtual oar movement.
- `kilteniEtAl2012senseEmbodiment` supports the visuomotor congruence / agency rationale.
- `waltemateEtAl2016latency` supports temporal feedback / latency relevance in full-body avatar VR, but should remain optional unless the final paragraph explicitly mentions timing, responsiveness, or temporal congruence.
- `harrisEtAl2019visionForAction` supports the caution that visual realism in VR is not the same as action-relevant sensorimotor fidelity.
- `murrayEtAl2016vrRowingPresence` and `arndtEtAl2018vrRowingWorkouts` are valid concrete VR rowing examples, but they are optional for this subsection and should not carry the main conceptual trade-off.

The pack is strongest where it separates source-backed premises from thesis-authored inference. That distinction should be preserved in any prose patch.

## Verification Method

I re-read the target subsection, checked the bibliography keys in `references.bib`, reviewed the final SOURCE-CHECK blocks in the evidence pack, and re-opened the raw page-marked markdown evidence windows for the sources used in the pack.

I checked these files directly:

- `chapters/01_introduction/02_core_design_tension.tex`
- `notes/01_introduction/02_core_design_tension_evidence_pack.md`
- `references.bib`
- `MD Papers/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_markdown_bundle/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_raw_page_marked.md`
- `MD Papers/soper_hume_2004_ideal_rowing_technique_biomechanics_markdown_bundle/soper_hume_2004_ideal_rowing_technique_biomechanics_raw_page_marked.md`
- `MD Papers/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_markdown_bundle/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_raw_page_marked.md`
- `MD Papers/kilteni_2012_sense_of_embodiment_markdown_bundle/kilteni_2012_sense_of_embodiment_raw_page_marked.md`
- `MD Papers/waltemate_2016_latency_perceptual_judgments_motor_performance_vr_markdown_bundle/waltemate_2016_latency_perceptual_judgments_motor_performance_vr_raw_page_marked.md`
- `MD Papers/neumann_2018_interactive_virtual_reality_sport_systematic_review_markdown_bundle/neumann_2018_interactive_virtual_reality_sport_systematic_review_raw_page_marked.md`
- `MD Papers/harris_2019_virtually_the_same_vr_vision_for_action_markdown_bundle/harris_2019_virtually_the_same_vr_vision_for_action_raw_page_marked.md`
- `MD Papers/murray_2016_presence_of_others_vr_rowing_exercise_markdown_bundle/murray_2016_presence_of_others_vr_rowing_exercise_raw_page_marked.md`
- `MD Papers/arndt_2018_vr_hmd_rowing_workouts_markdown_bundle/arndt_2018_vr_hmd_rowing_workouts_raw_page_marked.md`

Bibliography keys rechecked in `references.bib`:

- `lamb1989kinematicComparison`
- `soperHume2004rowingTechnique`
- `rauterEtAl2013rowingTransfer`
- `harrisEtAl2019visionForAction`
- `kilteniEtAl2012senseEmbodiment`
- `waltemateEtAl2016latency`
- `neumannEtAl2018interactiveVrSport`
- `murrayEtAl2016vrRowingPresence`
- `arndtEtAl2018vrRowingWorkouts`

All listed keys exist in `references.bib`.

## Paragraph-Level Verification

### Paragraph 1: Ergometer and Boat as Different Movement Interfaces

Verification verdict: ready for prose patch, with one wording caution.

The pack's citation spine is correct: `lamb1989kinematicComparison`, `soperHume2004rowingTechnique`, and `rauterEtAl2013rowingTransfer`.

What rechecked cleanly:

- Lamb directly compares on-water and ergometer rowing and reports that upper arm and forearm kinematics differ between the two, especially around catch and finish, while many leg/trunk drive variables are similar.
- Soper and Hume support both the normal use of ergometers in rowing training/testing and the limitation that common ergometers do not reproduce all on-water trunk and upper-limb patterns well.
- Rauter et al. strongly support the rower/boat/oar/water interface: continuous haptic interaction, oar-water forces, oar handling, oar blades entering/leaving water, oarlocks, oar angles, and boat propulsion.

Important caution:

- "Constrained path" is reasonable thesis prose for the ergometer handle, but the strongest source wording is about the central pulley, cable/rod resistance, handle, and sliding seat rather than a precise geometrical path. If the final text says "straight" or "linear," that should be checked against prototype/device documentation, not only these literature sources.

Confidence: verified.

### Paragraph 2: Ergometer-Congruent Representation

Verification verdict: ready for prose patch if implementation wording is checked elsewhere.

The pack correctly treats "ergometer-congruent representation" as a thesis-defined mode, not a literature category.

What rechecked cleanly:

- Kilteni et al. support the conceptual relevance of visuomotor congruence to agency: agency is framed through the match between predicted and actual sensory consequences, including synchronous visuomotor correlations.
- Waltemate et al. support temporal-feedback relevance in VR full-body avatar contexts: visual feedback delay affected motor performance, simultaneity, agency, and ownership judgments. This is valid support for timing/responsiveness language, not for rowing-specific thresholds.
- Neumann et al. support the general VR sport premise that physical effort on an ergometer can be translated into virtual sport performance or movement through a virtual course.

Important caution:

- The exact claim that the avatar is animated around the "actual handle path and seat motion" is implementation-specific. It may be true for this thesis, but it should be checked against the prototype/implementation chapter or code notes before being treated as verified.
- Waltemate should not be cited if the paragraph only says "movement alignment" and does not mention timing, latency, responsiveness, simultaneity, or temporal congruence.

Confidence: verified for conceptual source support; needs manual check for final implementation-specific wording.

### Paragraph 3: Boat-Centric Representation

Verification verdict: ready for prose patch with terminology and overclaim cautions.

The pack correctly treats "boat-centric" / "boat-realistic" as a thesis-defined representation strategy.

What rechecked cleanly:

- Rauter et al. strongly support the sport-specific action structure of rowing: boat, oars, blades, water, oar handling, oarlocks, oar angles, and propulsion.
- Neumann et al. directly support the VR sport mapping example: a rowing ergometer can be transformed into a virtual boat so that pulls on the ergometer handle are depicted as movements of virtual oars through water.
- Lamb supports the mismatch premise: ergometer and on-water rowing are related but not identical, especially in upper-limb/oar-related mechanics.
- Harris supports the general caution that visual realism in VR does not guarantee action-relevant sensory or haptic equivalence.
- Murray and Arndt provide concrete examples of VR rowing systems with ergometers, avatars/lakes/sculls, sensor-derived motion, and virtual environments, but they are not needed for the main trade-off unless the prose explicitly wants prior-system examples.

Important cautions:

- "More recognizable as rowing" is a plausible design rationale, but not directly measured by these sources. Keep "can make" or "is designed to make"; do not write "does make" as an established result.
- Standardize the label before final thesis cleanup. The repo framing prefers `boat-realistic` / `boat-centered` more than `boat-centric`.
- Harris is not rowing-specific. Use it as a caution, not as proof of the rowing trade-off.

Confidence: verified for source-backed premises; likely for the "recognizable as rowing" design inference.

### Paragraph 4: Both Representations Are Artificial in Different Ways

Verification verdict: usable, but this paragraph has the most thesis-authored synthesis and should keep a developer/source-check note.

The pack correctly identifies this as a thesis synthesis paragraph rather than a direct literature claim.

What rechecked cleanly:

- Lamb supports the related-but-not-identical relation between ergometer and on-water rowing.
- Rauter et al. support the boat/oar/water action structure that is absent or reduced in ordinary ergometer rowing.
- Neumann et al. support the exertion-interface transformation premise: a real ergometer can be represented virtually as a boat/oar action.
- Harris supports the general VR-action caution: visual appearance and action-relevant sensorimotor fidelity can diverge in VR.

Important cautions:

- "Visual and cultural logic" is not directly sourced by the checked literature. The pack's suggested replacement, "recognizable visual and sport-specific logic," is safer unless a sport-culture source is added.
- "Straight ergometer handle movement" is stronger than the checked source language. The checked sources support "real ergometer handle movement," "central-pulley/handle movement," and "cable/rod" more directly. Use "real ergometer handle movement" unless the actual device implementation documents straight/linear path wording.
- "There is no neutral third option" is a thesis-authored inference. It is defensible from the source-backed premises, but it is not stated by the literature.

Confidence: verified for premises; needs manual check for exact wording if "straight" or "cultural logic" remains.

### Paragraph 5: Broader XR Sport Design Problem

Verification verdict: ready for prose patch with cautious generalization.

The source mix is appropriate if the paragraph frames a broader XR sport problem without claiming the thesis has surveyed all XR sport systems.

What rechecked cleanly:

- Neumann et al. support the broad VR sport frame: VR sport uses computer-simulated sport-relevant content and interactivity; physical effort on ergometers/treadmills can be mapped into virtual sport performance; cycling/running/rowing are relatively easy to translate because the exertion interface can monitor speed/cadence/performance data.
- Harris supports the caution that virtual visual action can diverge from real-world action because of altered sensory and haptic information.
- Kilteni supports why this matters for embodiment/agency when visible movement and performed movement are being compared.

Important cautions:

- Do not make this paragraph sound like a complete claim about "many XR sport and exercise systems" unless it stays broad and cites Neumann as the VR sport review context.
- Do not imply that Neumann studied the exact ergometer-congruent vs boat-realistic comparison.

Confidence: verified.

### Paragraph 6: Visuomotor Congruence Versus Realistic Sport Depiction

Verification verdict: ready for prose patch; this is the clearest conceptual landing paragraph if the source mix stays balanced.

The pack correctly says not to cite only embodiment sources for the rowing-specific "come apart" claim. The final paragraph needs both embodiment/action sources and rowing mechanics sources.

What rechecked cleanly:

- Kilteni supports the visuomotor-congruence / agency side.
- Waltemate supports timing/latency/feedback relevance if temporal congruence remains explicit.
- Harris supports the distinction between visual realism and action-relevant fidelity in VR.
- Lamb and Rauter make the trade-off rowing-specific by grounding the difference between ergometer mechanics and boat/oar/water action.
- Neumann supports the general VR sport transformation of ergometer action into virtual boat/oar action.

Important cautions:

- Do not claim Kilteni, Waltemate, or Harris studied rowing.
- Do not use Waltemate's latency thresholds as design requirements for this prototype.
- Do not turn "realistic sport depiction" into a validated construct unless later operationalized in the study/questionnaire.

Confidence: verified.

## Source-by-Source Anchor Audit

### `lamb1989kinematicComparison`

Role in evidence pack: best source for the nuanced claim that ergometer and on-water rowing are related but not identical.

Checked anchors:

- MD: `MD Papers/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_markdown_bundle/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_raw_page_marked.md`, lines 20-63; PDF page 1
- MD: same file, lines 86-98; PDF page 1
- MD: same file, lines 381-407; PDF page 6
- MD: same file, lines 419-500; PDF pages 6-7

Evidence confirmed:

- The paper explicitly compares on-water and ergometer rowing.
- It reports significant differences in upper arm and forearm kinematics between ergometer and on-water rowing.
- It attributes finish differences to oar lifting/feathering mechanics that are part of on-water rowing but not present in the same way on an ergometer.
- It also preserves nuance: leg and trunk variables are broadly similar through much of the drive phase, and the ergometer can still be a valid simulator for some biomechanical testing purposes.

Best use:

- Ergometer and boat are related but not identical movement contexts.
- Upper-limb/oar-related mechanics differ at catch/finish.
- Avoid saying the ergometer is a poor or invalid training tool.

Confidence: verified.

### `soperHume2004rowingTechnique`

Role in evidence pack: supporting rowing biomechanics source for common ergometer use and ergometer limitations.

Checked anchors:

- MD: `MD Papers/soper_hume_2004_ideal_rowing_technique_biomechanics_markdown_bundle/soper_hume_2004_ideal_rowing_technique_biomechanics_raw_page_marked.md`, lines 79-85; PDF page 1
- MD: same file, lines 109-123; PDF page 2
- MD: same file, lines 475-504; PDF page 5
- MD: same file, lines 1072-1087; PDF pages 11-12

Evidence confirmed:

- Rowing ergometers are commonly used for performance testing, technique coaching, crew selection, and poor-weather training.
- Ergometers can physiologically simulate a 2000 m race and reproduce parts of the biomechanical stroke pattern, mostly for the lower limbs.
- Common ergometers do not reproduce trunk and upper-limb patterns especially well compared with on-water rowing/sculling, partly because of the central pulley system.
- The Concept2 and other air-braked ergometers are discussed as common equipment, with freely moving seat wording in the surrounding passage.

Important caution:

- Lines 1072-1087 are OCR-messy and sentence order is not clean. They are not necessary for the final SOURCE-CHECK. Prefer lines 79-85 and 109-123 for the core claim.

Best use:

- Establish ergometer legitimacy plus limitation.
- Support "common training/testing device" and "central-pulley limitation" wording.

Confidence: verified for core anchors; likely / use cautiously for the OCR-messy extended range 1072-1087.

### `rauterEtAl2013rowingTransfer`

Role in evidence pack: best source for rowing as rower/boat/oar/water interaction and for why ordinary ergometers omit oar-handling realism.

Checked anchors:

- MD: `MD Papers/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_markdown_bundle/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_raw_page_marked.md`, lines 149-199; PDF page 2
- MD: same file, lines 283-320; PDF page 3
- MD: same file, lines 397-407; PDF page 4
- MD: same file, lines 571-580; PDF page 6
- MD: same file, lines 785-798; PDF page 9

Evidence confirmed:

- Rowing involves continuous haptic interaction among rower, boat, oar, and water.
- A realistic rowing simulation requires visual, auditory, and haptic rendering of oar-water interactions.
- Ordinary indoor rowing ergometers render oar-water resistance through a cable-driven windmill, so the rower does not develop the same feeling for oar immersion height and cannot train oar handling in the same way.
- A rowing stroke includes catch, drive, release, and recovery; blades enter and leave the water; the rower performs a coordinated sequential movement of legs, trunk, and arms; oars propel the boat.
- Oars are fixed in oarlocks and reduced to rotational degrees of freedom in the simulator; oar forces and oar angles are measured.
- Oar-handling skills include catch slip, depth of blade immersion, and striking out before catch.

Best use:

- Boat/oar/water action structure.
- Ordinary ergometer limitation relative to oar handling and blade-water interaction.
- Sport-specific rationale for the boat-realistic mode.

Confidence: verified.

### `kilteniEtAl2012senseEmbodiment`

Role in evidence pack: best conceptual source for sense of embodiment components and agency/visuomotor congruence.

Checked anchors:

- MD: `MD Papers/kilteni_2012_sense_of_embodiment_markdown_bundle/kilteni_2012_sense_of_embodiment_raw_page_marked.md`, lines 190-226; PDF page 3
- MD: same file, lines 338-377; PDF pages 4-5
- MD: same file, lines 397-411; PDF page 5
- MD: same file, lines 436-444; PDF page 5
- MD: same file, lines 922-926; PDF page 11

Evidence confirmed:

- SoE toward a body is defined through processing properties of an artificial body as if they were properties of one's own biological body.
- Embodiment is associated with self-location, agency, and body ownership.
- Agency is linked to a comparison between predicted and actual sensory consequences and to synchronous visuomotor correlations under active movement.
- Discrepancies between visual feedback and actual movement can negatively affect agency.
- Temporal discrepancies between self-generated movement and visual feedback are relevant for agency.

Best use:

- Visuomotor congruence as conceptually relevant to agency and embodiment.
- Do not use as a rowing source.

Confidence: verified.

### `waltemateEtAl2016latency`

Role in evidence pack: optional support for temporal congruence/responsiveness in a full-body avatar VR context.

Checked anchors:

- MD: `MD Papers/waltemate_2016_latency_perceptual_judgments_motor_performance_vr_markdown_bundle/waltemate_2016_latency_perceptual_judgments_motor_performance_vr_raw_page_marked.md`, lines 37-60; PDF page 1
- MD: same file, lines 70-84; PDF page 1
- MD: same file, lines 221-229; PDF page 2
- MD: same file, lines 520-540; PDF page 5
- MD: same file, lines 796-821; PDF page 7
- MD: same file, lines 847-860; PDF page 7

Evidence confirmed:

- Latency between user movement and visual feedback is inevitable in VR.
- Delays were varied in a full-body avatar setup, and motor performance, agency, ownership, and simultaneity perception were measured.
- Increasing feedback delay reduced perceptual judgments and motor performance.
- Agency and ownership declined at higher delays but did not fully break down even at the highest tested delay.
- The authors stress that latency should be reported and considered in VR studies.

Best use:

- Temporal congruence, responsiveness, latency, and feedback-delay caution.
- Not necessary if the final 1.2 prose only discusses spatial/movement mapping without timing.

Confidence: verified.

### `neumannEtAl2018interactiveVrSport`

Role in evidence pack: best VR sport source for exertion interfaces and for the ergometer-as-virtual-boat mapping example.

Checked anchors:

- MD: `MD Papers/neumann_2018_interactive_virtual_reality_sport_systematic_review_markdown_bundle/neumann_2018_interactive_virtual_reality_sport_systematic_review_raw_page_marked.md`, lines 73-88; PDF page 3
- MD: same file, lines 105-123; PDF page 4
- MD: same file, lines 228-241; PDF page 7
- MD: same file, lines 304-337; PDF pages 9-10
- MD: same file, lines 404-419; PDF page 12
- MD: same file, lines 688-689; PDF page 19

Evidence confirmed:

- Interactive VR sport research includes performance, physiological, and psychological outcomes and is influenced by athlete, VR environment, task, and non-VR environment factors.
- VR sport involves sport-relevant computer-generated content and interactivity.
- Interaction can occur through an exertion interface; physical effort on a machine such as an ergometer can be related to movement through a virtual race course.
- VR environments or elements can move/change in response to the athlete.
- The paper explicitly gives the rowing example: an ergometer is an exertion interface transformed into a virtual boat, where handle pulls are depicted as virtual oar movements through water and greater exertion changes virtual movement through water/scenery.

Best use:

- VR sport context.
- Stationary equipment / exertion-interface translation.
- The exact virtual-boat/oar mapping premise.

Confidence: verified.

### `harrisEtAl2019visionForAction`

Role in evidence pack: best general caution source for visual realism versus action-relevant fidelity in VR.

Checked anchors:

- MD: `MD Papers/harris_2019_virtually_the_same_vr_vision_for_action_markdown_bundle/harris_2019_virtually_the_same_vr_vision_for_action_raw_page_marked.md`, lines 34-45; PDF page 1
- MD: same file, lines 70-78; PDF page 2
- MD: same file, lines 202-229; PDF page 3
- MD: same file, lines 251-286; PDF page 3
- MD: same file, lines 378-393; PDF page 4

Evidence confirmed:

- VR alters or conflicts depth cues and often lacks realistic haptic information.
- These sensory differences may affect motor skills and action control.
- Movements in VR can be effectively pantomimed where endpoint feedback is absent.
- Skills performed in VR may not be representative of real-world counterparts under altered perceptual inputs.
- More complex actions may diverge from real skills even if performed adequately in VR.

Best use:

- Caution that visual realism does not guarantee real-world action fidelity.
- Do not use as direct rowing evidence.

Confidence: verified.

### `murrayEtAl2016vrRowingPresence`

Role in evidence pack: optional concrete VR rowing example.

Checked anchors:

- MD: `MD Papers/murray_2016_presence_of_others_vr_rowing_exercise_markdown_bundle/murray_2016_presence_of_others_vr_rowing_exercise_raw_page_marked.md`, lines 42-55; PDF page 1
- MD: same file, lines 76-99; PDF page 1
- MD: same file, lines 188-216; PDF page 2
- MD: same file, lines 266-286; PDF page 3

Evidence confirmed:

- Participants rowed on a Concept2 ergometer in individual or companion VR conditions.
- The paper describes traditional exercise tasks, including ergometer rowing, where physical exertion on exercise equipment lets a user move through a virtual environment.
- The setup used a projected VR environment, a third-person avatar view, and a rowing course with river scenery; the timing of the avatar's rowing strokes matched the ergometer.
- The study focused on performance, motivation, affective response, and social/companion context.

Best use:

- Prior VR rowing example.
- Avatar timing / virtual river context.
- Better suited to Motivation or related-work context than to the core design-tension citation burden.

Confidence: verified.

### `arndtEtAl2018vrRowingWorkouts`

Role in evidence pack: optional concrete HMD rowing example.

Checked anchors:

- MD: `MD Papers/arndt_2018_vr_hmd_rowing_workouts_markdown_bundle/arndt_2018_vr_hmd_rowing_workouts_raw_page_marked.md`, lines 47-57; PDF page 1
- MD: same file, lines 175-190; PDF page 2
- MD: same file, lines 219-253; PDF page 2

Evidence confirmed:

- The paper describes an athlete rowing on a stationary rowing machine in a virtual environment.
- Movement data from sensors on the rowing machine are displayed in an HMD.
- The machine captures sledge and handlebar movement and performance/technique metrics.
- The virtual environment includes a lake and scull; movement on the lake depends on force applied to the oars.

Important caution:

- The paper says "very realistic haptic feedback" because real ergometer handles are used. That should not be generalized into a claim that the system fully reproduces on-water rowing haptics.

Best use:

- Concrete HMD indoor rowing example.
- Optional for this subsection.

Confidence: verified.

## Issues or Corrections Needed

### Mandatory corrections

None found. I did not find a source that was assigned to a claim it clearly cannot support, as long as the pack's own synthesis cautions remain visible.

### Recommended tightening before prose patch

1. Prefer `boat-realistic` or `boat-centered` consistently if that is the repo's final terminology. `Boat-centric` is understandable, but the repo framing appears to lean toward `boat-realistic`.
2. Replace or qualify `visual and cultural logic` unless a separate sport-culture source is introduced. Safer wording: `recognizable visual and sport-specific logic of rowing`.
3. Replace `straight ergometer handle movement` with `real ergometer handle movement` unless the implementation/device documentation is used as the source for straight/linear handle path.
4. Keep `Waltemate` only where the final prose explicitly mentions temporal congruence, timing, latency, responsiveness, or simultaneity.
5. Keep `Murray` and `Arndt` out of the main 1.2 citation group unless the paragraph explicitly wants concrete prior VR rowing examples. They are real and relevant, but optional here.
6. Treat `there is no neutral third option` as thesis synthesis, not as a sourced external claim.

## Ready Handoff Summary

For ChatGPT / Pro, the evidence pack can be used as written, but the prose rewrite should preserve the source/synthesis boundary:

- Source-backed: ergometer and on-water rowing differ mechanically; on-water rowing involves boat/oar/water interactions; ordinary ergometers simplify or replace oar-water interaction; VR sport systems can map exertion interfaces into virtual sport environments; visuomotor congruence matters for agency; VR visual realism can diverge from action fidelity.
- Thesis-authored: the two mode labels, the exact design trade-off for this prototype, the no-neutral-option framing, and the idea that one mode prioritizes congruence while the other prioritizes recognizable sport depiction.
- Still human-check: implementation-specific wording around handle path, seat motion, tracking, and actual prototype mappings.

Final verification verdict: ready for handoff, with the tightening points above kept visible.
