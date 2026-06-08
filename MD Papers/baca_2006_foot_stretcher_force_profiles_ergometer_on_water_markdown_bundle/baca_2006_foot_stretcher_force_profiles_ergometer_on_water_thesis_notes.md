# Thesis notes — Baca et al. 2006, “Comparison of Foot-Stretcher Force Profiles Between On-Water and Ergometer Rowing”

## Citation identity

Baca, A., Kornfeind, P., & Heller, M. (2006). *Comparison of foot-stretcher force profiles between on-water and ergometer rowing*. XXIV International Symposium on Biomechanics in Sports, Salzburg, Austria.

## What this paper is

This is a short biomechanics conference/symposium paper comparing foot-stretcher reaction force profiles between on-water single scull rowing and Concept2 ergometer rowing.

The study compares three conditions:

1. Concept2 static ergometer,
2. Concept2 ergometer on slides,
3. on-water single scull.

Four Austrian male elite rowers were tested at stroke rates of 20 and 30 strokes per minute. The authors measured horizontal and vertical reaction forces at the left and right foot stretcher. They then compared force-curve consistency within each condition and similarity between ergometer and boat force profiles.

This is not an XR, VR, embodiment, or avatar paper. It is a narrow rowing-biomechanics source. Its value for the thesis is as an optional support citation for the idea that the physical rowing interface affects how closely ergometer rowing approximates on-water rowing.

## Content summary

The paper starts from the observation that rowing ergometers are commonly used for land-based training, technique coaching, crew selection, biomechanical analysis, and performance tests. However, the authors note that opinions differ on how effectively ergometers simulate on-water rowing.

The study focuses on the foot stretcher because the rower applies force against the foot stretcher in order to exert force on the ergometer handle or to produce forward propulsion in the boat. If an ergometer is a good simulator for on-water rowing, similar foot-stretcher force curves should appear.

The authors tested four elite male rowers at 20 and 30 strokes/min on a Concept2 static ergometer, a Concept2 on slides, and in a single scull. For each condition, they measured reaction forces at the foot stretcher and compared five consecutive strokes.

The key result is that all conditions showed high inter-stroke consistency, but force curves from the Concept2 on slides were more similar to on-water force curves than force curves from the static Concept2. The authors conclude that rowing on the slide ergometer compares better to on-water rowing than exercising on the static ergometer.

They also observed that the pulling phase lasted longer in the boat than in either ergometer condition. Force asymmetries between left and right feet were visible in all conditions, but were largest in the boat, smaller on the slides ergometer, and smallest on the static ergometer.

The paper suggests that the differences can partly be explained by the different initial conditions at the beginning of the pulling phase. In the boat and on the ergometer with slides, the rower decelerates/accelerates the scull or ergometer, whereas on the static ergometer the rower's body must be decelerated/accelerated.

## Why it matters for the XR rowing thesis

This paper is useful as a small precision source for the ergometer/on-water approximation problem.

The thesis compares:

1. Erg-centered / high-congruence XR rowing:
   - the virtual avatar matches the real erg handle, seat, and body movement as closely as possible.

2. Boat-centered / sport-depiction XR rowing:
   - the user still rows on an erg, but the virtual avatar appears to row in a boat with oars, blades, oarlocks, and on-water rowing logic.

Baca et al. help support the limitation that the physical ergometer is not a perfect on-water simulator. More specifically, even within Concept2 rowing, the force-profile similarity changes depending on whether the machine is static or mounted on slides.

This is useful for the IK/system section because it supports treating the avatar motion as a controlled approximation rather than a fully biomechanically exact simulation of on-water rowing.

## Core findings / cheat sheet

- The study compared foot-stretcher force profiles between static Concept2, Concept2 on slides, and on-water single scull rowing.
- Four elite male rowers were tested at 20 and 30 strokes/min.
- Inter-stroke consistency was high in all conditions.
- Force curves from the slides ergometer were more similar to on-water force curves than force curves from the static ergometer.
- Pulling-phase duration was longer in the boat than on the ergometers.
- Force asymmetries between left and right feet occurred in all conditions.
- These asymmetries were largest in the boat, smaller on the slides ergometer, and smallest on the static ergometer.
- The authors conclude that the slide ergometer compares better to on-water rowing than the static ergometer.
- The paper suggests that differences may be explained by different rower/boat/ergometer acceleration conditions at the beginning of the drive.
- The physical configuration of the ergometer matters for how closely land-based rowing approximates on-water rowing.

## Relation to thesis concepts

### Ergometer versus on-water rowing

Useful as an optional add-on. Soper & Hume and Lamb are better main sources for the broad erg-vs-water difference. Baca et al. add a specific force-profile comparison showing that even within Concept2 rowing, static versus slides changes similarity to on-water rowing.

### IK / avatar motion mapping

Useful for limitations. The IK system can map handle, seat, body, and phase information into a plausible rowing avatar, but it cannot fully reproduce on-water force/inertia mechanics if the physical rowing hardware does not provide them.

This supports wording like:
- The virtual rowing avatar should be understood as a representation layer, not as a full biomechanical simulator.
- The boat-centered mode approximates on-water sport action visually, but it does not recreate all force and inertial properties of boat rowing.

### Physical/device congruence

Useful. The paper reinforces that the real rowing device is not neutral. A static erg, a slide erg, and a boat give different physical conditions. Therefore, device congruence depends on the actual machine being used.

