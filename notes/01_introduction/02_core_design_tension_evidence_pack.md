# Core Design Tension Evidence Pack

Status: deep source-grounding pack for `chapters/01_introduction/02_core_design_tension.tex`. This file audits the current Core Design Tension subsection paragraph by paragraph. It does not rewrite thesis prose, does not edit `.tex`, and does not add or remove citations. It is a working evidence layer for the author, ChatGPT, and future LLM passes.

Important scope note: this pack audits the split subsection file named in the prompt. Check later whether the split files or the merged `chapters/01_introduction.tex` file are the active compiled source before applying any prose or citation patch.

## Files Read

Instruction and framing files:

- `AGENTS.md`
- `notes/chapters/01_introduction_back_of_mind.md`
- `notes/01_introduction/02_problem_statement_outline.md`
- `notes/01_introduction/dossier_section_1.md`
- `notes/01_introduction/dossier_section_1_verification.md`
- `notes/global/thesis_spine.md`
- `notes/global/terminology.md`
- `notes/global/contribution_hierarchy.md`
- `references.bib`

Target file:

- `chapters/01_introduction/02_core_design_tension.tex`

Relevant paper bundles consulted:

- `MD Papers/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_markdown_bundle/`
- `MD Papers/soper_hume_2004_ideal_rowing_technique_biomechanics_markdown_bundle/`
- `MD Papers/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_markdown_bundle/`
- `MD Papers/harris_2019_virtually_the_same_vr_vision_for_action_markdown_bundle/`
- `MD Papers/kilteni_2012_sense_of_embodiment_markdown_bundle/`
- `MD Papers/waltemate_2016_latency_perceptual_judgments_motor_performance_vr_markdown_bundle/`
- `MD Papers/neumann_2018_interactive_virtual_reality_sport_systematic_review_markdown_bundle/`

Relevant additional VR rowing bundles considered but not made central here:

- `MD Papers/murray_2016_presence_of_others_vr_rowing_exercise_markdown_bundle/`
- `MD Papers/arndt_2018_vr_hmd_rowing_workouts_markdown_bundle/`

Rationale: Murray and Arndt are concrete VR rowing examples, but this subsection is primarily about the representation trade-off. They can remain in the Motivation or broader related-work/appendix layer unless the paragraph explicitly needs concrete VR rowing examples.

## Bibliography Key Check

All keys below exist in `references.bib`:

- `lamb1989kinematicComparison`
- `soperHume2004rowingTechnique`
- `rauterEtAl2013rowingTransfer`
- `harrisEtAl2019visionForAction`
- `kilteniEtAl2012senseEmbodiment`
- `waltemateEtAl2016latency`
- `neumannEtAl2018interactiveVrSport`
- `murrayEtAl2016vrRowingPresence`
- `arndtEtAl2018vrRowingWorkouts`

## Working Citation Labels

This evidence pack follows the AGENTS.md confidence labels:

- `verified`: source file, evidence passage, line range, and page anchor were checked.
- `likely`: source appears relevant, but the exact claim relation or wording still needs human review.
- `needs manual check`: the claim or source relationship needs manual verification before being treated as source-backed.
- `unsupported`: no adequate source support was found in the checked material.

Evidence type labels used here:

- `direct evidence`: the source directly states or demonstrates the relevant premise.
- `contextual support`: the source gives useful background context but does not prove the exact sentence.
- `methodological analogy`: the source is useful because its setup or measurement logic resembles the thesis context.
- `thesis-synthesis premise`: the source supports one premise in an inference authored by the thesis.
- `background only`: the source is useful context but should not carry the citation burden for this paragraph.

Core caution for this subsection: the two representation modes are thesis-defined categories. The literature supports the underlying premises: ergometer/on-water mismatch, rower-boat-oar-water action structure, VR sport action mapping, and embodiment relevance of visuomotor congruence. The checked literature does not name or validate the exact pair "ergometer-congruent" versus "boat-centric/boat-realistic" as established external categories.

# Paragraph 1: Ergometer and Boat as Different Movement Interfaces

## Paragraph 1: Ergometer and Boat as Different Movement Interfaces

### Current paragraph text

A rowing ergometer and a rowing boat do not provide the same movement interface. On an ergometer, the user sits on a sliding seat and pulls a handle along a constrained path. In a rowing boat, the rower interacts with oars that rotate around oarlocks, blades that interact with water, and a boat that moves relative to the environment. Even when the training movement is related, the physical apparatus and spatial logic are different.

### Paragraph function

This paragraph establishes the mechanical and spatial basis of the design tension. It needs to make the reader accept that an ergometer and a rowing boat are not interchangeable movement interfaces, even though ergometer rowing is related to on-water rowing. This paragraph should not yet argue about embodiment outcomes. Its function is narrower:

- define the physical mismatch between the real apparatus and the sport action being represented;
- establish why the later virtual representation choice is not just aesthetic;
- keep the relation nuanced: ergometer rowing is related to rowing training, but the apparatus and oar-water interface differ.

### Claim ledger

#### Claim CDT-P1-C1

- Exact claim: "A rowing ergometer and a rowing boat do not provide the same movement interface."
- Claim classification: directly source-backed.
- Source support needed: direct comparison of ergometer and on-water rowing mechanics; rowing simulator source describing ordinary ergometer limitations relative to oar-water interaction.
- Current support status: verified.
- Best support: `lamb1989kinematicComparison`; `soperHume2004rowingTechnique`; `rauterEtAl2013rowingTransfer`.
- Wording should be narrowed: no. This is the cleanest, source-backed opening for the subsection.

#### Claim CDT-P1-C2

- Exact claim: "On an ergometer, the user sits on a sliding seat and pulls a handle along a constrained path."
- Claim classification: directly source-backed for sliding seat/handle and central-pulley/ergometer apparatus; thesis/system wording for "constrained path."
- Source support needed: source describing ergometer seat/handle or central-pulley mechanics.
- Current support status: verified for seat/handle and central-pulley; likely for the exact phrase "constrained path."
- Best support: `soperHume2004rowingTechnique`; `lamb1989kinematicComparison`; internal apparatus knowledge.
- Wording should be narrowed: maybe. "Constrained path" is safer than "straight path" or "linear path," but the source support is stronger for "sliding seat and handle/central pulley" than for a precise path geometry.

#### Claim CDT-P1-C3

- Exact claim: "In a rowing boat, the rower interacts with oars that rotate around oarlocks, blades that interact with water, and a boat that moves relative to the environment."
- Claim classification: directly source-backed for rower-boat-oar-water interaction, oar angles, oarlocks, blades/water, and boat propulsion; thesis synthesis for "moves relative to the environment."
- Source support needed: rowing simulator/biomechanics source describing oar-water interaction, oarlocks/oar angles, blades entering/pulling through water, and boat propulsion.
- Current support status: verified.
- Best support: `rauterEtAl2013rowingTransfer`; supporting `lamb1989kinematicComparison` and `soperHume2004rowingTechnique`.
- Wording should be narrowed: no major narrowing needed. The oarlock phrase has direct Rauter support through oarlocks/oar angles, but do not over-develop detailed rowing mechanics here.

#### Claim CDT-P1-C4

- Exact claim: "Even when the training movement is related, the physical apparatus and spatial logic are different."
- Claim classification: thesis synthesis from directly source-backed premises.
- Source support needed: evidence that ergometer and on-water rowing have similarities but also meaningful differences.
- Current support status: verified.
- Best support: `lamb1989kinematicComparison`; `soperHume2004rowingTechnique`; `rauterEtAl2013rowingTransfer`.
- Wording should be narrowed: maybe. "Spatial logic" is a thesis phrase; it is acceptable in prose, but source evidence is stronger for mechanical/interface differences than for that exact term.

### Source cards

#### Source: `lamb1989kinematicComparison`

- Citation key: `lamb1989kinematicComparison`
- Source role: best.
- What the source is about, in plain language: a kinematic comparison of ergometer rowing and on-water rowing.
- What the source specifically says that matters here: Lamb reports that many drive-phase variables are similar, especially for legs and trunk, but upper arm and forearm kinematics differ between ergometer and on-water rowing. The differences are especially tied to the catch/finish and to on-water oar mechanics such as lifting or feathering the oar, which are not exhibited in ergometer rowing.
- Which exact part of the paragraph it supports: the opening claim that ergometer and boat do not provide the same movement interface; the final claim that the training movement is related but the apparatus/action logic differs.
- Why this source is used here instead of a broader/background source: it directly compares the two physical rowing forms and therefore supports the exact contrast in the paragraph.
- What this source does NOT support: it does not support VR embodiment, agency, ownership, or user preference. It also does not name the thesis' two representation modes.
- Evidence type: direct evidence for related-but-different mechanics; thesis-synthesis premise for the design tension.
- Confidence: verified.
- MD path: `MD Papers/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_markdown_bundle/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_raw_page_marked.md`
- MD line range: lines 20-63; lines 86-98; lines 381-407; lines 419-500
- PDF page if available: p. 1; p. 6; p. 7.

#### Source: `soperHume2004rowingTechnique`

- Citation key: `soperHume2004rowingTechnique`
- Source role: supporting.
- What the source is about, in plain language: a review of rowing technique and biomechanics, including ergometer use and limitations.
- What the source specifically says that matters here: rowing ergometers are common in rowing training/testing, and common ergometers such as Concept2 can reproduce parts of the body action while not reproducing trunk and upper-limb patterns particularly well compared with on-water rowing because of the central pulley system.
- Which exact part of the paragraph it supports: the ergometer apparatus side of the contrast, especially central-pulley/handle mechanics and the fact that ergometer action only partly reproduces on-water movement.
- Why this source is used here instead of only Lamb: it validates ergometer use and gives a biomechanics-review framing rather than one kinematic comparison alone.
- What this source does NOT support: it does not support the VR mapping decision directly; it should not be used to claim that ergometers are poor or invalid.
- Evidence type: direct evidence for ergometer use and limitations; thesis-synthesis premise.
- Confidence: verified.
- MD path: `MD Papers/soper_hume_2004_ideal_rowing_technique_biomechanics_markdown_bundle/soper_hume_2004_ideal_rowing_technique_biomechanics_raw_page_marked.md`
- MD line range: lines 79-85; lines 109-123; lines 475-504; lines 1072-1087
- PDF page if available: p. 1; p. 2; p. 5; pp. 11-12.

#### Source: `rauterEtAl2013rowingTransfer`

- Citation key: `rauterEtAl2013rowingTransfer`
- Source role: best.
- What the source is about, in plain language: a realistic scull rowing simulator and transfer study that emphasizes visual, auditory, and haptic oar-water interaction.
- What the source specifically says that matters here: rowing includes continuous haptic interaction among rower, boat, oar, and water. Ordinary ergometers render water resistance through cable-driven resistance and do not train oar handling or oar height in water. The paper also describes oar blades entering, moving through, and leaving water, sculling with two oars, oar angles, oarlocks, and virtual boat propulsion.
- Which exact part of the paragraph it supports: the boat-side action structure: oars, oarlocks, blades, water, boat movement, and the contrast with ordinary ergometer resistance.
- Why this source is used here instead of only Lamb/Soper: it is the strongest source for the rower-boat-oar-water interface and for explaining why oar/blade mechanics are not a decorative detail.
- What this source does NOT support: it does not prove that a visually boat-centric HMD rowing mode will improve embodiment; its simulator includes haptic robotics and is not equivalent to this thesis' prototype.
- Evidence type: direct evidence for rowing interface structure; thesis-synthesis premise.
- Confidence: verified.
- MD path: `MD Papers/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_markdown_bundle/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_raw_page_marked.md`
- MD line range: lines 149-199; lines 283-320; lines 397-407; lines 571-580; lines 785-798
- PDF page if available: p. 2; p. 3; p. 4; p. 6; p. 9.

### Evidence window

#### `lamb1989kinematicComparison`

Lamb is the cleanest source for the related-but-not-identical relation. The study directly compares ergometer and on-water rowing and reports that many drive-phase variables are similar, especially for legs and trunk, while upper arm and forearm kinematics differ. Lamb also describes the rowing stroke through catch, drive, finish, and recovery, where the oar is placed in water, moved through water, withdrawn, and prepared to reenter. The discussion links some differences to oar slippage and the nonstationary oar fulcrum in water, and to lifting/feathering the oar at the finish, which is not exhibited in ergometer rowing.

Representative excerpts:

- "upper arm and forearm segments were significantly different in the two types of rowing" (raw page-marked MD lines 44-52, PDF p. 1).
- "the subjects of this study exhibited similar kinematics between on-water and ergometer rowing" for legs/trunk, but the arm/oar-related variables differed (raw page-marked MD lines 428-496, PDF pp. 6-7).

This supports the paragraph's nuanced wording: the movement is related, but the interface is not the same.

#### `soperHume2004rowingTechnique`

Soper and Hume support both the legitimacy and limitation of the ergometer. The source states that ergometers are common in rowing training/testing contexts, but also notes that common ergometers reproduce only parts of rowing body action and do not reproduce trunk and upper-limb patterns particularly well compared with on-water rowing, partly because of the central pulley system. Later lines also discuss common ergometer designs and a freely moving seat.

Representative excerpts:

- Rowing ergometers are "commonly used for performance testing, technique coaching, crew selection and training" (raw page-marked MD lines 79-85, PDF p. 1).
- Common ergometers reproduce parts of body action but do not reproduce trunk and upper-limb patterns well, due to the central pulley system (raw page-marked MD lines 109-123, PDF p. 2).

This is strong support for saying "not the same movement interface" without devaluing the ergometer.

#### `rauterEtAl2013rowingTransfer`

Rauter et al. support the boat-side interface detail. The source explains that rowing is built around continuous haptic forces between rower, boat, oar, and water, and that high mean boat velocity depends on coordinated dynamic movement and oar-water interaction. It contrasts this with ordinary ergometers that use cable-driven resistance and do not train oar handling or oar height in water. It also describes the catch, drive, release, and recovery cycle in terms of oar blades entering and leaving water, pulling oars through water, and propelling the boat. The simulator instrumentation uses oar angles and oarlocks, which supports the oarlock/oar rotation language at the level needed for this Motivation paragraph.

Representative excerpts:

- "there are continuous haptic forces between the rower, the boat, the oar, and the water" (raw page-marked MD lines 149-165, PDF p. 2).
- Ordinary indoor ergometers do not train oar handling or oar height in water (raw page-marked MD lines 180-199, PDF p. 2).
- At the catch, oar blades enter the water; during the drive, the rower pulls oars through water and propels the boat (raw page-marked MD lines 283-302, PDF p. 3).

The source supports the paragraph's boat/oar/water interface claims. It should not be used as direct evidence for subjective embodiment outcomes in this thesis.

### Reasoning bridge

The source-backed premises are strong. Lamb establishes that ergometer and on-water rowing are similar in some body-motion respects but differ in upper-limb/oar-related mechanics. Soper and Hume establish that ergometers are common training/testing devices but do not fully reproduce on-water trunk and upper-limb patterns. Rauter et al. establish the richer boat/oar/water interface, including oar handling, blade-water interaction, oar angles, and boat propulsion.

