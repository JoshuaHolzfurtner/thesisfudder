# Thesis notes — Colombo et al. 2025, “Immersion and interaction during cycling in virtual reality: the influence on perceived effort and subjective experience”

## Citation identity

Colombo, V., Mondellini, M., Aliverti, A., & Sacco, M. (2025). *Immersion and interaction during cycling in virtual reality: the influence on perceived effort and subjective experience*. *Frontiers in Virtual Reality*, 6, Article 1490588. https://doi.org/10.3389/frvir.2025.1490588

**Source file:** `frvir-6-1490588.pdf`

**Verification note:** The uploaded PDF abstract appears to contain an anomalous duplicated/irrelevant “Methods” paragraph about a literature search and post-stroke populations. The actual article content is an original experimental study with stationary cycling in four conditions. Verify the publisher PDF before quoting the abstract.

## What this paper is

This is an original VR exergame / virtual sport / rehabilitation-adjacent cycling study. It investigates how **immersion** and **interaction** influence perceived effort and subjective experience during stationary cycling.

The study used a within-subjects design with healthy young adults. Thirty-five participants were recruited, and one participant was excluded from analysis because their heart rate exceeded the expected exercise range. The final analysis therefore used **34 participants**.

Participants completed one exercise session with four 10-minute cycling conditions in randomized order:

1. **Cycle only condition (A):** cycling in front of a black screen.
2. **TV condition (B):** virtual park shown on a TV screen.
3. **HMD condition (C):** virtual park shown in a head-mounted display.
4. **HMD + interaction condition (D):** head-mounted display plus a simple Go/No-Go task, where participants collected blue spheres and avoided red spheres with a joystick.

The system was implemented in Unity and used a cycle-ergometer. Cycling cadence controlled the virtual movement through a park route. The paper describes cadence being converted into virtual speed / flowing velocity, and the virtual environment continued to move briefly if the rider stopped, corresponding to ergometer wheel inertia.

This makes the paper highly relevant for stationary virtual sport systems: real cyclic effort is coupled to virtual locomotion through a simulated environment.

## Why it matters for the XR rowing thesis

My thesis compares:

1. **Erg-centered / high-congruence XR rowing**
   - real erg handle/seat/body motion mapped closely to the avatar
   - prioritizes visuomotor, spatial, temporal, haptic/proprioceptive congruence

2. **Boat-centered / sport-depiction XR rowing**
   - user still rows on an erg
   - virtual avatar appears to row in a boat with oars/oarlocks/blades
   - prioritizes sport-action realism
   - introduces mismatch because virtual oar handles move differently from the real erg handle

The central question:

**Does embodiment in XR rowing benefit more from precise movement correspondence or from more realistic sport depiction?**

Colombo et al. do not test rowing, embodiment, body ownership, avatar alignment, or oar/handle mismatch. However, they test a very close neighboring design problem:

**stationary cyclic exercise + effort-coupled virtual locomotion + display immersion + optional interaction.**

This is directly useful for the thesis background because XR rowing also maps stationary exercise to virtual locomotion. The cycling cadence-to-virtual-speed mapping is analogous to rowing pace/power/stroke-to-boat-speed mapping.

The paper supports the claim that virtual sport systems are not merely decorative overlays on exercise. Immersion and interaction can affect user experience variables such as enjoyment, attention, spatial presence, preference, and possibly the relation between actual and perceived effort.

For the thesis, this paper is strongest for the **virtual sport / exergame / stationary effort becomes meaningful virtual locomotion** layer. It is weaker for the strict embodiment theory layer.

## Core findings / cheat sheet

- **Perceived effort did not significantly differ between conditions.**
  - RPE stayed around 12, described as “somewhat hard,” across cycle only, TV, HMD, and HMD + interaction.
  - This means the paper should not be used to claim that VR automatically makes exercise feel easier.
  - Use strength: moderate, because it directly measured RPE but in a controlled workload protocol.

- **Heart rate did not significantly differ between conditions.**
  - Mean heart-rate percentage remained within the intended range across all conditions.
  - This supports that exercise intensity was controlled, at least broadly.
  - Use strength: moderate.

- **Cycling cadence did not significantly differ between conditions.**
  - Participants maintained about 60 RPM across the protocol.
  - This matters because the conditions were compared under broadly similar task demands.
  - Use strength: moderate.

