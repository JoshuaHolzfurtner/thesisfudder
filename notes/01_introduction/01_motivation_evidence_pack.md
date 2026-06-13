# Motivation Evidence Pack

Status: deep source-grounding pack for `chapters/01_introduction/01_motivation.tex`. This file audits the current Motivation subsection paragraph by paragraph. It does not rewrite thesis prose, does not edit `.tex`, and does not add or remove citations. It is a working evidence layer for the author and future LLM passes.

Important scope note: `main.tex` currently inputs `chapters/01_introduction`, which points to the merged file `chapters/01_introduction.tex`. The requested target file, `chapters/01_introduction/01_motivation.tex`, exists as the split Motivation subsection and is audited here exactly as requested. Before later patching the thesis, confirm whether the split subsection has again become the active compiled source or whether the merged file still needs the same treatment.

## Files Read

Instruction and framing files:

- `AGENTS.md`
- `notes/chapters/01_introduction_back_of_mind.md`
- `notes/01_introduction/01_motivation_outline.md`
- `notes/01_introduction/dossier_section_1.md`
- `notes/01_introduction/dossier_section_1_verification.md`
- `references.bib`

Target file:

- `chapters/01_introduction/01_motivation.tex`

Relevant source bundles consulted for this subsection:

- `MD Papers/soper_hume_2004_ideal_rowing_technique_biomechanics_markdown_bundle/`
- `MD Papers/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_markdown_bundle/`
- `MD Papers/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_markdown_bundle/`
- `MD Papers/murray_2016_presence_of_others_vr_rowing_exercise_markdown_bundle/`
- `MD Papers/arndt_2018_vr_hmd_rowing_workouts_markdown_bundle/`
- `MD Papers/neumann_2018_interactive_virtual_reality_sport_systematic_review_markdown_bundle/`
- `MD Papers/niehorster_2021_optic_flow_history_markdown_bundle/`
- `MD Papers/palmisano_2015_vection_research_challenges_markdown_bundle/`
- `MD Papers/kooijman_2024_measuring_vection_review_markdown_bundle/`

## Bibliography Key Check

All keys below exist in `references.bib` and may be used in later `.tex` citation passes:

- `soperHume2004rowingTechnique`
- `lamb1989kinematicComparison`
- `rauterEtAl2013rowingTransfer`
- `murrayEtAl2016vrRowingPresence`
- `arndtEtAl2018vrRowingWorkouts`
- `neumannEtAl2018interactiveVrSport`
- `niehorster2021opticFlowHistory`
- `palmisanoEtAl2015vectionChallenges`
- `kooijmanEtAl2024measuringVection`

## Working Citation Labels

This evidence pack follows the AGENTS.md confidence labels:

- `verified`: the source file, evidence passage, line range, and page anchor were checked.
- `likely`: the source appears relevant, but the exact claim relation or wording still needs human review.
- `needs manual check`: the claim or source relationship needs manual verification before being treated as source-backed.

Evidence type labels used here:

- `direct evidence`: the source directly states or demonstrates the relevant premise.
- `contextual support`: the source gives background context but does not directly prove the exact sentence.
- `methodological analogy`: the source is useful because its setup or measurement logic resembles the thesis context.
- `thesis-synthesis premise`: the source supports one premise in an inference authored by the thesis.
- `background only`: the source is useful context but should not carry the citation burden for this paragraph.

# Paragraph 1: Physical Rowing and Ergometer Baseline

## Paragraph 1: Physical Rowing and Ergometer Baseline

### Current paragraph text

Indoor rowing is a physically demanding and technically structured form of exercise. Unlike many stationary fitness activities, rowing involves a coordinated whole-body movement in which legs, trunk, arms, seat, handle, and rhythm are tightly coupled. On a rowing ergometer, this movement is reduced to a land-based training device: the user moves back and forth on a sliding seat and pulls a handle along a mostly linear path. The physical effort can approximate important aspects of rowing training, but the perceptual situation differs strongly from rowing on water. The user remains stationary in a room, the boat is absent, and the characteristic visual and spatial experience of moving through a rowing environment is largely missing.

### Paragraph function

This paragraph establishes the physical baseline for the thesis problem. It has to do four things at once:

- Introduce rowing as an active, coordinated, technically structured exercise rather than a passive or purely visual VR task.
- Establish that ergometer rowing is a legitimate rowing-training context, not an arbitrary indoor exercise.
- Mark the important limitation: ergometer rowing and on-water rowing are related but not identical.
- Prepare the later XR motivation: the physical action remains real, but the on-water perceptual and spatial context is absent.

The paragraph is therefore the thesis' bridge from rowing biomechanics into XR representation design. It should not sound as if the ergometer is a bad or invalid training tool. It should sound as if the ergometer is useful and rowing-like, while still removing boat, oar, water, and self-motion context.

### Claim ledger

#### Claim MOT-P1-C1

- Exact claim: "Indoor rowing is a physically demanding and technically structured form of exercise."
- Claim classification: directly source-backed, with some phrasing from thesis framing.
- Source support needed: rowing biomechanics or rowing simulator/training source showing that rowing involves forceful exercise and structured technique.
- Current support status: verified.
- Best support: `soperHume2004rowingTechnique`; `rauterEtAl2013rowingTransfer`.
- Wording should be narrowed: no major narrowing needed, but avoid adding unverified popularity, health, or market claims.

#### Claim MOT-P1-C2

- Exact claim: "Rowing involves a coordinated whole-body movement in which legs, trunk, arms, seat, handle, and rhythm are tightly coupled."
- Claim classification: directly source-backed for coordinated body sequence; partly thesis synthesis for seat/handle/rhythm coupling in this exact list.
- Source support needed: rowing technique source describing sequential coordination of legs, trunk, and arms; ergometer/on-water kinematic source describing seat and hand/handle movement.
- Current support status: verified for legs/trunk/arms and seat/hand movement; likely for "rhythm" as an introductory wording unless cited to technique/cycle evidence.
- Best support: `rauterEtAl2013rowingTransfer`; `lamb1989kinematicComparison`; supporting `soperHume2004rowingTechnique`.
- Wording should be narrowed: consider "coordinated movement of legs, trunk, and arms, expressed on the ergometer through seat and handle motion" if you want tighter source fidelity.

#### Claim MOT-P1-C3

- Exact claim: "On a rowing ergometer, this movement is reduced to a land-based training device: the user moves back and forth on a sliding seat and pulls a handle along a mostly linear path."
- Claim classification: thesis synthesis plus directly source-backed premises.
- Source support needed: sources showing ergometers are land-based rowing training devices; sources showing seat/hand or handle mechanics; sources showing ergometer differs from oar/boat/water rowing.
- Current support status: likely.
- Best support: `soperHume2004rowingTechnique`; `lamb1989kinematicComparison`; `rauterEtAl2013rowingTransfer`.
- Wording should be narrowed: yes. "Reduced" is rhetorically useful but can sound like a value judgment. "Mostly linear path" is plausible for Concept2-style ergometer handle motion, but the cited sources support central-pulley/handle and seat movement more cleanly than they support that exact geometrical phrase. Safer wording later would be "translated into sliding-seat and handle motion on a stationary machine."

#### Claim MOT-P1-C4

- Exact claim: "The physical effort can approximate important aspects of rowing training, but the perceptual situation differs strongly from rowing on water."
- Claim classification: thesis synthesis from directly source-backed premises.
- Source support needed: evidence that ergometers are used for rowing training/testing and reproduce some physical/physiological aspects; evidence that on-water rowing includes oar/boat/water mechanics not present on ordinary ergometers.
- Current support status: verified for physical/training approximation and mechanical difference; likely for "perceptual situation" unless the claim is kept as thesis framing rather than source-stated fact.
- Best support: `soperHume2004rowingTechnique`; `lamb1989kinematicComparison`; `rauterEtAl2013rowingTransfer`.
- Wording should be narrowed: maybe. "Perceptual situation differs strongly" is defensible as thesis synthesis, but if you want purely sourced wording use "the movement interface and rowing context differ from on-water rowing."

#### Claim MOT-P1-C5

- Exact claim: "The user remains stationary in a room, the boat is absent, and the characteristic visual and spatial experience of moving through a rowing environment is largely missing."
- Claim classification: internal project framing plus thesis synthesis.
- Source support needed: minimal external source support for ergometer stationary context and absence of oar/boat/water; the exact "visual and spatial experience" wording is thesis-authored motivation.
- Current support status: likely.
- Best support: `rauterEtAl2013rowingTransfer`; `neumannEtAl2018interactiveVrSport` later in Paragraph 2 for virtual movement through environments.
- Wording should be narrowed: maybe. Keep this as setup, but avoid presenting it as a measured claim about perception unless sources are added.

### Source cards

#### Source: `soperHume2004rowingTechnique`

- Source role: best for ergometer use and biomechanical caveat; supporting for stroke sequencing.
- What the source is about, in plain language: a sports biomechanics review of "ideal" rowing technique, including on-water and ergometer literature.
- What the source specifically says that matters here: rowing ergometers are commonly used for performance testing, technique coaching, crew selection, and training in poor weather. It also states that common ergometers such as the Concept2 can simulate the physiological profile of 2000 m rowing and reproduce parts of the body action, but do not reproduce trunk and upper-limb movement patterns particularly well because of the central pulley system.
- Which exact part of the paragraph it supports: the claim that indoor/ergometer rowing is a structured training context; the claim that an ergometer approximates important aspects of rowing training; the claim that ergometer rowing does not fully reproduce on-water rowing.
- Why this source is used here instead of a broader/background source: it is rowing-specific and explicitly discusses ergometer use and limitations. It is therefore stronger than a generic exercise or VR sport source for this paragraph.
- What this source does NOT support: it does not support XR embodiment, virtual self-motion, avatar ownership, or the thesis' two-mode mapping comparison. It should not be cited as evidence that one VR representation will feel better than another.
- Evidence type: direct evidence for ergometer use and limitations; thesis-synthesis premise for the design problem.
- Confidence: verified.
- MD path: `MD Papers/soper_hume_2004_ideal_rowing_technique_biomechanics_markdown_bundle/soper_hume_2004_ideal_rowing_technique_biomechanics_raw_page_marked.md`
- MD line range: lines 79-85; lines 109-123; lines 263-267; lines 1072-1138
- PDF page if available: p. 1; p. 2; p. 3; pp. 11-12.

#### Source: `lamb1989kinematicComparison`

- Source role: best for the ergometer/on-water kinematic comparison; supporting for stroke cycle and seat/hand movement.
- What the source is about, in plain language: a kinematic comparison of rowing on a Gjessing ergometer and on water.
- What the source specifically says that matters here: Lamb describes rowing as a stroke cycle and compares body-segment kinematics across ergometer and on-water rowing. The paper finds that most drive-phase variables are similar, especially for legs and trunk, but upper arm and forearm patterns differ, especially around the beginning and end of the stroke. It links part of the difference to on-water oar handling, such as lifting or feathering the oar, which is not exhibited in ergometer rowing.
- Which exact part of the paragraph it supports: the paragraph's "related but not identical" claim; the seat/hand motion basis; the statement that the physical effort can approximate important rowing-training aspects while not reproducing the on-water action context.
- Why this source is used here instead of a broader/background source: it directly compares ergometer and on-water rowing, which is the exact contrast the Motivation paragraph needs.
- What this source does NOT support: it does not support VR, embodiment, perceptual realism, self-motion, or user preference. It should not be used to imply that ergometer rowing is inferior in all respects.
- Evidence type: direct evidence for ergometer/on-water similarity and difference; thesis-synthesis premise for the design problem.
- Confidence: verified.
- MD path: `MD Papers/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_markdown_bundle/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_raw_page_marked.md`
- MD line range: lines 20-63; lines 86-98; lines 381-407; lines 419-500
- PDF page if available: p. 1; p. 6; p. 7.

#### Source: `rauterEtAl2013rowingTransfer`

- Source role: best for tool-, oar-, boat-, water-, and haptic-interaction framing; supporting for whole-body sequential rowing.
- What the source is about, in plain language: a study of a realistic rowing simulator and skill transfer from virtual to real rowing.
- What the source specifically says that matters here: Rauter et al. state that rowing involves continuous haptic interaction between rower, boat, oar, and water. They describe good rowing technique as coordinated dynamic movement and propulsion. They also explain that ordinary indoor ergometers provide resistance through a cable-driven windmill and cannot train oar handling or oar height in water.
- Which exact part of the paragraph it supports: the idea that rowing is not just isolated handle pulling; the whole-body/tool-mediated nature of rowing; the absence of boat/oar/water interaction in ordinary ergometer rowing.
- Why this source is used here instead of a broader/background source: it connects rowing technique to simulator design and explicitly contrasts ordinary ergometers with richer rowing simulators. That makes it a strong source for the thesis' later XR problem.
- What this source does NOT support: it does not evaluate this thesis' prototype or the specific ergometer-congruent versus boat-realistic mapping comparison. It should not be used as direct evidence for embodiment outcomes.
- Evidence type: direct evidence for rowing interaction structure and ordinary ergometer limitations; thesis-synthesis premise for XR representation problem.
- Confidence: verified.
- MD path: `MD Papers/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_markdown_bundle/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_raw_page_marked.md`
- MD line range: lines 149-199; lines 283-302; lines 305-320; lines 707-795; lines 2194-2214
- PDF page if available: p. 2; p. 3; pp. 8-9; p. 16.

### Evidence window

#### `soperHume2004rowingTechnique`

The strongest evidence window is the opening discussion of ergometer use and the later discussion of ergometer limitations. Soper and Hume state that rowing ergometers are used for performance testing, technique coaching, crew selection, and training when weather prevents on-water rowing. This supports the paragraph's baseline that indoor rowing is a legitimate rowing-training context rather than a random stationary exercise. The source also states that common air-braked ergometers can physiologically simulate aspects of 2000 m rowing and reproduce parts of the body action, but that common ergometers do not reproduce trunk and upper-limb movement patterns well compared with on-water rowing because they use a central pulley system.

Representative excerpts:

- "Rowing ergometers are commonly used for performance testing, technique coaching, crew selection and training in poor weather conditions" (raw page-marked MD lines 79-85, PDF p. 1).
- "Although these ergometers reproduce parts of the body action of on-water rowing ... they do not reproduce the trunk and upper-limb patterns particularly well" (raw page-marked MD lines 109-123, PDF p. 2).

This source is strong for the training/approximation side of the paragraph. It is also strong for cautioning that the ergometer is not a full reproduction of on-water rowing. It is not a source for visual or spatial experience.

#### `lamb1989kinematicComparison`

Lamb provides the cleanest support for "ergometer and on-water rowing are related but different." The abstract and discussion state that many drive-phase variables are similar, especially for leg and trunk movement, while upper arm and forearm motion differs significantly. The paper links some of these differences to on-water oar mechanics such as lifting or feathering the oar, which are absent from ergometer rowing. It also gives stroke-cycle language around catch, drive, finish, and recovery.

Representative excerpts:

- "Most of the parameters measured during the drive phase of the stroke cycle were similar" but "upper arm and forearm segments" differed significantly (raw page-marked MD lines 20-63, PDF p. 1).
- "Lifting the oar out of the water and 'feathering' it ... is essential in rowing but is not exhibited in ergometer rowing" (raw page-marked MD lines 453-483, PDF p. 7).

