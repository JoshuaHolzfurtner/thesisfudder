# Thesis notes — Kalckert & Ehrsson 2017, “The Onset Time of the Ownership Sensation in the Moving Rubber Hand Illusion”

## Citation identity

Kalckert, A., & Ehrsson, H. H. (2017). *The Onset Time of the Ownership Sensation in the Moving Rubber Hand Illusion*. Frontiers in Psychology, 8, Article 344. https://doi.org/10.3389/fpsyg.2017.00344

## What this paper is

This is an original experimental study on the moving rubber hand illusion. It investigates how long it takes for participants to begin experiencing ownership over a moving model hand when the model finger moves synchronously with the participant's hidden real finger.

It is not a VR rowing paper and not an avatar rowing paper. Its value for the XR rowing thesis is methodological: it gives a concrete timing reference for movement-based ownership illusions. It supports the idea that embodiment/ownership measures should not be collected immediately after exposure begins, because ownership may need time to build.

For the thesis, this is a high-priority source for evaluation design and test-duration justification, especially if the study asks participants to compare erg-centered and boat-centered representations.

## Content summary

The paper studies the onset time of ownership in the moving rubber hand illusion. In the moving rubber hand illusion, the participant's real hand is hidden inside a box while a visible model hand is placed above it. The model index finger moves either synchronously or asynchronously with the participant's real index finger. When the movements are synchronous, participants can experience the model hand as their own.

The authors tested 117 healthy participants. They compared active movement conditions, where participants intentionally moved their own finger, and passive movement conditions, where the experimenter moved the real and model fingers. In both cases, synchronous movement induced ownership, while asynchronous movement did not.

The paper first confirmed that synchronous movement produced higher ownership ratings than asynchronous movement. Approximately 80% of participants affirmed ownership in the active synchronous condition, and approximately 76% affirmed ownership in the passive synchronous condition.

The main contribution is the onset-time measurement. Participants who clearly experienced ownership in the synchronous condition but not in the asynchronous condition were tested again and asked to verbally indicate the moment when they felt that “the rubber hand was my hand.” This was repeated three times to calculate average onset time.

The average onset time was:
- active synchronous movement: approximately 22.8 seconds,
- passive synchronous movement: approximately 23.2 seconds.

Most participants experienced the illusion within the first minute. The 90th percentile was approximately:
- active synchronous: 50.0 seconds,
- passive synchronous: 50.6 seconds.

In a subgroup of participants who experienced the illusion in both active and passive synchronous conditions, active movement produced a slightly faster onset than passive movement. The active condition averaged about 20.9 seconds, while the passive condition averaged about 23.7 seconds. This suggests a possible facilitative effect of active movement, agency, or motor-control processes, although the difference is not the paper's only conclusion and should be worded cautiously.

The paper also discusses why this timing information matters for applied fields such as virtual reality, teleoperation, and prosthetic research. It notes that applied researchers want to induce ownership quickly and reliably, and that future studies may use onset time as an additional parameter for characterizing ownership illusions.

## Why it matters for the XR rowing thesis

This paper is useful because the XR rowing evaluation likely involves movement-based embodiment. Participants may need time to adapt to the virtual body, hands, handle, seat, oars, or avatar motion before they can give meaningful ownership/agency/location ratings.

The study supports a practical methodological rule:

- Do not measure ownership immediately after only a few seconds of exposure.
- Give participants at least a short stable familiarization period before asking embodiment questions.
- If comparing two conditions, give each condition enough time for ownership/agency impressions to develop before measurement.
- A one-minute minimum exposure has some support from moving rubber hand work, because most participants in this study reported ownership within the first minute.

This is especially relevant for your two modes:

1. Erg-centered / high-congruence mode:
   - likely easier to understand because real and virtual movement are closely aligned.
   - ownership/agency may build quickly if the hand/handle/avatar mapping is stable.

2. Boat-centered / sport-depiction mode:
   - may require more adaptation because the user physically pulls an erg handle while seeing oar-based rowing action.
   - short exposures might measure initial confusion rather than actual acceptability or embodiment.

