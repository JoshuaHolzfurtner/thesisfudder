# Thesis notes — Kooijman et al. 2024, “Measuring vection: a review and critical evaluation of different methods for quantifying illusory self-motion”

## Citation identity

Kooijman, L., Berti, S., Asadi, H., Nahavandi, S., & Keshavarz, B. (2024). *Measuring vection: a review and critical evaluation of different methods for quantifying illusory self-motion*. Behavior Research Methods, 56, 2292–2310. https://doi.org/10.3758/s13428-023-02148-8

## What this paper is

This is a measurement-focused review paper about vection. It does not study rowing, cycling, XR rowing, avatars, or embodiment directly. Its purpose is to review and critically evaluate the subjective methods researchers use to quantify vection, because objective or physiological measures are not yet established enough to replace subjective measures.

For the XR rowing thesis, this is the practical companion to Palmisano et al. 2015:
- Palmisano et al. 2015 = definition and conceptual challenges.
- Kooijman et al. 2024 = how to measure vection, and why measurement is messy.

## Content summary

The paper opens by defining vection as the subjective experience of self-motion in the absence of actual physical motion. It uses the classic “train illusion” as an example: a person sitting in a stationary train may feel as if their own train is moving when an adjacent train starts moving.

The authors explain that vection research has existed for over a century, but measurement remains difficult. Researchers often rely on subjective methods because objective measures or physiological correlates have not yet clearly emerged as robust standard methods.

The review groups vection measures into four broad categories:

1. Occurrence of vection
   - whether vection happened at all.
   - examples: yes/no binary choice, button press, verbal report.

2. Temporal characteristics of vection
   - when vection starts, how long it lasts, how it builds up, or when it drops out.
   - examples: onset latency, duration, build-up time, dropout.

3. Quality of the vection experience
   - how strong, intense, convincing, compelling, or saturated the vection felt.
   - examples: rating scales, magnitude estimation, two-alternative forced choice.

4. Indirect measures
   - measures that do not ask directly about vection but infer something about self-motion experience.
   - examples: perceived distance travelled, perceived ego-velocity, pointing tasks.

A major theme is that no single measure captures vection perfectly. Different measures answer different questions. For example, a binary yes/no response is simple, but loses detail. A rating scale can capture intensity or convincingness, but results depend heavily on wording and scale design. Temporal measures such as onset latency and duration can give richer time-course information, but they require clear instructions and may be affected by participant uncertainty or mental demands. Indirect measures such as distance travelled or ego-velocity may tell us something about functional self-motion perception, but they do not directly measure vection.

The paper also emphasizes that vection is not only a visual phenomenon. It can be multisensory and can be affected by auditory, biomechanical, tactile, or redundant sensory cues. Still, the paper’s focus is not on all vection theory, but on measurement practice.

The conclusion is methodological: researchers should explicitly define what they mean by vection, select measures that match the research question, consider combining measures, and report their instructions, scales, stimuli, and settings transparently so that studies can be compared.

## Why it matters for the XR rowing thesis

This paper is useful if the thesis mentions vection in evaluation, questionnaire design, or future work.

The XR rowing system almost certainly provides optic-flow cues and virtual locomotion cues: moving water, shoreline motion, route progression, boat movement, and effort-coupled forward travel. However, unless the study actually measures vection, the thesis should only say that the system may support vection.

Kooijman et al. are useful because they explain what would be needed to measure that claim more carefully:
- ask whether the user experienced self-motion,
- ask how strong or convincing it was,
- possibly ask whether it started quickly or lasted throughout the condition,
- and avoid confusing vection with presence, cybersickness, or visual motion alone.

This paper also supports a possible future-work claim: a later study could compare whether erg-centered and boat-centered XR rowing produce different vection ratings, even if the present thesis focuses mainly on embodiment and congruence.

## Core findings / cheat sheet

- Vection is the subjective experience of self-motion without actual physical motion.
- Objective or physiological vection measures are not yet established as robust standard measures, so subjective measures remain dominant.
- Vection measurement methods can be grouped into occurrence, temporal characteristics, quality of experience, and indirect measures.
- Occurrence measures are simple but coarse.
- Temporal measures such as latency, duration, build-up time, and dropout describe the time course of vection.
- Quality measures such as intensity, convincingness, compellingness, and saturation describe what vection felt like.
- Rating scales are easy to implement and sensitive to differences, but scale wording and intervals affect comparability.
- Magnitude estimation can be sensitive, but standard stimuli, anchoring, and between-participant variation complicate interpretation.
- Two-alternative forced choice can reduce some response bias, but may force a choice even when neither stimulus produced vection.
- Indirect measures such as distance travelled, ego-velocity, and pointing tasks can investigate functional self-motion processing, but do not directly measure vection.
- The authors recommend selecting measures based on the research question and the specific aspect of vection being studied.
- They recommend combining measures when appropriate.
- They strongly emphasize transparent reporting of definitions, instructions, stimuli, scales, and settings.

## Relation to thesis concepts

### Vection

High relevance. This paper is the measurement anchor for vection. It is useful if vection appears in the glossary, questionnaire, evaluation section, or future work.

### Optic flow

Relevant indirectly. Optic flow may induce vection, but this paper is less about optic-flow theory and more about how to measure the resulting subjective self-motion experience.

### Virtual locomotion

Relevant. XR rowing uses stationary effort to create virtual locomotion. Kooijman et al. help define how the subjective self-motion layer could be measured.

### Anti-Sisyphus effect

Useful as future-work support. If the “anti-Sisyphus” effect means that stationary effort feels like meaningful movement through a world, vection could be one measurable part of that effect. But vection is not the whole effect; enjoyment, agency, progress, motivation, and flow may also matter.