This source supports the paragraph's caution that the ergometer approximates important physical aspects but not the complete on-water movement interface. It does not directly support the paragraph's "perceptual situation" or "visual and spatial experience" language.

#### `rauterEtAl2013rowingTransfer`

Rauter et al. are most useful for explaining what ordinary ergometer rowing removes from the sport action. The source describes rowing as continuous haptic interaction between rower, boat, oar, and water. It emphasizes dynamic coordination and propulsion. It then contrasts this with ordinary indoor ergometers that render resistance through a cable-driven windmill and do not train oar handling or oar height in water. This is the strongest Motivation support for why "the boat is absent" is not just visual decoration; the missing oar-water interaction is part of rowing as a tool-mediated sport action.

Representative excerpts:

- "In rowing, there are continuous haptic forces between the rower, the boat, the oar and the water" (raw page-marked MD lines 149-165, PDF p. 2).
- Ordinary indoor ergometers "render a force that emulates water resistance via a cable driven windmill" and do not train oar handling or oar height in the water (raw page-marked MD lines 180-199, PDF p. 2).

This source is strong for boat/oar/water absence and whole-action structure. It is not direct evidence for subjective embodiment.

### Reasoning bridge

The rowing sources establish the source-backed premises that rowing is coordinated, forceful, and technically structured; that ergometers are standard training and testing devices; and that ergometer rowing is related to but mechanically incomplete relative to on-water rowing. `soperHume2004rowingTechnique` gives the training and biomechanics caveat. `lamb1989kinematicComparison` gives the exact ergometer-versus-on-water comparison. `rauterEtAl2013rowingTransfer` gives the broader rower-boat-oar-water interaction that an ordinary ergometer removes.

The thesis-authored inference is that this creates a useful XR problem: the body is doing real rowing-like effort indoors, but the on-water perceptual and spatial situation is missing. The paragraph may say that the boat, oars, water, and moving environment are absent because that follows from the ordinary ergometer contrast. It should be more careful with "perceptual situation differs strongly" because the cited rowing biomechanics sources primarily establish mechanical and interface differences, not a measured perceptual contrast.

Unsupported or only likely steps are "mostly linear path," "rhythm" as a separately evidenced component, and "visual and spatial experience" if presented as an empirically measured claim. These can stay as introductory thesis framing, but they should not be over-cited as if the biomechanics papers directly measured them.

### Overclaim boundaries

- Do not claim ergometers are poor training devices.
- Do not claim ergometers fail to approximate rowing in all respects.
- Do not claim `lamb1989kinematicComparison` or `soperHume2004rowingTechnique` studied VR.
- Do not claim rowing biomechanics sources prove embodiment, ownership, agency, presence, preference, or cybersickness outcomes.
- Do not claim "mostly linear path" as a precise biomechanical finding unless a source specifically supports it.
- Do not claim "perceptual situation" as a measured perceptual result from the rowing biomechanics papers.
- Do not use this paragraph to imply that boat-realistic VR is necessarily better or more rowing-like for embodiment.

### Suggested citation placement

- Place a citation after the first two sentences if they remain about technical rowing structure and whole-body coordination: cite `soperHume2004rowingTechnique` and `rauterEtAl2013rowingTransfer`.
- Place a citation after the ergometer approximation/difference sentence: cite `lamb1989kinematicComparison` and `soperHume2004rowingTechnique`.
- Use `rauterEtAl2013rowingTransfer` near the missing boat/oar/water action context, especially if the paragraph keeps "boat is absent" and later connects that to design.
- Citation density should be moderate. A single citation group near the middle/end of the paragraph may be enough if the paragraph is not split. If the paragraph is split into two paragraphs later, use one group for rowing/ergometer mechanics and one group for missing oar-water/boat context.

Suggested citation group:

```tex
\parencite{soperHume2004rowingTechnique,lamb1989kinematicComparison,rauterEtAl2013rowingTransfer}
```

Alternative if preserving a lighter first paragraph:

```tex
\parencite{soperHume2004rowingTechnique,lamb1989kinematicComparison}
```

with `rauterEtAl2013rowingTransfer` saved for Paragraph 3 or 4 where the missing boat/oar/water interaction becomes the actual design problem.

### Suggested developer note

```tex
\sourcechecknote{The Motivation opens from rowing and ergometer mechanics, not from VR theory. Soper and Hume support treating ergometer rowing as a normal rowing training and testing context while also warning that common ergometers reproduce only parts of on-water body action, especially less well for trunk and upper-limb patterns. Lamb gives the direct ergometer-versus-on-water kinematic comparison: leg and trunk movement are broadly similar in many drive-phase variables, but upper arm and forearm motion differ, especially around catch and finish, partly because on-water rowing includes oar handling such as lifting and feathering that is absent on the ergometer. Rauter et al. support the broader sport-action premise that rowing involves coordinated rower, boat, oar, and water interaction, whereas ordinary indoor ergometers replace this with cable-driven resistance and do not train oar handling or oar height in water. The thesis inference is that indoor rowing keeps real forceful rowing-like effort while removing boat, oar, water, and moving-environment context. These sources do not by themselves support embodiment outcomes, user preference, or any claim that ergometers are poor training devices.}
```

### Suggested SOURCE-CHECK comments

```tex
% SOURCE-CHECK:
%   key: soperHume2004rowingTechnique
%   md: MD Papers/soper_hume_2004_ideal_rowing_technique_biomechanics_markdown_bundle/soper_hume_2004_ideal_rowing_technique_biomechanics_raw_page_marked.md, lines 79-85; lines 109-123
%   pdf: p. 1; p. 2
%   evidence: Rowing ergometers are commonly used for performance testing, technique coaching, crew selection, and poor-weather training; common ergometers reproduce parts of body action but do not reproduce trunk and upper-limb patterns particularly well compared with on-water rowing.
%   confidence: verified
%   caution: Supports ergometer use and biomechanical caveat, not VR embodiment or preference.
%
% SOURCE-CHECK:
%   key: lamb1989kinematicComparison
%   md: MD Papers/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_markdown_bundle/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_raw_page_marked.md, lines 20-63; lines 419-500
%   pdf: p. 1; pp. 6-7
%   evidence: Ergometer and on-water rowing share many drive-phase variables, especially legs and trunk, but upper arm and forearm patterns differ around catch and finish; lifting/feathering the oar is part of on-water rowing but not ergometer rowing.
%   confidence: verified
%   caution: Supports related-but-not-identical mechanics, not visual self-motion or embodiment outcomes.
%
% SOURCE-CHECK:
%   key: rauterEtAl2013rowingTransfer
%   md: MD Papers/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_markdown_bundle/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_raw_page_marked.md, lines 149-199; lines 283-302
%   pdf: p. 2; p. 3
%   evidence: Rowing involves continuous haptic interaction among rower, boat, oar, and water and a coordinated legs-trunk-arms drive; ordinary indoor ergometers provide cable-driven resistance and do not train oar handling or oar height in water.
%   confidence: verified
%   caution: Strong for missing oar/boat/water interaction, but do not treat simulator transfer findings as evidence for this thesis' embodiment outcomes.
```

### Paragraph verdict

Needs narrower paragraph wording before a final prose patch.

The paragraph is conceptually strong and sourceable, but the safest later prose pass should narrow or clarify:

- "reduced to a land-based training device"
- "mostly linear path"
- "perceptual situation differs strongly"
- "characteristic visual and spatial experience"

These phrases can remain in draft mode, but the source-backed version should separate measured mechanics from thesis-authored experiential framing.

# Paragraph 2: VR as Experiential Context Restoration

## Paragraph 2: VR as Experiential Context Restoration

### Current paragraph text

Virtual reality offers an opportunity to reintroduce some of this missing experiential context. A virtual rowing system can place the user in a boat, on a river, or in a training environment that visually resembles the sport more closely than an ergometer display can. Such a system can add optic flow, spatial sound, avatar representation, opponents, teammates, and environmental feedback. In stationary exercise contexts, this visual motion through a virtual environment can also contribute to an impression of self-motion, even when the user's physical body remains in place.

### Paragraph function

This paragraph shifts the Motivation from rowing mechanics to XR/VR opportunity. Its job is not yet to define the thesis' two representation modes. Instead, it establishes why VR is relevant at all:

- VR can visually reintroduce context that the ergometer removes.
- Prior VR rowing and VR sport systems already use environments, avatars, exertion interfaces, virtual boats, and virtual movement.
- Visual motion through a virtual environment can support an impression of self-motion, but this must be phrased cautiously because the thesis does not necessarily measure vection.

This paragraph should be kept broad enough to motivate VR rowing, but not so broad that every possible VR feature is treated as equally sourced. "Spatial sound" is the weakest feature in the current list if it is presented as generic VR rowing capability. Rauter supports a soundscape in a specific CAVE rowing simulator, not a general claim that VR rowing systems usually include spatial sound.

### Claim ledger

#### Claim MOT-P2-C1

- Exact claim: "Virtual reality offers an opportunity to reintroduce some of this missing experiential context."
- Claim classification: thesis synthesis from directly source-backed premises.
- Source support needed: VR sport/exercise or VR rowing systems showing virtual rowing environments, boats, scenery, avatars, exertion-driven movement, or similar context restoration.
- Current support status: verified.
- Best support: `murrayEtAl2016vrRowingPresence`; `arndtEtAl2018vrRowingWorkouts`; `neumannEtAl2018interactiveVrSport`.
- Wording should be narrowed: no, if "some" remains. Avoid "fully reintroduce."

#### Claim MOT-P2-C2

- Exact claim: "A virtual rowing system can place the user in a boat, on a river, or in a training environment that visually resembles the sport more closely than an ergometer display can."
- Claim classification: directly source-backed for virtual boat/river/training environment; thesis synthesis for comparison with ordinary ergometer display.
- Source support needed: prior VR rowing examples with river, boat, scull, lake, avatar, projected or HMD environment.
- Current support status: verified.
- Best support: `murrayEtAl2016vrRowingPresence`; `arndtEtAl2018vrRowingWorkouts`; contextual `neumannEtAl2018interactiveVrSport`.
- Wording should be narrowed: "can" is appropriate. Avoid implying every VR rowing system places the user in a first-person boat; Murray uses a third-person avatar from behind in a projected environment, while Arndt uses HMD rowing on a lake with a scull.

#### Claim MOT-P2-C3

- Exact claim: "Such a system can add optic flow, spatial sound, avatar representation, opponents, teammates, and environmental feedback."
- Claim classification: mixed direct evidence, contextual support, and weak/optional claims.
- Source support needed: system descriptions or VR sport review showing these features.
- Current support status: verified for avatar representation and environmental movement/feedback; likely for opponents/teammates as broad social context; needs manual check or narrowing for "spatial sound" unless restricted to Rauter's simulator.
- Best support: `murrayEtAl2016vrRowingPresence`; `arndtEtAl2018vrRowingWorkouts`; `neumannEtAl2018interactiveVrSport`; `rauterEtAl2013rowingTransfer` for soundscape in one simulator; `niehorster2021opticFlowHistory` for optic-flow definition.
- Wording should be narrowed: yes. Consider "can add visual motion cues, avatar representation, social or competitive context, and environmental feedback." Keep "spatial sound" only if linked to Rauter as one simulator feature, not as a general VR rowing feature.

#### Claim MOT-P2-C4

- Exact claim: "In stationary exercise contexts, this visual motion through a virtual environment can also contribute to an impression of self-motion, even when the user's physical body remains in place."
- Claim classification: directly source-backed for optic flow and vection/self-motion definitions; thesis synthesis for applying it to stationary VR rowing.
- Source support needed: optic-flow definition; vection definition; optionally VR exercise source showing movement through environment from stationary exercise equipment.
- Current support status: verified if phrased as "can contribute to an impression" rather than "produces vection."
- Best support: `niehorster2021opticFlowHistory`; `palmisanoEtAl2015vectionChallenges`; optional `kooijmanEtAl2024measuringVection`; contextual `murrayEtAl2016vrRowingPresence` or `neumannEtAl2018interactiveVrSport`.
- Wording should be narrowed: yes if "self-motion" becomes theoretically loaded. Use "impression of self-motion" or "visual self-motion cues"; do not claim vection was measured unless the study actually measures it.

### Source cards

#### Source: `murrayEtAl2016vrRowingPresence`

- Source role: best for prior VR rowing with ergometer, avatar, river environment, passing scenery, social/companion context, and enjoyment/performance context.
- What the source is about, in plain language: an experimental study of ergometer rowing in non-VR, individual VR, and companion VR conditions, using a virtual rowing environment and avatar/companion setup.
- What the source specifically says that matters here: participants rowed on a Concept2 ergometer while viewing a virtual rowing environment. The setup used a third-person rowing avatar from behind, an individual or companion boat condition, a river course with turns, and passing scenery. The paper also states generally that VR exercise applications can let physical exertion on equipment move the individual through a virtual environment.
- Which exact part of the paragraph it supports: virtual rowing environment; avatar representation; river/scenery; companion/social context; exertion-driven movement through a virtual environment.
- Why this source is used here instead of a broader/background source: it is directly about VR rowing on an ergometer, so it is closer to the thesis than a generic VR exercise paper.
- What this source does NOT support: it does not study the thesis' two representation strategies, does not measure embodiment as ownership/agency/self-location, and does not directly support "spatial sound."
- Evidence type: direct evidence for prior VR rowing environment and social/companion context; contextual support for VR exercise motivation.
- Confidence: verified.
- MD path: `MD Papers/murray_2016_presence_of_others_vr_rowing_exercise_markdown_bundle/murray_2016_presence_of_others_vr_rowing_exercise_raw_page_marked.md`
- MD line range: lines 42-55; lines 76-99; lines 188-216; lines 266-286; lines 771-785
- PDF page if available: p. 1; p. 2; p. 3; p. 6.

#### Source: `arndtEtAl2018vrRowingWorkouts`

- Source role: best for HMD VR indoor rowing with sensors, virtual lake/scull, force-coupled movement, and environment feedback.
- What the source is about, in plain language: a VR indoor rowing workout prototype that maps ergometer sensor data into a Unity virtual lake/scull environment viewed through an HMD.
- What the source specifically says that matters here: the system uses a stationary rowing machine, sensors for handle/sledge movement and performance metrics, a virtual lake with a scull, and game-object interpolation based on ergometer parameters. The VR condition included steady movement on a lake depending on force applied to the oars.
- Which exact part of the paragraph it supports: virtual boat/lake context; HMD rowing system; environmental feedback; sensor-derived movement.
- Why this source is used here instead of a broader/background source: it is a concrete HMD indoor-rowing example and is therefore more directly relevant than a general VR sport review.
- What this source does NOT support: its subjective feedback is limited and should not be generalized; it does not prove that the thesis' representation comparison affects embodiment; it does not strongly support teammates/opponents except as possible requested future features.
- Evidence type: direct evidence for VR rowing prototype features; contextual support for VR rowing motivation.
- Confidence: verified.
- MD path: `MD Papers/arndt_2018_vr_hmd_rowing_workouts_markdown_bundle/arndt_2018_vr_hmd_rowing_workouts_raw_page_marked.md`
- MD line range: lines 47-57; lines 175-190; lines 219-253; lines 305-350; lines 600-608; lines 1074-1084
- PDF page if available: p. 1; p. 2; p. 3; p. 4; p. 6.

