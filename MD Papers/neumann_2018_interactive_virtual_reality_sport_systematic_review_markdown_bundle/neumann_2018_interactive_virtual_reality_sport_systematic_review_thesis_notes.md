# Thesis notes — Neumann et al. 2018, “A systematic review of the application of interactive virtual reality to sport”

## Citation identity

Neumann, D. L., Moffitt, R. L., Thomas, P. R., Loveday, K., Watling, D. P., Lombard, C. L., Antonova, S., & Tremeer, M. A. (2018). *A systematic review of the application of interactive virtual reality to sport*. Virtual Reality, 22, 183-198. https://doi.org/10.1007/s10055-017-0320-5

Uploaded file:
`NeumannPUB4061-2.pdf`

## What this paper is

This is a systematic review of empirical research on interactive virtual reality applications in sport and sport-related exercise with healthy human participants. The review identifies 20 articles and codes them by study aim, participant characteristics, sport type, VR technology, measures, and findings.

For the XR rowing thesis, this is not an embodiment paper and not a rowing technique paper. Its value is broader:

- it defines what counts as interactive VR in sport,
- it separates VR sport from general exergaming,
- it shows that early interactive VR sport research was heavily concentrated in endurance tasks such as running, cycling, and rowing,
- it identifies recurring factors in VR sport outcomes: presence of others, competitiveness, task autonomy, immersion, attentional focus, and feedback.

This makes it a strong green-yellow source for the introduction and related-work bridge.

## Why it matters for the XR rowing thesis

The thesis compares two XR rowing representations:

1. **Erg-centered / high-congruence mode**
   - real erg handle, seat, and body movement are mapped closely to the avatar,
   - prioritizes visuomotor, temporal, spatial, haptic/proprioceptive, and agency congruence.

2. **Boat-centered / sport-depiction mode**
   - the user still rows on an ergometer,
   - the virtual avatar appears to row with oars in a boat,
   - prioritizes sport-action realism and rowing-specific depiction,
   - introduces mismatch because the virtual oar/hand path differs from the real erg handle trajectory.

Neumann et al. help define the broader category this thesis belongs to: interactive VR sport. They define VR sport as involving sport-relevant computer-generated content plus interaction between the athlete and the virtual environment. Their examples explicitly include exertion interfaces, such as physical effort on an ergometer being mapped to movement speed through a virtual race course.

This is highly useful because the thesis prototype is not just a visual demo or a passive 3D scene. It is an interactive sport system in which physical rowing action drives a virtual rowing representation.

## Core findings / cheat sheet

- The review identified 20 empirical articles applying interactive VR to sport or sport-related exercise.
- VR sport is defined around computer-generated sport-relevant content and user interaction with the virtual environment.
- The review distinguishes VR sport applications from exergames and from non-interactive video/visual displays.
- In sport VR, interaction can occur through exertion interfaces, including ergometers where physical effort changes virtual race-course movement.
- Many included studies focused on endurance-type sports or sport-related exercise, especially running, cycling, and rowing.
- Reported outcomes included performance, physiological, and psychological variables.
- Important factors included:
  - presence of others in the virtual environment,
  - competitiveness,
  - task autonomy,
  - immersion,
  - attentional focus,
  - feedback.
- The review notes that more research is needed for skill-based sport VR.
- It also recommends better reporting standards for VR sport research.

## What this adds beyond the existing thesis stack

Before this paper, the thesis already had strong sources for embodiment, RHI, agency, latency, and rowing technique. Neumann et al. add the **VR sport landscape frame**.

They help answer:

> Why is an ergometer-driven rowing system a VR sport system rather than just a fitness game or a visualization?

They also help justify a claim like:

> Prior interactive VR sport work has often examined endurance tasks such as cycling, running, and rowing, but has mainly targeted performance, motivation, feedback, or social factors rather than the embodiment tradeoff between physically congruent and sport-faithful representations.

This is one of the best “setup” citations for the introduction.

## Relation to thesis concepts

### Interactive VR sport

Very high relevance. This paper gives a clean category definition for interactive VR sport. The thesis prototype fits this category because a real rowing movement interface controls a virtual rowing environment and avatar representation.

### Exertion interface

High relevance. The review explicitly discusses exertion interfaces, where physical effort on machines such as ergometers is translated into virtual sport performance. This maps directly to rowing ergometers.

### VR rowing related work

High relevance. The review situates rowing alongside cycling and running as one of the endurance/sport-related tasks commonly studied in early VR sport research. This supports a compact related-work sentence without needing to explain every individual VR rowing paper.

### Sport vs exergaming

High relevance. This distinction is useful if the thesis wants to avoid sounding like a generic exergame thesis. Neumann et al. separate sport-related VR tasks from general active videogames by focusing on recognized sports and sport-relevant equipment/tasks.

### Presence and plausibility

Moderate relevance. The paper draws on presence/realistic response language, including Slater-style ideas, but Slater 2009 and Skarbez 2017 should remain the main sources for presence theory.