### Presence

Relevant but separate. The paper notes that vection and presence have been positively associated in prior work, but it does not collapse the two concepts. For the thesis, vection should stay separate from presence and embodiment.

### Embodiment

Indirect relevance only. Vection does not measure body ownership or avatar embodiment. It measures perceived self-motion. It may be a secondary or future-work construct, not a core embodiment construct.

### Sense of agency

Indirect relevance. If the user’s rowing effort controls virtual movement, vection may interact with action-outcome congruence, but it is not agency by itself. A user can feel self-motion without feeling they caused it, and can feel agency without strong vection.

### Evaluation / questionnaire design

Very relevant. This paper is the best source so far for deciding whether and how to include vection items.

Possible minimal questionnaire use:
- Did you feel as if you were moving through the virtual environment?
- How strong was the sensation that you were moving?
- How convincing was the sensation of moving through the virtual rowing scene?
- Did the sensation of movement last throughout the trial, or only during parts of it?

For the current thesis, a light approach may be enough: one or two exploratory vection items rather than a full vection protocol.

## How it maps to my thesis modes

### Erg-centered mode

In the erg-centered mode, the avatar and handle may align more closely with the real rowing machine. This may support action-outcome congruence and agency, but it does not automatically imply stronger vection.

A future study could ask whether precise physical congruence affects vection indirectly by making the virtual forward movement feel more self-caused.

### Boat-centered mode

In the boat-centered mode, the visual scene may look more like actual on-water travel. The user sees a boat, water, oars, shoreline, and route progression. This might support stronger vection because the self-motion interpretation is more sport-natural.

However, this is not proven by the paper. Kooijman et al. only help define how such a question could be measured.

### Core tradeoff

The core thesis tradeoff remains bodily/device congruence versus sport-action congruence. Vection is an adjacent construct. It may help explain the virtual-locomotion layer, but it should not replace the embodiment question.

A possible future-work question:
- Does boat-centered sport depiction increase vection because it presents a more natural visual self-motion context?
- Or does erg-centered congruence increase perceived self-caused locomotion because the movement is better aligned with the real action?

## What not to overclaim

- Do not claim that vection is measured objectively by default.
- Do not claim one questionnaire item is a complete vection measure.
- Do not claim vection equals optic flow.
- Do not claim vection equals presence.
- Do not claim vection equals embodiment.
- Do not claim vection proves body ownership or agency.
- Do not claim indirect measures such as distance travelled directly measure vection.
- Do not claim that a binary yes/no item captures intensity or quality.
- Do not compare vection results across studies without checking definitions, stimuli, scales, and instructions.
- Do not make vection a central thesis construct unless it is actually measured with enough care.

## Thesis-use priority

High priority for:
- future-work evaluation of vection,
- questionnaire design,
- measurement caveats,
- explaining why vection should be treated carefully,
- distinguishing occurrence, intensity, duration, and indirect self-motion measures.

Medium priority for:
- glossary support,
- anti-Sisyphus effect,
- virtual locomotion discussion,
- presence/VR app context.

Low priority for:
- core embodiment theory,
- body ownership,
- avatar morphology,
- rowing biomechanics,
- erg-vs-boat kinematics,
- proving the thesis hypothesis.

Suggested placement:
- Evaluation methods, if vection is measured.
- Future work, if vection is not measured.
- Short theoretical-background note after Palmisano et al. 2015.
- Optional appendix note on questionnaire construction.

## Candidate thesis paragraph

Kooijman et al. review the main methods used to measure vection, defined as the subjective experience of self-motion in the absence of actual physical motion. They show that vection measurement is not standardized and that common measures capture different aspects of the experience, including occurrence, onset latency, duration, intensity, convincingness, magnitude estimation, and indirect estimates such as perceived distance travelled. For XR rowing, this suggests that vection should not be assumed merely because the environment provides optic-flow cues. If the study aims to evaluate whether stationary rowing felt like movement through a virtual environment, vection should be measured explicitly and kept separate from embodiment, presence, and agency.

## Candidate short thesis sentence

Kooijman et al. show that vection can be measured through occurrence, temporal, quality, and indirect self-motion measures, but that no single measure captures the construct completely.

## Candidate glossary wording

### Vection measurement

Vection can be measured in several different ways. Researchers may ask whether vection occurred at all, when it started, how long it lasted, how strong or convincing it felt, or how far/fast the participant felt they travelled. These measures do not all capture the same aspect of the experience. Therefore, in XR rowing, a simple item such as “I felt as if I was moving through the virtual environment” can be useful as an exploratory measure, but it should not be treated as a complete vection protocol.

### Occurrence, intensity, and duration

A user may experience vection only briefly, weakly, or not at all. Therefore, vection should not be treated as a binary all-or-nothing phenomenon unless the study only needs to know whether it occurred. If the research question concerns differences between XR rowing modes, intensity and convincingness ratings may be more useful than only asking yes/no.

## Codex / agent note

Use this paper as the measurement anchor for vection. Palmisano et al. 2015 should remain the conceptual definition anchor. Kooijman et al. 2024 should be used whenever the thesis discusses how vection could be measured, especially in future work or exploratory questionnaire design.

Recommended agent memory:
- Vection should be separated from optic flow, presence, embodiment, and agency.
- If vection is measured, specify which aspect is measured: occurrence, latency, duration, intensity, convincingness, magnitude, or indirect self-motion estimate.
- For the current thesis, do not overbuild a full vection study unless the evaluation really includes it.
- Best minimal use: one or two exploratory items about felt movement through the environment, clearly marked as exploratory.
- Stronger future work: compare erg-centered and boat-centered modes for vection intensity/convincingness and perceived self-caused locomotion.