#### Source: `neumannEtAl2018interactiveVrSport`

- Source role: best for broad VR sport/exercise framing and exertion-interface logic; supporting for rowing as an example.
- What the source is about, in plain language: a systematic review of interactive VR sport, including definitions and factors such as immersion, feedback, presence of others, competitiveness, and exertion interfaces.
- What the source specifically says that matters here: VR sport is defined as a computer-simulated sport environment with presence and interactivity. A sport-relevant exertion interface lets physical effort translate into virtual sport performance. The review explicitly uses rowing ergometer pulls being depicted as virtual oar movement and greater exertion creating faster movement through water and scenery.
- Which exact part of the paragraph it supports: VR sport context; physical exertion moving the user through a virtual environment; rowing ergometer-to-virtual-boat/oar example; social/competitive factors at a general level.
- Why this source is used here instead of only Murray/Arndt: Murray and Arndt are examples; Neumann supplies the broader review-level framing that these are instances of interactive VR sport.
- What this source does NOT support: it does not prove the exact thesis gap; it does not prove that adding features improves embodiment; it does not replace concrete system citations for specific rowing examples.
- Evidence type: contextual support and direct evidence for VR sport definitions and exertion-interface examples.
- Confidence: verified.
- MD path: `MD Papers/neumann_2018_interactive_virtual_reality_sport_systematic_review_markdown_bundle/neumann_2018_interactive_virtual_reality_sport_systematic_review_raw_page_marked.md`
- MD line range: lines 73-88; lines 105-123; lines 228-241; lines 304-337; lines 404-419; lines 783-792
- PDF page if available: p. 3; p. 4; p. 7; pp. 9-10; p. 12; p. 22.

#### Source: `niehorster2021opticFlowHistory`

- Source role: best for defining optic flow as visual motion linked to self-motion.
- What the source is about, in plain language: a review/history of optic flow research.
- What the source specifically says that matters here: optic flow is the global pattern of visual motion caused by and signaling self-motion. It can provide information about direction of self-motion and guide movement/posture.
- Which exact part of the paragraph it supports: "optic flow" and the idea that visual motion through an environment can signal self-motion.
- Why this source is used here instead of a vection source alone: optic flow and vection are related but not identical. This source supports the visual-motion cue language without forcing the paragraph to claim subjective vection.
- What this source does NOT support: it does not prove vection occurs in the thesis prototype; it does not prove embodiment, ownership, agency, or preference effects.
- Evidence type: direct evidence for optic-flow definition; background for visual self-motion cue wording.
- Confidence: verified.
- MD path: `MD Papers/niehorster_2021_optic_flow_history_markdown_bundle/niehorster_2021_optic_flow_history_raw_page_marked.md`
- MD line range: lines 28-34; lines 41-52; lines 70-79
- PDF page if available: p. 1; p. 2.

#### Source: `palmisanoEtAl2015vectionChallenges`

- Source role: best for cautious vection/self-motion definition and measurement caution.
- What the source is about, in plain language: a paper about challenges in vection research, including definition and measurement issues.
- What the source specifically says that matters here: vection often refers to visual illusions of self-motion in stationary observers, with the conscious subjective experience of self-motion as the common thread. The paper emphasizes that vection is subjective and measurement is not trivial.
- Which exact part of the paragraph it supports: the "impression of self-motion" sentence, if the paragraph needs vection-grounded support.
- Why this source is used here instead of only optic flow: optic flow defines the visual motion pattern; Palmisano supports the subjective self-motion concept in stationary observers.
- What this source does NOT support: it does not say that every optic-flow display produces vection; it does not say that vection was measured in this thesis; it does not support rowing-specific claims.
- Evidence type: direct evidence for vection definition and caution; background only for the Motivation unless vection remains explicit.
- Confidence: verified.
- MD path: `MD Papers/palmisano_2015_vection_research_challenges_markdown_bundle/palmisano_2015_vection_research_challenges_raw_page_marked.md`
- MD line range: lines 45-54; lines 96-104; lines 290-308; lines 899-904
- PDF page if available: p. 1; p. 3; p. 9.

#### Source: `kooijmanEtAl2024measuringVection`

- Source role: optional support for vection definition and measurement caution.
- What the source is about, in plain language: a review of methods for measuring vection.
- What the source specifically says that matters here: vection is subjective self-motion in the absence of actual physical motion. The review organizes subjective measures and warns that indirect measures do not directly measure vection.
- Which exact part of the paragraph it supports: only the self-motion/vection wording if kept.
- Why this source is used here instead of Palmisano: it is newer and measurement-focused, useful later for Chapter 4 if vection/self-motion is measured or explicitly avoided.
- What this source does NOT support: it does not support rowing, VR exercise, avatar representation, or the two-mode mapping comparison.
- Evidence type: background only in Chapter 1; direct evidence if Chapter 4 discusses vection measurement.
- Confidence: verified.
- MD path: `MD Papers/kooijman_2024_measuring_vection_review_markdown_bundle/kooijman_2024_measuring_vection_review_raw_page_marked.md`
- MD line range: lines 32-53; lines 207-260; lines 1184-1210
- PDF page if available: p. 1; p. 3; p. 12.

#### Source: `rauterEtAl2013rowingTransfer`

- Source role: weak/conditional for Paragraph 2; best only if "spatial sound" stays as a simulator feature.
- What the source is about, in plain language: a realistic rowing simulator study.
- What the source specifically says that matters here: the simulator used a CAVE, a sound wave field synthesis system with many speakers and subwoofers, and visible/audible oar-water interaction to propel a virtual boat.
- Which exact part of the paragraph it supports: spatial sound/soundscape, but only for one rowing simulator, not generic VR rowing.
- Why this source is used here instead of Murray/Arndt: Murray and Arndt are stronger for VR rowing environment and avatar/boat context; Rauter is stronger only for sound and haptic oar-water simulator realism.
- What this source does NOT support: it does not support HMD consumer VR rowing in general; it does not show that spatial sound is typical or necessary; it does not prove embodiment outcomes.
- Evidence type: direct evidence for one simulator's auditory feedback; background only for the general list.
- Confidence: likely for this paragraph because the exact phrase "spatial sound" is broader than the source's specific simulator soundscape.
- MD path: `MD Papers/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_markdown_bundle/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_raw_page_marked.md`
- MD line range: lines 305-320
- PDF page if available: p. 3.

### Evidence window

#### `murrayEtAl2016vrRowingPresence`

Murray et al. directly support the idea that VR rowing can add a virtual rowing environment and social/companion context to ergometer exercise. The study used a Concept2 ergometer and a projected virtual environment. Participants viewed a third-person rowing avatar from behind. The avatar's stroke timing matched the ergometer. The virtual course was a river with turns and passing scenery, and the companion condition placed a second boat in the environment. The paper also frames VR exercise applications as systems where physical exertion on equipment can move a person through a virtual environment.

Representative excerpts:

- "physical exertion on exercise equipment allows the individual to move through a virtual environment" (raw page-marked MD lines 76-99, PDF p. 1).
- Participants saw "a third person avatar from behind, with the timing of the avatar stroke matching the participants' ergometer stroke" and rowed through a river environment with scenery (raw page-marked MD lines 266-286, PDF p. 3).

This source is strong for virtual environment, avatar, river/scenery, and companion context. It is not strong for embodiment as ownership/agency and does not support spatial sound.

#### `arndtEtAl2018vrRowingWorkouts`

Arndt et al. directly support HMD-based indoor rowing where ergometer sensor data drive virtual environment feedback. The source describes a stationary rowing machine, movement data from sensors, a Unity virtual lake, a red scull, HMD display, and steady movement on the lake depending on the force applied to the oars. It is therefore a strong source for "a virtual rowing system can place the user in a boat/lake-like environment" and for environmental feedback.

Representative excerpts:

- The system lets an athlete row on a stationary rowing machine "into a virtual environment" using sensor-derived movement data and HMD output (raw page-marked MD lines 47-57, PDF p. 1).
- The virtual condition includes a lake, mountains, scull, and movement depending on force applied to the oars (raw page-marked MD lines 219-253, PDF p. 2).

This source also warns against overclaiming: participants reported less control in VR despite enjoying it more. That is useful later because it prevents assuming that visual context automatically improves every experience dimension.

#### `neumannEtAl2018interactiveVrSport`

Neumann et al. supply the review-level frame: VR sport is a computer-simulated sport environment with interactivity, where the environment responds to the athlete. The review explicitly mentions physical effort on an ergometer being related to speed through a virtual race course. It also gives a rowing example where handle pulls can be depicted as virtual oar movement and greater exertion produces faster movement through water and passing scenery.

Representative excerpts:

- VR sport includes a simulated sport environment and interactivity, where events move or change in response to the athlete (raw page-marked MD lines 228-241, PDF p. 7).
- In rowing, pulls on the ergometer handle can be depicted as movements of virtual oars, and higher exertion can cause faster movement through water and scenery (raw page-marked MD lines 404-419, PDF p. 12).

This source supports the paragraph's general VR sport/exercise logic but should not be used as evidence that the exact mapping comparison has already been studied.

#### `niehorster2021opticFlowHistory`

Niehorster supports the optic-flow part of the paragraph without forcing a vection claim. The source defines optic flow as the global pattern of visual motion caused by and signaling self-motion. It also describes how such visual motion can indicate direction of self-motion and support visual guidance. This is enough for "visual motion cues" or "optic flow can signal self-motion." It is not enough for "the participant experiences vection" unless paired with vection literature and measured carefully.

Representative excerpt:

- Optic flow is "the global pattern of visual motion that is both caused by and signals self-motion" (raw page-marked MD lines 28-34, PDF p. 1).

#### `palmisanoEtAl2015vectionChallenges`

Palmisano et al. support cautious self-motion wording. The source says vection is often used for visual illusions of self-motion in stationary observers and that the conscious subjective experience of self-motion is the common thread. It also emphasizes that vection is subjective and methodologically difficult to measure. Therefore it supports "impression of self-motion" but also argues against claiming measured vection unless the thesis actually measures it.

Representative excerpts:

- Vection is often used for "visual illusions of self-motion in stationary observers" (raw page-marked MD lines 45-54, PDF p. 1).
- Subjective experience of self-motion is central, and objective or auxiliary indicators should not replace self-report (raw page-marked MD lines 899-904, PDF p. 9).

#### `kooijmanEtAl2024measuringVection`

Kooijman et al. are optional here. They define vection as subjective self-motion in the absence of actual physical motion and review subjective measurement categories. The source is valuable if later Chapter 4 explicitly measures vection, but for this Motivation paragraph it may be more citation weight than needed. It can be cited if the author wants newer measurement-oriented support for the self-motion sentence.

Representative excerpt:

- Vection is "the subjective experience of self-motion in the absence of actual physical motion" (raw page-marked MD lines 43-53, PDF p. 1).

#### `rauterEtAl2013rowingTransfer`

Rauter only belongs in this paragraph if "spatial sound" remains in the list. The simulator used a CAVE and sound wave field synthesis with many speakers and subwoofers. Participants could hear and see the oar-water interaction propelling the virtual boat. This is a strong source for one simulator's auditory realism, but it is not a broad source for VR rowing systems in general.

Representative excerpt:

- The simulator used a realistic soundscape and allowed participants to hear and see oar-water interaction propelling a virtual boat (raw page-marked MD lines 305-320, PDF p. 3).

### Reasoning bridge

The VR rowing sources establish that prior systems already use virtual rowing environments, avatars, boats/sculls, rivers/lakes, passing scenery, and sensor- or exertion-coupled virtual movement. `murrayEtAl2016vrRowingPresence` is the clearest source for projected VR rowing, avatar timing, river scenery, and a companion boat. `arndtEtAl2018vrRowingWorkouts` is the clearest source for HMD indoor rowing with ergometer sensor data and a virtual lake/scull. `neumannEtAl2018interactiveVrSport` provides the general VR sport and exertion-interface framing and explicitly gives rowing as an example.

The self-motion sentence requires a different source family. `niehorster2021opticFlowHistory` supports optic flow as visual motion that signals self-motion. `palmisanoEtAl2015vectionChallenges` and optionally `kooijmanEtAl2024measuringVection` support the subjective self-motion concept in stationary observers. The thesis inference is that visual motion in a stationary VR rowing environment can contribute to an impression of self-motion. This should remain carefully phrased as an impression or cue, not a measured vection outcome.

The only weak part of the list is "spatial sound." Rauter supports realistic soundscape in a CAVE simulator, but Murray and Arndt do not support spatial sound as a general VR rowing feature in the lines checked. If the sentence stays broad, it should say "can include features such as..." and either remove spatial sound or cite Rauter very specifically.

### Overclaim boundaries

- Do not claim VR fully restores on-water rowing.
- Do not claim VR rowing systems already studied the thesis' exact ergometer-congruent versus boat-realistic comparison.
- Do not claim visual motion automatically produces vection.
- Do not claim vection was measured if the study only measures embodiment, realism, comfort, and preference.
- Do not cite `niehorster2021opticFlowHistory` as evidence for ownership, agency, presence, or preference.
- Do not cite `palmisanoEtAl2015vectionChallenges` or `kooijmanEtAl2024measuringVection` as rowing or VR sport sources.
- Do not present "spatial sound" as a common VR rowing feature unless more sources are added.
- Do not treat Murray's companion/avatar setup as evidence that teammates/opponents are central to this thesis unless the thesis actually includes them.

### Suggested citation placement

- After the first two sentences about VR reintroducing rowing context, cite `murrayEtAl2016vrRowingPresence`, `arndtEtAl2018vrRowingWorkouts`, and `neumannEtAl2018interactiveVrSport`.
- After the feature list, avoid a giant citation group if possible. If the list stays, either trim it or split it:
  - environment/avatar/social/feedback: `murrayEtAl2016vrRowingPresence`, `arndtEtAl2018vrRowingWorkouts`, `neumannEtAl2018interactiveVrSport`
  - optic flow/self-motion: `niehorster2021opticFlowHistory`, optionally `palmisanoEtAl2015vectionChallenges`
  - spatial sound: only `rauterEtAl2013rowingTransfer`, and only if framed as one simulator example.
- For the final self-motion sentence, cite `niehorster2021opticFlowHistory` and `palmisanoEtAl2015vectionChallenges`. Use `kooijmanEtAl2024measuringVection` only if you want newer measurement-review support or if Chapter 4 later uses vection terminology.

Suggested citation groups:

```tex
\parencite{murrayEtAl2016vrRowingPresence,arndtEtAl2018vrRowingWorkouts,neumannEtAl2018interactiveVrSport}
```

and for self-motion:

```tex
\parencite{niehorster2021opticFlowHistory,palmisanoEtAl2015vectionChallenges}
```

Optional if vection measurement language becomes explicit:

```tex
\parencite{kooijmanEtAl2024measuringVection}
```

### Suggested developer note