- **Breathing rate was significantly higher in the HMD + interaction condition.**
  - The combined immersive and interactive condition led to higher breathing rate than the other conditions.
  - Since RPE did not increase, the authors cautiously interpret this as a possible discrepancy between actual physical effort and perceived effort.
  - Use strength: useful but cautious. Breathing rate is relevant, but this does not by itself prove reduced perceived exertion.

- **Enjoyment increased with more immersive conditions.**
  - Enjoyment was lowest in cycle-only, higher with TV, and higher again in HMD conditions.
  - HMD + interaction had the highest enjoyment mean, but was not significantly different from HMD alone.
  - Use strength: high for subjective user-experience framing.

- **Self-perceived attention was highest in HMD + interaction.**
  - Adding the Go/No-Go task increased attention compared with the other conditions.
  - This supports the idea that simple interaction can increase engagement during virtual exercise.
  - Use strength: high for attention/engagement, but only for a simple cognitive interaction task.

- **Spatial presence was higher in HMD conditions than TV.**
  - HMD and HMD + interaction produced much higher spatial presence than TV.
  - Interaction did not significantly improve spatial presence over HMD alone.
  - Use strength: high for display immersion → spatial presence; weaker for interaction → presence.

- **Flow/time perception did not differ between conditions.**
  - The study used time-estimation as a proxy for the transformation-of-time dimension of flow.
  - No significant condition effect was found.
  - Use strength: low-to-moderate, because flow was measured very narrowly.

- **Most participants reported no cybersickness/discomfort in HMD conditions.**
  - In both HMD and HMD + interaction, 26 of 34 participants reported no discomfort.
  - Some participants reported disorientation, nausea, visual discomfort, or sweating.
  - Use strength: moderate for comfort discussion, but not as proof that VR cycling or VR rowing is broadly cybersickness-free.

- **Preference favored immersive VR, especially HMD + interaction.**
  - HMD + interaction received the highest overall preference score, followed by HMD, TV, and cycle only.
  - HMD + interaction was not significantly preferred over HMD alone.
  - Use strength: high for user preference in this sample and task.

## Relation to thesis concepts

### Sense of embodiment

This paper is not a direct sense-of-embodiment paper. It does not measure body ownership, self-location in a body, or embodiment questionnaires. It should therefore not be used as primary evidence for avatar embodiment.

However, it is relevant to the surrounding design space of embodied virtual sport because it studies how immersive display and effort-coupled interaction shape exercise experience.

### Sense of agency

The paper does not measure sense of agency in the strict embodiment-literature sense. Still, the system design contains an important agency-like mechanism: cycling cadence controls virtual movement through the environment.

For XR rowing, this is relevant because agency may be supported when the user’s own physical effort visibly causes virtual locomotion. Use the paper cautiously as evidence for effort-coupled virtual movement, not as direct agency evidence.

### Body ownership

The paper does not study body ownership. It does not test whether participants felt that a virtual body, avatar, bicycle, or limb was their own.

Do not cite this paper for body ownership claims.

### Self-location

The paper measures **spatial presence**, not self-location as a subcomponent of embodiment. It is relevant because HMD conditions increased the feeling of being in the virtual environment compared with TV. This can support a presence/place-illusion background section, but it should not be treated as direct evidence that the participant’s bodily self-location shifted into an avatar.

### Visuomotor congruence

The paper includes effort-to-motion coupling: the user’s cycling cadence controls virtual movement. This is a form of action/feedback congruence, but it is not a detailed visuomotor avatar-alignment study.

It supports the idea that virtual movement should be linked to the physical exercise action. It does not test fine-grained limb-motion congruence such as real handle path versus virtual oar path.

### Temporal congruence / latency

The paper does not focus on latency. It does imply real-time coupling between the cycle ergometer and virtual movement, but it should not be used to make strong claims about temporal congruence thresholds.

### Spatial alignment

The paper does not focus on spatial alignment between real and virtual equipment/body. It is therefore not useful for your markerless erg alignment argument except as a broader VR exercise context.

### Action-outcome congruence

This is one of the strongest thesis links. The paper’s virtual cycling system maps real cycling cadence to virtual speed through the park. This makes the user’s physical action produce visible virtual consequences.

For XR rowing, the analogous mechanism is:

**real stroke / power / pace → virtual boat speed / avatar motion / optic flow / route progress**