Therefore, this source can justify including a familiarization period before collecting questionnaire ratings or performance data.

## Core findings / cheat sheet

- The moving rubber hand illusion can be induced by synchronous finger movement between the real hidden hand and visible model hand.
- Both active and passive synchronous movements can induce ownership.
- Asynchronous movement strongly reduces ownership.
- In a sample of 117 participants, about 80% affirmed ownership in active synchronous movement and about 76% in passive synchronous movement.
- Average ownership onset was approximately 22.8 seconds for active synchronous movement and 23.2 seconds for passive synchronous movement.
- Most participants experienced ownership within the first minute.
- The 90th percentile onset time was approximately 50 seconds for both active and passive synchronous movements.
- In a within-participant subgroup, active movement produced a slightly faster onset than passive movement.
- The authors suggest onset time may be a useful additional behavioral measure of ownership illusions.
- The paper is relevant for applied VR, teleoperation, and prosthetic research because designers need to know how long ownership induction may take.

## Relation to thesis concepts

### Body ownership

High relevance. The paper gives a concrete timing estimate for ownership emergence in a movement-based body illusion.

### Sense of agency

Moderate relevance. The paper compares active and passive movement. Active movement includes motor intention, efference copy, sensory prediction, and agency, while passive movement does not. The active condition showed slightly stronger/faster ownership in some analyses, suggesting that motor-control processes may facilitate ownership, but this should be worded cautiously.

### Visuomotor congruence

High relevance. The moving RHI depends on synchrony between seen model-hand movement and felt real-hand movement. This maps well to the erg-centered mode, where virtual hand/handle/avatar motion should follow the real handle/body motion.

### Temporal congruence

High relevance. Synchronous movement produced ownership; asynchronous movement reduced it. For XR rowing, timing between real handle movement and virtual avatar/oar response should be treated as a core design variable.

### Spatial congruence

Moderate relevance. The study used a model hand positioned above the real hand with a spatial offset. The discussion notes that virtual reality experiments often superimpose virtual hands more directly on real hand positions and may therefore provide more cues. It also notes that too-large discrepancies can abolish the illusion. This is relevant for offset virtual oar-arm IK.

### Evaluation timing

Very high relevance. This is the strongest thesis use. It gives a source-backed argument for a minimum familiarization/exposure period before embodiment ratings.

### Avatar embodiment

Indirect relevance. The paper is a rubber-hand setup, not a full avatar or VR rowing study. But it is relevant because it discusses ownership of simulated/robotic body parts and applications in VR and prosthetics.

### Tool-mediated rowing / virtual oars

Indirect relevance. The paper does not discuss tools or oars, but it warns that ownership-like experiences need time and depend on movement synchrony. This is important if the boat-centered mode uses offset oar IK or prerecorded/procedural rowing animation.

## How it maps to my thesis modes

### Erg-centered mode

The erg-centered mode should benefit from the kind of movement synchrony emphasized by this paper. If the virtual hands, handle, arms, and body follow the real handle/seat/body motion with low delay and stable spatial alignment, ownership and agency impressions may emerge quickly.

This paper can support a practical claim:
- The evaluation should allow enough time for participants to experience the movement mapping before measuring ownership.

### Boat-centered mode

The boat-centered mode may need more familiarization because the mapping is less literal. Participants physically pull a central erg handle, but see oar/boat motion. If the virtual oar-arm animation is temporally coherent and sport-legible, users may adapt; if not, the mismatch may weaken ownership/agency.

This paper does not prove that users can adapt to boat-centered offset IK. It only supports the timing point that movement-based ownership can emerge within about a minute when congruence is strong.

### Core tradeoff

The paper supports the central importance of congruent movement feedback:
- Erg-centered mode: direct visuomotor congruence.
- Boat-centered mode: potentially reduced direct hand/handle congruence but stronger sport-action depiction.

For the thesis, this suggests that the comparison should include enough exposure time to avoid measuring only initial confusion, especially for the boat-centered mode.

## What not to overclaim

