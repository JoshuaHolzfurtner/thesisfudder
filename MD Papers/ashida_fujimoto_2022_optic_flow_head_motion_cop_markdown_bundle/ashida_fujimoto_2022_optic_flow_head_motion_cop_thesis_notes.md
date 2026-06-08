# Thesis notes — Ashida & Fujimoto 2022, “Comparing measurements of head motion and centre of pressure for body sway induced by optic flow on a head-mounted display”

## Citation identity
Ashida, H., & Fujimoto, K. (2022). *Comparing measurements of head motion and centre of pressure for body sway induced by optic flow on a head-mounted display*. Frontiers in Virtual Reality, 3, Article 1026718. https://doi.org/10.3389/frvir.2022.1026718

## What this paper is
This is a brief VR perception / optic-flow / postural-control measurement study. It compares two ways of measuring visually induced body sway while participants stand still and view optic-flow stimuli in a head-mounted display:

- head motion measured through the HMD tracking system;
- centre of pressure (CoP) measured with a force-plate-like Wii Balance Board.

The stimulus was deliberately simple: a radial dot-field optic flow shown in an Oculus Rift CV1. The dot field simulated alternating forward and backward self-motion by expanding and contracting. Participants stood on the balance board, wore the HMD, and were asked to stand still while looking at the centre of the optic flow. After trials, participants gave a subjective body-movement rating from 0 to 100.

The study is not about rowing, cycling, exergaming, or avatar embodiment. It is useful because it shows that even abstract optic-flow stimulation in VR can produce measurable bodily/postural responses, and that HMD head tracking may approximate traditional CoP sway measures under the tested conditions.

## Why it matters for the XR rowing thesis
My thesis compares:

1. Erg-centered / high-congruence XR rowing:
    - real erg handle/seat/body motion mapped closely to the virtual avatar;
    - prioritizes visuomotor, spatial, temporal, haptic/proprioceptive congruence.
2. Boat-centered / sport-depiction XR rowing:
    - user still rows on an erg;
    - virtual avatar appears to row in a boat with oars/oarlocks/blades;
    - prioritizes sport-action realism;
    - introduces mismatch because virtual oar handles move differently from the real erg handle.

This paper does not answer the main embodiment comparison. Its value is narrower: it supports the optic-flow / vection / VR-measurement side of the thesis.

The paper is useful for arguing that visual self-motion cues in HMD VR are not merely decorative. Even a rudimentary radial dot-field can produce subjective feelings of body movement and measurable postural responses. This helps support the idea that effort-coupled rowing scenery, water flow, shoreline motion, and route progression may have perceptual consequences beyond simple visual feedback.

However, the paper should not be used to claim that XR rowing users necessarily experience vection, embodiment, or body ownership. It shows a controlled optic-flow/postural-response effect, not rowing-specific embodiment.

## Core findings / cheat sheet

- **Optic flow induced strong subjective body-movement ratings.**
  - Baseline stationary dots produced a much lower subjective movement rating than the optic-flow conditions.
  - Why it matters: even abstract dot-flow in an HMD can make participants report a strong feeling of body movement.
  - Use strength: good for optic-flow/vection background, but not as proof of rowing-specific vection.

- **Optic flow induced measurable postural/body-sway responses.**
  - Head motion and CoP were modulated by the forward/backward optic-flow changes.
  - Why it matters: visual self-motion cues can influence the body’s postural system.
  - Use strength: useful as objective bodily-response support, but not a direct “embodiment measure.”

- **HMD-tracked head motion resembled centre-of-pressure sway.**
  - Head motion and CoP had similar time-course shapes, high correlations, no clear relative temporal delay, similar frequency-domain stimulus peaks, and strong phase-lag correlations.
  - Why it matters: HMD telemetry may be a practical auxiliary measurement channel in VR studies.
  - Use strength: good for a methods/future-work note.

- **The measures were similar, but not identical.**
  - CoP amplitude was smaller than head motion, and detrended fluctuation analysis suggested some differences in signal smoothness.
  - Why it matters: HMD head tracking should not be treated as a perfect substitute for full-body or force-plate measurement in all conditions.
  - Use strength: important caveat.

- **The authors explicitly limit the generality.**
  - They tested anterior-posterior sway, forward/backward optic flow, relatively slow direction changes, standing posture, and a specific HMD/measurement setup.
  - Why it matters: the result should not be generalized too freely to seated rowing, rich environments, waves, oars, or clinical balance assessment.

## Relation to thesis concepts

### Optic flow
This is the most relevant concept. The paper presents optic flow as visual stimulation that can induce a feeling of self-motion and influence postural control. It supports the thesis glossary distinction between optic flow as the visual motion pattern and vection as a subjective self-motion feeling that may arise from it.

### Vection
The paper links optic flow to vection and reports subjective body-movement ratings. It is useful as support that HMD optic flow can create a self-motion-like experience. However, it should be framed as a vection-related bodily/postural response, not as a pure or direct measurement of vection.

### Spatial presence / Place Illusion
Indirect only. The paper does not measure presence or Place Illusion. Still, it helps explain why visual motion in VR can become bodily meaningful: the body reacts to self-motion cues even when the physical body is stationary.

### Temporal congruence / latency
The paper is relevant because it compares the timing of head motion and CoP responses. For the thesis, it can be mentioned as part of the broader idea that visual-motion cues and body responses can be analyzed in time and frequency domains.