The thesis-authored inference is that these differences can be summarized as different "movement interfaces" and different "spatial logic." Those terms are not quoted from the sources, but they are faithful to the source-backed premises. The paragraph should stay descriptive and should not yet claim that these mechanical differences cause a particular embodiment result.

Unsupported or only likely steps: "constrained path" is reasonable but should not be over-specified as a precise geometry unless the prose later cites implementation details or a source about the actual handle path. "Spatial logic" is a thesis phrase and should be understood as an explanatory summary, not as a technical term from the rowing literature.

### Overclaim boundaries

- Do not claim the ergometer is a poor training device.
- Do not claim ergometer rowing and on-water rowing are unrelated.
- Do not claim all ergometers have the same handle path or seat mechanics.
- Do not claim the rowing biomechanics sources studied VR embodiment.
- Do not claim Rauter's high-fidelity simulator is equivalent to the thesis prototype.
- Do not claim the movement-interface difference by itself predicts ownership, agency, or preference.

### Suggested citation placement

Place a citation group at the end of the paragraph, after "the physical apparatus and spatial logic are different." This lets one group support the entire descriptive contrast.

Suggested citation group:

```tex
\parencite{lamb1989kinematicComparison,soperHume2004rowingTechnique,rauterEtAl2013rowingTransfer}
```

This group is justified because each source has a distinct role:

- `lamb1989kinematicComparison`: direct ergometer/on-water comparison.
- `soperHume2004rowingTechnique`: ergometer use and central-pulley/body-action caveat.
- `rauterEtAl2013rowingTransfer`: rower-boat-oar-water interface and ordinary ergometer limitations.

Do not add embodiment sources to this paragraph. They belong later when visuomotor congruence and agency are introduced.

### Suggested developer note

```tex
\sourcechecknote{This paragraph grounds the design tension in rowing mechanics rather than in VR theory. Lamb directly compares ergometer and on-water rowing and supports the nuanced premise that the movements are related but not identical: leg and trunk patterns are broadly similar in many drive-phase variables, while upper arm and forearm patterns differ, especially around catch and finish where on-water rowing involves oar-water mechanics such as lifting and feathering that are absent from ergometer rowing. Soper and Hume support the status of the ergometer as a normal rowing training/testing device while also noting that common ergometers reproduce only parts of on-water body action and do not reproduce trunk and upper-limb patterns particularly well because of the central pulley system. Rauter et al. support the boat-side interface: rowing involves continuous rower-boat-oar-water interaction, ordinary ergometers replace this with cable-driven resistance, and realistic rowing includes oar handling, blade-water interaction, oar angles, and boat propulsion. The thesis inference is that these source-backed differences amount to different movement interfaces and spatial action logics. These sources do not support VR embodiment outcomes or any claim that the ergometer is invalid as training equipment.}
```

### Suggested SOURCE-CHECK comments

```tex
% SOURCE-CHECK:
%   key: lamb1989kinematicComparison
%   md: MD Papers/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_markdown_bundle/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_raw_page_marked.md, lines 20-63; lines 419-500
%   pdf: p. 1; pp. 6-7
%   evidence: Ergometer and on-water rowing share many drive-phase variables, especially legs and trunk, but upper arm and forearm patterns differ around catch/finish; on-water rowing includes oar lifting/feathering not exhibited in ergometer rowing.
%   confidence: verified
%   caution: Supports related-but-different mechanics, not VR embodiment or preference.
%
% SOURCE-CHECK:
%   key: soperHume2004rowingTechnique
%   md: MD Papers/soper_hume_2004_ideal_rowing_technique_biomechanics_markdown_bundle/soper_hume_2004_ideal_rowing_technique_biomechanics_raw_page_marked.md, lines 79-85; lines 109-123
%   pdf: p. 1; p. 2
%   evidence: Rowing ergometers are common training/testing tools; common ergometers reproduce parts of body action but do not reproduce trunk and upper-limb patterns particularly well compared with on-water rowing because of the central pulley system.
%   confidence: verified
%   caution: Supports ergometer use and limitation; do not use to claim ergometers are poor or invalid.
%
% SOURCE-CHECK:
%   key: rauterEtAl2013rowingTransfer
%   md: MD Papers/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_markdown_bundle/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_raw_page_marked.md, lines 149-199; lines 283-320; lines 397-407
%   pdf: p. 2; p. 3; p. 4
%   evidence: Rowing involves continuous rower-boat-oar-water interaction; ordinary ergometers use cable-driven resistance and do not train oar handling/oar height; rowing with oars involves blades entering/pulling through/leaving water and oar angles/oarlocks.
%   confidence: verified
%   caution: Strong for oar/boat/water interface, not direct evidence for this thesis' embodiment outcomes.
```

### Appendix / broader-review note

No appendix note needed for this paragraph. It should stay focused on the physical interface contrast. Broader rowing-simulator examples can be moved to related work or an appendix if later prose becomes survey-like.

### Paragraph verdict

Ready for prose patch, with minor caution.

The paragraph is sourceable. The only wording to watch is "constrained path" and "spatial logic"; both are acceptable as thesis prose, but the source-backed core is the apparatus/interface mismatch rather than a precise geometrical handle-path claim.

# Paragraph 2: Ergometer-Congruent Representation

## Paragraph 2: Ergometer-Congruent Representation

### Current paragraph text

A VR rowing system can respond to this difference in at least two plausible ways. In an ergometer-congruent representation, the virtual body, handle, and rowing apparatus are aligned primarily with the user's real machine and movement. The visible hands and handle can remain close to where the user feels them, and the avatar can be animated around the actual handle path and seat motion. This preserves the physical logic of the user's current interaction.

### Paragraph function

This paragraph introduces the first thesis-defined representation mode. It explains what "ergometer-congruent" means at the design level:

- the visual body/apparatus is organized around the real ergometer;
- the visible hands/handle are kept near felt/proprioceptive hand/handle locations;
- avatar movement follows actual handle and seat motion;
- the mode prioritizes the real action loop over a fully boat-like depiction.

This paragraph is not mainly a literature claim. It is a definition of the thesis' first mode. Sources should support why congruence between performed and seen movement matters, and why preserving the actual ergometer interface is meaningful, but no source should be cited as if it invented this exact mode label.

### Claim ledger

#### Claim CDT-P2-C1

- Exact claim: "A VR rowing system can respond to this difference in at least two plausible ways."
- Claim classification: thesis synthesis and rhetorical bridge.
- Source support needed: source-backed premises that there is a difference to respond to; VR sport source showing systems can map physical effort into virtual action.
- Current support status: verified as thesis synthesis.
- Best support: Paragraph 1 sources plus `neumannEtAl2018interactiveVrSport`.
- Wording should be narrowed: no.

#### Claim CDT-P2-C2

- Exact claim: "In an ergometer-congruent representation, the virtual body, handle, and rowing apparatus are aligned primarily with the user's real machine and movement."
- Claim classification: internal project framing.
- Source support needed: no external source defines this mode; sources can support why machine/movement congruence is relevant.
- Current support status: verified as thesis-defined mode.
- Best support: internal thesis framing; supporting `kilteniEtAl2012senseEmbodiment`; supporting `waltemateEtAl2016latency` if temporal responsiveness is emphasized.
- Wording should be narrowed: no, as long as it is presented as this thesis' design definition.

#### Claim CDT-P2-C3

- Exact claim: "The visible hands and handle can remain close to where the user feels them."
- Claim classification: thesis design description plus embodiment/theory-relevant premise.
- Source support needed: source showing agency/body ownership can be influenced by visuomotor and multisensory/proprioceptive correspondence; optionally source showing delayed/misaligned avatar feedback affects agency/ownership/performance.
- Current support status: likely.
- Best support: `kilteniEtAl2012senseEmbodiment`; optional `waltemateEtAl2016latency`.
- Wording should be narrowed: maybe. This is an implementation/design claim about what the mode can do. If the final text says the mode actually does this, confirm against Chapter 3 implementation details.

#### Claim CDT-P2-C4

- Exact claim: "The avatar can be animated around the actual handle path and seat motion."
- Claim classification: internal implementation framing.
- Source support needed: no literature support needed if this describes the prototype; if kept as general VR sport mapping, use VR sport/action mapping source.
- Current support status: needs manual check for final implementation accuracy; likely as a design-mode description.
- Best support: internal implementation docs once Chapter 3 is stable; contextual `neumannEtAl2018interactiveVrSport`.
- Wording should be narrowed: yes if implementation is not finalized. Use "can" rather than "does" unless verified in the prototype chapter.

#### Claim CDT-P2-C5

- Exact claim: "This preserves the physical logic of the user's current interaction."
- Claim classification: thesis synthesis.
- Source support needed: premises about actual ergometer action and visuomotor congruence; no external source states the exact phrase.
- Current support status: verified as thesis framing.
- Best support: `lamb1989kinematicComparison`; `soperHume2004rowingTechnique`; `kilteniEtAl2012senseEmbodiment`.
- Wording should be narrowed: no, but avoid making it a measured result before the study.

### Source cards

#### Source: internal thesis framing

- Citation key: not a bibliography key; internal project framing only.
- Source role: best.
- What the source is about, in plain language: the thesis' own definition of the two representation strategies.
- What the source specifically says that matters here: the ergometer-congruent mode prioritizes close spatial and temporal alignment between the user's real ergometer movement and the virtual avatar, mapping real handle and seat motion as directly as possible to the virtual body.
- Which exact part of the paragraph it supports: the term "ergometer-congruent representation" and its design definition.
- Why this source is used here instead of an external source: the checked literature does not name this exact mode.
- What this source does NOT support: it is not external thesis evidence and should not be cited in final bibliography.
- Evidence type: internal project framing.
- Confidence: verified.
- MD path: `AGENTS.md`; `notes/global/thesis_spine.md`; `notes/global/contribution_hierarchy.md`
- MD line range: AGENTS core framing; thesis spine lines 5-17; contribution hierarchy lines 5-14
- PDF page if available: not applicable.

#### Source: `kilteniEtAl2012senseEmbodiment`

- Citation key: `kilteniEtAl2012senseEmbodiment`
- Source role: supporting.
- What the source is about, in plain language: a conceptual framework for sense of embodiment in VR, including self-location, agency, and ownership.
- What the source specifically says that matters here: sense of agency is connected to predicted and actual sensory consequences and synchronous visuomotor correlations; discrepancies between visual feedback and actual movement negatively affect agency. The paper also discusses body ownership and visuomotor/visuotactile correlations.
- Which exact part of the paragraph it supports: why keeping seen hands/handle/avatar movement close to felt/performed movement is relevant to embodiment-related experience, especially agency.
- Why this source is used here instead of rowing biomechanics: rowing sources support the mechanical mismatch; Kilteni supports why visual-motor correspondence matters for embodiment constructs.
- What this source does NOT support: it does not define the ergometer-congruent mode, does not study rowing, and does not prove this prototype will produce higher agency.
- Evidence type: contextual support and thesis-synthesis premise.
- Confidence: verified.
- MD path: `MD Papers/kilteni_2012_sense_of_embodiment_markdown_bundle/kilteni_2012_sense_of_embodiment_raw_page_marked.md`
- MD line range: lines 338-377; lines 397-411; lines 922-926
- PDF page if available: pp. 4-5; p. 11.

#### Source: `waltemateEtAl2016latency`

- Citation key: `waltemateEtAl2016latency`
- Source role: supporting/optional.
- What the source is about, in plain language: an experiment on how latency in full-body avatar feedback affects perceptual judgments and motor performance in VR.
- What the source specifically says that matters here: delayed avatar feedback affects motor performance, perceived simultaneity, agency, and ownership. The paper systematically varied feedback delays between 45 and 350 ms in a virtual mirror/avatar setup.
- Which exact part of the paragraph it supports: if the paragraph or surrounding text emphasizes temporal congruence, responsiveness, or close action-feedback timing.
- Why this source is used here instead of Kilteni alone: Kilteni gives the conceptual agency/visuomotor basis; Waltemate gives VR full-body latency evidence.
- What this source does NOT support: it does not establish a latency threshold for the rowing prototype and should not be converted into a hard design requirement.
- Evidence type: methodological analogy and contextual support.
- Confidence: verified.
- MD path: `MD Papers/waltemate_2016_latency_perceptual_judgments_motor_performance_vr_markdown_bundle/waltemate_2016_latency_perceptual_judgments_motor_performance_vr_raw_page_marked.md`
- MD line range: lines 37-60; lines 70-84; lines 221-229; lines 520-540; lines 796-821
- PDF page if available: p. 1; p. 2; p. 5; p. 7.

#### Source: `neumannEtAl2018interactiveVrSport`

- Citation key: `neumannEtAl2018interactiveVrSport`
- Source role: background/supporting.
- What the source is about, in plain language: a systematic review of interactive VR sport.
- What the source specifically says that matters here: physical effort on an exertion interface can be translated into virtual sport performance, and rowing handle pulls can be depicted as movements of virtual oars.
- Which exact part of the paragraph it supports: the general premise that VR sport systems can map physical exercise-device movement into virtual action.
- Why this source is used here instead of only embodiment sources: it grounds the VR sport/action-mapping context.
- What this source does NOT support: it does not support embodiment theory and does not define the thesis' modes.
- Evidence type: contextual support.
- Confidence: verified.
- MD path: `MD Papers/neumann_2018_interactive_virtual_reality_sport_systematic_review_markdown_bundle/neumann_2018_interactive_virtual_reality_sport_systematic_review_raw_page_marked.md`
- MD line range: lines 105-123; lines 404-419
- PDF page if available: p. 4; p. 12.

### Evidence window

#### Internal thesis framing

The thesis framing defines the ergometer-congruent mode as the mode that prioritizes close spatial and temporal alignment between real ergometer movement and virtual avatar movement. The evidence pack should treat this as a design definition, not as an external literature category. The paragraph's specific language about virtual body, handle, apparatus, felt hand location, handle path, and seat motion belongs primarily to the prototype design.

#### `kilteniEtAl2012senseEmbodiment`

Kilteni et al. support the theoretical relevance of visual-motor correspondence. The agency section states that agency has been proposed to result from comparisons between predicted and actual sensory consequences and that synchronous visuomotor correlations under active movement contribute to feeling oneself as the agent. The same passage notes that discrepancies between visual feedback and actual movement negatively affect agency. This supports why an ergometer-congruent mapping may be relevant to agency and embodiment, without predicting a result.

Representative excerpt:

- "the presence of synchronous visuomotor correlations under active movement" is linked to agency, and discrepancies between visual feedback and actual movement negatively affect agency (raw page-marked MD lines 349-377, PDF pp. 4-5).

#### `waltemateEtAl2016latency`

Waltemate et al. provide a VR full-body avatar example where delayed visual feedback affects perception and motor performance. The abstract states that feedback delays were varied between 45 and 350 ms and that motor performance, agency, ownership, and simultaneity were measured. Results show motor performance and simultaneity affected at lower latencies than agency/ownership, and that increasing delay generally decreased perceptual judgments and performance. This is useful if the final paragraph discusses temporal congruence or responsiveness. It should remain optional in this paragraph unless timing/responsiveness is explicit.

