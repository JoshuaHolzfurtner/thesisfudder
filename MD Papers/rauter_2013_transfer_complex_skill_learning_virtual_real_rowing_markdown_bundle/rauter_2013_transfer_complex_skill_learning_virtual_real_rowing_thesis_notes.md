# Thesis notes — Rauter et al. (2013), “Transfer of Complex Skill Learning from Virtual to Real Rowing”

## Citation identity

Rauter, G., Sigrist, R., Koch, C., Crivelli, F., van Raai, M., Riener, R., & Wolf, P. (2013). Transfer of Complex Skill Learning from Virtual to Real Rowing. *PLOS ONE*, 8(12), e82145.

## What this paper is

This paper investigates whether training on a high-fidelity virtual scull-rowing simulator can transfer to real on-water rowing.

The setup was a CAVE-based rowing simulator with:
- visual rendering,
- auditory rendering,
- haptic oar-water interaction,
- a trimmed skiff,
- two trimmed sculling oars,
- tendon-based parallel robots for haptic oar interaction,
- a real-time rowing model.

The study compared:
- one group training on water,
- one group training in the simulator.

Both groups trained four times over two weeks with the same licensed rowing trainer. Transfer was assessed through on-water biomechanical measures and blinded video evaluation by an independent rowing trainer.

## Why it matters for the XR rowing thesis

This is one of the most directly relevant rowing-simulator papers for your thesis.

It supports several important claims:

1. Rowing simulation is a serious research topic, not just fitness-game fluff.
2. Oar-water interaction and oar handling are critical for realistic rowing simulation.
3. Simulator fidelity matters when the goal is transfer to real rowing.
4. Realistic virtual rowing systems can support meaningful skill gains, at least in a small pilot-style study.
5. Quantitative biomechanical metrics may not fully capture rowing-skill development; expert video evaluation can reveal broader improvement.

For your thesis, it is useful as a rowing-domain anchor next to the embodiment papers.

## Core findings / cheat sheet

### 1) Simulator training transferred to on-water rowing

The authors conclude that realistic simulator training fostered skill gains to a similar extent as training in the real environment and enabled transfer to the real environment.

Use carefully: the sample is tiny, with four participants per group, so treat this as evidence/pilot support, not definitive proof.

### 2) High-fidelity haptics were central to their simulator rationale

The paper explicitly contrasts rowing with sports like table tennis or juggling. In rowing, haptic interaction forces between rower, boat, oar, and water are continuously present and large amounts of energy are transferred.

This is highly relevant to your project because it supports the idea that rowing simulation is not only visual. Realistic rowing depends on action forces, oar handling, and how the user feels the stroke.

### 3) Standard ergometers are limited as rowing simulators

The authors discuss indoor rowing ergometers such as RowPerfect and Concept2. These render resistance through a cable-driven windmill, but do not allow the rower to develop a feel for oar height in water and do not train oar handling because the user pulls a single rod/cable.

This is very relevant to your erg-vs-boat thesis:
- the erg is a standardized and useful rowing interface,
- but it omits crucial oar handling and blade-water components,
- therefore a virtual boat/oar representation can add rowing-specific depiction that the erg alone lacks.

### 4) The paper defines rowing cycle phases clearly

The paper divides the rowing cycle into:
- catch,
- drive phase,
- release,
- recovery phase.

It explains that at the catch, blades enter the water; during drive, legs/trunk/arms coordinate to pull oars through the water; at release, blades leave the water; recovery brings the oars back for the next stroke.

This is useful for your glossary, implementation, and appendix.

### 5) Their simulator measured exactly the kind of variables you care about

The simulator and on-water setup measured:
- horizontal oar angle,
- vertical oar angle,
- oar rotation around the longitudinal axis,
- oar forces,
- seat position,
- upper-body/shoulder movement.

This strongly overlaps your system’s conceptual variables:
- handle/seat tracking,
- oar-angle representation,
- feathering/squaring,
- body/IK motion,
- stroke phase detection.

### 6) Oar handling and body-segment coordination were central performance categories