### Haptic / force congruence

Useful. The paper is specifically about foot-stretcher reaction forces. It can support the idea that haptic/force congruence is limited in boat-centered XR when the user rows on a static erg.

### Sport-action congruence

Indirectly relevant. A boat-centered visual representation may increase sport-action realism, but this paper reminds the reader that visual boat realism does not automatically mean physical force-profile realism.

### Rowing biomechanics

Narrow relevance. It is not a broad rowing-technique source. Use Soper & Hume as the main source, and Baca et al. only for static/slides/on-water foot-stretcher force-profile nuance.

### Embodiment

Indirect relevance only. The paper does not study embodiment, body ownership, agency, or VR. It can support the physical-congruence side of the thesis but not the psychological outcome.

## How it maps to my thesis modes

### Erg-centered mode

The erg-centered mode has strong congruence with the real rowing hardware the user actually feels. If the user rows on a static erg, the avatar can match static-erg handle/seat motion, but that does not mean it perfectly represents on-water force/inertia. Baca et al. support this nuance.

### Boat-centered mode

The boat-centered mode can visually restore on-water rowing elements such as a shell, oars, blades, oarlocks, and water response. However, if the physical hardware is a static erg, the force-profile and inertial behavior may remain less boat-like than a slide erg or actual boat. This supports describing the boat-centered avatar as a sport-depiction approximation, not an exact biomechanical reproduction.

### Core tradeoff

This paper supports the thesis's careful distinction between different types of realism/congruence:

- visual sport-action congruence: the rowing looks like on-water rowing,
- physical/device congruence: the virtual motion matches the real erg,
- force/haptic congruence: the physical forces match what the user sees,
- biomechanical similarity: the measured kinematics/kinetics resemble on-water rowing.

Baca et al. are mostly useful for the force/haptic/biomechanical-similarity layer.

## What not to overclaim

- Do not claim that slide ergs perfectly reproduce on-water rowing.
- Do not claim that static Concept2 rowing is invalid.
- Do not claim that this paper proves anything about VR rowing embodiment.
- Do not claim that this paper proves the boat-centered or erg-centered mode is better.
- Do not use this as the main rowing technique source.
- Do not generalize strongly from four elite male rowers.
- Do not overemphasize foot-stretcher forces if the thesis does not measure them.
- Do not turn the thesis into a detailed sports-biomechanics comparison of static, slides, RowPerfect, tanks, and boats.

## Thesis-use priority

Medium priority for:
- IK/system limitations,
- erg-vs-boat approximation,
- static erg versus slides nuance,
- physical device configuration,
- force/haptic congruence,
- saying the virtual boat mode is an approximation.

Low priority for:
- main embodiment theory,
- body ownership,
- agency measurement,
- rowing glossary,
- general stroke phases,
- questionnaire design.

Suggested placement:
- One sentence or footnote in the IK/system section.
- One sentence in limitations.
- Optional note in rowing biomechanics background if discussing static versus dynamic/slides ergs.

## Candidate thesis paragraph

Baca et al. provide a useful reminder that the physical rowing device changes the degree to which ergometer rowing resembles on-water rowing. In their comparison of foot-stretcher force profiles, a Concept2 ergometer mounted on slides showed higher similarity to on-water single sculling than a static Concept2. For the present XR rowing prototype, this supports treating avatar motion as a controlled approximation rather than a full biomechanical reconstruction of on-water rowing. Even when the virtual scene depicts a shell and oars, the user’s physical force and inertia remain constrained by the actual ergometer setup.

## Candidate short thesis sentence

Baca et al. found that foot-stretcher force profiles from a Concept2 on slides were more similar to on-water single sculling than those from a static Concept2, suggesting that ergometer configuration affects how closely land-based rowing approximates boat rowing.

## Candidate footnote

Even within ergometer rowing, the hardware configuration changes biomechanical similarity to on-water rowing. Baca et al. compared foot-stretcher force profiles on a static Concept2, a Concept2 on slides, and a single scull, finding higher similarity between the slide ergometer and on-water sculling than between the static ergometer and on-water sculling. This supports treating the virtual boat representation as an approximation rather than a physically exact simulation.

## Candidate glossary wording

### Static ergometer versus slides

A static ergometer fixes the machine in place, so the rower’s body moves relative to a stationary frame. An ergometer on slides allows the machine itself to move back and forth during the stroke, making the rower-machine system more similar to the rower-boat interaction in on-water rowing. In XR rowing, this matters because the physical ergometer configuration affects the force and inertia cues available to the user. A virtual boat view can depict on-water rowing, but it cannot automatically reproduce boat-like force profiles if the physical machine remains a static erg.

## Codex / agent note

Use this paper sparingly. It is not a main source. It is useful for one limitation/footnote-level point: the real rowing hardware affects how closely land-based rowing approximates on-water rowing. In the thesis, cite it when saying the IK/avatar system is a representation layer and cannot fully reproduce on-water force/inertia mechanics from a static erg alone.

Do not expand this into a long sports-science section. The best use is a short limitation sentence or footnote after Soper & Hume/Lamb:
- Soper & Hume = broad biomechanics review.
- Lamb = kinematic comparison.
- Baca et al. = static Concept2 vs slides vs boat foot-stretcher force-profile nuance.
