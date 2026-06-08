# Thesis notes — Soper & Hume 2004, “Towards an Ideal Rowing Technique for Performance”

## Citation identity

Soper, C., & Hume, P. A. (2004). *Towards an ideal rowing technique for performance: The contributions from biomechanics*. Sports Medicine, 34(12), 825-848.

## What this paper is

This is a rowing biomechanics review article. It is not a VR, XR, or embodiment paper. Its value for the thesis is that it gives a credible sport-science basis for the rowing movement itself: ergometer versus on-water rowing, stroke phases, drive/recovery structure, body segment coordination, stroke rate, stroke length, boat velocity, oar forces, foot-stretcher forces, anthropometry, and equipment.

The paper reviews the biomechanics literature rather than presenting one new experiment. It repeatedly emphasizes that rowing technique contributes to performance, but that no simple universal “ideal technique” is clearly established for all rowers. This caution is useful for the thesis: the XR prototype does not need to claim to reproduce a single perfect rowing technique, but it should represent the major structural differences between ergometer movement and on-water rowing.

## What this paper is useful for in the XR rowing thesis

This paper is a core rowing-background source. It can support the rowing section and the explanation of the IK/motion-mapping system without turning the thesis into a sports-science thesis.

Use it for:
- basic rowing biomechanics terminology,
- the stroke cycle and drive/recovery timing,
- the sequential body movement pattern of legs, trunk, arms, and wrists,
- why ergometer rowing is related to but not identical with on-water rowing,
- why a straight central erg handle is mechanically different from oars moving through arcs around oarlocks,
- why boat-centered XR can restore sport-action elements that common ergs remove or simplify,
- why erg-centered XR has strong physical/device congruence but not full sport-action congruence.

Do not use it for:
- embodiment claims,
- VR/XR claims,
- proof that one representation mode is better,
- proof of a universal rowing technique.

## Why it matters for the XR rowing thesis

The thesis compares:

1. Erg-centered / high-congruence XR rowing:
   - the user's real erg handle, seat, and body motion are mapped closely to the avatar,
   - prioritizes physical alignment, visuomotor congruence, visuoproprioceptive congruence, haptic consistency, and agency.

2. Boat-centered / sport-depiction XR rowing:
   - the user still rows on an erg,
   - the avatar appears to row in a shell with oars, oarlocks, blades, catch, drive, finish, recovery, feathering/squaring, and boat movement,
   - prioritizes sport-action congruence,
   - introduces mismatch because virtual oar handles do not follow the same trajectory as the real erg handle.

Soper and Hume are useful because they show that this is not an artificial distinction. Ergometers are widely used and can reproduce parts of rowing, but they do not fully reproduce on-water rowing biomechanics. The review explicitly notes that common ergometers reproduce some body action, especially lower-limb patterns, but do not reproduce trunk and upper-limb body patterns as well as on-water rowing or sculling because many common ergometers use a central pulley system.

This is almost exactly the design tension of the thesis:
- The erg-centered mode can match the real machine.
- The boat-centered mode can visually restore the missing on-water logic.
- Neither mode is simply “more realistic” in every way.

## Core findings / cheat sheet

- Rowing ergometers are widely used for performance testing, technique coaching, crew selection, and training during poor weather.
- Ergometers can physiologically simulate rowing performance, especially 2000 m tests, but they do not necessarily reproduce all on-water kinematics and kinetics.
- Common ergometers reproduce parts of the body action, especially lower limbs, but do not reproduce trunk and upper-limb patterns as well as on-water rowing/sculling because of the central pulley system.
- Technique contributes to rowing performance, but the literature does not provide one clear universal biomechanical “ideal” stroke for every rower.
- Stroke rate and stroke length relate to boat velocity, but more rate is not simply always better because boat drag and intra-stroke velocity fluctuations matter.
- Sequential movement of lower limbs, trunk, and arms may lead to a more effective rowing stroke and greater boat velocity.
- The drive/recovery timing structure is central: total stroke time runs from catch to catch, and drive time runs from catch to finish.
- The “Rosenberg style” sequence is described as legs, lower trunk, mid-trunk, arms, and wrist segments accelerating the boat.
- Oar force and foot-stretcher force timing are important but complex; clear universal guidelines are limited.
- On-water rowing contains oar-specific movements at the catch and finish, including blade placement and feathering, which are not reproduced in the same way on ergometers.
- In rowing/sculling, oars move through arcs around oarlocks, making the boat representation mechanically different from a straight-line erg handle pull.

## Relation to thesis concepts

### Rowing stroke phases

The paper supports the basic stroke-cycle terminology:
- catch,
- drive,
- finish,
- recovery.

It describes drive time as the time from catch to finish, when the blade leaves the water, and total stroke time as catch-to-catch. This is useful for the glossary and for explaining how the avatar/IK system tracks stroke phase.

### Segmental coordination

The paper is especially useful for the sequence:
- lower limbs initiate the drive,
- trunk movement follows,
- arms/wrists complete the stroke.