Representative excerpt:

- "sense of agency, ownership, and perceived simultaneity decreased, and motor performance worsened, with increasing delay" (raw page-marked MD lines 520-540, PDF p. 5).

#### `neumannEtAl2018interactiveVrSport`

Neumann et al. support the broad VR sport mapping premise. Physical effort on an exercise machine can be related to speed of movement through a virtual race course, and physical actions can be translated into virtual sport performance. The rowing example later says ergometer handle pulls can be depicted as virtual oar movements. This supports the general idea that the VR system maps real machine movement into virtual action, but it is not specifically an ergometer-congruent mapping source.

### Reasoning bridge

The source-backed premises are that visuomotor correspondence matters for agency and embodiment-related experience, and that VR sport systems can map physical exercise-device movement into virtual action. The thesis-authored inference is the definition of an "ergometer-congruent" response to the rowing mismatch: instead of forcing the virtual body into a fully boat-like oar action, the system can keep visible hands, handle, body, and apparatus close to the real interaction.

Unsupported or only likely steps are implementation-specific: "actual handle path and seat motion" should be checked against the current prototype implementation before the final prose claims that the mode does exactly this. As a design description, "can be animated" is safe.

### Overclaim boundaries

- Do not claim the literature names "ergometer-congruent representation" as a standard category.
- Do not claim the ergometer-congruent mode necessarily produces stronger agency or ownership before the study data.
- Do not claim Kilteni studied rowing or exercise equipment.
- Do not claim Waltemate's latency thresholds directly apply to the rowing prototype.
- Do not claim close hand/handle alignment is fully verified unless Chapter 3 implementation supports it.
- Do not treat "physical logic" as a measured construct unless it becomes an operationalized measure.

### Suggested citation placement

This paragraph is mostly a mode definition, so avoid citation stuffing. Good options:

- No citation immediately after the mode definition if the surrounding paragraph makes clear this is thesis terminology.
- If citing theory, place one citation after the sentence about visible hands/handle remaining close to where the user feels them:

```tex
\parencite{kilteniEtAl2012senseEmbodiment}
```

- Add `waltemateEtAl2016latency` only if the text explicitly says "temporal alignment," "responsiveness," "delay," or "latency."
- Add `neumannEtAl2018interactiveVrSport` only if the text needs broader VR sport mapping context; it may be better in Paragraph 5.

### Suggested developer note

```tex
\sourcechecknote{This paragraph defines the thesis' ergometer-congruent representation rather than importing a named mode from the literature. The mode is thesis-defined as a representation that keeps the virtual body, handle, apparatus, and avatar movement aligned primarily with the user's real ergometer interaction. Kilteni et al. support why this kind of mapping is theoretically relevant: agency is linked to comparisons between predicted and actual sensory consequences and to synchronous visuomotor correlations, while discrepancies between visual feedback and actual movement can reduce agency. Waltemate et al. can support temporal-congruence language if the final prose mentions responsiveness or delay, because their full-body avatar study shows that delayed feedback affects motor performance, simultaneity, agency, and ownership. Neumann et al. only provides broad VR sport context, showing that physical exertion interfaces can be translated into virtual sport action. None of these sources names this mode or proves it will improve embodiment in rowing; the implementation-specific claim that the avatar follows actual handle path and seat motion should be checked against the prototype chapter before final wording.}
```

### Suggested SOURCE-CHECK comments

```tex
% SOURCE-CHECK:
%   key: kilteniEtAl2012senseEmbodiment
%   md: MD Papers/kilteni_2012_sense_of_embodiment_markdown_bundle/kilteni_2012_sense_of_embodiment_raw_page_marked.md, lines 338-377
%   pdf: pp. 4-5
%   evidence: Agency is linked to predicted versus actual sensory consequences and synchronous visuomotor correlations; discrepancies between visual feedback and actual movement negatively affect agency.
%   confidence: verified
%   caution: Supports why congruent action-feedback mapping is relevant, not a prediction that the ergometer-congruent mode will score higher.
%
% SOURCE-CHECK:
%   key: waltemateEtAl2016latency
%   md: MD Papers/waltemate_2016_latency_perceptual_judgments_motor_performance_vr_markdown_bundle/waltemate_2016_latency_perceptual_judgments_motor_performance_vr_raw_page_marked.md, lines 37-60; lines 520-540
%   pdf: p. 1; p. 5
%   evidence: Full-body avatar feedback delays affected motor performance, perceived simultaneity, agency, and ownership; increasing delay generally worsened perceptual judgments and motor performance.
%   confidence: verified
%   caution: Use only for temporal congruence/responsiveness; do not import its latency thresholds as design requirements for rowing.
```

### Appendix / broader-review note

No appendix note needed. This paragraph should stay a compact thesis-mode definition, with only minimal theory support.

### Paragraph verdict

Ready for prose patch, with implementation check.

The paragraph is strong as a mode definition. Before final thesis use, verify that Chapter 3 actually describes handle and seat tracking in a way consistent with "actual handle path and seat motion."

# Paragraph 3: Boat-Centric Representation

## Paragraph 3: Boat-Centric Representation

### Current paragraph text

In a boat-centric representation, the system instead prioritizes the visual and sport-specific logic of rowing on water. The user may appear to sit in a boat, move through a river, and row with oars. This can make the virtual scene more recognizable as rowing, but it may require transforming the user's real handle movement into a virtual oar movement that does not fully coincide with the felt motion of the hands and handle.

### Paragraph function

This paragraph defines the second thesis mode. It explains that the boat-centric or boat-realistic representation gives priority to recognizable on-water rowing depiction: boat, river, oars, movement through environment, and sport-specific rowing imagery. It also introduces the cost of that choice: the system may have to transform real ergometer handle motion into virtual oar motion, producing a mismatch between felt movement and seen movement.

### Claim ledger

#### Claim CDT-P3-C1

- Exact claim: "In a boat-centric representation, the system instead prioritizes the visual and sport-specific logic of rowing on water."
- Claim classification: internal project framing.
- Source support needed: no source defines this exact mode; rowing and VR sport sources support the ingredients.
- Current support status: verified as thesis-defined mode.
- Best support: internal thesis framing; supporting `rauterEtAl2013rowingTransfer`; supporting `neumannEtAl2018interactiveVrSport`.
- Wording should be narrowed: maybe. "Boat-centric" should be standardized against "boat-realistic" or "boat-centered" terminology before final thesis cleanup.

#### Claim CDT-P3-C2

- Exact claim: "The user may appear to sit in a boat, move through a river, and row with oars."
- Claim classification: directly source-backed for VR rowing/VR sport possibilities; also internal prototype/design framing.
- Source support needed: VR rowing or VR sport sources showing boat/river/scenery/oar depiction; rowing sources explaining oars/boat/water action.
- Current support status: verified for general VR rowing/VR sport context; needs manual check for actual prototype if stated as implemented.
- Best support: `neumannEtAl2018interactiveVrSport`; optional concrete support from `murrayEtAl2016vrRowingPresence` and `arndtEtAl2018vrRowingWorkouts`; rowing-action support from `rauterEtAl2013rowingTransfer`.
- Wording should be narrowed: no if "may" remains. If changed to "does," verify against implementation.

#### Claim CDT-P3-C3

- Exact claim: "This can make the virtual scene more recognizable as rowing."
- Claim classification: thesis synthesis/design rationale.
- Source support needed: rowing sources showing boat/oar/water are core to rowing; VR sport sources showing virtual rowing depiction. No checked source directly measures "recognizable as rowing" for this mode.
- Current support status: likely.
- Best support: `rauterEtAl2013rowingTransfer`; `neumannEtAl2018interactiveVrSport`; optional `murrayEtAl2016vrRowingPresence` and `arndtEtAl2018vrRowingWorkouts`.
- Wording should be narrowed: maybe. Use "visually recognizable" or "designed to be more recognizable" rather than implying a measured perception unless study measures it.

#### Claim CDT-P3-C4

- Exact claim: "It may require transforming the user's real handle movement into a virtual oar movement that does not fully coincide with the felt motion of the hands and handle."
- Claim classification: thesis synthesis from source-backed rowing mismatch and VR sport mapping.
- Source support needed: source showing ergometer/on-water/oar mechanics differ; source showing VR sport can depict handle pulls as virtual oar movement; embodiment source if tying mismatch to agency later.
- Current support status: verified as thesis synthesis.
- Best support: `lamb1989kinematicComparison`; `rauterEtAl2013rowingTransfer`; `neumannEtAl2018interactiveVrSport`; supporting `harrisEtAl2019visionForAction` for visual depiction/action-fidelity caution.
- Wording should be narrowed: no; "may require" is appropriately cautious.

### Source cards

#### Source: internal thesis framing

- Citation key: not a bibliography key; internal project framing only.
- Source role: best.
- What the source is about, in plain language: the thesis' definition of a boat-realistic/boat-centered representation.
- What the source specifically says that matters here: the boat-realistic mode prioritizes sport-faithful depiction of rowing on water even when real ergometer handle motion and realistic oar motion diverge.
- Which exact part of the paragraph it supports: the boat-centric mode definition and the idea that visual/sport depiction can come at a congruence cost.
- Why this source is used here instead of an external source: the checked external literature does not name this exact mode.
- What this source does NOT support: external empirical evidence.
- Evidence type: internal project framing.
- Confidence: verified.
- MD path: `AGENTS.md`; `notes/global/thesis_spine.md`; `notes/global/terminology.md`
- MD line range: AGENTS core framing; thesis spine lines 5-17; terminology "Cyborg's Dilemma" entry.
- PDF page if available: not applicable.

#### Source: `rauterEtAl2013rowingTransfer`

- Citation key: `rauterEtAl2013rowingTransfer`
- Source role: best.
- What the source is about, in plain language: realistic scull-rowing simulator and transfer to on-water rowing.
- What the source specifically says that matters here: rowing involves rower-boat-oar-water interaction, oar blades entering/pulling through/leaving water, two-oar sculling, oar angles, oar rotation, oarlocks, and virtual boat propulsion in the simulator.
- Which exact part of the paragraph it supports: why boat/oar depiction is sport-specific and not merely decorative.
- Why this source is used here instead of a generic VR sport source: it explains what is rowing-specific about boat/oar/water representation.
- What this source does NOT support: it does not prove that a visual boat-centric HMD mode improves embodiment; its simulator includes haptic elements not present in an ordinary HMD ergometer system.
- Evidence type: direct evidence for rowing-specific action structure; thesis-synthesis premise.
- Confidence: verified.
- MD path: `MD Papers/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_markdown_bundle/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_raw_page_marked.md`
- MD line range: lines 149-199; lines 283-320; lines 397-407; lines 571-580; lines 785-798
- PDF page if available: p. 2; p. 3; p. 4; p. 6; p. 9.

#### Source: `neumannEtAl2018interactiveVrSport`

- Citation key: `neumannEtAl2018interactiveVrSport`
- Source role: best for VR sport mapping context.
- What the source is about, in plain language: systematic review of interactive VR sport.
- What the source specifically says that matters here: in a rowing example, an ergometer can be transformed into a virtual boat, handle pulls can be depicted as virtual oar movements through water, and greater exertion can produce faster movement through virtual water and scenery.
- Which exact part of the paragraph it supports: the possibility of making the user appear to row virtually with oars and moving through a rowing environment, and the idea that real handle movement can be transformed into virtual oar movement.
- Why this source is used here instead of only Rauter: it explicitly describes ergometer-to-virtual-boat/oar mapping in VR sport language.
- What this source does NOT support: it does not analyze the mismatch between felt handle motion and seen oar motion in the thesis' sense; it does not discuss embodiment outcomes.
- Evidence type: direct evidence for VR sport action mapping; thesis-synthesis premise.
- Confidence: verified.
- MD path: `MD Papers/neumann_2018_interactive_virtual_reality_sport_systematic_review_markdown_bundle/neumann_2018_interactive_virtual_reality_sport_systematic_review_raw_page_marked.md`
- MD line range: lines 105-123; lines 228-241; lines 404-419
- PDF page if available: p. 4; p. 7; p. 12.

#### Source: `lamb1989kinematicComparison`

- Citation key: `lamb1989kinematicComparison`
- Source role: supporting.
- What the source is about, in plain language: direct kinematic comparison of ergometer and on-water rowing.
- What the source specifically says that matters here: the upper arm and forearm kinematics differ between ergometer and on-water rowing, and on-water finish/catch actions involve oar handling not exhibited in ergometer rowing.
- Which exact part of the paragraph it supports: the claim that transforming handle movement into virtual oar movement may not fully coincide with felt hand/handle motion.
- Why this source is used here instead of only Neumann: Neumann gives the virtual mapping possibility; Lamb explains why the physical movement may not naturally match the on-water/oar action.
- What this source does NOT support: it does not support virtual scene recognizability or VR embodiment.
- Evidence type: thesis-synthesis premise.
- Confidence: verified.
- MD path: `MD Papers/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_markdown_bundle/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_raw_page_marked.md`
- MD line range: lines 20-63; lines 419-500
- PDF page if available: p. 1; pp. 6-7.

#### Source: `harrisEtAl2019visionForAction`

- Citation key: `harrisEtAl2019visionForAction`
- Source role: supporting/background.
- What the source is about, in plain language: a mini-review warning that visually realistic VR can still differ from real-world action because depth cues and haptic information are impaired or altered.
- What the source specifically says that matters here: VR can present visually convincing scenes while action-relevant sensory information, especially haptic feedback and depth cues, differs from the real world.
- Which exact part of the paragraph it supports: the caution that a visually sport-specific depiction does not automatically preserve felt action congruence.
- Why this source is used here instead of embodiment sources alone: it directly addresses visual realism versus action-relevant sensorimotor information.
- What this source does NOT support: it does not study rowing or the thesis' two modes; it should not be used to claim VR action is invalid.
- Evidence type: contextual support and caution source.
- Confidence: verified.
- MD path: `MD Papers/harris_2019_virtually_the_same_vr_vision_for_action_markdown_bundle/harris_2019_virtually_the_same_vr_vision_for_action_raw_page_marked.md`
- MD line range: lines 34-45; lines 202-229; lines 251-286; lines 378-393
- PDF page if available: p. 1; p. 3; p. 4.

#### Source: `murrayEtAl2016vrRowingPresence`

- Citation key: `murrayEtAl2016vrRowingPresence`
- Source role: optional.
- What the source is about, in plain language: VR rowing on a Concept2 ergometer with a virtual river, avatar, and companion condition.
- What the source specifically says that matters here: the virtual environment included a rowing avatar, river/scenery, and companion boat; avatar stroke timing matched the ergometer.
- Which exact part of the paragraph it supports: concrete evidence that VR rowing systems can depict river/boat/avatar rowing contexts.
- Why this source is optional here: the Motivation pack already uses it; the core design tension can remain lean with Neumann and rowing mechanics unless concrete examples are needed.
- What this source does NOT support: it does not study the thesis' two modes or a visual/felt oar mismatch.
- Evidence type: contextual support.
- Confidence: verified.
- MD path: `MD Papers/murray_2016_presence_of_others_vr_rowing_exercise_markdown_bundle/murray_2016_presence_of_others_vr_rowing_exercise_raw_page_marked.md`
- MD line range: lines 266-286
- PDF page if available: p. 3.