```tex
\sourcechecknote{This paragraph uses prior VR rowing and VR sport work only to motivate what virtual environments can add to ergometer rowing. Murray et al. support a Concept2 rowing setup with a projected virtual river, a third-person rowing avatar whose stroke timing matched the ergometer, passing scenery, and an individual or companion boat condition. Arndt et al. support an HMD rowing prototype in which ergometer sensor data drove a virtual lake/scull environment and virtual movement depended on rowing force. Neumann et al. provide the broader interactive VR sport frame and explicitly describe how rowing ergometer pulls can be represented as virtual oar movement and faster movement through water and scenery. The self-motion wording is supported separately: Niehorster defines optic flow as global visual motion that signals self-motion, while Palmisano et al. define vection as subjective self-motion in stationary observers and caution that it is a subjective phenomenon. The thesis inference is that visual motion in a stationary VR rowing context can contribute to an impression of self-motion. This should not be overstated as measured vection, embodiment, or proof that visual rowing context improves agency or ownership. Spatial sound is only specifically supported by Rauter et al.'s CAVE simulator soundscape and should not be treated as a generic VR rowing feature without additional evidence.}
```

### Suggested SOURCE-CHECK comments

```tex
% SOURCE-CHECK:
%   key: murrayEtAl2016vrRowingPresence
%   md: MD Papers/murray_2016_presence_of_others_vr_rowing_exercise_markdown_bundle/murray_2016_presence_of_others_vr_rowing_exercise_raw_page_marked.md, lines 76-99; lines 266-286
%   pdf: p. 1; p. 3
%   evidence: VR exercise can let physical exertion on equipment move a person through a virtual environment; the rowing setup used a Concept2 ergometer, virtual river/scenery, third-person rowing avatar with stroke timing matched to the ergometer, and individual/companion boat conditions.
%   confidence: verified
%   caution: Supports VR rowing context and companion/avatar setup, not this thesis' embodiment mapping comparison.
%
% SOURCE-CHECK:
%   key: arndtEtAl2018vrRowingWorkouts
%   md: MD Papers/arndt_2018_vr_hmd_rowing_workouts_markdown_bundle/arndt_2018_vr_hmd_rowing_workouts_raw_page_marked.md, lines 47-57; lines 175-190; lines 219-253
%   pdf: p. 1; p. 2
%   evidence: HMD indoor-rowing prototype used stationary rowing machine sensors to capture handle/sledge and performance data, then displayed a virtual lake/scull environment with movement depending on rowing force.
%   confidence: verified
%   caution: Useful as an HMD rowing example; do not generalize its informal feedback as evidence for this thesis' outcomes.
%
% SOURCE-CHECK:
%   key: neumannEtAl2018interactiveVrSport
%   md: MD Papers/neumann_2018_interactive_virtual_reality_sport_systematic_review_markdown_bundle/neumann_2018_interactive_virtual_reality_sport_systematic_review_raw_page_marked.md, lines 228-241; lines 404-419
%   pdf: p. 7; p. 12
%   evidence: VR sport is a computer-simulated sport environment with interactivity; rowing ergometer handle pulls can be depicted as virtual oar movements and greater exertion can produce faster movement through virtual water and scenery.
%   confidence: verified
%   caution: Broad VR sport framing, not proof that the exact thesis comparison has been studied.
%
% SOURCE-CHECK:
%   key: niehorster2021opticFlowHistory
%   md: MD Papers/niehorster_2021_optic_flow_history_markdown_bundle/niehorster_2021_optic_flow_history_raw_page_marked.md, lines 28-34; lines 70-79
%   pdf: p. 1; p. 2
%   evidence: Optic flow is the global pattern of visual motion caused by and signaling self-motion and can provide information for direction of self-motion and visual guidance.
%   confidence: verified
%   caution: Supports visual self-motion cue language, not vection measurement or embodiment outcomes.
%
% SOURCE-CHECK:
%   key: palmisanoEtAl2015vectionChallenges
%   md: MD Papers/palmisano_2015_vection_research_challenges_markdown_bundle/palmisano_2015_vection_research_challenges_raw_page_marked.md, lines 45-54; lines 899-904
%   pdf: p. 1; p. 9
%   evidence: Vection is often used for visual illusions of self-motion in stationary observers; subjective experience of self-motion is central and measurement is methodologically cautious.
%   confidence: verified
%   caution: Use only for cautious self-motion/vection wording; do not claim vection was measured unless the study measures it.
%
% SOURCE-CHECK:
%   key: rauterEtAl2013rowingTransfer
%   md: MD Papers/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_markdown_bundle/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_raw_page_marked.md, lines 305-320
%   pdf: p. 3
%   evidence: A realistic rowing simulator used a CAVE and sound wave field synthesis to provide a realistic soundscape and audible/visible oar-water interaction.
%   confidence: likely
%   caution: Supports spatial sound only as a feature of this specific simulator; weak support for a broad generic VR rowing feature list.
```

### Paragraph verdict

Needs narrower paragraph wording before a final prose patch.

The paragraph is useful and mostly sourceable. The main corrections for a later prose pass are:

- Reduce the broad feature list or split it into sourced feature families.
- Treat "spatial sound" as optional or Rauter-specific.
- Keep "impression of self-motion" cautious and avoid claiming vection unless measured.
- Avoid implying prior VR rowing work already studied the thesis' mapping comparison.

# Paragraph 3: VR Restores the Visual Scene but Not the Physical Interface

## Paragraph 3: VR Restores the Visual Scene but Not the Physical Interface

### Current paragraph text

However, this opportunity also introduces a design problem. The ergometer makes rowing available indoors by replacing the boat and oars with a machine. Virtual reality can visually restore the boat, oars, water, and motion through space, but it cannot remove the fact that the user is still physically rowing on an ergometer. The system must therefore decide how the real movement should become a virtual rowing action.

### Paragraph function

This paragraph states the core Motivation synthesis. It turns the previous two paragraphs into the thesis' design problem:

- The ergometer enables indoor rowing by replacing the boat/oar/water interface.
- VR can visually reintroduce that missing scene.
- The physical interface remains the ergometer.
- Therefore, the prototype must choose how real ergometer movement is mapped into virtual rowing action.

This is the first place where the Introduction should make action congruence visible. The key idea is not only "rowing realism" versus "movement match." It is that the virtual action should appear to be caused by, and meaningfully coupled to, the participant's real rowing effort.

### Claim ledger

#### Claim MOT-P3-C1

- Exact claim: "This opportunity also introduces a design problem."
- Claim classification: thesis synthesis.
- Source support needed: no source directly states this thesis design problem; sources need only support the premises.
- Current support status: verified as thesis synthesis from checked premises.
- Best support: premises from `soperHume2004rowingTechnique`, `lamb1989kinematicComparison`, `rauterEtAl2013rowingTransfer`, `murrayEtAl2016vrRowingPresence`, `arndtEtAl2018vrRowingWorkouts`, `neumannEtAl2018interactiveVrSport`.
- Wording should be narrowed: no. This is the thesis' own framing.

#### Claim MOT-P3-C2

- Exact claim: "The ergometer makes rowing available indoors by replacing the boat and oars with a machine."
- Claim classification: directly source-backed premise plus thesis phrasing.
- Source support needed: ergometer training/use source; ordinary ergometer limitations compared with oar/boat/water rowing.
- Current support status: verified.
- Best support: `soperHume2004rowingTechnique`; `rauterEtAl2013rowingTransfer`; supporting `lamb1989kinematicComparison`.
- Wording should be narrowed: no, but "replacing" should be read functionally, not as a historical claim about why ergometers were invented.

#### Claim MOT-P3-C3

- Exact claim: "Virtual reality can visually restore the boat, oars, water, and motion through space."
- Claim classification: directly source-backed for prior systems; thesis synthesis for "restore."
- Source support needed: VR rowing systems with virtual boat/scull/river/lake/scenery and exertion-coupled virtual movement; simulator source with oars/water if needed.
- Current support status: verified.
- Best support: `murrayEtAl2016vrRowingPresence`; `arndtEtAl2018vrRowingWorkouts`; `neumannEtAl2018interactiveVrSport`; optional `rauterEtAl2013rowingTransfer`.
- Wording should be narrowed: maybe. "Visually restore" is acceptable if it means represent in VR, not recreate physically or haptically.

#### Claim MOT-P3-C4

- Exact claim: "VR cannot remove the fact that the user is still physically rowing on an ergometer."
- Claim classification: internal project framing and physical setup premise.
- Source support needed: minimal; the thesis prototype and cited VR rowing sources all involve ergometer/stationary rowing.
- Current support status: verified as thesis/project premise, with contextual source support.
- Best support: `murrayEtAl2016vrRowingPresence`; `arndtEtAl2018vrRowingWorkouts`; internal project framing.
- Wording should be narrowed: no.

#### Claim MOT-P3-C5

- Exact claim: "The system must therefore decide how the real movement should become a virtual rowing action."
- Claim classification: thesis synthesis and central design framing.
- Source support needed: not direct proof; source premises showing real ergometer action and virtual rowing action can diverge.
- Current support status: verified as thesis synthesis.
- Best support: `lamb1989kinematicComparison`; `rauterEtAl2013rowingTransfer`; `neumannEtAl2018interactiveVrSport`; internal thesis framing.
- Wording should be narrowed: no. This is one of the strongest sentences in the Motivation and should remain central.

### Source cards

#### Source: `soperHume2004rowingTechnique`

- Source role: supporting.
- What the source is about, in plain language: rowing technique and biomechanics review including ergometer use and limitations.
- What the source specifically says that matters here: ergometers are commonly used in rowing contexts and reproduce parts of rowing body action, while common ergometer designs do not fully reproduce trunk/upper-limb patterns.
- Which exact part of the paragraph it supports: the ergometer as indoor rowing/training device and the caveat that the machine is not the same as on-water rowing.
- Why this source is used here instead of only Rauter: Soper/Hume gives standard ergometer use; Rauter gives simulator/oar-water detail.
- What this source does NOT support: the VR mapping decision itself.
- Evidence type: thesis-synthesis premise.
- Confidence: verified.
- MD path: `MD Papers/soper_hume_2004_ideal_rowing_technique_biomechanics_markdown_bundle/soper_hume_2004_ideal_rowing_technique_biomechanics_raw_page_marked.md`
- MD line range: lines 79-85; lines 109-123
- PDF page if available: p. 1; p. 2.

#### Source: `rauterEtAl2013rowingTransfer`

- Source role: best for the "boat/oars/water replaced by machine" premise.
- What the source is about, in plain language: realistic rowing simulator and transfer from simulator to real rowing.
- What the source specifically says that matters here: rowing involves rower, boat, oar, and water interaction; ordinary indoor ergometers use cable-driven resistance and do not train oar handling or oar height in water; a richer simulator can show and sonify oar-water interaction.
- Which exact part of the paragraph it supports: the absent boat/oar/water interface and the idea that visual/auditory/haptic rendering can reintroduce parts of that action scene.
- Why this source is used here instead of only Lamb/Soper: it explicitly frames ordinary ergometers against oar-water interaction and simulator representation.
- What this source does NOT support: the thesis' exact two-mode comparison or embodiment outcomes.
- Evidence type: direct evidence for missing rowing interaction; thesis-synthesis premise.
- Confidence: verified.
- MD path: `MD Papers/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_markdown_bundle/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_raw_page_marked.md`
- MD line range: lines 149-199; lines 283-320; lines 2194-2214
- PDF page if available: p. 2; p. 3; p. 16.

#### Source: `lamb1989kinematicComparison`

- Source role: supporting.
- What the source is about, in plain language: direct comparison of ergometer and on-water rowing kinematics.
- What the source specifically says that matters here: ergometer and on-water rowing share important leg/trunk drive characteristics but differ in upper-limb/oar-related patterns, especially around catch and finish.
- Which exact part of the paragraph it supports: real movement does not map one-to-one onto on-water oar action; the system must choose how to turn ergometer movement into virtual rowing action.
- Why this source is used here instead of only rowing simulator sources: it directly establishes the kinematic mismatch at the heart of the mapping problem.
- What this source does NOT support: visual restoration or VR system design.
- Evidence type: thesis-synthesis premise.
- Confidence: verified.
- MD path: `MD Papers/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_markdown_bundle/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_raw_page_marked.md`
- MD line range: lines 20-63; lines 419-500
- PDF page if available: p. 1; pp. 6-7.

#### Source: `murrayEtAl2016vrRowingPresence`

- Source role: supporting.
- What the source is about, in plain language: VR rowing exercise with ergometer, virtual river, avatar, and companion condition.
- What the source specifically says that matters here: the user rows on an ergometer while viewing a virtual environment in which the avatar stroke timing matches the ergometer and the participant moves through a river course.
- Which exact part of the paragraph it supports: VR can add visual rowing context while the participant remains on an ergometer.
- Why this source is used here instead of only Neumann: it is a concrete rowing example.
- What this source does NOT support: HMD embodiment or the thesis' exact mapping modes.
- Evidence type: direct evidence for prior VR rowing setup; thesis-synthesis premise.
- Confidence: verified.
- MD path: `MD Papers/murray_2016_presence_of_others_vr_rowing_exercise_markdown_bundle/murray_2016_presence_of_others_vr_rowing_exercise_raw_page_marked.md`
- MD line range: lines 266-286
- PDF page if available: p. 3.

#### Source: `arndtEtAl2018vrRowingWorkouts`

- Source role: supporting.
- What the source is about, in plain language: HMD indoor-rowing VR prototype.
- What the source specifically says that matters here: stationary rowing machine movement data are mapped to a virtual lake/scull environment; movement on the lake depends on force applied to the oars.
- Which exact part of the paragraph it supports: VR visually reintroducing boat/lake movement while keeping the physical ergometer.
- Why this source is used here instead of only Murray: it is an HMD rowing example closer to the thesis medium.
- What this source does NOT support: exact representation comparison or embodiment outcomes.
- Evidence type: direct evidence for HMD VR rowing; thesis-synthesis premise.
- Confidence: verified.
- MD path: `MD Papers/arndt_2018_vr_hmd_rowing_workouts_markdown_bundle/arndt_2018_vr_hmd_rowing_workouts_raw_page_marked.md`
- MD line range: lines 47-57; lines 219-253
- PDF page if available: p. 1; p. 2.

#### Source: `neumannEtAl2018interactiveVrSport`

- Source role: best for the abstract "real exertion becomes virtual sport action" logic.
- What the source is about, in plain language: systematic review and conceptual framing of interactive VR sport.
- What the source specifically says that matters here: physical effort on an exertion interface can be translated into sport-relevant virtual performance; the review gives rowing handle pulls becoming virtual oar movement and faster virtual movement through water/scenery as an example.
- Which exact part of the paragraph it supports: "how the real movement should become a virtual rowing action."
- Why this source is used here instead of only concrete rowing examples: it generalizes the interaction logic and supplies the language of exertion interface and virtual sport performance.
- What this source does NOT support: that this thesis' two mappings have already been compared.
- Evidence type: direct evidence for exertion-interface-to-virtual-action principle; thesis-synthesis premise.
- Confidence: verified.
- MD path: `MD Papers/neumann_2018_interactive_virtual_reality_sport_systematic_review_markdown_bundle/neumann_2018_interactive_virtual_reality_sport_systematic_review_raw_page_marked.md`
- MD line range: lines 105-123; lines 228-241; lines 404-419
- PDF page if available: p. 4; p. 7; p. 12.