This can support the IK system explanation. The avatar should not be posed as a random arm-pull machine. Even if the system is approximate, the rowing body should remain plausible by using the key stroke sequence: legs first on the drive; arms/body/seat return in the recovery.

### Ergometer versus on-water rowing

This is the most thesis-relevant section. The paper supports the claim that ergometer rowing is not identical to on-water rowing. It is useful because it does not dismiss ergometers: they are common, controllable, reliable, and useful. But it also makes clear that ergometer mechanics are only a partial simulation.

This is perfect for explaining why the thesis has two modes:
- erg-centered mode: real-machine congruence,
- boat-centered mode: sport-action depiction.

### Feathering and squaring

The paper directly mentions feathering in the context of on-water rowing differences. In the Stanford ergometer/on-water comparison, upper-arm and lower-arm contributions differed at catch and finish because of specific oar movements required during on-water rowing: blade placement at the catch and feathering at the finish.

The paper is therefore useful for supporting the claim that boat rowing includes oar/blade-specific upper-limb actions that common ergometers do not reproduce. However, it does not appear to provide a full explanatory definition of feathering and squaring. For a precise definition of squaring/feathering, use a rowing coaching manual or rulebook alongside this paper.

### IK / avatar motion mapping

This paper is useful for the IK section in a supporting way. It does not discuss IK, avatars, or XR. But it gives the rowing movement constraints that an IK system should respect:
- the stroke is cyclic,
- the body sequence matters,
- lower-limb, trunk, arm, and wrist motion are coordinated,
- ergometer motion differs from on-water motion,
- oar/blade actions add upper-limb and wrist-specific requirements.

For the thesis, this can justify why the avatar pose system is not just a generic seated animation. It must approximate the rowing stroke sequence and must decide whether to prioritize real erg handle alignment or virtual oar/boat plausibility.

### Sport-action congruence

Very useful. The paper provides the sport-science basis for the term “sport-action congruence” in rowing. In rowing, the expected sport action includes catch, drive, finish, recovery, oar arc, oarlock behavior, blade placement, blade extraction, feathering/squaring, and boat response.

A boat-centered XR condition can be said to prioritize this expected sport-action logic, even if the real erg handle trajectory does not match the virtual oar handle trajectory exactly.

### Visuomotor / visuoproprioceptive congruence

The paper does not discuss these XR terms, but it provides the movement facts that create the conflict. The user's proprioception comes from pulling the erg handle and moving the seat on a real machine. The boat-centered visual display may show hands/oars moving in arcs, which can be visually sport-faithful but not exactly congruent with the real handle path.

### Haptic / force congruence

Useful indirectly. The ergometer provides real grip, resistance, foot pressure, and seat motion. The boat-centered view can show water/oar forces, but unless the ergometer/haptic system reproduces oar-water force dynamics, there is a force-congruence gap. The paper's force-profile sections help explain that rowing force application is complex and oar-specific.

## How it maps to my thesis modes

### Erg-centered mode

Soper and Hume support the erg-centered mode as a legitimate physical baseline. Ergometers are commonly used for training, testing, coaching, and selection, and they can reproduce important parts of rowing performance.

For the erg-centered representation, the key argument is:
- the virtual handle, seat, and avatar can closely follow the real user and machine,
- this maximizes direct visuomotor, spatial, haptic, and proprioceptive congruence,
- the user sees what they physically do.

But the limitation is:
- this representation may not fully depict on-water rowing,
- it lacks or simplifies oars, oarlocks, blade work, feathering/squaring, and boat-water interaction,
- it may therefore be less sport-action congruent.

### Boat-centered mode

Soper and Hume strongly support why a boat-centered representation is meaningful. On-water rowing involves oar and boat mechanics that common ergometers simplify or remove. In boat-centered XR, the system can visually restore the expected rowing action: shell, oars, oarlocks, blades, catch, drive, finish, recovery, and feathering/squaring.

But the limitation is:
- the user is still physically pulling a central erg handle,
- the virtual oar handle path and real handle path may diverge,
- physical force and visual oar-water force may not fully match,
- the mode may gain sport-action congruence while sacrificing bodily/device congruence.

### Core tradeoff

This paper supports the central tradeoff of the thesis very well:

The question is not “more realism vs less realism.” The question is which kind of realism/congruence matters more for embodiment:
- bodily/device congruence with the real erg,
- or sport-action congruence with on-water rowing.

Soper and Hume justify the premise that these are not the same thing.

## What not to overclaim

- Do not claim this paper proves an ideal rowing technique.
- Do not claim this paper proves any XR embodiment effect.
- Do not claim this paper proves boat-centered XR is better.
- Do not claim this paper proves erg-centered XR is better.
- Do not claim Concept2/central-pulley ergs are biomechanically invalid.
- Do not claim ergometers cannot be useful for performance testing or training.
- Do not use this paper as the only source for defining squaring if a precise definition is needed.
- Do not overdo the sports-science detail in the thesis. This paper can carry most of the rowing biomechanics background, with one or two additional sources for specific technique definitions if needed.