#### Source: `arndtEtAl2018vrRowingWorkouts`

- Citation key: `arndtEtAl2018vrRowingWorkouts`
- Source role: optional.
- What the source is about, in plain language: HMD indoor-rowing prototype with a virtual lake and scull driven by ergometer data.
- What the source specifically says that matters here: the system displays a virtual lake and scull while the user rows on a stationary machine, with movement depending on rowing force.
- Which exact part of the paragraph it supports: concrete boat/lake/scull VR rowing depiction.
- Why this source is optional here: useful example, but not necessary if the paragraph is defining the thesis mode rather than surveying prior systems.
- What this source does NOT support: the thesis' exact congruence-versus-sport-depiction comparison.
- Evidence type: contextual support.
- Confidence: verified.
- MD path: `MD Papers/arndt_2018_vr_hmd_rowing_workouts_markdown_bundle/arndt_2018_vr_hmd_rowing_workouts_raw_page_marked.md`
- MD line range: lines 47-57; lines 219-253
- PDF page if available: p. 1; p. 2.

### Evidence window

#### `rauterEtAl2013rowingTransfer`

Rauter et al. support why a boat/oar depiction is sport-specific. The source does not merely say rowing happens on water; it describes rowing as coordinated rower-boat-oar-water interaction, with oar blades entering and leaving water, pulling through water, and propelling the boat. The paper also details oar angles and oarlocks as meaningful simulator/measurement elements. This makes virtual oars and boat context plausible as sport-specific rowing representation rather than arbitrary visuals.

Representative excerpts:

- Rowing involves continuous haptic forces among rower, boat, oar, and water (raw page-marked MD lines 149-165, PDF p. 2).
- At catch and drive, blades move into water and the rower pulls oars through water to propel the boat (raw page-marked MD lines 283-302, PDF p. 3).

#### `neumannEtAl2018interactiveVrSport`

Neumann et al. provide the closest source for the idea that an ergometer can be visually transformed into a virtual boat/oar action. The review explicitly states that a rowing ergometer can function as the exertion interface and be transformed into a virtual boat, with ergometer handle pulls depicted as virtual oar movements through water and higher exertion producing faster virtual movement.

Representative excerpt:

- The ergometer is "transformed into a virtual boat" such that handle pulls are depicted as virtual oar movements and higher exertion changes virtual movement through water/scenery (raw page-marked MD lines 405-409, PDF p. 12).

#### `lamb1989kinematicComparison`

Lamb supports the mismatch side. If on-water rowing includes oar-related arm mechanics that differ from ergometer mechanics, then a virtual oar depiction may need to transform what the user actually does with the ergometer handle. This is the mechanical basis for the paragraph's "does not fully coincide with felt motion" claim.

#### `harrisEtAl2019visionForAction`

Harris et al. are not rowing-specific, but they are useful as a caution against treating visual realism as action equivalence. The abstract states that depth cues can be impaired or in conflict in VR and that realistic haptic information is largely absent from current VR systems; these conflicts may affect motor skills. The later conclusion warns that complex actions in VR may diverge from real-world actions. This supports the paragraph's careful distinction between recognizable rowing scene and congruent felt movement.

Representative excerpt:

- "realistic haptic information is all but absent from current VR systems" and conflicts may affect motor skills (raw page-marked MD lines 34-45, PDF p. 1).

#### `murrayEtAl2016vrRowingPresence` and `arndtEtAl2018vrRowingWorkouts`

These are useful concrete examples if the paragraph needs them. Murray supports virtual river/avatar/companion rowing with an ergometer. Arndt supports HMD virtual lake/scull rowing with sensor-derived movement. They are not necessary for the core trade-off unless the prose needs concrete prior-system examples.

### Reasoning bridge

The source-backed premises are that rowing on water involves boat/oar/blade/water mechanics, that VR sport can depict an ergometer as a virtual boat/oar action, and that ergometer/on-water movements are related but not identical. The thesis-authored inference is the boat-centric mode: prioritize the recognizable sport depiction, while accepting that the virtual oar motion may not coincide perfectly with the user's felt handle motion.

Unsupported or only likely steps: "more recognizable as rowing" is a reasonable design rationale, but it is not directly measured by the cited sources. It should remain "can make" or "is designed to make," not "does make" unless supported by data. "Boat-centric" should be standardized with "boat-realistic" or "boat-centered."

### Overclaim boundaries

- Do not claim the literature names "boat-centric representation" as a standard category.
- Do not claim the boat-centric mode necessarily reduces agency or ownership.
- Do not claim visual sport depiction equals embodiment.
- Do not claim Neumann studied the mismatch between felt ergometer handle motion and virtual oar motion.
- Do not claim Rauter's haptic simulator is equivalent to this thesis' visual/IK boat mode.
- Do not claim recognizability or realism was measured unless the study includes such measures.

### Suggested citation placement

For the boat/oar/rowing-specific premise, cite:

```tex
\parencite{rauterEtAl2013rowingTransfer}
```

For the ergometer-to-virtual-oar mapping and broader VR sport context, cite:

```tex
\parencite{neumannEtAl2018interactiveVrSport}
```

For the mismatch between actual ergometer movement and oar/on-water movement, cite:

```tex
\parencite{lamb1989kinematicComparison}
```

If the paragraph stays compact, a combined group is acceptable:

```tex
\parencite{lamb1989kinematicComparison,rauterEtAl2013rowingTransfer,neumannEtAl2018interactiveVrSport}
```

Use `harrisEtAl2019visionForAction` only if the paragraph explicitly contrasts visual realism with action-relevant sensorimotor fidelity. Otherwise save Harris for Paragraph 4 or 6.

### Suggested developer note

```tex
\sourcechecknote{This paragraph defines the thesis' boat-centric or boat-realistic representation, not a standard term from the literature. Rauter et al. support why boat, oars, blades, water, and oar handling are sport-specific rowing elements: their rowing simulator paper describes continuous rower-boat-oar-water interaction, oar blades entering and leaving the water, oar angles, oarlocks, and virtual boat propulsion. Neumann et al. support the VR sport mapping premise by explicitly describing how a rowing ergometer can be transformed into a virtual boat so that handle pulls are depicted as virtual oar movements through water and greater exertion changes virtual movement through scenery. Lamb supports the mismatch premise: ergometer and on-water rowing are related but upper-limb/oar-related mechanics differ, especially around catch and finish. The thesis inference is that a boat-centric representation can make the scene visually more recognizable as rowing, but may require transforming felt ergometer handle motion into virtual oar motion. Harris et al. can be used as a caution that visual realism in VR does not automatically preserve action-relevant sensory and haptic fidelity, but Harris is not rowing-specific and should not be overused here.}
```

### Suggested SOURCE-CHECK comments

```tex
% SOURCE-CHECK:
%   key: rauterEtAl2013rowingTransfer
%   md: MD Papers/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_markdown_bundle/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_raw_page_marked.md, lines 149-199; lines 283-320; lines 397-407
%   pdf: p. 2; p. 3; p. 4
%   evidence: Rowing is a rower-boat-oar-water interaction; blades enter/pull through/leave water, oars and oar angles/oarlocks are central to rowing simulation and measurement.
%   confidence: verified
%   caution: Supports rowing-specific boat/oar depiction, not a claim that this thesis' boat mode improves embodiment.
%
% SOURCE-CHECK:
%   key: neumannEtAl2018interactiveVrSport
%   md: MD Papers/neumann_2018_interactive_virtual_reality_sport_systematic_review_markdown_bundle/neumann_2018_interactive_virtual_reality_sport_systematic_review_raw_page_marked.md, lines 404-419
%   pdf: p. 12
%   evidence: A rowing ergometer can act as an exertion interface transformed into a virtual boat; handle pulls can be depicted as virtual oar movements and exertion can drive faster virtual movement through water/scenery.
%   confidence: verified
%   caution: Supports VR sport mapping possibility, not the thesis' exact two-mode comparison as prior work.
%
% SOURCE-CHECK:
%   key: lamb1989kinematicComparison
%   md: MD Papers/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_markdown_bundle/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_raw_page_marked.md, lines 20-63; lines 419-500
%   pdf: p. 1; pp. 6-7
%   evidence: On-water and ergometer rowing are related but differ in upper-limb/oar-related patterns around catch and finish, partly because on-water rowing includes oar handling not exhibited on the ergometer.
%   confidence: verified
%   caution: Supports why virtual oar action may not fully coincide with felt ergometer handle motion.
%
% SOURCE-CHECK:
%   key: harrisEtAl2019visionForAction
%   md: MD Papers/harris_2019_virtually_the_same_vr_vision_for_action_markdown_bundle/harris_2019_virtually_the_same_vr_vision_for_action_raw_page_marked.md, lines 34-45; lines 251-286
%   pdf: p. 1; p. 3
%   evidence: VR may present altered/conflicting depth cues and limited realistic haptic information, so visually guided actions in VR may differ from real-world action control.
%   confidence: verified
%   caution: Caution source for visual realism versus action fidelity; not rowing-specific.
```

### Appendix / broader-review note

If the final prose wants to mention multiple prior VR rowing systems with boats, rivers, lakes, avatars, and sculls, do not cite-stuff this paragraph. Add a broader note such as: "See Appendix X for a broader overview of rowing-related VR, simulation, and commercial visualization systems." Keep the main paragraph focused on the mode definition and cite only the sources needed for the trade-off.

### Paragraph verdict

Needs narrower paragraph wording.

The mode definition is strong, but "more recognizable as rowing" and "boat-centric" are thesis/design terms. Keep them cautious, and standardize the label later.

# Paragraph 4: Both Representations Are Artificial in Different Ways

## Paragraph 4: Both Representations Are Artificial in Different Ways

### Current paragraph text

The comparison is therefore not between a real and an artificial representation of rowing. Both representations are artificial in different ways. The ergometer-congruent condition preserves the physical logic of the user's actual device and movement, but may depict an indoor machine as if it were moving through a virtual rowing environment. The boat-centric condition preserves the visual and cultural logic of the sport, but must transform the user's straight ergometer handle movement into a boat-and-oar action. There is no neutral third option in which the indoor ergometer becomes on-water rowing without remainder.

### Paragraph function

This paragraph prevents a false hierarchy. It tells the reader not to read the comparison as "real rowing versus fake rowing" or "correct rowing versus wrong rowing." Instead, both representations are compromises:

- the ergometer-congruent mode is faithful to the real device and felt movement, but visually places an indoor machine/action into a virtual rowing context;
- the boat-centric mode is faithful to recognizable boat/oar rowing, but must transform the real ergometer handle movement;
- neither mode can make the participant physically be rowing on water.

This is one of the most important conceptual safeguards in Chapter 1 because it keeps the thesis from overclaiming before data collection.

### Claim ledger

#### Claim CDT-P4-C1

- Exact claim: "The comparison is not between a real and an artificial representation of rowing."
- Claim classification: thesis synthesis and rhetorical bridge.
- Source support needed: source-backed premises that both modes involve representations/mappings and that ergometer/on-water rowing are related but different.
- Current support status: verified as thesis framing.
- Best support: internal thesis framing; `lamb1989kinematicComparison`; `rauterEtAl2013rowingTransfer`; `neumannEtAl2018interactiveVrSport`.
- Wording should be narrowed: no. This is a useful conceptual guardrail.

#### Claim CDT-P4-C2

- Exact claim: "Both representations are artificial in different ways."
- Claim classification: thesis synthesis.
- Source support needed: no source states this exact claim; support comes from the premises that both are virtual mappings of an indoor ergometer situation.
- Current support status: verified as thesis synthesis.
- Best support: internal framing plus mechanical/VR mapping sources.
- Wording should be narrowed: no, but use "artificial" carefully so it does not sound dismissive.

#### Claim CDT-P4-C3

- Exact claim: "The ergometer-congruent condition preserves the physical logic of the user's actual device and movement, but may depict an indoor machine as if it were moving through a virtual rowing environment."
- Claim classification: internal project framing plus thesis synthesis.
- Source support needed: source support for real ergometer action and VR movement-through-environment mappings.
- Current support status: likely.
- Best support: `lamb1989kinematicComparison`; `soperHume2004rowingTechnique`; `neumannEtAl2018interactiveVrSport`; optional `murrayEtAl2016vrRowingPresence`/`arndtEtAl2018vrRowingWorkouts`.
- Wording should be narrowed: maybe. Confirm actual prototype visual design before claiming an indoor machine is depicted moving through the environment.

#### Claim CDT-P4-C4

- Exact claim: "The boat-centric condition preserves the visual and cultural logic of the sport, but must transform the user's straight ergometer handle movement into a boat-and-oar action."
- Claim classification: internal project framing plus thesis synthesis.
- Source support needed: rowing sources for oar/boat/water mechanics and mismatch; VR sport source for handle-to-oar mapping; caution source for visual/action mismatch.
- Current support status: likely.
- Best support: `rauterEtAl2013rowingTransfer`; `lamb1989kinematicComparison`; `neumannEtAl2018interactiveVrSport`; supporting `harrisEtAl2019visionForAction`.
- Wording should be narrowed: yes. "Visual and cultural logic" is not directly sourced; "straight ergometer handle movement" is probably implementation/common-device wording, but the checked sources support "handle movement/central-pulley ergometer" more directly than exact straightness.

#### Claim CDT-P4-C5

- Exact claim: "There is no neutral third option in which the indoor ergometer becomes on-water rowing without remainder."
- Claim classification: thesis synthesis and rhetorical bridge.
- Source support needed: premises that ergometer/on-water differ and VR representations are mappings.
- Current support status: verified as thesis synthesis.
- Best support: `lamb1989kinematicComparison`; `rauterEtAl2013rowingTransfer`; `harrisEtAl2019visionForAction`.
- Wording should be narrowed: no. This is a strong thesis sentence if the tone fits.

### Source cards

#### Source: internal thesis framing

- Citation key: not a bibliography key.
- Source role: best.
- What the source is about, in plain language: the thesis' own definition of the two modes and their trade-off.
- What the source specifically says that matters here: neither mode is assumed to be universally better; the thesis explores trade-offs between movement correspondence and realistic rowing depiction.
- Which exact part of the paragraph it supports: the "both artificial in different ways" logic and the no-neutral-option framing.
- Why this source is used here instead of external sources: external sources support premises but do not make this exact thesis comparison.
- What this source does NOT support: citable external evidence.
- Evidence type: internal project framing.
- Confidence: verified.
- MD path: `AGENTS.md`; `notes/global/thesis_spine.md`; `notes/global/terminology.md`
- MD line range: AGENTS core framing; thesis spine lines 5-24; terminology "Cyborg's Dilemma" entry.
- PDF page if available: not applicable.