Their performance measures included:
- catch slip,
- depth of blade immersion,
- striking out before catch,
- overlap of legs and trunk,
- overlap of trunk and arms,
- catch angle,
- release angle,
- stroke length,
- maximal handle power,
- mean handle power.

For your app, this is gold for a form-analysis appendix or later technical roadmap. It also shows that oar handling is not a decorative detail; it is one of their core training/assessment categories.

### 7) Quantitative metrics were limited, expert qualitative judgment still mattered

The authors found that biomechanical measures gave limited insight into rowers’ development, while the blinded trainer could rate the rowers’ overall impression.

This is important for your methods:
- if your thesis does not deeply evaluate rowing technique, say so clearly;
- for embodiment, questionnaires may be primary;
- for rowing realism/quality, expert ratings or qualitative notes can be useful but should not be over-interpreted.

## How it connects to your two modes

### Erg-centered mode

This paper helps explain why an erg-centered mode is mechanically clean but rowing-incomplete:
- the erg can provide strong handle/seat congruence,
- but it cannot fully represent oar height, blade immersion, and oar-water handling.

So the erg mode is strong for visuomotor congruence but not fully sport-realistic.

### Boat-centered mode

This paper supports the motivation for a boat/oar-realistic mode:
- rowing depends on oar-water interaction,
- oar handling is a real skill category,
- catch/release/blade depth/angles matter,
- sculling uses two oars and coordinated oar movement.

Your boat mode can be framed as a visual/IK attempt to restore some of the rowing-specific action structure that the erg removes, even if the real physical handle path remains erg-like.

## Feathering and squaring relevance

This paper is very useful for defending why oar rotation matters.

It measures q, the rotation of the oar around its longitudinal axis, defining the blade as parallel to the water surface at 0° and vertical to the water surface at -90°. That is essentially the measurement axis for feathered vs squared blade orientation.

Important nuance:
- Their ten biomechanical performance measures did not ultimately use q because of measurement/evaluation constraints.
- But the simulator and on-water measurement system did measure oar rotation.
- Therefore, blade orientation is part of serious rowing-simulator instrumentation, even if not always included in simplified performance metrics.

For your thesis:
- feathering/squaring can be described as part of the boat-mode representation and IK/oar state machine,
- but you do not need to evaluate it as a primary rowing-technique outcome unless your study specifically does so.

## What not to overclaim

Do not claim this paper proves VR rowing embodiment. It is about simulator skill transfer, not sense of embodiment.

Do not claim the results are definitive; the sample size is very small.

Do not claim their simulator is comparable to a consumer HMD erg app. Their setup included CAVE projection, real oars, haptic robots, sound, and a real-time rowing model.

Do not claim that visual realism alone enabled transfer. Their simulator was multimodal and especially haptic.

Do not use it to prove your boat mode is more embodied. Use it to justify why rowing-specific oar/boat representation is a meaningful design dimension.

## Thesis-use priority

High priority for:
- rowing simulator prior work,
- ergometer limitations,
- rowing cycle phases,
- oar handling as a serious technical category,
- skill-transfer framing,
- form-analysis appendix variables.

Medium priority for:
- VR motor learning,
- augmented feedback,
- simulator fidelity.

Suggested placement:
- related work: XR/VR rowing and rowing simulators,
- system rationale: why the boat mode includes virtual oars/blades,
- appendix: rowing form metrics and possible future form-analysis variables,
- limitations: your system lacks physical oar-water haptics compared with high-fidelity simulators.

## Candidate thesis sentence

“Prior rowing-simulator work emphasizes that rowing differs from many visually dominated motor tasks because haptic oar-water interactions and oar handling are continuously present and central to technique. Rauter et al.’s scull simulator therefore included visual, auditory, and haptic rendering of oar-water interaction and assessed technical variables such as catch slip, blade depth, oar angles, body-segment coordination, and handle power. This supports treating the boat-centered oar depiction in the present system as a rowing-specific action representation rather than a purely cosmetic visual layer.”

Verify exact wording and page references against the original PDF before final submission.