- Do not claim this paper proves XR rowing avatar ownership.
- Do not claim a one-minute exposure guarantees embodiment in XR rowing.
- Do not claim active movement always creates stronger ownership than passive movement; the active advantage was limited and should be described cautiously.
- Do not claim moving rubber hand results transfer perfectly to full-body rowing avatars.
- Do not use this as evidence that offset oar IK will be embodied.
- Do not use it as a rowing or sport-VR source.
- Do not claim body ownership emerges instantly.
- Do not claim all participants experience ownership; responder rates vary.

## Thesis-use priority

High priority for:
- evaluation/test duration,
- familiarization period,
- movement-based ownership onset,
- justifying not measuring immediately,
- discussion of temporal buildup in embodiment measures.

Medium priority for:
- active versus passive movement,
- motor-control contribution to ownership,
- onset time as possible behavioral measure,
- VR/prosthetic application background.

Low priority for:
- rowing biomechanics,
- virtual rowing related work,
- tool use,
- threat response,
- vection,
- sport-action congruence.

Suggested placement:
- Methods: study procedure / familiarization phase.
- Evaluation design: condition duration and questionnaire timing.
- Theoretical background: movement-based body ownership.
- Discussion/limitations: embodiment effects need time and may depend on exposure duration.

## Candidate thesis paragraph

Kalckert and Ehrsson measured the onset time of ownership in the moving rubber hand illusion, in which a visible model finger moved synchronously or asynchronously with a participant's hidden real finger. In a large sample, synchronous movement induced ownership, with average onset times of approximately 23 seconds in both active and passive movement conditions, and most participants reporting ownership within the first minute. For the XR rowing study, this supports including a sufficient familiarization period before collecting embodiment ratings. In particular, the boat-centered mode may require users to interpret a less literal mapping between real erg-handle motion and virtual oar action, so very short exposures could measure initial confusion rather than stabilized ownership, agency, or acceptability.

## Candidate short thesis sentence

Kalckert and Ehrsson found that ownership in the moving rubber hand illusion typically emerged within the first minute, supporting the use of a familiarization period before measuring movement-based embodiment in XR rowing.

## Candidate footnote

In the moving rubber hand illusion, Kalckert and Ehrsson found mean ownership-onset times of about 23 seconds and 90th percentile onset times around 50 seconds, suggesting that movement-based ownership measures should allow at least a short period of stable exposure before assessment.

## Candidate glossary wording

### Ownership onset time

Ownership onset time is the time it takes until a participant first reports that an artificial or virtual body part feels like their own. In movement-based body illusions, ownership does not necessarily appear instantly. Kalckert and Ehrsson found that ownership in the moving rubber hand illusion emerged after roughly 23 seconds on average, with most participants reporting it within one minute. In XR rowing, this suggests that participants should be allowed to experience each avatar mapping for a sufficient period before answering embodiment questions.

### Familiarization period

A familiarization period is a short exposure phase before formal measurement. It allows users to understand the mapping between their real movement and the virtual body or tool. In XR rowing, this is especially important when comparing erg-centered and boat-centered modes, because the boat-centered mode may require users to interpret virtual oars as a sport-action representation rather than a literal copy of the real erg handle path.

## Codex / agent note

Use this paper as a high-priority methods source for timing and familiarization. It is not a core theory paper and not a rowing paper.

Core use:
- justify giving participants at least around one minute of stable interaction before embodiment ratings,
- explain that movement-based ownership can take time to emerge,
- avoid collecting ownership judgments immediately after condition onset,
- support the idea that onset time may be a useful additional measure.

Do not overuse:
- Do not cite it as proof that XR rowing avatar ownership will occur.
- Do not cite it as proof that offset oar IK is accepted.
- Do not generalize too strongly from a rubber-hand finger task to full-body rowing.
- Use it as a timing/familiarization reference only.

Best practical instruction for study design:
- For each condition, include a familiarization period before questionnaires.
- If possible, measure after a stable period rather than during the first few seconds.
- If comparing erg-centered and boat-centered modes, make sure both get comparable familiarization time.