This supports your argument that virtual sport systems depend on believable coupling between exertion and world response.

### Optic flow / vection

The paper is relevant to optic-flow-like virtual movement because cycling cadence controls virtual speed and visual flow through the park. However, it does not explicitly measure vection, and it should not be used as direct evidence that participants felt vection.

Use it for:

- stationary effort coupled to visual locomotion
- immersive display increasing spatial presence
- virtual environment movement as exercise feedback

Do not use it to claim:

- vection occurred
- vection reduced perceived exertion
- optic flow solved motion sickness

### Presence / Place Illusion / Plausibility Illusion

The paper directly measures spatial presence with a single 0–100 item for the VR/TV conditions. HMD conditions produced higher spatial presence than the TV condition.

This is useful for your thesis because it supports the intuitive idea that HMD-based virtual sport can feel more spatially present than screen-based virtual sport.

However, the authors note they did not perform an extensive evaluation of place illusion or plausibility illusion. So this should be used narrowly.

### Flow / absorption

The paper discusses immersion and flow conceptually and uses time-estimation as a proxy for the transformation-of-time dimension of flow. It found no significant differences between conditions.

This is useful as a caution: higher immersion and enjoyment do not automatically mean measurable flow, especially if flow is assessed only through time perception.

### VR motion sickness / cybersickness

The paper includes a short cybersickness/discomfort control question for HMD conditions. Most participants reported no discomfort, but some reported disorientation, nausea, visual discomfort, or sweating.

For XR rowing, this is useful as a comparison point: stationary exercise in HMD VR can be acceptable for many users when virtual movement is synchronized with physical action and the route avoids abrupt turns. But this cannot be generalized too strongly.

### Rowing biomechanics

The paper is not about rowing and does not address rowing biomechanics. It can support analogies to cycling as stationary cyclic exercise, but not claims about rowing stroke mechanics.

### Erg vs on-water rowing

The paper does not compare ergometer rowing with on-water rowing. It does not address handle path, oars, oarlocks, blades, feathering/squaring, boat motion, or water interaction.

### Tool embodiment / virtual oars

Not addressed. Do not use this paper for tool-embodiment claims.

## How it maps to my thesis modes

### Erg-centered mode

This paper supports the erg-centered mode indirectly but strongly at the level of **effort-coupled virtual locomotion**.

In Colombo et al., the physical cycling cadence controls the virtual bicycle movement. This is analogous to an erg-centered XR rowing setup where the user’s real stroke, handle, and seat motion produce tightly coupled avatar and boat/world feedback.

The strongest takeaway for the erg-centered mode:

**The closer the virtual movement is coupled to the real exercise action, the more plausible it becomes to treat the virtual environment as a meaningful extension of stationary effort.**

This does not prove body ownership, but it supports the design logic that real physical exertion should have immediate and believable virtual consequences.

### Boat-centered mode

The paper is less directly useful for the boat-centered mode because its virtual sport representation is not obviously mismatched. Pedaling a stationary bicycle to move a virtual bicycle is visually and motorically compatible.

The boat-centered rowing mode is more complicated because the user pulls a straight erg handle while seeing a virtual oar/oarlock system with a different hand path and sport-specific motion logic.

So Colombo et al. can support the general value of immersive virtual sport environments, but it cannot answer whether sport-realistic rowing depiction can compensate for movement mismatch.

### Core tradeoff

The paper contributes mostly to the **effort-coupled virtual sport** side of the thesis, not directly to the **erg-centered vs boat-centered embodiment tradeoff**.

It helps establish that:

- stationary exercise can be meaningfully connected to virtual locomotion,
- HMD immersion can increase spatial presence and enjoyment,
- interaction can increase attention and preference,
- actual effort and perceived effort may diverge in immersive interactive exercise.

It does not determine whether the best rowing representation is the one with greatest bodily/device congruence or the one with greatest sport-action congruence.

## What not to overclaim