### Evidence window

The strongest combined evidence window is split across rowing mechanics and VR sport sources. `rauterEtAl2013rowingTransfer` establishes that ordinary ergometers replace the oar-water interaction with cable-driven resistance, while `lamb1989kinematicComparison` establishes that ergometer and on-water arm/oar-related movement are not the same. `murrayEtAl2016vrRowingPresence`, `arndtEtAl2018vrRowingWorkouts`, and `neumannEtAl2018interactiveVrSport` then show that virtual rowing systems can represent boats, rivers/lakes, oars, scenery, avatars, and virtual movement while the user remains physically on exercise equipment.

Important evidence snippets:

- Ordinary ergometers render resistance through a cable-driven windmill and do not train oar handling or oar height in water (`rauterEtAl2013rowingTransfer`, raw page-marked MD lines 180-199, PDF p. 2).
- Lifting or feathering the oar is essential on water but not exhibited in ergometer rowing (`lamb1989kinematicComparison`, raw page-marked MD lines 453-483, PDF p. 7).
- Rowing handle pulls can be depicted as virtual oar movement, and greater exertion can produce faster virtual movement through water and scenery (`neumannEtAl2018interactiveVrSport`, raw page-marked MD lines 404-419, PDF p. 12).
- Arndt et al.'s HMD prototype displays a virtual lake and scull, with movement depending on rowing force (`arndtEtAl2018vrRowingWorkouts`, raw page-marked MD lines 219-253, PDF p. 2).

No single source states the thesis design problem in the exact form "the system must decide how real movement becomes virtual rowing action." That sentence is the thesis' own synthesis and should be kept as such.

### Reasoning bridge

The source-backed premises are strong. Rowing is a tool-mediated action involving rower, boat, oar, and water. Ordinary ergometers keep rowing-like effort and some body movement but remove or alter the oar-water interface. VR rowing systems can display rowing environments and virtual movement while the user still acts through an ergometer. Interactive VR sport can translate physical exertion into virtual sport action.

The thesis-authored inference is the design problem: once VR visually represents boat/oar/water rowing while the participant physically performs ergometer rowing, the prototype must choose a mapping between real action and virtual action. This is not a literature category imported from a paper; it is the thesis' analytic framing.

Unsupported or only likely steps are minimal in this paragraph. The only caution is "visually restore": VR can visually represent boat/oar/water/motion, but it does not restore the full haptic or mechanical realities of on-water rowing.

### Overclaim boundaries

- Do not claim any paper names the thesis' two exact modes.
- Do not claim VR restores on-water rowing physically or haptically.
- Do not claim prior VR rowing systems solved the mapping problem.
- Do not claim that virtual oar movement is automatically more realistic or more embodied than ergometer-congruent movement.
- Do not claim Rauter's simulator results transfer directly to this HMD ergometer prototype.
- Do not claim Neumann's rowing example is evidence that the thesis' specific comparison has been studied.

### Suggested citation placement

The paragraph can use one carefully placed citation group after the second or third sentence:

```tex
\parencite{soperHume2004rowingTechnique,lamb1989kinematicComparison,rauterEtAl2013rowingTransfer,murrayEtAl2016vrRowingPresence,arndtEtAl2018vrRowingWorkouts,neumannEtAl2018interactiveVrSport}
```

That group is defensible but dense. A cleaner alternative is to split the support:

- Ergometer replaces/changes boat-oar-water action:

```tex
\parencite{soperHume2004rowingTechnique,lamb1989kinematicComparison,rauterEtAl2013rowingTransfer}
```

- VR can display rowing environments and translate effort to virtual action:

```tex
\parencite{murrayEtAl2016vrRowingPresence,arndtEtAl2018vrRowingWorkouts,neumannEtAl2018interactiveVrSport}
```

The final sentence, "The system must therefore decide...", does not need its own external citation if the premises immediately before it are cited. It is the thesis inference.

### Suggested developer note

```tex
\sourcechecknote{This paragraph is the thesis synthesis point rather than a claim copied from one source. The rowing sources establish the first premise: ordinary ergometer rowing is a legitimate indoor rowing/training form but replaces or alters the boat-oar-water interaction. Soper and Hume support common ergometer use and biomechanical caveats, Lamb directly compares ergometer and on-water rowing and identifies upper-limb/oar-related differences, and Rauter et al. emphasize that rowing involves continuous rower-boat-oar-water interaction while ordinary ergometers use cable-driven resistance and do not train oar handling or oar height. The VR sources establish the second premise: virtual rowing systems can visually present rowing environments and couple ergometer effort to virtual action. Murray et al. use an ergometer with a virtual river/avatar setup, Arndt et al. use an HMD rowing prototype with a virtual lake/scull driven by ergometer sensor data, and Neumann et al. describe interactive VR sport in which rowing handle pulls can become virtual oar movements and exertion can drive faster movement through water and scenery. The thesis inference is that VR rowing must choose how the real ergometer movement becomes a virtual rowing action. This should not be overread as a claim that VR restores full on-water haptics or that prior work has already studied the exact two-mode comparison.}
```

### Suggested SOURCE-CHECK comments

```tex
% SOURCE-CHECK:
%   key: rauterEtAl2013rowingTransfer
%   md: MD Papers/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_markdown_bundle/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_raw_page_marked.md, lines 149-199; lines 305-320
%   pdf: p. 2; p. 3
%   evidence: Rowing involves continuous rower-boat-oar-water interaction; ordinary ergometers use cable-driven resistance and do not train oar handling/oar height, while a richer simulator can render oar-water interaction.
%   confidence: verified
%   caution: Use as premise for missing boat/oar/water interaction, not as embodiment outcome evidence.
%
% SOURCE-CHECK:
%   key: neumannEtAl2018interactiveVrSport
%   md: MD Papers/neumann_2018_interactive_virtual_reality_sport_systematic_review_markdown_bundle/neumann_2018_interactive_virtual_reality_sport_systematic_review_raw_page_marked.md, lines 105-123; lines 404-419
%   pdf: p. 4; p. 12
%   evidence: In interactive VR sport, physical effort on an exertion interface translates to virtual sport performance; rowing handle pulls can be depicted as virtual oar movements and greater exertion can drive faster virtual movement through water and scenery.
%   confidence: verified
%   caution: Supports exertion-to-virtual-action logic, not the claim that this exact mapping comparison already exists in prior work.
%
% SOURCE-CHECK:
%   key: murrayEtAl2016vrRowingPresence; arndtEtAl2018vrRowingWorkouts
%   md: MD Papers/murray_2016_presence_of_others_vr_rowing_exercise_markdown_bundle/murray_2016_presence_of_others_vr_rowing_exercise_raw_page_marked.md, lines 266-286; MD Papers/arndt_2018_vr_hmd_rowing_workouts_markdown_bundle/arndt_2018_vr_hmd_rowing_workouts_raw_page_marked.md, lines 219-253
%   pdf: Murray p. 3; Arndt p. 2
%   evidence: Prior VR rowing examples keep the user on an ergometer while displaying virtual rowing environments, avatars/sculls, scenery, and force- or stroke-coupled virtual movement.
%   confidence: verified
%   caution: Concrete examples only; neither paper directly studies the thesis' two representation strategies.
```

### Paragraph verdict

Ready for prose patch.

This paragraph is well aligned with the thesis framing. Later editing should preserve the core sentence "The system must therefore decide how the real movement should become a virtual rowing action." That sentence makes action congruence explicit and keeps the Introduction centered on representation mapping rather than generic VR attractiveness.

# Paragraph 4: Two Forms of Fidelity

## Paragraph 4: Two Forms of Fidelity

### Current paragraph text

This decision matters because indoor rowing in VR is not simply a question of adding a more attractive background to exercise. The user performs a real, repetitive, forceful movement while seeing a mediated version of that movement in a virtual environment. The virtual scene can make the activity feel more like rowing on water, but the physical interface remains the ergometer. As a result, the system must balance two different forms of fidelity: fidelity to the user's actual sensorimotor interaction with the machine, and fidelity to the visual and cultural form of the sport.

### Paragraph function

This paragraph sharpens the design problem into a trade-off. It moves from "VR can restore context" to "the mapping is not only decoration." It introduces the two forms of fidelity that later become the two thesis modes:

- Fidelity to the user's actual sensorimotor interaction with the ergometer.
- Fidelity to the recognizable visual/sport form of rowing on water.

This is the key Motivation paragraph for later embodiment framing. It should explicitly protect the action-congruence point: the user is performing real forceful action, and the virtual stroke should either preserve that real action mapping or transform it into a more recognizable rowing depiction.

### Claim ledger

#### Claim MOT-P4-C1

- Exact claim: "Indoor rowing in VR is not simply a question of adding a more attractive background to exercise."
- Claim classification: thesis synthesis and rhetorical bridge.
- Source support needed: no direct source needed; source premises should show that VR sport involves interactive exertion and that rowing involves meaningful body/tool interaction.
- Current support status: verified as thesis framing.
- Best support: `neumannEtAl2018interactiveVrSport`; `rauterEtAl2013rowingTransfer`.
- Wording should be narrowed: no. This is a strong thesis sentence and should stay, but do not over-cite it as if a source said this exact phrase.

#### Claim MOT-P4-C2

- Exact claim: "The user performs a real, repetitive, forceful movement while seeing a mediated version of that movement in a virtual environment."
- Claim classification: directly source-backed premise plus project framing.
- Source support needed: rowing movement/force/coordinated stroke; VR systems mapping ergometer movement to virtual environment/avatar/oars.
- Current support status: verified.
- Best support: `rauterEtAl2013rowingTransfer`; `lamb1989kinematicComparison`; `arndtEtAl2018vrRowingWorkouts`; `murrayEtAl2016vrRowingPresence`; `neumannEtAl2018interactiveVrSport`.
- Wording should be narrowed: maybe. "Forceful" is safe as plain language, but if the final thesis needs technical rigor, use "physical" or "effortful" unless a force/power-specific source is cited nearby.

#### Claim MOT-P4-C3

- Exact claim: "The virtual scene can make the activity feel more like rowing on water, but the physical interface remains the ergometer."
- Claim classification: thesis synthesis from source-backed premises.
- Source support needed: virtual rowing systems display rowing/on-water environments; physical interface remains ergometer; ergometer differs from on-water rowing.
- Current support status: likely.
- Best support: `murrayEtAl2016vrRowingPresence`; `arndtEtAl2018vrRowingWorkouts`; `neumannEtAl2018interactiveVrSport`; `lamb1989kinematicComparison`; `rauterEtAl2013rowingTransfer`.
- Wording should be narrowed: yes. "Can make the activity feel more like rowing on water" is plausible but subjective. Safer: "can make the activity look or be framed more like rowing on water." If "feel" remains, cite carefully and do not imply measured realism unless the study measures it.

#### Claim MOT-P4-C4

- Exact claim: "The system must balance two different forms of fidelity: fidelity to the user's actual sensorimotor interaction with the machine, and fidelity to the visual and cultural form of the sport."
- Claim classification: internal project framing and thesis synthesis.
- Source support needed: source support for the premises only; no external source names this exact two-fidelity balance.
- Current support status: verified as thesis framing; likely for "cultural form" unless broadened from sport-specific recognizability.
- Best support: internal thesis spine; `lamb1989kinematicComparison`; `rauterEtAl2013rowingTransfer`; `harrisEtAl2019visionForAction` would be relevant later but was not in the requested source set for this pack.
- Wording should be narrowed: yes. "Visual and cultural form" is conceptually good but not directly supported by the requested sources. "Visual and sport-specific form" or "recognizable boat-and-oar form of the sport" is better source-aligned.

### Source cards

#### Source: `neumannEtAl2018interactiveVrSport`

- Source role: best for "not just background" because it defines VR sport through interactivity and exertion interface.
- What the source is about, in plain language: a systematic review of interactive VR sport.
- What the source specifically says that matters here: VR sport is not merely a visual scene; it includes interactivity and sport-relevant actions translating into virtual performance. The source explicitly describes physical effort on ergometers translating into virtual race-course speed and rowing handle pulls depicted as virtual oar movements.
- Which exact part of the paragraph it supports: "not simply a more attractive background"; real movement becoming mediated virtual action; exertion/action coupling.
- Why this source is used here instead of only rowing biomechanics: it links sport action to virtual feedback and interactivity.
- What this source does NOT support: the exact two-fidelity framing, the term "cultural form," or embodiment outcomes.
- Evidence type: direct evidence for interactive VR sport/action coupling; thesis-synthesis premise.
- Confidence: verified.
- MD path: `MD Papers/neumann_2018_interactive_virtual_reality_sport_systematic_review_markdown_bundle/neumann_2018_interactive_virtual_reality_sport_systematic_review_raw_page_marked.md`
- MD line range: lines 105-123; lines 228-241; lines 404-419
- PDF page if available: p. 4; p. 7; p. 12.

#### Source: `rauterEtAl2013rowingTransfer`

- Source role: best for the real rowing action as forceful, coordinated, and tool-mediated.
- What the source is about, in plain language: realistic rowing simulator and transfer to real rowing.
- What the source specifically says that matters here: rowing involves coordinated dynamic movement of legs, trunk, and arms and continuous haptic interaction among rower, boat, oar, and water; ordinary ergometers omit important oar-handling elements.
- Which exact part of the paragraph it supports: real movement is a meaningful sport action, not just generic exercise; virtual rowing must deal with missing oar-water interaction.
- Why this source is used here instead of only Lamb/Soper: it foregrounds interaction and simulation relevance.
- What this source does NOT support: subjective "feel more like rowing" unless used only as premise.
- Evidence type: direct evidence for rowing action structure; thesis-synthesis premise.
- Confidence: verified.
- MD path: `MD Papers/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_markdown_bundle/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_raw_page_marked.md`
- MD line range: lines 149-199; lines 283-302; lines 707-795
- PDF page if available: p. 2; p. 3; pp. 8-9.

#### Source: `lamb1989kinematicComparison`

- Source role: supporting for the sensorimotor fidelity side.
- What the source is about, in plain language: kinematic comparison of ergometer and on-water rowing.
- What the source specifically says that matters here: ergometer and on-water rowing differ in upper arm and forearm patterns, especially around catch/finish, while legs/trunk are more similar.
- Which exact part of the paragraph it supports: the need to distinguish fidelity to actual ergometer movement from fidelity to boat/oar rowing depiction.
- Why this source is used here instead of only Rauter: it gives direct kinematic contrast rather than simulator/training context.
- What this source does NOT support: visual/cultural fidelity as a theory term.
- Evidence type: thesis-synthesis premise.
- Confidence: verified.
- MD path: `MD Papers/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_markdown_bundle/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_raw_page_marked.md`
- MD line range: lines 20-63; lines 419-500
- PDF page if available: p. 1; pp. 6-7.

#### Source: `murrayEtAl2016vrRowingPresence`