### Performance and motivation

Moderate relevance. Many included studies concern performance or psychological outcomes. Use this only to situate prior work, not as a claim that the present prototype improves performance.

### Embodiment

Low direct relevance. Neumann et al. do not provide a body-ownership or embodiment framework. Use Kilteni, Mottelson, Girondini, Kalckert/Ehrsson, VEQ, and Waltemate for embodiment.

### Rowing technique

Low direct relevance. The paper is not a rowing technique source. Use World Rowing/FISA, Lamb, Flood/Simpson, or rowing biomechanics sources for stroke-phase and erg-vs-boat claims.

## How it maps to my thesis modes

### Erg-centered mode

Neumann et al. support the general idea that a real exertion interface, such as an ergometer, can drive virtual sport performance. This helps frame the erg-centered mode as a clear interactive VR sport configuration: physical rowing action is tightly coupled to the virtual body/action outcome.

### Boat-centered mode

The review also helps frame the boat-centered mode as sport-relevant VR content: it maps real physical action into a computer-generated rowing environment. However, Neumann et al. do not address the mismatch problem between the real erg handle path and the virtual oar/boat motion.

### Core tradeoff

The paper does not directly answer the thesis tradeoff. Its contribution is to frame the research gap:

- prior VR sport systems translate physical activity into virtual sport content;
- prior research often studies performance, motivation, or social effects;
- the present thesis studies embodiment and representational mapping.

## Candidate thesis paragraph

Interactive VR sport can be understood as a sport-relevant computer-generated environment in which the athlete can interact with the virtual system through physical action. Neumann et al.’s systematic review notes that exertion interfaces, including ergometer-based mappings, can translate physical effort into virtual movement through a race course. This is useful for situating XR rowing as an interactive VR sport application rather than a passive visualization. However, much of the reviewed VR sport literature focuses on outcomes such as performance, physiological response, motivation, feedback, or social competition. The present thesis instead uses rowing as a test case for an embodiment-specific design problem: whether a virtual rowing body should prioritize close congruence with the real ergometer movement or a more sport-faithful depiction of on-water rowing with oars.

## Candidate short thesis sentence

Neumann et al. situate rowing within interactive VR sport, where physical athlete action can be mapped through an exertion interface into a sport-relevant virtual environment.

## Candidate glossary wording

### Interactive VR sport

Interactive VR sport describes a system in which sport-relevant computer-generated content responds to the user’s physical actions. In rowing, this can mean that an ergometer or other rowing interface controls virtual movement through a race course or environment.

### Exertion interface

An exertion interface is a physical exercise or sport device through which the user’s bodily effort is translated into virtual action. In XR rowing, the ergometer functions as an exertion interface: real pulling, seat movement, and effort become virtual rowing movement and avatar/boat response.

### VR sport versus exergame

VR sport systems use sport-relevant tasks, equipment, or performance mappings, while exergames may promote physical activity through game-like movement without necessarily preserving a recognized sport task. The thesis should frame XR rowing as VR sport, not merely as an exergame, because it preserves the rowing ergometer as the physical input device and compares different sport representations.

## What not to overclaim

- Do not cite this paper as evidence for body ownership or agency.
- Do not claim it proves VR rowing embodiment.
- Do not claim VR sport generally improves performance in all contexts.
- Do not claim screen/projection VR and HMD XR are equivalent.
- Do not claim all exergames are VR sport.
- Do not use it for detailed rowing technique or erg-vs-boat biomechanics.
- Do not let this paper shift the thesis toward performance enhancement; it is mainly a landscape and definition source.

## Thesis-use priority

High priority for:
- introduction,
- VR sport related work,
- defining interactive VR sport,
- distinguishing VR sport from generic exergames,
- showing that rowing has appeared in interactive VR sport research.

Medium priority for:
- motivation/performance prior-work framing,
- social/competitor/factor overview,
- explaining why many prior studies are not embodiment-focused.

Low priority for:
- body ownership,
- agency,
- self-location,
- rowing technique,
- IK,
- spatial alignment,
- threat response.

Suggested placement:
- Introduction: one paragraph placing XR rowing in interactive VR sport.
- Related work: compact VR sport/rowing table.
- Discussion: explain how the thesis differs from performance/motivation-oriented VR sport work.

## Codex / agent note

Use Neumann et al. 2018 as a green-yellow source for framing the thesis as interactive VR sport. It is not an embodiment paper.

Best use:
- define interactive VR sport,
- mention exertion interfaces such as ergometers,
- situate rowing as part of early VR sport research,
- show that prior VR sport work often focuses on performance, physiology, psychology, competitiveness, presence of others, feedback, and immersion.

Core thesis contrast:
- Existing interactive VR sport literature supports the general category.
- This thesis contributes a more specific embodiment comparison: erg-centered physical congruence vs boat-centered sport depiction.

Do not use:
- for ownership/agency theory,
- for rowing biomechanics,
- for questionnaire design,
- as proof that VR rowing improves technique.
