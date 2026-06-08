# Thesis notes — Skarbez, Brooks & Whitton (2017), “A Survey of Presence and Related Concepts”

## Citation identity

Skarbez, R., Brooks, F. P. Jr., & Whitton, M. C. (2017). A Survey of Presence and Related Concepts. *ACM Computing Surveys*, 50(6), Article 96.

## What this paper is

This is a broad, high-value survey of presence and related constructs in virtual environments. It reviews:
- presence,
- immersion,
- social presence,
- copresence,
- realism and fidelity,
- Place Illusion and Plausibility Illusion,
- coherence,
- embodiment,
- body ownership,
- self-presence,
- agency,
- transportation,
- reality judgment,
- presence models,
- presence measurement.

For the XR rowing thesis, this paper is useful as a construct-cleanup and terminology source. It helps prevent “presence,” “immersion,” “realism,” “embodiment,” and “agency” from being mixed into one vague concept.

## Why it is core-relevant for the thesis

Your thesis compares:
- an erg-centered, high-visuomotor-congruence mode,
- a boat-centered, sport-realistic but less movement-congruent mode.

That comparison touches several constructs at once:
- embodiment: ownership, agency, self-location toward the avatar/body,
- presence / Place Illusion: feeling located in the virtual environment,
- Plausibility Illusion: feeling that what happens in the virtual scene is really happening,
- fidelity: how closely the virtual system emulates rowing / erg / boat interaction,
- coherence: whether the virtual scenario behaves consistently with the user’s expectations,
- agency: whether the user feels they cause the stroke/avatar/oar/boat motion.

Skarbez et al. helps organize these as distinct but related constructs.

## Core thesis-use takeaways

### 1) Presence is not the same as embodiment

Presence is most commonly associated with the sense of “being there” in a virtual environment. Embodiment concerns the body/avatar and the feeling that a body or body part is processed as one’s own.

Thesis implication:
- “I feel present on the river” is not the same as “these avatar arms/body are mine.”
- A participant could feel present in the rowing scene but not own the avatar.
- A participant could feel agency over the rowing action without strong Place Illusion.

Use presence/presence-like measures as complementary, not interchangeable with SoE.

### 2) Immersion should be treated as a system property, not just a feeling

The survey follows Slater in treating immersion as an objective property of the VE system: what valid actions and sensory channels the system supports.

Thesis implication:
- High-resolution graphics, HMD field of view, tracking, hand input, seat/handle tracking, audio, and interaction possibilities are immersion/system features.
- The user’s subjective response to those features is presence / Place Illusion / plausibility / embodiment, not immersion itself.

This is useful for precise writing:
- Avoid saying “participants had more immersion” if you mean “participants reported more presence.”
- Say “the system provides higher interaction fidelity/immersion” vs “participants experienced higher presence.”

### 3) Presence is not automatically task performance

The paper warns that more presence is not necessarily always better for task performance, and that evidence linking presence and performance is mixed.

Thesis implication:
- Do not assume the more visually realistic boat mode is better because it may feel more present.
- Do not assume the more physically congruent erg mode is better because it may support performance.
- Keep outcome measures separate: embodiment, realism/presence, agency, performance/form metrics.

### 4) Place Illusion vs Plausibility Illusion is a strong lens

The paper reviews Slater’s distinction:
- Place Illusion: the illusion of being in a place.
- Plausibility Illusion: the illusion that what is apparently happening is really happening.

Thesis implication:
- Boat-centered mode may increase Plausibility Illusion for rowing as a sport depiction because it shows a plausible boat/oar action.
- Erg-centered mode may increase sensorimotor plausibility for the user’s own body because the avatar motion matches the real handle/seat.
- Both modes could produce Place Illusion if the river/rowing environment is convincing, but they differ in bodily/action plausibility.

This helps separate:
- “I feel like I am on a river”
from
- “I feel like this rowing stroke is really happening through my body.”

### 5) Coherence may be more useful than realism alone

The survey discusses coherence as internal logical and behavioral consistency: does the VE behave in a way that fits the scenario and user expectations?

Thesis implication:
- The boat mode does not need to be perfectly physically identical to on-water rowing; it must be coherent enough that the avatar/oar/boat behavior makes sense.
- The erg mode may be less sport-realistic but highly coherent with the physical device.
- Mismatches become problematic when they are incoherent: e.g., the user’s handle goes straight while the virtual hands/oars visibly do something that violates expectations without explanation.

Coherence is a great term for your erg-vs-boat dilemma.

### 6) Fidelity can be separated into different dimensions

The paper discusses fidelity as the extent to which a VE emulates the real world and mentions physical, functional, psychological, stimulus, experiential, and action fidelity.

Thesis implication:
Your two modes emphasize different fidelities:
- Erg-centered mode: high physical/action fidelity to the indoor erg task.
- Boat-centered mode: higher visual/sport depiction fidelity to on-water rowing.
- Neither is simply “more realistic” overall; each is realistic with respect to a different reference.

This is a key conceptual cleanup:
Do not write “boat mode is more realistic” without specifying realistic relative to what.
Say “boat mode is more faithful to on-water sport depiction, while erg mode is more faithful to the user’s physical indoor rowing action.”

### 7) Valid actions matter