- Source role: supporting.
- What the source is about, in plain language: VR rowing exercise with avatar, virtual river, and companion condition.
- What the source specifically says that matters here: the virtual avatar stroke timing matched the ergometer stroke; the virtual environment included river/scenery and a companion boat condition.
- Which exact part of the paragraph it supports: seeing a mediated virtual version of real ergometer movement; virtual environment can represent rowing context.
- Why this source is used here instead of only Arndt: it explicitly mentions avatar stroke timing matched to the ergometer.
- What this source does NOT support: the two-fidelity framework or thesis embodiment claims.
- Evidence type: direct evidence for mediated movement/virtual rowing environment.
- Confidence: verified.
- MD path: `MD Papers/murray_2016_presence_of_others_vr_rowing_exercise_markdown_bundle/murray_2016_presence_of_others_vr_rowing_exercise_raw_page_marked.md`
- MD line range: lines 266-286
- PDF page if available: p. 3.

#### Source: `arndtEtAl2018vrRowingWorkouts`

- Source role: supporting.
- What the source is about, in plain language: HMD VR indoor rowing system using ergometer sensor data.
- What the source specifically says that matters here: movement data from the rowing machine are used in a virtual lake/scull environment; real haptic feedback comes from the ergometer handles; virtual motion depends on force.
- Which exact part of the paragraph it supports: real ergometer interaction plus mediated virtual representation.
- Why this source is used here instead of only Murray: it directly uses HMD and sensor-driven VR rowing.
- What this source does NOT support: visual/cultural fidelity as a formal construct or general preference claims.
- Evidence type: direct evidence for mediated VR rowing action.
- Confidence: verified.
- MD path: `MD Papers/arndt_2018_vr_hmd_rowing_workouts_markdown_bundle/arndt_2018_vr_hmd_rowing_workouts_raw_page_marked.md`
- MD line range: lines 175-190; lines 219-253; lines 305-350
- PDF page if available: p. 2; p. 3.

#### Source: internal thesis framing

- Source role: best for the exact two-fidelity language.
- What the source is about, in plain language: the thesis' own conceptual framing.
- What the source specifically says that matters here: the thesis compares ergometer-congruent mapping and boat-realistic/sport-depiction mapping.
- Which exact part of the paragraph it supports: the distinction between fidelity to sensorimotor interaction and fidelity to recognizable rowing depiction.
- Why this source is used here instead of pretending external papers say it: no checked source defines this exact pair of thesis modes.
- What this source does NOT support: external evidence. Internal notes are not thesis evidence by themselves.
- Evidence type: internal project framing.
- Confidence: verified.
- MD path: `notes/global/thesis_spine.md`; `notes/chapters/01_introduction_back_of_mind.md`
- MD line range: thesis spine lines 5-23; back-of-mind note lines 5-29
- PDF page if available: not applicable.

### Evidence window

`neumannEtAl2018interactiveVrSport` is the main source for why VR sport is not just background decoration. It defines VR sport in terms of simulated sport environments and interactivity, and it ties physical effort on an interface to virtual sport performance. The rowing example is especially useful because it says handle pulls can be represented as virtual oar movements and exertion can drive faster virtual movement through water and scenery.

`rauterEtAl2013rowingTransfer` and `lamb1989kinematicComparison` provide the other side of the trade-off. They show that rowing is a coordinated, tool-mediated action and that ergometer rowing is not mechanically identical to on-water rowing. This gives the rationale for why fidelity to the actual ergometer interaction and fidelity to recognizable on-water rowing depiction can come apart.

`murrayEtAl2016vrRowingPresence` and `arndtEtAl2018vrRowingWorkouts` supply concrete examples of mediated virtual rowing. Murray matched avatar stroke timing to the ergometer and used a virtual river/scenery environment. Arndt used ergometer sensors and a virtual lake/scull environment. Arndt is also useful as a caution because participants in VR reported less control despite enjoying the environment more; visual enhancement does not automatically imply better control or embodiment.

Important evidence snippets:

- VR sport involves interactivity where virtual events respond to the athlete (`neumannEtAl2018interactiveVrSport`, raw page-marked MD lines 228-241, PDF p. 7).
- Rowing handle pulls can be depicted as virtual oar movement, with greater exertion causing faster movement through virtual water/scenery (`neumannEtAl2018interactiveVrSport`, raw page-marked MD lines 404-419, PDF p. 12).
- Arndt et al. state that real haptic feedback came from the ergometer handles while the virtual system displayed rowing on a lake (`arndtEtAl2018vrRowingWorkouts`, raw page-marked MD lines 219-253, PDF p. 2).
- Lamb found on-water and ergometer upper-limb patterns differ around catch/finish and oar handling (`lamb1989kinematicComparison`, raw page-marked MD lines 419-500, PDF pp. 6-7).

### Reasoning bridge

The source-backed premises are that VR sport is interactive and action-coupled, that rowing is physically and technically structured, and that ergometer and on-water rowing are not identical. The concrete VR rowing sources show that real rowing-machine movement can be displayed as avatar or boat/scull movement in a virtual environment. The rowing mechanics sources show that the real ergometer action cannot simply be assumed to equal on-water oar action.

The thesis-authored inference is the two-fidelity balance. "Sensorimotor interaction with the machine" is the thesis' label for fidelity to the real user-device action loop. "Visual and cultural form of the sport" is the thesis' label for the recognizable boat/oar/water depiction. The sources support the premises, but the two-label distinction is the thesis' own analytical framing.

The main only-likely step is "feel more like rowing on water." The current sources show that VR can visually represent on-water rowing contexts; they do not directly prove that users feel more like they are rowing on water unless the cited study measured that specific perception. A later prose patch should consider "look more like" or "be framed more like."

### Overclaim boundaries

- Do not claim "more attractive background" as a source claim; it is the thesis' rhetorical contrast.
- Do not claim visual rowing context necessarily increases embodiment.
- Do not claim sport realism and visuomotor congruence always trade off; say they can come apart in this prototype/design problem.
- Do not claim "cultural form" is a validated construct unless a source is added.
- Do not imply that Murray or Arndt evaluated the same two-fidelity comparison.
- Do not cite Arndt's positive enjoyment findings without also noting its less-control finding if making claims about control/agency.
- Do not claim real ergometer motion is "wrong"; it is the actual physical basis of the system.

### Suggested citation placement

Use a source group after the sentence about real movement and mediated virtual movement:

```tex
\parencite{rauterEtAl2013rowingTransfer,murrayEtAl2016vrRowingPresence,arndtEtAl2018vrRowingWorkouts,neumannEtAl2018interactiveVrSport}
```

Use a second source group if the paragraph explicitly says ergometer and on-water movement differ:

```tex
\parencite{lamb1989kinematicComparison,soperHume2004rowingTechnique}
```

Do not force an external citation after the final two-fidelity sentence. It is the thesis' own framing. If a citation is added, it should support the premise, not pretend the source invented the categories.

### Suggested developer note

```tex
\sourcechecknote{This paragraph reframes VR rowing as an action-mapping problem rather than background decoration. Neumann et al. support this by defining interactive VR sport through a simulated sport environment and athlete interactivity, and by giving the rowing example where ergometer handle pulls become virtual oar movements and exertion changes virtual speed through water and scenery. Murray et al. and Arndt et al. provide concrete VR rowing systems in which real ergometer movement is mediated as avatar, boat, scull, river, lake, or scenery movement. Rauter et al. and Lamb explain why this is not a trivial one-to-one mapping: rowing is a rower-boat-oar-water interaction, ordinary ergometers replace important oar-water mechanics, and ergometer/on-water kinematics differ especially around upper-limb and oar-related parts of the stroke. The thesis inference is the two-fidelity tension: fidelity to the user's actual sensorimotor interaction with the machine versus fidelity to the recognizable visual/sport form of on-water rowing. The sources support the premises for this tension, but not the exact label "cultural form" and not any conclusion that one form of fidelity is superior.}
```

### Suggested SOURCE-CHECK comments

```tex
% SOURCE-CHECK:
%   key: neumannEtAl2018interactiveVrSport
%   md: MD Papers/neumann_2018_interactive_virtual_reality_sport_systematic_review_markdown_bundle/neumann_2018_interactive_virtual_reality_sport_systematic_review_raw_page_marked.md, lines 228-241; lines 404-419
%   pdf: p. 7; p. 12
%   evidence: Interactive VR sport requires athlete interactivity; rowing handle pulls can be represented as virtual oar movement and exertion can drive virtual movement through water and scenery.
%   confidence: verified
%   caution: Supports action-coupled VR sport, not the thesis' exact two-fidelity terminology.
%
% SOURCE-CHECK:
%   key: rauterEtAl2013rowingTransfer; lamb1989kinematicComparison
%   md: MD Papers/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_markdown_bundle/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_raw_page_marked.md, lines 149-199; MD Papers/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_markdown_bundle/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_raw_page_marked.md, lines 419-500
%   pdf: Rauter p. 2; Lamb pp. 6-7
%   evidence: Rowing is a rower-boat-oar-water interaction; ordinary ergometers use cable-driven resistance and omit oar handling/oar height; ergometer and on-water rowing differ in upper-limb/oar-related motion around catch and finish.
%   confidence: verified
%   caution: Supports why real ergometer interaction and boat/oar depiction can diverge; does not prove embodiment outcomes.
%
% SOURCE-CHECK:
%   key: murrayEtAl2016vrRowingPresence; arndtEtAl2018vrRowingWorkouts
%   md: MD Papers/murray_2016_presence_of_others_vr_rowing_exercise_markdown_bundle/murray_2016_presence_of_others_vr_rowing_exercise_raw_page_marked.md, lines 266-286; MD Papers/arndt_2018_vr_hmd_rowing_workouts_markdown_bundle/arndt_2018_vr_hmd_rowing_workouts_raw_page_marked.md, lines 219-253
%   pdf: Murray p. 3; Arndt p. 2
%   evidence: Concrete VR rowing systems mediate ergometer movement as virtual avatar/scull/environment movement; Arndt notes real haptic feedback came from ergometer handles while virtual movement occurred on the lake.
%   confidence: verified
%   caution: Supports mediated movement examples, not the exact two-mode comparison.
```

### Paragraph verdict

Needs narrower paragraph wording before a final prose patch.

The paragraph is central and should stay, but later prose should probably revise "visual and cultural form of the sport" to "recognizable visual and sport-specific form of rowing" unless a culture/sport-meaning source is added. The phrase "feel more like rowing on water" should also be handled cautiously unless it is clearly a design aim rather than a sourced empirical claim.

# Paragraph 5: Thesis Focus on the Representation Balance

## Paragraph 5: Thesis Focus on the Representation Balance

### Current paragraph text

This thesis investigates that balance. It examines VR indoor rowing as a case where a physical exercise device stands in for a more complex sport action. The central question is whether the virtual representation should preserve the user's actual interaction with the ergometer as directly as possible, or transform that interaction into the boat- and oar-based action associated with rowing on water.

### Paragraph function

This paragraph closes the Motivation by naming the thesis object. It should not introduce new literature. Its purpose is to:

- State that the thesis investigates the balance introduced in Paragraph 4.
- Define VR indoor rowing as a case where a physical exercise device stands in for a more complex sport action.
- Preview the two representation strategies without yet fully theorizing them.
- Make clear that the research question is comparative and open, not a claim that one mapping is already better.

This paragraph is primarily thesis-internal. External sources are useful only as support for the premises that ergometer rowing differs from on-water rowing and that VR sport maps physical exertion to virtual action.

### Claim ledger

#### Claim MOT-P5-C1

- Exact claim: "This thesis investigates that balance."
- Claim classification: internal project framing.
- Source support needed: none.
- Current support status: verified as thesis statement.
- Best support: internal thesis framing, not literature.
- Wording should be narrowed: no.

#### Claim MOT-P5-C2

- Exact claim: "VR indoor rowing is a case where a physical exercise device stands in for a more complex sport action."
- Claim classification: thesis synthesis from source-backed premises.
- Source support needed: rowing sources showing sport action complexity and ergometer simplification; VR sport source showing exercise devices/exertion interfaces can drive virtual sport action.
- Current support status: verified.
- Best support: `rauterEtAl2013rowingTransfer`; `lamb1989kinematicComparison`; `soperHume2004rowingTechnique`; `neumannEtAl2018interactiveVrSport`.
- Wording should be narrowed: no, if "stands in for" is understood as thesis framing rather than source quote.

#### Claim MOT-P5-C3

- Exact claim: "The central question is whether the virtual representation should preserve the user's actual interaction with the ergometer as directly as possible, or transform that interaction into the boat- and oar-based action associated with rowing on water."
- Claim classification: internal project framing and thesis synthesis.
- Source support needed: source support for the underlying mismatch and virtual-action mapping, but no source should be cited as if it posed this exact thesis question.
- Current support status: verified as thesis framing.
- Best support: internal thesis spine; `lamb1989kinematicComparison`; `rauterEtAl2013rowingTransfer`; `neumannEtAl2018interactiveVrSport`.
- Wording should be narrowed: no. This is a strong central-question sentence.

### Source cards

#### Source: internal thesis framing

- Source role: best for the exact thesis question.
- What the source is about, in plain language: internal notes defining the thesis' two representation strategies and scope.
- What the source specifically says that matters here: the thesis compares an ergometer-congruent representation, where the user's real movement is mapped directly, with a boat-realistic representation, where the movement is transformed into recognizable boat/oar rowing.
- Which exact part of the paragraph it supports: the central question and comparative scope.
- Why this source is used here instead of external papers: no checked external paper defines this exact thesis comparison. Treating the comparison as thesis-authored avoids fabricating a literature category.
- What this source does NOT support: citable external evidence.
- Evidence type: internal project framing.
- Confidence: verified.
- MD path: `notes/global/thesis_spine.md`; `notes/global/contribution_hierarchy.md`; `notes/chapters/01_introduction_back_of_mind.md`
- MD line range: thesis spine lines 5-23; contribution hierarchy lines 5-23; back-of-mind note lines 5-29
- PDF page if available: not applicable.

#### Source: `rauterEtAl2013rowingTransfer`

- Source role: best external support for "complex sport action."
- What the source is about, in plain language: realistic rowing simulator and transfer to real rowing.
- What the source specifically says that matters here: rowing involves coordinated legs/trunk/arms movement, rower-boat-oar-water haptic interaction, oar handling, and oar height; ordinary ergometers omit important oar-water handling.
- Which exact part of the paragraph it supports: "physical exercise device stands in for a more complex sport action."
- Why this source is used here instead of only Lamb: it frames rowing as a simulator-relevant, tool-mediated, haptic sport action.
- What this source does NOT support: the thesis' exact central question or representation labels.
- Evidence type: thesis-synthesis premise.
- Confidence: verified.
- MD path: `MD Papers/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_markdown_bundle/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_raw_page_marked.md`
- MD line range: lines 149-199; lines 283-302; lines 707-795
- PDF page if available: p. 2; p. 3; pp. 8-9.

#### Source: `lamb1989kinematicComparison`

- Source role: best external support for the mismatch that motivates the two alternatives.
- What the source is about, in plain language: kinematic comparison between ergometer and on-water rowing.
- What the source specifically says that matters here: legs and trunk are broadly similar in many drive-phase variables, while arm/oar-related kinematics differ around catch and finish.
- Which exact part of the paragraph it supports: why "preserve actual ergometer interaction" and "transform into boat/oar action" are distinct options.
- Why this source is used here instead of only Rauter: it directly compares the two physical forms.
- What this source does NOT support: embodiment outcomes or the thesis' exact design alternatives.
- Evidence type: thesis-synthesis premise.
- Confidence: verified.
- MD path: `MD Papers/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_markdown_bundle/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_raw_page_marked.md`
- MD line range: lines 20-63; lines 419-500
- PDF page if available: p. 1; pp. 6-7.