### Visuomotor congruence
Indirect only. The participants did not actively move through the scene, and the visual movement was not caused by their own action. Therefore, it does not test visuomotor congruence in the rowing sense. It is more about visual-postural coupling.

### Action-outcome congruence
Not directly relevant. In this paper, optic flow is externally presented rather than being coupled to participant action. For XR rowing, this distinction is important: rowing would ideally make optic flow action-coupled, whereas this paper studies passive visual motion.

### VR motion sickness / cybersickness
The paper is relevant only as background. It notes that vection can be useful in assessing VR experiences as an indicator of immersion and possibly sickness, but it does not provide a cybersickness study. Do not use it as direct evidence that head motion detects cybersickness.

### Evaluation / measurement
This is a useful measurement paper. It supports the idea that HMD head tracking may provide a lightweight auxiliary signal for bodily responses to visual motion. For a thesis or future work section, this can motivate logging headset motion during XR rowing to explore whether visual locomotion, waves, or boat motion create measurable postural/head responses.

## How it maps to my thesis modes

### Erg-centered mode
The paper is only indirectly relevant. In an erg-centered rowing mode, the user is seated and physically constrained by the rowing machine, so standing postural sway is not the main response. However, HMD head motion could still be logged as a lightweight signal for discomfort, visual-motion response, or motion-coupling effects.

Use cautiously:
- The paper supports head-motion telemetry as potentially meaningful in HMD optic-flow studies.
- It does not prove anything about seated rowing embodiment.

### Boat-centered mode
The boat-centered mode may produce stronger visual self-motion cues through water flow, shoreline motion, boat travel, and possibly wave/boat motion. This paper supports the general idea that optic-flow cues in HMD VR can create bodily responses.

Use cautiously:
- It supports the idea that visual motion cues can affect the body.
- It does not test realistic rowing scenes, oars, water, waves, or sport-action realism.

### Core tradeoff
The paper does not directly contribute to the central tradeoff between bodily/device congruence and sport-action congruence.

Its contribution is adjacent:

- It supports optic flow and visually induced self-motion as bodily meaningful in VR.
- It suggests built-in HMD tracking can serve as a lightweight auxiliary measure.
- It reminds the thesis that visual realism and visual motion can have bodily effects even when the user is physically stationary.

## What not to overclaim

- Do not claim this proves XR rowing embodiment.
- Do not claim this proves body ownership, agency, or self-location in rowing.
- Do not claim this proves virtual rowing creates vection.
- Do not claim postural sway is a direct or exclusive measure of vection.
- Do not claim head tracking replaces force plates or full-body tracking in all VR studies.
- Do not claim standing optic-flow sway generalizes cleanly to seated rowing.
- Do not claim a dot-field optic-flow experiment is equivalent to a rich rowing environment.
- Do not claim this proves cybersickness can be detected from head motion.
- Do not claim that more optic flow is always better; visual motion can also contribute to discomfort, instability, or sickness.

## Thesis-use priority

High priority for:
- Optic-flow / vection background if that section becomes important.
- Objective-ish bodily correlates of visual self-motion.
- HMD telemetry as future-work measurement.

Medium priority for:
- Evaluation-methods discussion.
- Cybersickness / comfort / visually guided postural-control background.
- Arguing that visual self-motion cues in VR are bodily meaningful.

Low priority for:
- Core embodiment theory.
- Body ownership.
- Sense of agency.
- Avatar realism.
- Rowing biomechanics.
- Erg-centered vs boat-centered mode comparison.

Suggested placement:
- Theoretical background: optic flow / vection subsection.
- Methods or discussion: optional auxiliary measurement / future work.
- Discussion: caution that visual locomotion in HMD VR can affect bodily/postural systems.
- Not a central source for the main embodiment argument.

## Candidate thesis paragraph
Optic flow is relevant to XR rowing not only as a visual design element, but as a perceptual cue for self-motion that can influence bodily responses. Ashida and Fujimoto showed that radial optic-flow stimuli presented in an HMD produced strong subjective body-movement ratings and measurable postural responses, and that HMD-tracked head motion closely resembled centre-of-pressure measurements under their tested conditions. For XR rowing, this suggests that effort-coupled visual motion, such as water and shoreline movement, may become bodily meaningful rather than merely decorative. However, the study used standing participants and abstract dot-field motion, so it should only be used as background evidence for optic-flow-induced self-motion and possible auxiliary measurement, not as direct evidence for rowing embodiment.

## Candidate short thesis sentence
Even abstract HMD optic-flow stimuli can induce subjective self-motion-related reports and measurable postural responses, suggesting that visual locomotion cues in XR exercise may have bodily effects beyond simple scenery motion.

## Codex / agent note
Use this paper narrowly. It is not a rowing or embodiment source. It is best used for the optic-flow/vection/measurability section and possibly future work on logging HMD head motion during XR rowing. Preserve the distinction between optic flow, vection, and postural response. The tempting sentence “optic flow scientifically proves vection” is too strong. Better wording: “optic-flow-induced postural sway can serve as an objective bodily correlate or auxiliary measure of visually induced self-motion, but it is not a direct vection meter.”

Important phrasing for thesis:
- “objective bodily correlate” is safer than “objective measure of vection.”
- “rudimentary dot-field optic flow can induce subjective body-motion ratings and measurable postural responses” is safe.
- “transplant vection into the user” is too strong unless rewritten as “visually induce self-motion-related experience.”