Many presence models include action possibilities, sensorimotor valid actions, or supported action as central. The survey links presence to affordances and valid perception/action coupling.

Thesis implication:
- Rowing is action-heavy. The system should not be judged only by visual resemblance.
- The erg-centered mode supports valid actions relative to the real erg.
- The boat-centered mode supports visually meaningful rowing actions, but the action validity may be partially transformed.

This supports your central comparison.

### 8) Embodiment section is directly useful for glossary cleanup

The survey distinguishes computing usage of embodiment (the representation of a user/avatar in a VE) from psychology/philosophy usage (subjective experience of having/using a body). It then references Kilteni et al.’s SoE framework: self-location, agency, and body ownership.

Thesis implication:
- State clearly which sense of “embodiment” you use.
- For this thesis, use sense of embodiment as subjective avatar/body experience, not merely the existence of an avatar model.
- Avoid “embodiment” meaning just “avatar representation.”

## How it maps to your thesis modes

### Erg-centered mode

Likely strengths:
- high action fidelity to real erg interaction,
- high physical/tactile/proprioceptive coherence,
- strong visuomotor congruence,
- potentially high agency,
- avatar body may feel better coupled to the user’s actual movement.

Possible weakness:
- lower sport-depiction fidelity to on-water rowing because no real oars/boat mechanics are physically present.

### Boat-centered mode

Likely strengths:
- higher on-water rowing depiction fidelity,
- more coherent with rowing culture/sport imagery,
- stronger plausibility as “rowing in a boat” if the visual scene/oars/blades behave well,
- supports future body-tool/oar embodiment framing.

Possible weakness:
- reduced action fidelity to the real physical erg handle path,
- potential incoherence if the displayed oar/hand path visibly conflicts with what the user feels.

## Best thesis placement

Use this paper in:
- theoretical background section before or after SoE definitions,
- glossary/construct cleanup,
- discussion of presence vs embodiment vs realism,
- design rationale for separating visuomotor congruence from sport depiction,
- methods section if you include presence/realism ratings,
- limitations section if you discuss that embodiment, presence, realism, and task performance are different outcomes.

Suggested subsection title:
“Presence, fidelity, coherence, and embodiment as distinct constructs”

## Suggested outline integration

### 2.x Presence, realism, and embodiment are related but distinct

This section can say:
- Presence/Place Illusion concerns feeling located in the virtual place.
- Plausibility Illusion concerns whether events feel as if they are really happening.
- Fidelity concerns how closely the system emulates a target real-world task or environment.
- Coherence concerns whether the virtual scenario behaves consistently with user expectations.
- Embodiment concerns processing the virtual body/avatar as one’s own, commonly decomposed into self-location, agency, and ownership.

Then bridge:
- The rowing comparison is not simply high vs low realism.
- It is a conflict between different kinds of fidelity and coherence:
  - bodily/erg-action congruence,
  - sport/oar/boat depiction realism.

## Candidate thesis paragraph

“Skarbez et al. emphasize that presence, immersion, fidelity, coherence, and embodiment should not be treated as interchangeable concepts. Presence is commonly associated with the cognitive feeling of being in a place, while immersion can be understood as an objective property of the system that supports valid actions and sensory feedback. Fidelity describes the extent to which a virtual environment emulates a real-world target, and coherence describes whether the scenario behaves consistently with user expectations. This distinction is important for XR rowing because the erg-centered and boat-centered modes are not simply ‘less’ or ‘more’ realistic. Rather, they emphasize different forms of fidelity: the erg-centered mode prioritizes fidelity to the user’s physical indoor rowing action, whereas the boat-centered mode prioritizes fidelity to the sport depiction of on-water rowing.”

## Candidate short thesis sentence

“The comparison is therefore not merely between high and low realism, but between different forms of fidelity and coherence: physical-action fidelity to the ergometer versus sport-depiction fidelity to on-water rowing.”

## What not to overclaim

Do not use this as a primary source for body ownership mechanisms. It is a presence survey, not an RHI/SoE experimental paper.

Do not treat presence as the same as sense of embodiment.

Do not claim more presence always improves performance. The survey explicitly cautions against using presence as a universal effectiveness measure.

Do not use the paper to replace Kilteni et al. for SoE. Use it to clarify constructs and connect SoE to broader VE evaluation language.

## Thesis-use priority

High priority for:
- terminology cleanup,
- presence vs immersion,
- fidelity/coherence vocabulary,
- Place Illusion / Plausibility Illusion,
- explaining why “realism” is multidimensional,
- preventing construct soup.

Medium priority for:
- measurement caveats,
- presence questionnaires,
- broad VE evaluation framing.

Low priority for:
- primary embodiment evidence,
- rowing biomechanics,
- implementation details.

## Codex/agent note

When using this in thesis drafts, do not write “immersion” when the intended construct is subjective presence, and do not write “realism” without specifying the reference target.

Recommended terminology:
- “system immersion” or “immersive affordances” for technical capabilities,
- “presence” or “Place Illusion” for being-there experience,
- “Plausibility Illusion” or “coherence” for events feeling like they make sense,
- “fidelity to indoor erg action” vs “fidelity to on-water rowing depiction,”
- “sense of embodiment” only for self-location/agency/ownership toward the avatar/body.

This paper is the cleanup layer that keeps the thesis vocabulary disciplined.