#### Source: `neumannEtAl2018interactiveVrSport`

- Source role: supporting for virtual representation/action translation.
- What the source is about, in plain language: interactive VR sport review.
- What the source specifically says that matters here: physical effort on an interface can translate into virtual sport performance; rowing handle pulls can become virtual oar movement.
- Which exact part of the paragraph it supports: the idea that a VR system can preserve or transform real interaction into virtual sport action.
- Why this source is used here instead of only concrete rowing systems: it states the general exertion-interface principle and gives a rowing example.
- What this source does NOT support: the thesis' exact comparative question as a known literature gap.
- Evidence type: thesis-synthesis premise.
- Confidence: verified.
- MD path: `MD Papers/neumann_2018_interactive_virtual_reality_sport_systematic_review_markdown_bundle/neumann_2018_interactive_virtual_reality_sport_systematic_review_raw_page_marked.md`
- MD line range: lines 105-123; lines 404-419
- PDF page if available: p. 4; p. 12.

#### Source: `soperHume2004rowingTechnique`

- Source role: supporting/background.
- What the source is about, in plain language: rowing technique review.
- What the source specifically says that matters here: ergometers are normal rowing training/testing tools but do not fully reproduce on-water trunk/upper-limb patterns.
- Which exact part of the paragraph it supports: the "physical exercise device stands in for a more complex sport action" premise.
- Why this source is used here instead of only Rauter/Lamb: it grounds the ergometer as standard training equipment and not a strawman.
- What this source does NOT support: the thesis' exact comparison or VR system details.
- Evidence type: contextual support.
- Confidence: verified.
- MD path: `MD Papers/soper_hume_2004_ideal_rowing_technique_biomechanics_markdown_bundle/soper_hume_2004_ideal_rowing_technique_biomechanics_raw_page_marked.md`
- MD line range: lines 79-85; lines 109-123
- PDF page if available: p. 1; p. 2.

### Evidence window

This paragraph should rely mostly on internal thesis framing, with external sources supporting the premises already established earlier. `rauterEtAl2013rowingTransfer` supports the description of rowing as a more complex sport action involving rower, boat, oar, water, haptics, and coordinated whole-body movement. `lamb1989kinematicComparison` supports the reason the two options are not identical: ergometer and on-water rowing share some leg/trunk structure but differ in upper-limb/oar-related movement. `neumannEtAl2018interactiveVrSport` supports the idea that VR sport systems translate physical exertion into virtual sport action and explicitly gives rowing handle pulls becoming virtual oar movement as an example.

Important evidence snippets:

- Rowing involves continuous haptic forces between rower, boat, oar, and water (`rauterEtAl2013rowingTransfer`, raw page-marked MD lines 149-165, PDF p. 2).
- Ordinary ergometers omit oar handling and oar height in water (`rauterEtAl2013rowingTransfer`, raw page-marked MD lines 180-199, PDF p. 2).
- Ergometer and on-water rowing differ in upper-limb/oar-related patterns around catch and finish (`lamb1989kinematicComparison`, raw page-marked MD lines 419-500, PDF pp. 6-7).
- Rowing handle pulls can be depicted as virtual oar movements (`neumannEtAl2018interactiveVrSport`, raw page-marked MD lines 404-419, PDF p. 12).

No external source should be made to carry the exact thesis question. That question belongs to the author.

### Reasoning bridge

The source-backed premises are that on-water rowing is a coordinated, tool-mediated sport action; that ergometers are legitimate but incomplete stand-ins for that action; and that VR sport can map physical exertion into virtual sport action. The thesis inference is that this creates a central representation choice: either keep the virtual representation close to what the user is actually doing on the ergometer, or transform the action into a more boat/oar-based rowing depiction.

There is no unsupported step if the paragraph remains framed as the thesis' question. It would become unsupported only if it claimed that prior literature already identifies this exact comparison as the central unresolved problem.

### Overclaim boundaries

- Do not claim the central question comes from a prior source.
- Do not claim the thesis will determine a universally superior representation.
- Do not claim the boat/oar-based action is more correct in every respect.
- Do not claim preserving ergometer interaction is less realistic in all respects.
- Do not claim the thesis resolves general embodiment theory.
- Do not claim the evidence already predicts which mode will score higher.

### Suggested citation placement

This paragraph does not need heavy citations because it is the thesis' own scope statement. If citations are used, place one group after "more complex sport action" or after the final sentence to support the underlying premises:

```tex
\parencite{rauterEtAl2013rowingTransfer,lamb1989kinematicComparison,neumannEtAl2018interactiveVrSport}
```

Avoid citing internal notes in the thesis. Internal notes can guide drafting but are not external evidence.

### Suggested developer note

```tex
\sourcechecknote{This closing Motivation paragraph states the thesis' own research focus. External sources should only support the premises, not be presented as if they posed the exact central question. Rauter et al. support the idea that rowing is a complex sport action involving coordinated body movement and rower-boat-oar-water interaction, while ordinary ergometers omit oar handling and oar height in water. Lamb supports the kinematic mismatch that makes preserving actual ergometer movement and transforming it into boat/oar action meaningfully different choices. Neumann et al. support the interactive VR sport premise that physical exertion on an interface can become virtual sport action, including the example of rowing handle pulls represented as virtual oar movements. The thesis-authored question is whether the virtual representation should stay close to the user's real ergometer interaction or transform that interaction into the recognizable boat-and-oar action of on-water rowing. This paragraph should stay comparative and open-ended, without implying that one mapping is already known to be superior.}
```

### Suggested SOURCE-CHECK comments

```tex
% SOURCE-CHECK:
%   key: rauterEtAl2013rowingTransfer
%   md: MD Papers/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_markdown_bundle/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_raw_page_marked.md, lines 149-199; lines 283-302
%   pdf: p. 2; p. 3
%   evidence: Rowing is a coordinated rower-boat-oar-water action; ordinary ergometers omit oar handling and oar height in water.
%   confidence: verified
%   caution: Supports complex sport-action premise, not the exact thesis research question.
%
% SOURCE-CHECK:
%   key: lamb1989kinematicComparison
%   md: MD Papers/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_markdown_bundle/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_raw_page_marked.md, lines 20-63; lines 419-500
%   pdf: p. 1; pp. 6-7
%   evidence: Ergometer and on-water rowing share many drive-phase variables but differ in arm/oar-related movement, especially around catch and finish.
%   confidence: verified
%   caution: Supports why preserving actual ergometer interaction and depicting boat/oar action are not identical.
%
% SOURCE-CHECK:
%   key: neumannEtAl2018interactiveVrSport
%   md: MD Papers/neumann_2018_interactive_virtual_reality_sport_systematic_review_markdown_bundle/neumann_2018_interactive_virtual_reality_sport_systematic_review_raw_page_marked.md, lines 105-123; lines 404-419
%   pdf: p. 4; p. 12
%   evidence: Interactive VR sport translates physical effort on an interface into virtual sport performance; rowing handle pulls can be depicted as virtual oar movements.
%   confidence: verified
%   caution: Supports virtual-action translation premise, not the thesis' exact two-mode comparison as a prior finding.
```

### Paragraph verdict

Ready for prose patch.

This paragraph is one of the strongest pieces of the Motivation. Later citation work should keep it clean and not overload it with citations. Its job is to state the thesis question, not to survey literature.

# Subsection Summary

## Stable Citation Spine

These sources should remain central to the Motivation subsection unless the prose changes substantially:

- `soperHume2004rowingTechnique`: best for establishing rowing ergometers as normal rowing training/testing tools while also noting biomechanical limitations.
- `lamb1989kinematicComparison`: best for the direct ergometer-versus-on-water kinematic contrast. This is essential for the "related but not identical" premise.
- `rauterEtAl2013rowingTransfer`: best for rowing as a coordinated rower-boat-oar-water action and for the ordinary-ergometer limitation around oar handling/oar height.
- `murrayEtAl2016vrRowingPresence`: best concrete prior VR rowing source for ergometer plus virtual river/avatar/companion/scenery.
- `arndtEtAl2018vrRowingWorkouts`: best concrete HMD indoor-rowing source for ergometer sensors, virtual lake/scull, and force-coupled virtual movement.
- `neumannEtAl2018interactiveVrSport`: best broad VR sport source for interactivity, exertion interfaces, and the rowing handle-pull-to-virtual-oar example.
- `niehorster2021opticFlowHistory`: best narrow source for defining optic flow as visual motion that signals self-motion.
- `palmisanoEtAl2015vectionChallenges`: best cautionary source for subjective self-motion/vection in stationary observers if the Motivation keeps self-motion wording.

## Optional or Weak Sources

- `kooijmanEtAl2024measuringVection`: optional in the Motivation. It is stronger for Chapter 4 if vection/self-motion measurement is discussed. For Chapter 1, it may be more citation weight than needed unless "vection" becomes explicit.
- `rauterEtAl2013rowingTransfer` for spatial sound: strong for one realistic CAVE rowing simulator soundscape; weak for a broad feature list about VR rowing in general.
- `arndtEtAl2018vrRowingWorkouts` for teammates/opponents: weak if used as implemented-feature evidence. The checked lines support participant interest/future requests, not necessarily an implemented teammate/opponent condition.
- `murrayEtAl2016vrRowingPresence` for teammates: support is better phrased as "companion" or "presence of others" than generic teammates/opponents.

## Thesis Synthesis Points

These inferences are authored by the thesis and should not be attributed to a single external source:

- Indoor rowing is useful for XR embodiment because it keeps real, forceful, rowing-like action while removing boat/oar/water and moving-environment context.
- VR rowing creates a representation problem because the virtual scene can show on-water rowing while the physical interface remains an ergometer.
- The system must decide how real ergometer movement becomes virtual rowing action.
- Fidelity to the user's actual sensorimotor interaction with the machine and fidelity to the recognizable visual/sport form of rowing can come apart.
- The central thesis question is whether virtual representation should preserve real ergometer interaction as directly as possible or transform it into boat- and oar-based action.
- The comparison is exploratory and should not imply that either representation is superior in advance.

## Claims Needing Manual Verification

- "Mostly linear path" for the ergometer handle: plausible, but the checked sources support central-pulley/handle and seat movement more directly than this exact geometric phrasing.
- "Perceptual situation differs strongly": plausible thesis framing, but the checked rowing sources mainly establish mechanical/interface differences. Use cautious wording or support with a perceptual/experience source.
- "Spatial sound" as a generic VR rowing feature: checked support is limited to Rauter's simulator soundscape. Remove, narrow, or cite as a specific example.
- "Opponents, teammates" in the broad feature list: Murray supports companion/social context; Neumann supports presence of others/competitiveness generally. If the thesis does not implement these, keep as broad possible-feature context or remove from Motivation.
- "Feel more like rowing on water": plausible design motivation, but subjective. Safer later wording: "look more like," "be framed more like," or "visually resemble."
- "Visual and cultural form of the sport": conceptually useful but not directly supported by the checked sources. Safer later wording: "recognizable visual and sport-specific form of rowing."
- Exact absence of prior work comparing these two mappings: not part of this Motivation file, but should remain `TODO:VERIFY` elsewhere until a paper-first gap audit is done.

## Recommended Wording Changes

These are not `.tex` edits, only guidance for a later prose pass:

- Replace "this movement is reduced to a land-based training device" with a less value-loaded phrase such as "this movement is translated into sliding-seat and handle motion on a stationary training device."
- Replace "mostly linear path" with "handle motion on the ergometer" unless a stronger source for handle path geometry is added.
- Replace "perceptual situation differs strongly" with "the movement interface and visual-spatial situation differ from on-water rowing" or similar.
- Replace the broad feature list "optic flow, spatial sound, avatar representation, opponents, teammates, and environmental feedback" with a narrower, source-aligned list: "visual motion cues, avatar representation, social or competitive context, and environmental feedback." Mention spatial sound only as a simulator-specific possible feature.
- Keep "impression of self-motion" rather than "vection" unless vection is measured or explicitly discussed.
- Replace "visual and cultural form of the sport" with "recognizable visual and sport-specific form of rowing" unless a sport culture/meaning source is added.
- Keep "The system must therefore decide how the real movement should become a virtual rowing action." This sentence is central and sourceable as thesis synthesis.

## Final Developer Notes

These are the proposed `\sourcechecknote{...}` texts in subsection order. They are intentionally long because the author wants an auditable developer-mode layer.

### Developer note for Paragraph 1

```tex
\sourcechecknote{The Motivation opens from rowing and ergometer mechanics, not from VR theory. Soper and Hume support treating ergometer rowing as a normal rowing training and testing context while also warning that common ergometers reproduce only parts of on-water body action, especially less well for trunk and upper-limb patterns. Lamb gives the direct ergometer-versus-on-water kinematic comparison: leg and trunk movement are broadly similar in many drive-phase variables, but upper arm and forearm motion differ, especially around catch and finish, partly because on-water rowing includes oar handling such as lifting and feathering that is absent on the ergometer. Rauter et al. support the broader sport-action premise that rowing involves coordinated rower, boat, oar, and water interaction, whereas ordinary indoor ergometers replace this with cable-driven resistance and do not train oar handling or oar height in water. The thesis inference is that indoor rowing keeps real forceful rowing-like effort while removing boat, oar, water, and moving-environment context. These sources do not by themselves support embodiment outcomes, user preference, or any claim that ergometers are poor training devices.}
```

### Developer note for Paragraph 2

```tex
\sourcechecknote{This paragraph uses prior VR rowing and VR sport work only to motivate what virtual environments can add to ergometer rowing. Murray et al. support a Concept2 rowing setup with a projected virtual river, a third-person rowing avatar whose stroke timing matched the ergometer, passing scenery, and an individual or companion boat condition. Arndt et al. support an HMD rowing prototype in which ergometer sensor data drove a virtual lake/scull environment and virtual movement depended on rowing force. Neumann et al. provide the broader interactive VR sport frame and explicitly describe how rowing ergometer pulls can be represented as virtual oar movement and faster movement through water and scenery. The self-motion wording is supported separately: Niehorster defines optic flow as global visual motion that signals self-motion, while Palmisano et al. define vection as subjective self-motion in stationary observers and caution that it is a subjective phenomenon. The thesis inference is that visual motion in a stationary VR rowing context can contribute to an impression of self-motion. This should not be overstated as measured vection, embodiment, or proof that visual rowing context improves agency or ownership. Spatial sound is only specifically supported by Rauter et al.'s CAVE simulator soundscape and should not be treated as a generic VR rowing feature without additional evidence.}
```

### Developer note for Paragraph 3