#### Source: `lamb1989kinematicComparison`

- Citation key: `lamb1989kinematicComparison`
- Source role: best for why there is no neutral identity between ergometer and on-water rowing.
- What the source is about, in plain language: kinematic comparison of ergometer and on-water rowing.
- What the source specifically says that matters here: ergometer and on-water rowing share some leg/trunk drive characteristics but differ in upper-limb/oar-related motion; oar lifting/feathering at the finish is not exhibited in ergometer rowing.
- Which exact part of the paragraph it supports: the claim that neither representation simply equals on-water rowing; the transformation needed for boat/oar depiction.
- Why this source is used here instead of only Rauter: Lamb directly documents the ergometer/on-water kinematic relation.
- What this source does NOT support: the two-mode framework or "cultural logic."
- Evidence type: thesis-synthesis premise.
- Confidence: verified.
- MD path: `MD Papers/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_markdown_bundle/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_raw_page_marked.md`
- MD line range: lines 20-63; lines 419-500
- PDF page if available: p. 1; pp. 6-7.

#### Source: `rauterEtAl2013rowingTransfer`

- Citation key: `rauterEtAl2013rowingTransfer`
- Source role: best for why boat/oar action is not just visual decoration.
- What the source is about, in plain language: a realistic rowing simulator and transfer study.
- What the source specifically says that matters here: realistic rowing includes haptic oar-water interaction, oar handling, oar height/blade immersion, oar angles, and boat propulsion; ordinary ergometers lack important oar-handling components.
- Which exact part of the paragraph it supports: the boat-centric condition's need to transform ergometer handle movement into boat/oar action; the no-neutral-option claim.
- Why this source is used here instead of only Lamb: it frames the boat/oar/water action structure in simulator terms.
- What this source does NOT support: the exact thesis-mode labels, or the claim that visual boat depiction produces stronger embodiment.
- Evidence type: thesis-synthesis premise.
- Confidence: verified.
- MD path: `MD Papers/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_markdown_bundle/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_raw_page_marked.md`
- MD line range: lines 149-199; lines 283-320; lines 397-407; lines 785-798
- PDF page if available: p. 2; p. 3; p. 4; p. 9.

#### Source: `neumannEtAl2018interactiveVrSport`

- Citation key: `neumannEtAl2018interactiveVrSport`
- Source role: supporting.
- What the source is about, in plain language: interactive VR sport review.
- What the source specifically says that matters here: ergometers can serve as exertion interfaces that are transformed into virtual sport action; in rowing, handle pulls can be depicted as virtual oars moving through water.
- Which exact part of the paragraph it supports: both representations are mappings from a physical ergometer into a virtual rowing environment/action.
- Why this source is used here instead of only concrete VR rowing examples: it gives the abstract exertion-interface/mapping logic.
- What this source does NOT support: it does not discuss the thesis' no-neutral-option claim or the exact two modes.
- Evidence type: contextual support and thesis-synthesis premise.
- Confidence: verified.
- MD path: `MD Papers/neumann_2018_interactive_virtual_reality_sport_systematic_review_markdown_bundle/neumann_2018_interactive_virtual_reality_sport_systematic_review_raw_page_marked.md`
- MD line range: lines 105-123; lines 404-419
- PDF page if available: p. 4; p. 12.

#### Source: `harrisEtAl2019visionForAction`

- Citation key: `harrisEtAl2019visionForAction`
- Source role: supporting/background.
- What the source is about, in plain language: a cautionary source about action in VR.
- What the source specifically says that matters here: virtual environments can alter or conflict depth cues and often lack realistic haptic information, so visually guided action in VR may differ from real-world action.
- Which exact part of the paragraph it supports: the idea that virtual representation is not simply real on-water action, even if it looks realistic.
- Why this source is used here instead of only rowing biomechanics: it supports the VR-specific action-fidelity caution.
- What this source does NOT support: it does not support rowing-specific mechanics or the exact two modes.
- Evidence type: contextual support.
- Confidence: verified.
- MD path: `MD Papers/harris_2019_virtually_the_same_vr_vision_for_action_markdown_bundle/harris_2019_virtually_the_same_vr_vision_for_action_raw_page_marked.md`
- MD line range: lines 34-45; lines 251-286; lines 378-393
- PDF page if available: p. 1; p. 3; p. 4.

### Evidence window

The sources do not directly state "both representations are artificial in different ways." That is the thesis' synthesis. The evidence supports the premises: ergometer and on-water rowing differ, boat/oar/water interaction is meaningful, VR sport systems transform physical exertion into virtual action, and VR action is not automatically real-world action just because it looks realistic.

`lamb1989kinematicComparison` supports that the actual ergometer movement and on-water movement are related but not identical. `rauterEtAl2013rowingTransfer` supports why boat/oar mechanics cannot be treated as a purely cosmetic overlay. `neumannEtAl2018interactiveVrSport` supports the idea that the ergometer can be transformed into virtual boat/oar action. `harrisEtAl2019visionForAction` supports the broader caution that visual realism in VR does not eliminate action-relevant sensory differences.

Representative evidence:

- Lamb: upper-limb/oar-related patterns differ between ergometer and on-water rowing, especially around catch/finish (raw page-marked MD lines 419-500, PDF pp. 6-7).
- Rauter: ordinary ergometers do not train oar handling or oar height in water (raw page-marked MD lines 180-199, PDF p. 2).
- Neumann: ergometer handle pulls can be depicted as virtual oar movements through water (raw page-marked MD lines 404-419, PDF p. 12).
- Harris: VR may contain altered/conflicting depth cues and limited haptic feedback, which can affect action control (raw page-marked MD lines 34-45, PDF p. 1).

### Reasoning bridge

The source-backed premises are that neither the actual ergometer nor a virtual boat/oar depiction is identical to on-water rowing. The ergometer preserves the real device interaction but omits boat/oar/water mechanics. The boat-centric visual representation restores recognizable boat/oar elements but remains a virtual transformation layered onto an ergometer. VR action more generally can differ from real-world action because of altered sensory and haptic information.

The thesis-authored inference is the "no neutral third option" statement. This is not a literature finding; it is the conceptual conclusion drawn from the physical and virtual constraints.

Unsupported or only likely steps: "visual and cultural logic" remains broad. "Straight ergometer handle movement" is plausible but should not be treated as a precise source quote. If you want tighter source alignment, use "real ergometer handle movement" or "single-handle ergometer movement."

### Overclaim boundaries

- Do not claim the boat-centric mode is "real rowing" and the ergometer-congruent mode is artificial.
- Do not claim the ergometer-congruent mode is objectively less realistic in every respect; it may be more faithful to the user's real device interaction.
- Do not claim the boat-centric mode necessarily improves sport realism unless measured or phrased as design intent.
- Do not claim Harris proves rowing-specific mapping conflicts; Harris is general VR action caution.
- Do not claim "cultural logic" as a sourced term unless an additional sport sociology/culture source is added.
- Do not claim there is no possible future technology that could reduce the mismatch; the sentence is about this indoor ergometer setup, not all possible simulators.

### Suggested citation placement

This paragraph is synthesis-heavy. Do not cite every sentence. Use one support group after the sentence about both representations being artificial or after the final "without remainder" sentence:

```tex
\parencite{lamb1989kinematicComparison,rauterEtAl2013rowingTransfer,neumannEtAl2018interactiveVrSport,harrisEtAl2019visionForAction}
```

If this group feels too dense, split it:

- Ergometer/on-water mismatch:

```tex
\parencite{lamb1989kinematicComparison,rauterEtAl2013rowingTransfer}
```

- VR action/representation caution:

```tex
\parencite{neumannEtAl2018interactiveVrSport,harrisEtAl2019visionForAction}
```

Do not add Kilteni or Waltemate here unless the paragraph explicitly discusses agency, ownership, or temporal congruence.

### Suggested developer note

```tex
\sourcechecknote{This paragraph is a thesis synthesis: it argues that neither representation should be treated as the simply "real" one. Lamb supports the premise that ergometer and on-water rowing are related but not identical, with upper-limb and oar-related kinematic differences around catch and finish. Rauter et al. support the rowing-specific action structure that the boat-centric mode tries to depict: rower-boat-oar-water interaction, oar handling, blade-water contact, oar angles, and boat propulsion. Neumann et al. support the VR sport mapping premise that an ergometer can be used as an exertion interface and transformed into a virtual boat/oar action. Harris et al. support the broader caution that visually realistic VR action may still differ from real-world action because of altered depth cues and limited haptic information. The thesis inference is that the ergometer-congruent condition preserves the user's actual device interaction but remains a virtual depiction, while the boat-centric condition preserves recognizable boat/oar rowing imagery but must transform felt handle motion. These sources support the premises, not a direct literature claim that "both modes are artificial" or that either mode is superior.}
```

### Suggested SOURCE-CHECK comments

```tex
% SOURCE-CHECK:
%   key: lamb1989kinematicComparison; rauterEtAl2013rowingTransfer
%   md: MD Papers/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_markdown_bundle/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_raw_page_marked.md, lines 419-500; MD Papers/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_markdown_bundle/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_raw_page_marked.md, lines 149-199; lines 283-320
%   pdf: Lamb pp. 6-7; Rauter p. 2; p. 3
%   evidence: Ergometer and on-water rowing are related but differ in oar/upper-limb mechanics; ordinary ergometers omit oar handling/oar height, while on-water rowing involves rower-boat-oar-water interaction.
%   confidence: verified
%   caution: Supports the no-neutral-option premise, not a result about embodiment.
%
% SOURCE-CHECK:
%   key: neumannEtAl2018interactiveVrSport
%   md: MD Papers/neumann_2018_interactive_virtual_reality_sport_systematic_review_markdown_bundle/neumann_2018_interactive_virtual_reality_sport_systematic_review_raw_page_marked.md, lines 105-123; lines 404-419
%   pdf: p. 4; p. 12
%   evidence: Physical effort on an exertion interface can translate into virtual sport performance; rowing handle pulls can be depicted as virtual oar movements through water.
%   confidence: verified
%   caution: Supports virtual mapping logic, not the exact thesis mode comparison as prior work.
%
% SOURCE-CHECK:
%   key: harrisEtAl2019visionForAction
%   md: MD Papers/harris_2019_virtually_the_same_vr_vision_for_action_markdown_bundle/harris_2019_virtually_the_same_vr_vision_for_action_raw_page_marked.md, lines 34-45; lines 251-286; lines 378-393
%   pdf: p. 1; p. 3; p. 4
%   evidence: VR can alter/conflict depth cues and lacks realistic haptic information, so visually guided actions in VR may diverge from real-world action.
%   confidence: verified
%   caution: General VR action caution, not rowing-specific evidence.
```

### Appendix / broader-review note

No appendix note needed unless the paragraph begins listing multiple VR rowing systems. The paragraph should stay conceptual.

### Paragraph verdict

Needs narrower paragraph wording.

The logic is strong, but two phrases should be reviewed: "visual and cultural logic" and "straight ergometer handle movement." Both are plausible thesis prose, but not directly supported as exact source language.

# Paragraph 5: Broader XR Sport Design Problem

## Paragraph 5: Broader XR Sport Design Problem

### Current paragraph text

This makes VR indoor rowing a useful case for studying a broader XR design problem. Many XR sport and exercise systems use stationary or simplified physical equipment to represent more complex activities. The system can either make the virtual action correspond closely to the user's real movement, or it can transform the movement to better match the represented activity. Both choices solve one part of the problem while introducing another.

### Paragraph function

This paragraph generalizes the rowing case without leaving the scope of the thesis. It says that the rowing mismatch is an instance of a broader XR sport/exercise design problem: physical devices often simplify the represented sport activity, so designers choose between real-movement congruence and activity depiction. The paragraph should situate the thesis in VR sport without pretending that the thesis proves a universal XR law.

### Claim ledger

#### Claim CDT-P5-C1

- Exact claim: "VR indoor rowing is a useful case for studying a broader XR design problem."
- Claim classification: thesis synthesis.
- Source support needed: source support for VR sport/exercise systems using exertion interfaces and sport-relevant virtual mappings; source support for rowing as a relevant example.
- Current support status: verified as thesis framing.
- Best support: `neumannEtAl2018interactiveVrSport`; supporting rowing mechanics sources.
- Wording should be narrowed: no if "useful case" remains, not "representative of all XR sport."

#### Claim CDT-P5-C2

- Exact claim: "Many XR sport and exercise systems use stationary or simplified physical equipment to represent more complex activities."
- Claim classification: directly source-backed in broad terms; may be too broad if "many" implies quantified prevalence.
- Source support needed: VR sport/exercise review discussing exertion interfaces, ergometers/treadmills/cycling/running/rowing, and translation of physical action to virtual sport performance.
- Current support status: likely.
- Best support: `neumannEtAl2018interactiveVrSport`.
- Wording should be narrowed: yes. Consider "VR sport and exercise systems often use exertion interfaces..." or "some systems..." unless a quantitative review statement is cited carefully.

#### Claim CDT-P5-C3

- Exact claim: "The system can either make the virtual action correspond closely to the user's real movement, or transform the movement to better match the represented activity."
- Claim classification: thesis synthesis.
- Source support needed: embodiment/congruence sources for the real-movement correspondence side; VR sport mapping/action sources for transformation side.
- Current support status: verified as thesis synthesis.
- Best support: `kilteniEtAl2012senseEmbodiment`; `neumannEtAl2018interactiveVrSport`; `harrisEtAl2019visionForAction`.
- Wording should be narrowed: no, if presented as design framing.

#### Claim CDT-P5-C4

- Exact claim: "Both choices solve one part of the problem while introducing another."
- Claim classification: thesis synthesis/rhetorical bridge.
- Source support needed: no direct source; the paragraph's premises support the trade-off.
- Current support status: verified as thesis framing.
- Best support: internal thesis framing plus source-backed premises.
- Wording should be narrowed: no.

### Source cards

#### Source: `neumannEtAl2018interactiveVrSport`

- Citation key: `neumannEtAl2018interactiveVrSport`
- Source role: best.
- What the source is about, in plain language: a systematic review of interactive VR sport that discusses virtual sport environments, interactivity, exertion interfaces, and sport/exercise examples such as cycling, running, and rowing.
- What the source specifically says that matters here: VR sport can use physical effort on machines such as ergometers as exertion interfaces; physical actions can translate into virtual sport performance; rowing, cycling, and running are examples where an ergometer/treadmill interface can map into virtual movement.
- Which exact part of the paragraph it supports: the broader XR/VR sport design problem and the use of stationary/simplified equipment to represent sport activity.
- Why this source is used here instead of individual rowing papers: it provides review-level context and examples across VR sport/exercise systems.
- What this source does NOT support: embodiment theory, rowing biomechanics detail, or the exact thesis mode comparison.
- Evidence type: direct evidence for VR sport/exertion-interface context; thesis-synthesis premise.
- Confidence: verified.
- MD path: `MD Papers/neumann_2018_interactive_virtual_reality_sport_systematic_review_markdown_bundle/neumann_2018_interactive_virtual_reality_sport_systematic_review_raw_page_marked.md`
- MD line range: lines 73-88; lines 105-123; lines 228-241; lines 304-337; lines 404-419; lines 688-689
- PDF page if available: p. 3; p. 4; p. 7; pp. 9-10; p. 12; p. 19.