- Do not claim this proves VR rowing embodiment.
- Do not claim this proves body ownership, self-location in a virtual body, or full sense of embodiment.
- Do not claim this proves virtual oars can feel like body parts or tools incorporated into the body schema.
- Do not claim VR automatically reduces perceived exertion; the study found no significant RPE differences.
- Do not claim HMD + interaction significantly beat HMD alone for enjoyment, spatial presence, or overall preference; the trend favored HMD + interaction, but not always significantly.
- Do not claim vection was measured; it was not.
- Do not claim cybersickness was absent; most participants reported no discomfort, but some did report symptoms.
- Do not generalize strongly to older adults, patients, rowers, or people with respiratory disease; the analyzed sample consisted of healthy young adults.
- Do not use this as rowing biomechanics evidence.
- Do not use this as evidence for erg vs on-water rowing differences.
- Do not treat the paper’s flow result as a full flow analysis; it only used perceived passage of time as a proxy.
- Do not overuse the abstract without checking it, because the uploaded PDF appears to contain an anomalous abstract paragraph.

## Thesis-use priority

High priority for:

- VR exergame / virtual sport background
- stationary exercise mapped to virtual locomotion
- effort-coupled visual movement
- immersion and interaction in exercise VR
- perceived effort vs actual effort
- enjoyment, attention, preference, and spatial presence
- comfort / cybersickness discussion for HMD exercise

Medium priority for:

- action-outcome congruence
- Zwift-like exercise logic
- optic-flow-like route progression
- rehabilitation motivation and acceptability
- evaluation questionnaire design

Low priority for:

- strict sense of embodiment
- body ownership
- self-location as bodily self-location
- strict sense of agency measurement
- avatar morphology
- tool embodiment / virtual oars
- rowing biomechanics
- erg vs on-water rowing mismatch

Suggested placement:

- Theoretical background: VR exergames / virtual sport systems
- Theoretical background: stationary exercise and virtual locomotion
- Related work: immersive cycling / VR exercise studies
- Methods: justification for measuring RPE, attention, enjoyment, spatial presence, and cybersickness
- Discussion: interpreting effort, presence, and preference in XR rowing
- Limitations: caution about generalizing from cycling to rowing and from presence to embodiment

## Candidate thesis paragraph

Colombo et al. provide a useful comparison point for XR rowing because their stationary cycling study maps physical cadence to movement through a virtual park and compares exercise without VR, screen-based VR, HMD-based VR, and HMD-based VR with an additional interaction task. They found no significant differences in rated perceived exertion across conditions, but the immersive interactive condition produced higher breathing rate while perceived effort remained stable. At the same time, the HMD conditions increased enjoyment and spatial presence, and the HMD plus interaction condition produced the highest attention and preference scores. For XR rowing, this suggests that effort-coupled immersive environments may improve engagement and spatial experience even when they do not directly reduce reported exertion. However, the study should not be treated as direct evidence for rowing embodiment, because it did not examine avatar ownership, rowing-specific movement mappings, or mismatches between real erg motion and virtual sport depiction.

## Candidate short thesis sentence

In stationary cycling, Colombo et al. found that HMD-based virtual exercise increased enjoyment and spatial presence, while an immersive interactive condition increased breathing rate without increasing perceived exertion, suggesting that virtual sport systems can alter exercise experience even when perceived effort remains unchanged.

## Codex / agent note

Use this paper as a **high-value related-work source for virtual sport / exergame design**, not as a primary embodiment paper.

Best concepts to attach:

- stationary exercise → virtual locomotion
- effort-coupled movement
- immersion
- interaction
- perceived effort vs actual effort
- enjoyment
- attention
- spatial presence
- preference
- cybersickness comfort checks

Good thesis locations:

- background section on virtual sport / exergames
- optic flow / virtual locomotion discussion
- methods justification for RPE, breathing/HR, enjoyment, attention, spatial presence, cybersickness
- discussion comparison for why HMD mode may be preferred even if effort ratings do not improve

Do not use it for:

- body ownership
- SoE subcomponents except very indirectly
- avatar morphology
- virtual oars / tool embodiment
- rowing biomechanics
- direct evidence that sport-realistic boat rowing beats erg-centered congruence

Terminology to preserve:

- **immersion**: technological/experiential engagement through display and multisensory blocking of physical reality
- **interaction**: user engagement with virtual content / task
- **spatial presence**: feeling of being in the virtual environment
- **perceived effort / RPE**: subjective exertion, not identical to physical effort
- **breathing rate**: used as a marker of actual physical effort in this study
- **preference**: participants’ ranked condition preference after the session

Important caution for extraction:

The PDF abstract appears to include a mismatched systematic-review paragraph that does not fit the experimental paper. Keep this in raw/clean extraction for traceability, but flag it in notes and verify with the source before citing the abstract.