```tex
\sourcechecknote{This paragraph is the thesis synthesis point rather than a claim copied from one source. The rowing sources establish the first premise: ordinary ergometer rowing is a legitimate indoor rowing/training form but replaces or alters the boat-oar-water interaction. Soper and Hume support common ergometer use and biomechanical caveats, Lamb directly compares ergometer and on-water rowing and identifies upper-limb/oar-related differences, and Rauter et al. emphasize that rowing involves continuous rower-boat-oar-water interaction while ordinary ergometers use cable-driven resistance and do not train oar handling or oar height. The VR sources establish the second premise: virtual rowing systems can visually present rowing environments and couple ergometer effort to virtual action. Murray et al. use an ergometer with a virtual river/avatar setup, Arndt et al. use an HMD rowing prototype with a virtual lake/scull driven by ergometer sensor data, and Neumann et al. describe interactive VR sport in which rowing handle pulls can become virtual oar movements and exertion can drive faster movement through water and scenery. The thesis inference is that VR rowing must choose how the real ergometer movement becomes a virtual rowing action. This should not be overread as a claim that VR restores full on-water haptics or that prior work has already studied the exact two-mode comparison.}
```

### Developer note for Paragraph 4

```tex
\sourcechecknote{This paragraph reframes VR rowing as an action-mapping problem rather than background decoration. Neumann et al. support this by defining interactive VR sport through a simulated sport environment and athlete interactivity, and by giving the rowing example where ergometer handle pulls become virtual oar movements and exertion changes virtual speed through water and scenery. Murray et al. and Arndt et al. provide concrete VR rowing systems in which real ergometer movement is mediated as avatar, boat, scull, river, lake, or scenery movement. Rauter et al. and Lamb explain why this is not a trivial one-to-one mapping: rowing is a rower-boat-oar-water interaction, ordinary ergometers replace important oar-water mechanics, and ergometer/on-water kinematics differ especially around upper-limb and oar-related parts of the stroke. The thesis inference is the two-fidelity tension: fidelity to the user's actual sensorimotor interaction with the machine versus fidelity to the recognizable visual/sport form of on-water rowing. The sources support the premises for this tension, but not the exact label "cultural form" and not any conclusion that one form of fidelity is superior.}
```

### Developer note for Paragraph 5

```tex
\sourcechecknote{This closing Motivation paragraph states the thesis' own research focus. External sources should only support the premises, not be presented as if they posed the exact central question. Rauter et al. support the idea that rowing is a complex sport action involving coordinated body movement and rower-boat-oar-water interaction, while ordinary ergometers omit oar handling and oar height in water. Lamb supports the kinematic mismatch that makes preserving actual ergometer movement and transforming it into boat/oar action meaningfully different choices. Neumann et al. support the interactive VR sport premise that physical exertion on an interface can become virtual sport action, including the example of rowing handle pulls represented as virtual oar movements. The thesis-authored question is whether the virtual representation should stay close to the user's real ergometer interaction or transform that interaction into the recognizable boat-and-oar action of on-water rowing. This paragraph should stay comparative and open-ended, without implying that one mapping is already known to be superior.}
```

## Final SOURCE-CHECK Blocks

These are the consolidated SOURCE-CHECK blocks in subsection order. They are written as exact LaTeX comments that can be copied into a draft, but this evidence-pack task did not edit `.tex`.

### SOURCE-CHECK block for Paragraph 1

```tex
% SOURCE-CHECK:
%   key: soperHume2004rowingTechnique
%   md: MD Papers/soper_hume_2004_ideal_rowing_technique_biomechanics_markdown_bundle/soper_hume_2004_ideal_rowing_technique_biomechanics_raw_page_marked.md, lines 79-85; lines 109-123
%   pdf: p. 1; p. 2
%   evidence: Rowing ergometers are commonly used for performance testing, technique coaching, crew selection, and poor-weather training; common ergometers reproduce parts of body action but do not reproduce trunk and upper-limb patterns particularly well compared with on-water rowing.
%   confidence: verified
%   caution: Supports ergometer use and biomechanical caveat, not VR embodiment or preference.
%
% SOURCE-CHECK:
%   key: lamb1989kinematicComparison
%   md: MD Papers/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_markdown_bundle/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_raw_page_marked.md, lines 20-63; lines 419-500
%   pdf: p. 1; pp. 6-7
%   evidence: Ergometer and on-water rowing share many drive-phase variables, especially legs and trunk, but upper arm and forearm patterns differ around catch and finish; lifting/feathering the oar is part of on-water rowing but not ergometer rowing.
%   confidence: verified
%   caution: Supports related-but-not-identical mechanics, not visual self-motion or embodiment outcomes.
%
% SOURCE-CHECK:
%   key: rauterEtAl2013rowingTransfer
%   md: MD Papers/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_markdown_bundle/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_raw_page_marked.md, lines 149-199; lines 283-302
%   pdf: p. 2; p. 3
%   evidence: Rowing involves continuous haptic interaction among rower, boat, oar, and water and a coordinated legs-trunk-arms drive; ordinary indoor ergometers provide cable-driven resistance and do not train oar handling or oar height in water.
%   confidence: verified
%   caution: Strong for missing oar/boat/water interaction, but do not treat simulator transfer findings as evidence for this thesis' embodiment outcomes.
```

### SOURCE-CHECK block for Paragraph 2

```tex
% SOURCE-CHECK:
%   key: murrayEtAl2016vrRowingPresence
%   md: MD Papers/murray_2016_presence_of_others_vr_rowing_exercise_markdown_bundle/murray_2016_presence_of_others_vr_rowing_exercise_raw_page_marked.md, lines 76-99; lines 266-286
%   pdf: p. 1; p. 3
%   evidence: VR exercise can let physical exertion on equipment move a person through a virtual environment; the rowing setup used a Concept2 ergometer, virtual river/scenery, third-person rowing avatar with stroke timing matched to the ergometer, and individual/companion boat conditions.
%   confidence: verified
%   caution: Supports VR rowing context and companion/avatar setup, not this thesis' embodiment mapping comparison.
%
% SOURCE-CHECK:
%   key: arndtEtAl2018vrRowingWorkouts
%   md: MD Papers/arndt_2018_vr_hmd_rowing_workouts_markdown_bundle/arndt_2018_vr_hmd_rowing_workouts_raw_page_marked.md, lines 47-57; lines 175-190; lines 219-253
%   pdf: p. 1; p. 2
%   evidence: HMD indoor-rowing prototype used stationary rowing machine sensors to capture handle/sledge and performance data, then displayed a virtual lake/scull environment with movement depending on rowing force.
%   confidence: verified
%   caution: Useful as an HMD rowing example; do not generalize its informal feedback as evidence for this thesis' outcomes.
%
% SOURCE-CHECK:
%   key: neumannEtAl2018interactiveVrSport
%   md: MD Papers/neumann_2018_interactive_virtual_reality_sport_systematic_review_markdown_bundle/neumann_2018_interactive_virtual_reality_sport_systematic_review_raw_page_marked.md, lines 228-241; lines 404-419
%   pdf: p. 7; p. 12
%   evidence: VR sport is a computer-simulated sport environment with interactivity; rowing ergometer handle pulls can be depicted as virtual oar movements and greater exertion can produce faster movement through virtual water and scenery.
%   confidence: verified
%   caution: Broad VR sport framing, not proof that the exact thesis comparison has been studied.
%
% SOURCE-CHECK:
%   key: niehorster2021opticFlowHistory
%   md: MD Papers/niehorster_2021_optic_flow_history_markdown_bundle/niehorster_2021_optic_flow_history_raw_page_marked.md, lines 28-34; lines 70-79
%   pdf: p. 1; p. 2
%   evidence: Optic flow is the global pattern of visual motion caused by and signaling self-motion and can provide information for direction of self-motion and visual guidance.
%   confidence: verified
%   caution: Supports visual self-motion cue language, not vection measurement or embodiment outcomes.
%
% SOURCE-CHECK:
%   key: palmisanoEtAl2015vectionChallenges
%   md: MD Papers/palmisano_2015_vection_research_challenges_markdown_bundle/palmisano_2015_vection_research_challenges_raw_page_marked.md, lines 45-54; lines 899-904
%   pdf: p. 1; p. 9
%   evidence: Vection is often used for visual illusions of self-motion in stationary observers; subjective experience of self-motion is central and measurement is methodologically cautious.
%   confidence: verified
%   caution: Use only for cautious self-motion/vection wording; do not claim vection was measured unless the study measures it.
%
% SOURCE-CHECK:
%   key: rauterEtAl2013rowingTransfer
%   md: MD Papers/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_markdown_bundle/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_raw_page_marked.md, lines 305-320
%   pdf: p. 3
%   evidence: A realistic rowing simulator used a CAVE and sound wave field synthesis to provide a realistic soundscape and audible/visible oar-water interaction.
%   confidence: likely
%   caution: Supports spatial sound only as a feature of this specific simulator; weak support for a broad generic VR rowing feature list.
```

### SOURCE-CHECK block for Paragraph 3

```tex
% SOURCE-CHECK:
%   key: rauterEtAl2013rowingTransfer
%   md: MD Papers/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_markdown_bundle/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_raw_page_marked.md, lines 149-199; lines 305-320
%   pdf: p. 2; p. 3
%   evidence: Rowing involves continuous rower-boat-oar-water interaction; ordinary ergometers use cable-driven resistance and do not train oar handling/oar height, while a richer simulator can render oar-water interaction.
%   confidence: verified
%   caution: Use as premise for missing boat/oar/water interaction, not as embodiment outcome evidence.
%
% SOURCE-CHECK:
%   key: neumannEtAl2018interactiveVrSport
%   md: MD Papers/neumann_2018_interactive_virtual_reality_sport_systematic_review_markdown_bundle/neumann_2018_interactive_virtual_reality_sport_systematic_review_raw_page_marked.md, lines 105-123; lines 404-419
%   pdf: p. 4; p. 12
%   evidence: In interactive VR sport, physical effort on an exertion interface translates to virtual sport performance; rowing handle pulls can be depicted as virtual oar movements and greater exertion can drive faster virtual movement through water and scenery.
%   confidence: verified
%   caution: Supports exertion-to-virtual-action logic, not the claim that this exact mapping comparison already exists in prior work.
%
% SOURCE-CHECK:
%   key: murrayEtAl2016vrRowingPresence; arndtEtAl2018vrRowingWorkouts
%   md: MD Papers/murray_2016_presence_of_others_vr_rowing_exercise_markdown_bundle/murray_2016_presence_of_others_vr_rowing_exercise_raw_page_marked.md, lines 266-286; MD Papers/arndt_2018_vr_hmd_rowing_workouts_markdown_bundle/arndt_2018_vr_hmd_rowing_workouts_raw_page_marked.md, lines 219-253
%   pdf: Murray p. 3; Arndt p. 2
%   evidence: Prior VR rowing examples keep the user on an ergometer while displaying virtual rowing environments, avatars/sculls, scenery, and force- or stroke-coupled virtual movement.
%   confidence: verified
%   caution: Concrete examples only; neither paper directly studies the thesis' two representation strategies.
```

### SOURCE-CHECK block for Paragraph 4

```tex
% SOURCE-CHECK:
%   key: neumannEtAl2018interactiveVrSport
%   md: MD Papers/neumann_2018_interactive_virtual_reality_sport_systematic_review_markdown_bundle/neumann_2018_interactive_virtual_reality_sport_systematic_review_raw_page_marked.md, lines 228-241; lines 404-419
%   pdf: p. 7; p. 12
%   evidence: Interactive VR sport requires athlete interactivity; rowing handle pulls can be represented as virtual oar movement and exertion can drive virtual movement through water and scenery.
%   confidence: verified
%   caution: Supports action-coupled VR sport, not the thesis' exact two-fidelity terminology.
%
% SOURCE-CHECK:
%   key: rauterEtAl2013rowingTransfer; lamb1989kinematicComparison
%   md: MD Papers/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_markdown_bundle/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_raw_page_marked.md, lines 149-199; MD Papers/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_markdown_bundle/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_raw_page_marked.md, lines 419-500
%   pdf: Rauter p. 2; Lamb pp. 6-7
%   evidence: Rowing is a rower-boat-oar-water interaction; ordinary ergometers use cable-driven resistance and omit oar handling/oar height; ergometer and on-water rowing differ in upper-limb/oar-related motion around catch and finish.
%   confidence: verified
%   caution: Supports why real ergometer interaction and boat/oar depiction can diverge; does not prove embodiment outcomes.
%
% SOURCE-CHECK:
%   key: murrayEtAl2016vrRowingPresence; arndtEtAl2018vrRowingWorkouts
%   md: MD Papers/murray_2016_presence_of_others_vr_rowing_exercise_markdown_bundle/murray_2016_presence_of_others_vr_rowing_exercise_raw_page_marked.md, lines 266-286; MD Papers/arndt_2018_vr_hmd_rowing_workouts_markdown_bundle/arndt_2018_vr_hmd_rowing_workouts_raw_page_marked.md, lines 219-253
%   pdf: Murray p. 3; Arndt p. 2
%   evidence: Concrete VR rowing systems mediate ergometer movement as virtual avatar/scull/environment movement; Arndt notes real haptic feedback came from ergometer handles while virtual movement occurred on the lake.
%   confidence: verified
%   caution: Supports mediated movement examples, not the exact two-mode comparison.
```

### SOURCE-CHECK block for Paragraph 5

```tex
% SOURCE-CHECK:
%   key: rauterEtAl2013rowingTransfer
%   md: MD Papers/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_markdown_bundle/rauter_2013_transfer_complex_skill_learning_virtual_real_rowing_raw_page_marked.md, lines 149-199; lines 283-302
%   pdf: p. 2; p. 3
%   evidence: Rowing is a coordinated rower-boat-oar-water action; ordinary ergometers omit oar handling and oar height in water.
%   confidence: verified
%   caution: Supports complex sport-action premise, not the exact thesis research question.
%
% SOURCE-CHECK:
%   key: lamb1989kinematicComparison
%   md: MD Papers/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_markdown_bundle/lamb_1989_kinematic_comparison_ergometer_on_water_rowing_raw_page_marked.md, lines 20-63; lines 419-500
%   pdf: p. 1; pp. 6-7
%   evidence: Ergometer and on-water rowing share many drive-phase variables but differ in arm/oar-related movement, especially around catch and finish.
%   confidence: verified
%   caution: Supports why preserving actual ergometer interaction and depicting boat/oar action are not identical.
%
% SOURCE-CHECK:
%   key: neumannEtAl2018interactiveVrSport
%   md: MD Papers/neumann_2018_interactive_virtual_reality_sport_systematic_review_markdown_bundle/neumann_2018_interactive_virtual_reality_sport_systematic_review_raw_page_marked.md, lines 105-123; lines 404-419
%   pdf: p. 4; p. 12
%   evidence: Interactive VR sport translates physical effort on an interface into virtual sport performance; rowing handle pulls can be depicted as virtual oar movements.
%   confidence: verified
%   caution: Supports virtual-action translation premise, not the thesis' exact two-mode comparison as a prior finding.
```

## Final Audit Verdict

The Motivation subsection is sourceable and conceptually aligned with the thesis, but it should be treated as a synthesis-heavy introduction rather than a literature-review paragraph. The safest citation strategy is:

- Use rowing biomechanics/simulator sources to ground the ergometer/on-water difference.
- Use VR rowing and VR sport sources to ground virtual context and action-coupled virtual movement.
- Use optic-flow/vection sources only for cautious self-motion wording.
- Keep the two-mode balance as thesis-authored framing.
- Do not overstuff the final prose with every possible citation; use this evidence pack as the deeper audit layer.