#### Source: `harrisEtAl2019visionForAction`

- Citation key: `harrisEtAl2019visionForAction`
- Source role: supporting.
- What the source is about, in plain language: a review arguing that visually guided action in VR may differ from real-world action because sensory information is altered or incomplete.
- What the source specifically says that matters here: visually realistic virtual action may not preserve all action-relevant sensory/haptic information.
- Which exact part of the paragraph it supports: the caution that transforming movement to match a represented activity can introduce another problem.
- Why this source is used here instead of only Neumann: Neumann situates VR sport; Harris explains why action representation in VR can be problematic even when visually plausible.
- What this source does NOT support: stationary exercise equipment prevalence or rowing mechanics.
- Evidence type: contextual support.
- Confidence: verified.
- MD path: `MD Papers/harris_2019_virtually_the_same_vr_vision_for_action_markdown_bundle/harris_2019_virtually_the_same_vr_vision_for_action_raw_page_marked.md`
- MD line range: lines 34-45; lines 251-286; lines 378-393
- PDF page if available: p. 1; p. 3; p. 4.

#### Source: `kilteniEtAl2012senseEmbodiment`

- Citation key: `kilteniEtAl2012senseEmbodiment`
- Source role: supporting.
- What the source is about, in plain language: sense of embodiment framework in VR.
- What the source specifically says that matters here: visuomotor correlations and discrepancies between visual feedback and actual movement affect agency.
- Which exact part of the paragraph it supports: the "correspond closely to the user's real movement" side of the design problem.
- Why this source is used here instead of only VR sport sources: it provides the embodiment reason why real-movement correspondence matters.
- What this source does NOT support: broad XR sport system prevalence or rowing-specific trade-offs.
- Evidence type: contextual support and thesis-synthesis premise.
- Confidence: verified.
- MD path: `MD Papers/kilteni_2012_sense_of_embodiment_markdown_bundle/kilteni_2012_sense_of_embodiment_raw_page_marked.md`
- MD line range: lines 338-377; lines 922-926
- PDF page if available: pp. 4-5; p. 11.

### Evidence window

`neumannEtAl2018interactiveVrSport` is the central source. It defines interactive VR sport around a computer-simulated sport environment and interactivity. It also discusses exertion interfaces: physical effort on a machine such as an ergometer can be related to speed through a virtual race course, and physical actions can translate into virtual sport performance. The rowing example directly says an ergometer can be transformed into a virtual boat and handle pulls can be depicted as virtual oar movements.

Representative excerpts:

- "physical effort on a machine such as an ergometer can be related to the speed of movement through a virtual race course" (raw page-marked MD lines 105-123, PDF p. 4).
- Rowing handle pulls can be depicted as virtual oar movements through water (raw page-marked MD lines 404-419, PDF p. 12).

`harrisEtAl2019visionForAction` supports the caution that visual activity representation is not automatically action-equivalent. `kilteniEtAl2012senseEmbodiment` supports the other side: preserving correspondence between seen and performed movement matters for agency. Together, these support the thesis' broader framing that one can prioritize real-movement correspondence or represented-activity match, and both have trade-offs.

### Reasoning bridge

The source-backed premises are that interactive VR sport often maps physical exercise/sport interfaces into virtual sport environments, and that rowing is one example. Embodiment/action sources support the idea that correspondence between performed and seen movement matters for agency, while VR action caution sources support the idea that visual representations can differ from real-world action conditions.

The thesis-authored inference is the general design problem: XR sport systems can either preserve the user's actual movement closely or transform it to better match the represented activity. This is a useful thesis framing, not a formal taxonomy established by Neumann, Kilteni, or Harris.

Unsupported or only likely steps: "Many XR sport and exercise systems" could be too broad if read quantitatively. Use "many" only as a general review-based claim, or narrow to "VR sport and exercise systems often..." / "some systems..."

### Overclaim boundaries

- Do not claim the thesis solves the broader XR sport design problem generally.
- Do not claim all XR sport systems use stationary/simplified equipment.
- Do not claim Neumann discusses embodiment, ownership, or agency.
- Do not claim Harris proves the rowing trade-off.
- Do not claim Kilteni studied sport or rowing.
- Do not claim transforming movement is bad by default; it solves sport depiction while introducing congruence questions.

### Suggested citation placement

Place `neumannEtAl2018interactiveVrSport` after the sentence about stationary/simplified equipment and complex activities:

```tex
\parencite{neumannEtAl2018interactiveVrSport}
```

If the next sentence explicitly connects real-movement correspondence to embodiment/agency, cite:

```tex
\parencite{kilteniEtAl2012senseEmbodiment}
```

If it emphasizes visual activity match versus action fidelity, cite:

```tex
\parencite{harrisEtAl2019visionForAction}
```

Do not cite all three unless the prose explicitly includes all three concepts. The paragraph may work with only Neumann, leaving Kilteni/Harris for Paragraph 6.

### Suggested developer note

```tex
\sourcechecknote{This paragraph broadens the rowing case to interactive VR sport without claiming that the thesis solves XR sport design in general. Neumann et al. are the main support: their review defines interactive VR sport through a simulated sport environment and interactivity, discusses exertion interfaces, and gives examples where physical effort on machines such as ergometers is translated into virtual race-course or sport performance. Their rowing example explicitly describes an ergometer being transformed into a virtual boat, with handle pulls depicted as virtual oar movements through water. Kilteni et al. can support the real-movement-correspondence side because agency is linked to synchronous visuomotor correlations and affected by discrepancies between seen feedback and actual movement. Harris et al. can support the action-fidelity caution because visually guided action in VR can differ from real-world action when depth cues and haptic information are altered or absent. The thesis inference is that XR sport systems may choose between close correspondence to real movement and transformation toward the represented activity; this is a design framing, not a formal taxonomy established by the cited sources.}
```

### Suggested SOURCE-CHECK comments

```tex
% SOURCE-CHECK:
%   key: neumannEtAl2018interactiveVrSport
%   md: MD Papers/neumann_2018_interactive_virtual_reality_sport_systematic_review_markdown_bundle/neumann_2018_interactive_virtual_reality_sport_systematic_review_raw_page_marked.md, lines 105-123; lines 228-241; lines 404-419
%   pdf: p. 4; p. 7; p. 12
%   evidence: Interactive VR sport uses simulated sport environments and interactivity; physical effort on machines such as ergometers can translate into virtual sport performance; rowing ergometer handle pulls can be depicted as virtual oar movements.
%   confidence: verified
%   caution: Supports broader VR sport/exertion-interface context, not embodiment theory or the exact thesis comparison as prior work.
%
% SOURCE-CHECK:
%   key: kilteniEtAl2012senseEmbodiment
%   md: MD Papers/kilteni_2012_sense_of_embodiment_markdown_bundle/kilteni_2012_sense_of_embodiment_raw_page_marked.md, lines 338-377
%   pdf: pp. 4-5
%   evidence: Sense of agency is linked to predicted/actual sensory consequences and synchronous visuomotor correlations; discrepancies between visual feedback and actual movement negatively affect agency.
%   confidence: verified
%   caution: Use only if the paragraph explicitly invokes real-movement correspondence as embodiment-relevant.
%
% SOURCE-CHECK:
%   key: harrisEtAl2019visionForAction
%   md: MD Papers/harris_2019_virtually_the_same_vr_vision_for_action_markdown_bundle/harris_2019_virtually_the_same_vr_vision_for_action_raw_page_marked.md, lines 34-45; lines 251-286
%   pdf: p. 1; p. 3
%   evidence: VR can impair or conflict depth cues and lacks realistic haptic information, so visually guided action in VR may differ from real-world action.
%   confidence: verified
%   caution: General VR action caution; do not use as evidence for rowing-specific outcomes.
```

### Appendix / broader-review note

Potentially useful if this paragraph grows. If the thesis wants to list multiple stationary-equipment XR sport systems, add an appendix or related-work table instead of citation-stuffing the Introduction paragraph.

Suggested note idea:

```text
See Appendix X for a broader overview of rowing-related VR, simulation, and exercise-interface systems.
```

### Paragraph verdict

Needs narrower paragraph wording.

The logic is good. Consider narrowing "many XR sport and exercise systems" to "VR sport and exercise systems often..." or "some interactive VR sport systems..." unless the final text cites Neumann's review more explicitly.

# Paragraph 6: Visuomotor Congruence Versus Realistic Sport Depiction

## Paragraph 6: Visuomotor Congruence Versus Realistic Sport Depiction

### Current paragraph text

In this thesis, this design problem is framed as a trade-off between visuomotor congruence and realistic sport depiction. Visuomotor congruence refers to the correspondence between the user's performed movement and the movement they see in the virtual environment. Realistic sport depiction refers to the extent to which the virtual scene and action resemble the sport being represented. The two can support each other, but in indoor rowing they can also come apart.

### Paragraph function

This paragraph gives the conceptual label for the subsection. It defines the trade-off in terms that can carry into the rest of the thesis:

- visuomotor congruence: the seen movement corresponds to performed movement;
- realistic sport depiction: the scene/action resembles recognizable rowing;
- in indoor rowing these can align, but can also diverge because the ergometer movement and boat/oar action are not identical.

This paragraph is the bridge into embodiment theory. It should cite embodiment/agency sources for visuomotor congruence, rowing mechanics sources for why the trade-off comes apart specifically in rowing, and VR action caution sources for why visual realism does not automatically equal action fidelity.

### Claim ledger

#### Claim CDT-P6-C1

- Exact claim: "This design problem is framed as a trade-off between visuomotor congruence and realistic sport depiction."
- Claim classification: thesis synthesis and internal project framing.
- Source support needed: sources for visuomotor congruence relevance, action-fidelity caution, and rowing-specific mismatch.
- Current support status: verified as thesis framing; source-backed premises verified.
- Best support: `kilteniEtAl2012senseEmbodiment`; `harrisEtAl2019visionForAction`; `lamb1989kinematicComparison`; `rauterEtAl2013rowingTransfer`.
- Wording should be narrowed: maybe. "Realistic sport depiction" is thesis terminology; "recognizable sport depiction" may be safer if realism is not measured yet.

#### Claim CDT-P6-C2

- Exact claim: "Visuomotor congruence refers to the correspondence between the user's performed movement and the movement they see in the virtual environment."
- Claim classification: directly source-backed in concept, thesis wording in definition.
- Source support needed: embodiment/agency source linking synchronous visuomotor correlations and visual feedback/action correspondence to agency.
- Current support status: verified.
- Best support: `kilteniEtAl2012senseEmbodiment`; optional `waltemateEtAl2016latency` if timing/responsiveness is discussed.
- Wording should be narrowed: no. This is clear and source-aligned.

#### Claim CDT-P6-C3

- Exact claim: "Realistic sport depiction refers to the extent to which the virtual scene and action resemble the sport being represented."
- Claim classification: internal project framing/thesis definition.
- Source support needed: no source defines this term exactly; source support can ground rowing-specific visual/action ingredients and VR action caution.
- Current support status: likely.
- Best support: internal thesis framing; `rauterEtAl2013rowingTransfer`; `neumannEtAl2018interactiveVrSport`; `harrisEtAl2019visionForAction`.
- Wording should be narrowed: maybe. If "realistic" implies objective sport realism or measured realism, clarify as "depiction" or "recognizable visual/action resemblance."

#### Claim CDT-P6-C4

- Exact claim: "The two can support each other, but in indoor rowing they can also come apart."
- Claim classification: thesis synthesis from multiple source-backed premises.
- Source support needed: rowing mismatch sources plus embodiment/congruence and VR action/realism caution sources.
- Current support status: likely/verified with combined support; was flagged too broad in the old verification unless rowing-specific sources are included.
- Best support: `lamb1989kinematicComparison`; `rauterEtAl2013rowingTransfer`; `kilteniEtAl2012senseEmbodiment`; `harrisEtAl2019visionForAction`; optional `waltemateEtAl2016latency`.
- Wording should be narrowed: no if "can" remains. Avoid "necessarily conflict."

### Source cards

#### Source: `kilteniEtAl2012senseEmbodiment`

- Citation key: `kilteniEtAl2012senseEmbodiment`
- Source role: best for visuomotor congruence and agency.
- What the source is about, in plain language: a conceptual VR embodiment paper defining sense of embodiment and its subcomponents.
- What the source specifically says that matters here: agency is linked to matching predicted and actual sensory consequences and synchronous visuomotor correlations; discrepancies between visual feedback and actual movement negatively affect agency. The paper also frames SoE through self-location, agency, and body ownership.
- Which exact part of the paragraph it supports: the definition and relevance of visuomotor congruence.
- Why this source is used here instead of rowing biomechanics: rowing sources establish the physical mismatch; Kilteni explains why movement/visual correspondence matters for embodiment.
- What this source does NOT support: sport realism, rowing mechanics, or the thesis' exact trade-off.
- Evidence type: direct conceptual support and thesis-synthesis premise.
- Confidence: verified.
- MD path: `MD Papers/kilteni_2012_sense_of_embodiment_markdown_bundle/kilteni_2012_sense_of_embodiment_raw_page_marked.md`
- MD line range: lines 190-226; lines 338-377; lines 397-411; lines 436-444; lines 922-926
- PDF page if available: p. 3; pp. 4-5; p. 11.

#### Source: `waltemateEtAl2016latency`

- Citation key: `waltemateEtAl2016latency`
- Source role: supporting/optional.
- What the source is about, in plain language: a full-body avatar latency study in VR.
- What the source specifically says that matters here: feedback delays affect motor performance, simultaneity, agency, and ownership; the paper defines latency as delay between user interaction and feedback.
- Which exact part of the paragraph it supports: temporal side of visuomotor congruence if the thesis later mentions timing, responsiveness, or delays.
- Why this source is used here instead of only Kilteni: Kilteni is conceptual; Waltemate is VR full-body evidence.
- What this source does NOT support: rowing-specific mapping, sport realism, or a direct latency threshold for this prototype.
- Evidence type: methodological analogy and contextual support.
- Confidence: verified.
- MD path: `MD Papers/waltemate_2016_latency_perceptual_judgments_motor_performance_vr_markdown_bundle/waltemate_2016_latency_perceptual_judgments_motor_performance_vr_raw_page_marked.md`
- MD line range: lines 37-60; lines 70-84; lines 221-229; lines 520-540; lines 796-821; lines 847-860
- PDF page if available: p. 1; p. 2; p. 5; p. 7.

#### Source: `harrisEtAl2019visionForAction`

