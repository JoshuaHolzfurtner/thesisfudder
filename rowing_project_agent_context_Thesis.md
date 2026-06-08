## 12. Thesis/research track: VR rowing embodiment

This project overlaps with a thesis about VR rowing embodiment. The current favored title direction is approximately:

> Visuomotor congruence or realistic sport depiction in virtual reality indoor rowing: a comparison of ergometer-based and boat-based avatar embodiment.



### 12.1 Core research contrast

Two VR rowing embodiment conditions are being compared:

#### Condition 1: Ergometer-congruent / erg-centric IK

The virtual handle closely matches the real erg handle.

Characteristics:

- Real erg handle and virtual handle align as closely as possible.
- Strong visuomotor congruence between what user feels and what user sees.
- The erg handle is the tactile/visual anchor.
- Seat position may be inferred/tracked from alignment.
- Head + hands + inferred hips/seat can drive full-body approximation.
- May feel less like being in a real boat, but more spatially congruent to the actual body/action.

#### Condition 2: Boat-realistic / boat-centric IK

The user sees themselves rowing in a boat with oars, but the hand/oar kinematics differ from the erg’s straight-line handle path.

Characteristics:

- Visual scene matches sport depiction more realistically: boat, oars, water.
- Hands are IK retargeted to an oar arc rather than straight erg handle motion.
- The rigid handle/finger contact still gives some congruence,and also the finger animations are still fully retargeted to miniimized the incongruency.
- More realistic as rowing imagery, less congruent as exact motor mapping.
- The key difference from condition 1 should be how arms/hands are driven.

### 12.2 Experimental principle

The deliberate difference between the two conditions should be constrained:

- Same realistic VR environment where possible.
- Same user/task/session duration where possible.
- Same base avatar quality where possible.
- Main manipulated difference: erg-congruent handle/body mapping vs boat-realistic oar/hand mapping.

Do not introduce confounds casually. If one condition has better visuals, more fun, more feedback, better lighting, or different latency, it can contaminate the comparison.

### 12.3 Embodiment terms

Relevant conceptual terms:

- Sense of embodiment (SoE).
- Body ownership / sense of ownership (SoO).
- Sense of agency (SoA).
- Self-location / sense of self-location (SoL).
- Bodily self-consciousness.
- Multisensory integration.
- Visuomotor congruence.
- Visuotactile congruence.
- Proprioceptive alignment.
- Temporal synchrony / latency.
- Body schema and tool extension, but use cautiously.

Joshua is converging on **visuomotor congruence** as the umbrella term for spatial/kinematic matching between seen and performed movement, possibly including timing/latency aspects.

### 12.4 Rubber hand illusion analogy

The setup can be framed as a kind of RHI-inspired extension, but carefully.

Analogy:

- In RHI, synchronous visual and tactile cues can induce ownership over a rubber hand.
- In the erg-congruent mode, the real erg handle acts as a tactile/visual anchor similar to the brush/touch synchrony logic.
- In boat mode, the mapping is less exact but still partially anchored by rigid handle/finger contact.

Safe wording:

- “RHI-style logic” or “inspired by multisensory congruence paradigms.”
- Do not claim the rowing setup is simply a rubber hand illusion.
- Do not claim the handle becomes part of the self unless actually measured.

### 12.5 Tool/body extension caution

Joshua likes the sword/handle/tool-extension idea conceptually, but it may not be central to the thesis.

Current stance:

- Tool extension literature may be useful as a bridge, but do not overstate it.
- The thesis does not primarily measure “the handle becomes part of me.”
- The handle is more relevant as a sensorimotor/tactile anchor than as an ownership target.
- If included, put it in a short glossary/footnote, not as a main claim.

### 12.6 Latency

Latency matters for agency/ownership.

Notes from prior discussions:

- Virtual Desktop can add around 50 ms.
- Total delays above around 100 ms can start degrading agency/ownership feelings according to general literature, though exact thresholds vary.
- Discrepancies around 150 ms have been discussed as reducing agency in some contexts.
- Joshua personally observed that below ~100 ms can still feel like a rubber glove attached, but this is personal observation, not formal evidence.
- Stroke direction changes/turnaround detection can create local perceived delays, even if average tracking latency is acceptable.

Thesis/product guidance:

- Document latency explicitly.
- Distinguish system latency, network/streaming latency, input processing delay, and animation event delay.
- Do not hide this as an implementation detail; it can affect embodiment.

### 12.7 Measures

Possible measures discussed:

- Embodiment questionnaires.
- Ownership/agency/self-location subscales.
- Pre/post measures.
- Threat/protectiveness-style responses, e.g. fake threat visuals and heart-rate jump.
- Heart-rate as a correlate, not a replacement for ownership.

Do not claim physiological threat response proves ownership by itself.

---