## Thesis-use priority

High priority for:
- rowing biomechanics background,
- ergometer versus on-water distinction,
- stroke phases,
- drive/recovery timing,
- legs-trunk-arms sequence,
- IK-system movement rationale,
- sport-action congruence,
- why boat-centered XR restores missing on-water visual logic,
- why erg-centered XR preserves real-device congruence.

Medium priority for:
- oar force,
- foot-stretcher force,
- stroke rate,
- stroke length,
- boat velocity,
- equipment setup,
- crew synchrony.

Low priority for:
- embodiment theory,
- VR/XR,
- body ownership,
- self-location,
- avatar realism,
- preference/evaluation.

Suggested placement:
- Rowing background / sport-specific context.
- System/prototype section when explaining avatar IK and motion constraints.
- Related work when explaining ergometers versus on-water rowing.
- Discussion when explaining the core congruence tradeoff.

## Candidate thesis paragraph

Soper and Hume's review provides the rowing-biomechanics basis for distinguishing between ergometer-congruent and on-water-congruent representations. They note that rowing ergometers are widely used for training, testing, technique coaching, and selection, and can reproduce important parts of rowing performance, but that common ergometers do not fully reproduce on-water trunk and upper-limb movement patterns because of their central pulley structure. This distinction is central for XR rowing: an erg-centered representation can align closely with the user's real handle, seat, and bodily movement, while a boat-centered representation can restore the visual logic of on-water rowing, including oars, blade placement, and feathering. The design problem is therefore not simply whether one version is more realistic, but whether embodiment is better supported by direct physical congruence with the erg or by sport-action congruence with the expected rowing movement.

## Candidate short thesis sentence

Soper and Hume's rowing biomechanics review supports the key premise that ergometer rowing is a useful but partial simulation of on-water rowing, making the thesis distinction between erg-centered bodily congruence and boat-centered sport-action congruence biomechanically meaningful.

## Candidate glossary wording

### Rowing stroke phases

The rowing stroke is a cyclical movement from catch to catch. At the catch, the rower is forward on the slide and prepares to apply force. During the drive, the rower applies force and moves from catch toward finish. The drive is commonly described as a coordinated body sequence in which the legs initiate the movement, followed by trunk swing and then arm pull. At the finish, the blade leaves the water and the rower transitions into the recovery. During the recovery, the rower returns toward the next catch. In the thesis prototype, these phases are used not only as sport terminology but also as animation/IK states for the virtual avatar.

### Ergometer versus on-water rowing

An ergometer is a stationary rowing machine used for training, testing, coaching, and selection. It can reproduce important parts of rowing effort and body movement, but it does not fully reproduce on-water rowing mechanics. Common ergometers simplify the sport into a central handle pull, while on-water rowing uses one or two oars moving through arcs around oarlocks. For XR rowing, this creates a central design tension: an erg-centered avatar can match the real machine closely, while a boat-centered avatar can visually restore the rowing-specific logic of a shell, oars, oarlocks, blades, catch, drive, finish, recovery, and feathering/squaring.

### Feathering and squaring

Feathering and squaring are oar/blade rotation actions specific to on-water rowing. Before the drive, the blade is squared so that it can enter the water and apply force. During the recovery, the blade is feathered so that it travels flatter through the air. Soper and Hume's review supports the broader biomechanical distinction by noting that on-water rowing requires specific oar movements at the catch and finish, including blade placement and feathering. Most common ergometers remove or simplify these oar-specific actions because the rower pulls a central handle rather than controlling oars through arcs around oarlocks.

### IK / rowing avatar motion

In this thesis, the avatar IK system uses the rowing stroke structure as a constraint. The system does not merely place hands on a target; it must make the seated body appear to row plausibly. This means respecting the main rowing sequence: leg drive, trunk swing, arm pull, finish, and recovery. In the erg-centered mode, IK prioritizes matching the real handle, seat, and user posture. In the boat-centered mode, IK prioritizes the visual logic of on-water rowing, including oar-handle positions and blade actions, even where this creates a controlled mismatch with the real erg handle.

## Codex / agent note

Use this paper as the main rowing-biomechanics source for the thesis, especially for the rowing terms and IK/motion-mapping rationale. The thesis should not become a sports-science paper, so avoid overloading the main text with too much detail about force profiles, anthropometry, or hydrodynamics. The best use is to establish the important distinction: ergometers are valid and widely used, but they only partially reproduce on-water rowing mechanics. This justifies the thesis's core comparison between a physically congruent erg-centered avatar and a sport-action-congruent boat-centered avatar.

Potential additional sources to add later:
- a rowing coaching/manual source for clean definitions of squaring and feathering,
- a rowing biomechanics source focused specifically on ergometer vs on-water kinematics, if a deeper claim is needed,
- a rowing technique source for common coaching sequence language.

For now, Soper and Hume can carry most of the rowing-background section. Use it carefully and quote-check all exact wording against the PDF.