- Citation key: `harrisEtAl2019visionForAction`
- Source role: best for visual realism versus action-fidelity caution.
- What the source is about, in plain language: a review arguing that VR action may differ from real-world action because sensory information is altered.
- What the source specifically says that matters here: depth cues can be impaired or in conflict in VR, realistic haptic information is largely absent, and complex actions in VR may diverge from real-world action control even if virtual scenes are visually compelling.
- Which exact part of the paragraph it supports: the distinction between visual/sport depiction and action-relevant sensorimotor congruence.
- Why this source is used here instead of only embodiment sources: embodiment sources support congruence; Harris supports caution around visual realism/action equivalence.
- What this source does NOT support: rowing-specific mismatch or the exact thesis terms.
- Evidence type: direct caution source for VR action; thesis-synthesis premise.
- Confidence: verified.
- MD path: `MD Papers/harris_2019_virtually_the_same_vr_vision_for_action_markdown_bundle/harris_2019_virtually_the_same_vr_vision_for_action_raw_page_marked.md`
- MD line range: lines 34-45; lines 70-78; lines 202-229; lines 251-286; lines 378-393
- PDF page if available: p. 1; p. 2; p. 3; p. 4.

#### Source: `lamb1989kinematicComparison`

- Citation key: `lamb1989kinematicComparison`
- Source role: best for rowing-specific "come apart" premise.
- What the source is about, in plain language: direct comparison of ergometer and on-water rowing kinematics.
- What the source specifically says that matters here: ergometer and on-water rowing share some movement features but differ in arm/oar-related mechanics, especially around catch and finish.
- Which exact part of the paragraph it supports: why visuomotor congruence to the actual ergometer and visual resemblance to boat/oar rowing can diverge in indoor rowing.
- Why this source is used here instead of only Harris/Kilteni: Harris and Kilteni are general; Lamb makes the trade-off rowing-specific.
- What this source does NOT support: embodiment theory or sport depiction as a psychological construct.
- Evidence type: direct rowing mechanics premise.
- Confidence: verified.
- MD path: `MD Papers/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_markdown_bundle/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_raw_page_marked.md`
- MD line range: lines 20-63; lines 419-500
- PDF page if available: p. 1; pp. 6-7.

#### Source: `rauterEtAl2013rowingTransfer`

- Citation key: `rauterEtAl2013rowingTransfer`
- Source role: best for rowing-specific sport-action depiction.
- What the source is about, in plain language: realistic rowing simulator and transfer study.
- What the source specifically says that matters here: rowing includes continuous rower-boat-oar-water interaction, oar handling, blade immersion, oar angles, and coordinated drive/recovery action. Ordinary ergometers omit some of these rowing-specific components.
- Which exact part of the paragraph it supports: the sport-depiction side and why it can diverge from the actual ergometer interaction.
- Why this source is used here instead of only Lamb: it gives the rowing-specific action structure and simulator relevance.
- What this source does NOT support: visual realism alone, embodiment outcomes, or the exact thesis comparison as prior work.
- Evidence type: direct rowing-action premise.
- Confidence: verified.
- MD path: `MD Papers/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_markdown_bundle/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_raw_page_marked.md`
- MD line range: lines 149-199; lines 283-320; lines 785-798
- PDF page if available: p. 2; p. 3; p. 9.

#### Source: `neumannEtAl2018interactiveVrSport`

- Citation key: `neumannEtAl2018interactiveVrSport`
- Source role: supporting.
- What the source is about, in plain language: interactive VR sport review.
- What the source specifically says that matters here: physical actions can be translated into virtual sport performance; rowing ergometer handle pulls can be represented as virtual oar movements.
- Which exact part of the paragraph it supports: the represented-activity mapping side of the trade-off.
- Why this source is used here instead of concrete examples: it provides the broad VR sport action-mapping context.
- What this source does NOT support: embodiment/congruence theory or rowing biomechanics.
- Evidence type: contextual support and thesis-synthesis premise.
- Confidence: verified.
- MD path: `MD Papers/neumann_2018_interactive_virtual_reality_sport_systematic_review_markdown_bundle/neumann_2018_interactive_virtual_reality_sport_systematic_review_raw_page_marked.md`
- MD line range: lines 105-123; lines 404-419
- PDF page if available: p. 4; p. 12.

### Evidence window

#### `kilteniEtAl2012senseEmbodiment`

Kilteni et al. are the core source for the visuomotor congruence side. The agency section links agency to comparisons between predicted and actual sensory consequences and to synchronous visuomotor correlations during active movement. It also states that discrepancies between visual feedback and actual movement negatively affect agency. This supports defining visuomotor congruence as correspondence between performed movement and seen movement in VR.

Representative excerpt:

- Synchronous visuomotor correlations under active movement support agency, while discrepancies between visual feedback and actual movement negatively affect agency (raw page-marked MD lines 349-377, PDF pp. 4-5).

#### `waltemateEtAl2016latency`

Waltemate et al. are optional but useful if temporal congruence appears in the final prose. Their full-body avatar study manipulated visual feedback delays and measured motor performance, simultaneity, agency, and ownership. They found increasing delay affected these perceptual and performance outcomes, but the exact thresholds should not be imported into this thesis.

Representative excerpt:

- "sense of agency, ownership, and perceived simultaneity decreased, and motor performance worsened, with increasing delay" (raw page-marked MD lines 520-540, PDF p. 5).

#### `harrisEtAl2019visionForAction`

Harris et al. support the distinction between visual realism and action-relevant fidelity. The paper warns that VR may impair or conflict depth cues and lacks realistic haptic feedback, with possible consequences for motor skills and action control. This source helps prevent the phrase "realistic sport depiction" from being equated with embodied/action fidelity.

Representative excerpt:

- "realistic haptic information is all but absent from current VR systems" and these conflicts can affect motor skills (raw page-marked MD lines 34-45, PDF p. 1).

#### `lamb1989kinematicComparison` and `rauterEtAl2013rowingTransfer`

These sources make the "come apart in indoor rowing" claim sourceable. Lamb establishes that ergometer and on-water rowing are related but kinematically different in arm/oar-related parts of the stroke. Rauter establishes that rowing's sport-specific action includes oar-water interaction and oar handling that ordinary ergometers do not train. Together they show why a virtual action can either track the actual ergometer interaction or depict a boat/oar action more recognizably, and those goals can diverge.

#### `neumannEtAl2018interactiveVrSport`

Neumann supports the VR sport mapping side: physical effort and handle pulls can be translated into virtual sport action. It is not an embodiment source, but it helps connect the trade-off to interactive VR sport.

### Reasoning bridge

The source-backed premises are:

- Visuomotor congruence matters for agency and embodiment-related experience because seen movement and performed movement need to correspond.
- VR action can be visually realistic while still differing from real-world action due to sensory/haptic constraints.
- Ergometer rowing and on-water rowing are related but not identical, especially in oar/upper-limb and boat/oar/water mechanics.
- VR sport systems can transform physical exercise-device input into virtual sport action.

The thesis-authored inference is the exact trade-off label: "visuomotor congruence versus realistic sport depiction." This is not a literature category. It is the thesis' way of naming the rowing-specific conflict between preserving the user's real action loop and preserving the recognizable sport form.

Unsupported or only likely steps: "realistic sport depiction" is internally defined and likely, not externally validated. If the final study uses a "rowing realism" measure, Chapter 4 can operationalize it. Until then, "recognizable sport depiction" may be safer than "realistic sport depiction."

### Overclaim boundaries

- Do not claim sport depiction is equivalent to embodiment.
- Do not claim visuomotor congruence always dominates sport realism.
- Do not claim the two always conflict; the paragraph correctly says they can support each other and can come apart.
- Do not claim Harris, Kilteni, or Waltemate studied rowing.
- Do not claim Lamb or Rauter studied ownership/agency.
- Do not use Waltemate's latency values as direct thresholds for the rowing prototype.
- Do not claim "realistic sport depiction" is a validated construct unless it is operationalized in the study.

### Suggested citation placement

For the visuomotor congruence definition:

```tex
\parencite{kilteniEtAl2012senseEmbodiment}
```

If temporal congruence/responsiveness is mentioned in the final prose:

```tex
\parencite{waltemateEtAl2016latency}
```

For the distinction between visual realism/sport depiction and action fidelity:

```tex
\parencite{harrisEtAl2019visionForAction}
```

For "in indoor rowing they can also come apart":

```tex
\parencite{lamb1989kinematicComparison,rauterEtAl2013rowingTransfer}
```

Suggested combined group for the final sentence:

```tex
\parencite{lamb1989kinematicComparison,rauterEtAl2013rowingTransfer,kilteniEtAl2012senseEmbodiment,harrisEtAl2019visionForAction}
```

Use `waltemateEtAl2016latency` only if the final wording explicitly includes temporal congruence/responsiveness.

### Suggested developer note

```tex
\sourcechecknote{This paragraph names the thesis' core trade-off. Kilteni et al. support the visuomotor-congruence side: agency is linked to comparisons between predicted and actual sensory consequences and to synchronous visuomotor correlations, while discrepancies between visual feedback and actual movement can reduce agency. Waltemate et al. can support temporal-congruence or responsiveness wording if used, because their full-body avatar study shows that visual feedback delays affect motor performance, perceived simultaneity, agency, and ownership; their specific latency thresholds should not be imported as rowing design requirements. Harris et al. support the distinction between visual realism and action fidelity by warning that VR can alter depth cues and lacks realistic haptic information, so visually guided action in VR may diverge from real-world action. Lamb and Rauter make the trade-off rowing-specific: ergometer and on-water rowing are related but differ in upper-limb/oar mechanics, and ordinary ergometers omit oar handling, blade-water interaction, and other boat/oar action components. The thesis inference is that indoor VR rowing can pursue close correspondence to the real ergometer movement or recognizable sport depiction of boat-and-oar rowing, and these goals can support each other but can also come apart.}
```

### Suggested SOURCE-CHECK comments

```tex
% SOURCE-CHECK:
%   key: kilteniEtAl2012senseEmbodiment
%   md: MD Papers/kilteni_2012_sense_of_embodiment_markdown_bundle/kilteni_2012_sense_of_embodiment_raw_page_marked.md, lines 338-377; lines 922-926
%   pdf: pp. 4-5; p. 11
%   evidence: Agency is linked to predicted/actual sensory consequences and synchronous visuomotor correlations; discrepancies between visual feedback and actual movement negatively affect agency.
%   confidence: verified
%   caution: Supports visuomotor congruence relevance, not rowing-specific outcomes.
%
% SOURCE-CHECK:
%   key: harrisEtAl2019visionForAction
%   md: MD Papers/harris_2019_virtually_the_same_vr_vision_for_action_markdown_bundle/harris_2019_virtually_the_same_vr_vision_for_action_raw_page_marked.md, lines 34-45; lines 251-286; lines 378-393
%   pdf: p. 1; p. 3; p. 4
%   evidence: VR can alter/conflict depth cues and lacks realistic haptic information, so visually guided actions in VR may differ from real-world action even when visually convincing.
%   confidence: verified
%   caution: Supports visual realism/action-fidelity distinction, not rowing-specific mapping outcomes.
%
% SOURCE-CHECK:
%   key: lamb1989kinematicComparison; rauterEtAl2013rowingTransfer
%   md: MD Papers/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_markdown_bundle/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_raw_page_marked.md, lines 20-63; lines 419-500; MD Papers/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_markdown_bundle/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_raw_page_marked.md, lines 149-199; lines 283-320
%   pdf: Lamb p. 1; Lamb pp. 6-7; Rauter p. 2; Rauter p. 3
%   evidence: Ergometer and on-water rowing are related but differ in upper-limb/oar mechanics; rowing includes rower-boat-oar-water interaction and ordinary ergometers omit oar handling/oar height.
%   confidence: verified
%   caution: Supports why congruence and sport depiction can come apart in rowing; not direct embodiment evidence.
%
% SOURCE-CHECK:
%   key: waltemateEtAl2016latency
%   md: MD Papers/waltemate_2016_latency_perceptual_judgments_motor_performance_vr_markdown_bundle/waltemate_2016_latency_perceptual_judgments_motor_performance_vr_raw_page_marked.md, lines 37-60; lines 520-540; lines 796-821
%   pdf: p. 1; p. 5; p. 7
%   evidence: Full-body avatar feedback delays affected motor performance, perceived simultaneity, agency, and ownership.
%   confidence: verified
%   caution: Optional; use only for temporal congruence/responsiveness wording and do not transfer latency thresholds directly to rowing.
```

### Appendix / broader-review note

No appendix note needed. This paragraph should carry the conceptual label, not become a literature survey.

### Paragraph verdict

Ready for prose patch if wording remains cautious.

The final claim is sourceable when combining rowing mechanics sources with embodiment/action sources. Do not cite only Kilteni/Harris/Waltemate for the rowing-specific "come apart" claim; include Lamb and/or Rauter.

# Subsection Summary

## Stable Citation Spine

These sources should remain central to the Core Design Tension subsection:

- `lamb1989kinematicComparison`: best for direct ergometer/on-water kinematic comparison and the "related but not identical" premise.
- `soperHume2004rowingTechnique`: best supporting source for ergometer use, central-pulley limitations, and body-action reproduction caveats.
- `rauterEtAl2013rowingTransfer`: best for rowing as rower-boat-oar-water action and for ordinary ergometer limits around oar handling/oar height.
- `neumannEtAl2018interactiveVrSport`: best for broader VR sport/exertion-interface mapping, especially the rowing ergometer transformed into virtual boat/oars.
- `kilteniEtAl2012senseEmbodiment`: best for visuomotor congruence and agency as embodiment-relevant concepts.
- `harrisEtAl2019visionForAction`: best caution source for visual realism versus action-relevant sensorimotor/haptic fidelity in VR.

## Optional or Weak Sources

- `waltemateEtAl2016latency`: useful only when the final wording includes temporal congruence, responsiveness, delay, latency, or simultaneity. Do not use it for general spatial congruence unless the paragraph explicitly discusses timing.
- `murrayEtAl2016vrRowingPresence`: useful concrete VR rowing example, but probably belongs more in Motivation or related work than in this mode-definition subsection unless the text wants a concrete river/avatar example.
- `arndtEtAl2018vrRowingWorkouts`: useful concrete HMD rowing example, but optional here for the same reason as Murray.
- `harrisEtAl2019visionForAction` in Paragraph 3 or 4: useful but can become too broad if overused. It is strongest in Paragraph 6 where the visual-realism/action-fidelity distinction is explicit.

## Thesis Synthesis Points

These inferences are authored by the thesis rather than directly stated in one source:

- "Movement interface" is the thesis' summary term for the ergometer/boat apparatus difference.
- "Ergometer-congruent representation" is a thesis-defined mode, not a literature category.
- "Boat-centric" or "boat-realistic representation" is a thesis-defined mode, not a literature category.
- The comparison is not "real versus artificial"; both modes are representations with different compromises.
- The no-neutral-third-option claim is thesis synthesis from ergometer/on-water mismatch and VR mapping constraints.
- The broader XR design problem is thesis framing built on VR sport/exertion-interface literature.
- The exact trade-off label "visuomotor congruence versus realistic sport depiction" is thesis framing; sources support the underlying concepts.
- The claim that these can "come apart" in indoor rowing requires combining embodiment/action sources with rowing-specific mismatch sources.

## Claims Needing Manual Verification

- `actual handle path and seat motion`: verify against current prototype implementation before changing "can be animated" into "is animated."
- `straight ergometer handle movement`: source support is stronger for handle/central-pulley/single-handle ergometer movement than for exact straightness. Prefer "real ergometer handle movement" unless implementation documentation supports straight/linear path wording.
- `visual and cultural logic`: not directly sourced in the checked literature. Prefer "recognizable visual and sport-specific logic" unless adding a sport-culture source.
- `more recognizable as rowing`: plausible design rationale, but not directly measured by the checked sources. Use "designed to be more recognizable" unless measured.
- `many XR sport and exercise systems`: supported in broad terms by Neumann, but avoid quantitative interpretation. Prefer "some" or "often" depending on final phrasing.
- `boat-centric` terminology: standardize against "boat-realistic" or "boat-centered" before final cleanup.
- `realistic sport depiction`: if this becomes a measured construct, Chapter 4 should operationalize it. Otherwise "recognizable sport depiction" may be safer.

## Recommended Wording Changes

- Keep Paragraph 1 mostly as is, but consider "constrained handle movement" rather than "constrained path" if exact path geometry is not discussed.
- Keep "ergometer-congruent representation" as thesis terminology, but do not cite it as a literature term.
- In Paragraph 2, keep "can be animated" until implementation is verified; avoid "is animated" unless Chapter 3 confirms it.
- In Paragraph 3, consider standardizing "boat-centric" to "boat-realistic" if that is the final thesis term.
- Replace "visual and cultural logic of the sport" with "recognizable visual and sport-specific logic of rowing" unless a culture/source layer is added.
- Replace "straight ergometer handle movement" with "real ergometer handle movement" unless the handle path has been technically verified.
- Narrow "Many XR sport and exercise systems..." to "Some interactive VR sport and exercise systems..." or cite Neumann more explicitly.
- Consider "recognizable sport depiction" rather than "realistic sport depiction" if realism is not yet operationalized.

## Final Developer Notes

### Final developer note 1

```tex
\sourcechecknote{This paragraph grounds the design tension in rowing mechanics rather than in VR theory. Lamb directly compares ergometer and on-water rowing and supports the nuanced premise that the movements are related but not identical: leg and trunk patterns are broadly similar in many drive-phase variables, while upper arm and forearm patterns differ, especially around catch and finish where on-water rowing involves oar-water mechanics such as lifting and feathering that are absent from ergometer rowing. Soper and Hume support the status of the ergometer as a normal rowing training/testing device while also noting that common ergometers reproduce only parts of on-water body action and do not reproduce trunk and upper-limb patterns particularly well because of the central pulley system. Rauter et al. support the boat-side interface: rowing involves continuous rower-boat-oar-water interaction, ordinary ergometers replace this with cable-driven resistance, and realistic rowing includes oar handling, blade-water interaction, oar angles, and boat propulsion. The thesis inference is that these source-backed differences amount to different movement interfaces and spatial action logics. These sources do not support VR embodiment outcomes or any claim that the ergometer is invalid as training equipment.}
```

### Final developer note 2

```tex
\sourcechecknote{This paragraph defines the thesis' ergometer-congruent representation rather than importing a named mode from the literature. The mode is thesis-defined as a representation that keeps the virtual body, handle, apparatus, and avatar movement aligned primarily with the user's real ergometer interaction. Kilteni et al. support why this kind of mapping is theoretically relevant: agency is linked to comparisons between predicted and actual sensory consequences and to synchronous visuomotor correlations, while discrepancies between visual feedback and actual movement can reduce agency. Waltemate et al. can support temporal-congruence language if the final prose mentions responsiveness or delay, because their full-body avatar study shows that delayed feedback affects motor performance, simultaneity, agency, and ownership. Neumann et al. only provides broad VR sport context, showing that physical exertion interfaces can be translated into virtual sport action. None of these sources names this mode or proves it will improve embodiment in rowing; the implementation-specific claim that the avatar follows actual handle path and seat motion should be checked against the prototype chapter before final wording.}
```

### Final developer note 3

```tex
\sourcechecknote{This paragraph defines the thesis' boat-centric or boat-realistic representation, not a standard term from the literature. Rauter et al. support why boat, oars, blades, water, and oar handling are sport-specific rowing elements: their rowing simulator paper describes continuous rower-boat-oar-water interaction, oar blades entering and leaving the water, oar angles, oarlocks, and virtual boat propulsion. Neumann et al. support the VR sport mapping premise by explicitly describing how a rowing ergometer can be transformed into a virtual boat so that handle pulls are depicted as virtual oar movements through water and greater exertion changes virtual movement through scenery. Lamb supports the mismatch premise: ergometer and on-water rowing are related but upper-limb/oar-related mechanics differ, especially around catch and finish. The thesis inference is that a boat-centric representation can make the scene visually more recognizable as rowing, but may require transforming felt ergometer handle motion into virtual oar motion. Harris et al. can be used as a caution that visual realism in VR does not automatically preserve action-relevant sensory and haptic fidelity, but Harris is not rowing-specific and should not be overused here.}
```

### Final developer note 4

```tex
\sourcechecknote{This paragraph is a thesis synthesis: it argues that neither representation should be treated as the simply "real" one. Lamb supports the premise that ergometer and on-water rowing are related but not identical, with upper-limb and oar-related kinematic differences around catch and finish. Rauter et al. support the rowing-specific action structure that the boat-centric mode tries to depict: rower-boat-oar-water interaction, oar handling, blade-water contact, oar angles, and boat propulsion. Neumann et al. support the VR sport mapping premise that an ergometer can be used as an exertion interface and transformed into a virtual boat/oar action. Harris et al. support the broader caution that visually realistic VR action may still differ from real-world action because of altered depth cues and limited haptic information. The thesis inference is that the ergometer-congruent condition preserves the user's actual device interaction but remains a virtual depiction, while the boat-centric condition preserves recognizable boat/oar rowing imagery but must transform felt handle motion. These sources support the premises, not a direct literature claim that "both modes are artificial" or that either mode is superior.}
```

### Final developer note 5

```tex
\sourcechecknote{This paragraph broadens the rowing case to interactive VR sport without claiming that the thesis solves XR sport design in general. Neumann et al. are the main support: their review defines interactive VR sport through a simulated sport environment and interactivity, discusses exertion interfaces, and gives examples where physical effort on machines such as ergometers is translated into virtual race-course or sport performance. Their rowing example explicitly describes an ergometer being transformed into a virtual boat, with handle pulls depicted as virtual oar movements through water. Kilteni et al. can support the real-movement-correspondence side because agency is linked to synchronous visuomotor correlations and affected by discrepancies between seen feedback and actual movement. Harris et al. can support the action-fidelity caution because visually guided action in VR can differ from real-world action when depth cues and haptic information are altered or absent. The thesis inference is that XR sport systems may choose between close correspondence to real movement and transformation toward the represented activity; this is a design framing, not a formal taxonomy established by the cited sources.}
```

### Final developer note 6

```tex
\sourcechecknote{This paragraph names the thesis' core trade-off. Kilteni et al. support the visuomotor-congruence side: agency is linked to comparisons between predicted and actual sensory consequences and to synchronous visuomotor correlations, while discrepancies between visual feedback and actual movement can reduce agency. Waltemate et al. can support temporal-congruence or responsiveness wording if used, because their full-body avatar study shows that visual feedback delays affect motor performance, perceived simultaneity, agency, and ownership; their specific latency thresholds should not be imported as rowing design requirements. Harris et al. support the distinction between visual realism and action fidelity by warning that VR can alter depth cues and lacks realistic haptic information, so visually guided action in VR may diverge from real-world action. Lamb and Rauter make the trade-off rowing-specific: ergometer and on-water rowing are related but differ in upper-limb/oar mechanics, and ordinary ergometers omit oar handling, blade-water interaction, and other boat/oar action components. The thesis inference is that indoor VR rowing can pursue close correspondence to the real ergometer movement or recognizable sport depiction of boat-and-oar rowing, and these goals can support each other but can also come apart.}
```

## Final SOURCE-CHECK Blocks

### Final SOURCE-CHECK block 1

```tex
% SOURCE-CHECK:
%   key: lamb1989kinematicComparison; soperHume2004rowingTechnique; rauterEtAl2013rowingTransfer
%   md: MD Papers/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_markdown_bundle/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_raw_page_marked.md, lines 20-63; lines 419-500; MD Papers/soper_hume_2004_ideal_rowing_technique_biomechanics_markdown_bundle/soper_hume_2004_ideal_rowing_technique_biomechanics_raw_page_marked.md, lines 79-85; lines 109-123; MD Papers/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_markdown_bundle/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_raw_page_marked.md, lines 149-199; lines 283-320; lines 397-407
%   pdf: Lamb p. 1 and pp. 6-7; Soper/Hume p. 1 and p. 2; Rauter p. 2, p. 3, and p. 4
%   evidence: Ergometer and on-water rowing are related but not identical; common ergometers reproduce parts of body action but not all trunk/upper-limb/oar mechanics; rowing boat action involves rower-boat-oar-water interaction, blades, oar angles, and oarlocks.
%   confidence: verified
%   caution: Supports movement-interface mismatch, not embodiment outcomes.
```

### Final SOURCE-CHECK block 2

```tex
% SOURCE-CHECK:
%   key: kilteniEtAl2012senseEmbodiment; waltemateEtAl2016latency
%   md: MD Papers/kilteni_2012_sense_of_embodiment_markdown_bundle/kilteni_2012_sense_of_embodiment_raw_page_marked.md, lines 338-377; MD Papers/waltemate_2016_latency_perceptual_judgments_motor_performance_vr_markdown_bundle/waltemate_2016_latency_perceptual_judgments_motor_performance_vr_raw_page_marked.md, lines 37-60; lines 520-540
%   pdf: Kilteni pp. 4-5; Waltemate p. 1 and p. 5
%   evidence: Agency is linked to predicted/actual sensory consequences and synchronous visuomotor correlations; delayed full-body avatar feedback affects motor performance, simultaneity, agency, and ownership.
%   confidence: verified
%   caution: Supports congruence relevance, not a claim that the ergometer-congruent mode will necessarily perform better. Waltemate is optional unless temporal congruence/responsiveness is explicit.
```

### Final SOURCE-CHECK block 3

```tex
% SOURCE-CHECK:
%   key: rauterEtAl2013rowingTransfer; neumannEtAl2018interactiveVrSport; lamb1989kinematicComparison; harrisEtAl2019visionForAction
%   md: MD Papers/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_markdown_bundle/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_raw_page_marked.md, lines 149-199; lines 283-320; MD Papers/neumann_2018_interactive_virtual_reality_sport_systematic_review_markdown_bundle/neumann_2018_interactive_virtual_reality_sport_systematic_review_raw_page_marked.md, lines 404-419; MD Papers/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_markdown_bundle/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_raw_page_marked.md, lines 20-63; lines 419-500; MD Papers/harris_2019_virtually_the_same_vr_vision_for_action_markdown_bundle/harris_2019_virtually_the_same_vr_vision_for_action_raw_page_marked.md, lines 34-45; lines 251-286
%   pdf: Rauter p. 2 and p. 3; Neumann p. 12; Lamb p. 1 and pp. 6-7; Harris p. 1 and p. 3
%   evidence: Boat/oar/water action is central to rowing; a rowing ergometer can be transformed into virtual boat/oar action; ergometer and on-water kinematics differ; visually realistic VR action can still differ from real-world action because of sensory/haptic constraints.
%   confidence: verified
%   caution: Supports boat-centric mode rationale and mismatch caution, not a measured claim that boat-centric depiction improves embodiment.
```

### Final SOURCE-CHECK block 4

```tex
% SOURCE-CHECK:
%   key: neumannEtAl2018interactiveVrSport; harrisEtAl2019visionForAction; kilteniEtAl2012senseEmbodiment
%   md: MD Papers/neumann_2018_interactive_virtual_reality_sport_systematic_review_markdown_bundle/neumann_2018_interactive_virtual_reality_sport_systematic_review_raw_page_marked.md, lines 105-123; lines 228-241; lines 404-419; MD Papers/harris_2019_virtually_the_same_vr_vision_for_action_markdown_bundle/harris_2019_virtually_the_same_vr_vision_for_action_raw_page_marked.md, lines 34-45; lines 251-286; MD Papers/kilteni_2012_sense_of_embodiment_markdown_bundle/kilteni_2012_sense_of_embodiment_raw_page_marked.md, lines 338-377
%   pdf: Neumann p. 4, p. 7, and p. 12; Harris p. 1 and p. 3; Kilteni pp. 4-5
%   evidence: Interactive VR sport uses exertion interfaces and action mapping; VR action can differ from real-world action because of sensory/haptic limits; agency is linked to visuomotor correspondence.
%   confidence: verified
%   caution: Supports broader XR sport design framing, not a universal claim about all XR sport systems.
```

### Final SOURCE-CHECK block 5

```tex
% SOURCE-CHECK:
%   key: kilteniEtAl2012senseEmbodiment; harrisEtAl2019visionForAction; lamb1989kinematicComparison; rauterEtAl2013rowingTransfer
%   md: MD Papers/kilteni_2012_sense_of_embodiment_markdown_bundle/kilteni_2012_sense_of_embodiment_raw_page_marked.md, lines 338-377; lines 922-926; MD Papers/harris_2019_virtually_the_same_vr_vision_for_action_markdown_bundle/harris_2019_virtually_the_same_vr_vision_for_action_raw_page_marked.md, lines 34-45; lines 251-286; lines 378-393; MD Papers/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_markdown_bundle/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_raw_page_marked.md, lines 20-63; lines 419-500; MD Papers/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_markdown_bundle/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_raw_page_marked.md, lines 149-199; lines 283-320
%   pdf: Kilteni pp. 4-5 and p. 11; Harris p. 1, p. 3, and p. 4; Lamb p. 1 and pp. 6-7; Rauter p. 2 and p. 3
%   evidence: Visuomotor correspondence matters for agency; visual realism in VR does not guarantee action-fidelity; ergometer and on-water rowing differ in oar/upper-limb mechanics and rowing includes rower-boat-oar-water interaction omitted by ordinary ergometers.
%   confidence: verified
%   caution: Use the combined source set for the rowing-specific "come apart" claim; do not rely only on embodiment sources.
```

## Final Audit Verdict

The Core Design Tension subsection is sourceable and conceptually strong, but it is synthesis-heavy. The safest strategy is:

- Cite rowing mechanics sources for the ergometer/boat mismatch.
- Present both representation modes as thesis-defined.
- Cite Kilteni for visuomotor congruence/agency relevance.
- Use Waltemate only when temporal congruence/responsiveness is explicit.
- Use Harris as a caution that visual realism is not action equivalence.
- Use Neumann for broad VR sport/exertion-interface mapping.
- Avoid turning "boat-centric" or "realistic sport depiction" into validated external constructs unless later operationalized.
