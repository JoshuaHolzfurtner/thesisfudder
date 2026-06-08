# Thesis notes — Kocur et al. (2025), “Investigating the Impact of Customized Avatars and the Proteus Effect during Physical Exercise in Virtual Reality”

## Citation identity

Kocur, M., Kloss, M., Schaufler, C., Schwind, V., & Henze, N. (2025). Investigating the Impact of Customized Avatars and the Proteus Effect during Physical Exercise in Virtual Reality. *CHI ’25: Proceedings of the 2025 CHI Conference on Human Factors in Computing Systems*.

## What this paper is

This paper studies whether customized avatars can strengthen avatar effects during physical exercise in VR.

The theoretical background is the Proteus effect: the idea that an avatar’s visual appearance can influence the user’s behavior, perception, or physiology. Prior work suggested that athletic or muscular avatars may reduce perceived exertion or improve physical performance, but such effects can fail when users do not feel ownership of or identify with the avatar.

The paper therefore asks whether customization makes an athletic avatar more effective during exercise.

## Study design

Participants: 24 participants.

Design:
- repeated-measures / within-subject design,
- two independent variables:
  - Customization: customized vs randomized avatar,
  - Athleticism: athletic vs non-athletic avatar.

Each participant embodied four avatars:
- customized athletic,
- customized non-athletic,
- randomized athletic,
- randomized non-athletic.

Important design detail:
The randomized avatars were not one generic stock avatar for everyone. Instead, each participant received avatars created by the previous participant. This made the randomized condition more ecologically valid than using a single generic avatar.

## Avatar creation / customization setup

The authors built a VR customization editor in Unity.

Participants embodied an avatar while customizing it, with mirrors available to inspect the body from multiple angles.

The avatar system used DAZ Genesis 8.1 male/female characters and morph targets for:
- body fat,
- muscularity,
- height,
- face details,
- skin / hair / eye color,
- clothing,
- hairstyles.

Participants first created a baseline self-resembling avatar. Then they created:
- an athletic version: their appearance after one year of healthy active lifestyle, regular exercise, and healthy diet,
- a non-athletic version: their appearance after one year of unhealthy inactive lifestyle, no exercise, and unhealthy diet.

This is highly relevant for your future avatar/customization pipeline because it supports the idea that avatar customization during embodiment can increase connection to the avatar.

## Exercise tasks

The experiment used three physical tasks:

### 1) Reaction wall
A virtual wall with 16 fields; participants touched as many lit-up fields as possible in 45 seconds.

Measure:
- number of correct hits.

### 2) Biceps curls
Participants performed as many curls as possible in 30 seconds using 2 kg dumbbells.

Measures:
- number of curls,
- perceived exertion,
- heart rate.

### 3) Holding weights
Participants held 1 kg weights in each hand for 60 seconds at 90° shoulder abduction in the scapular plane.

Measures:
- perceived exertion at 20, 40, and 55 seconds,
- heart rate.

## Measures

Main outcomes:
- perceived exertion using Borg RPE scale,
- heart rate using a Polar OH1 monitor,
- physical performance via number of biceps curls / reaction wall hits.

Control / moderator measures:
- body ownership using Body Representation Questionnaire (BRQ),
- avatar identification using Player Identification Scale (PIS),
- self-perceived fitness using Self-Perceived Fitness Questionnaire (SPF),
- presence using one item from the Igroup Presence Questionnaire (IPQ).

This measurement stack is very relevant to your thesis because it separates:
- body ownership,
- agency,
- avatar identification,
- presence,
- perceived exertion,
- physiological response,
- physical performance.

## Core findings / cheat sheet

### 1) Athletic avatars reduced perceived exertion

Participants reported lower perceived exertion when embodying athletic avatars compared with non-athletic avatars.

This held for:
- holding weights,
- biceps curls.

Thesis use:
Avatar appearance can affect physical effort perception during VR exercise.

### 2) Customized avatars reduced perceived exertion during weight holding

Customization also significantly reduced perceived exertion during the holding-weights task.

For biceps curls, customization alone did not significantly reduce perceived exertion, but athleticism did.

Thesis use:
Customization may matter, but effects can depend on the exercise type/task.

### 3) Athletic avatars reduced heart rate during weight holding — but only when customized

The paper found a significant Customization × Athleticism interaction for heart rate while holding weights.

Interpretation:
The athletic avatar’s physiological effect depended on whether the avatar was customized.

This is one of the paper’s strongest and most thesis-relevant findings:
- avatar athleticism alone may not be enough,
- the user-avatar connection can moderate whether appearance effects show up physiologically.

### 4) Heart rate during biceps curls was not significantly affected by avatar athleticism or customization

For biceps curls, heart rate increased over time as expected, but avatar condition did not significantly affect it.

Thesis use:
Physiological avatar effects are task-specific and should not be assumed universally.

### 5) Customized avatars improved biceps-curl performance

Participants performed significantly more biceps curls when embodying customized avatars compared with randomized avatars, regardless of athleticism.

No significant performance effects were found for the reaction wall task.

Thesis use:
Customization may improve some exercise performance outcomes, but again the effects depend on task type.

### 6) Customized and athletic avatars increased body ownership

The BRQ results suggest that participants experienced higher body ownership for:
- customized avatars compared with randomized avatars,
- athletic avatars compared with non-athletic avatars.

Subscales included:
- body seen when looking down,
- body seen in mirror,
- visual feature resemblance,
- two-bodies item,
- agency item.

Important nuance:
Body ownership was not just a background assumption; they measured it as a possible moderator.

### 7) Customized and athletic avatars increased avatar identification

The PIS results suggest higher avatar identification for:
- customized avatars,
- athletic avatars.

Dimensions included:
- embodied presence,
- similarity identification,
- wishful identification.

This is useful because your thesis may need to distinguish body ownership from avatar identification:
- ownership: “this body feels like mine,”
- identification: “this avatar represents me / fits my self-concept / ideal self.”

### 8) Presence did not significantly differ

General presence, measured with an IPQ item, did not show significant differences between avatar conditions.

This is a very useful construct-cleanup result:
Avatar customization and athleticism affected ownership, identification, perceived exertion, and some physiological/performance measures, but did not necessarily change general presence.

Thesis use:
Do not collapse presence, embodiment, identification, and exertion into one “immersion” score.

## Why it matters for the XR rowing thesis

This is a strong modern CHI anchor for the exercise-avatar side of your thesis.

Your thesis compares an erg-centered mode and a boat-centered sport-depiction mode. This paper is not about rowing, but it is about:
- embodied avatars during physical exercise,
- avatar appearance effects,
- customized vs randomly assigned avatars,
- body ownership and avatar identification as moderators,
- perceived exertion and heart rate.

It supports the idea that avatar appearance and avatar-user connection can influence exercise perception and physiology.

## Relation to your rowing modes

### Erg-centered mode

The erg-centered mode prioritizes physical and visuomotor congruence. If paired with a customized or self-similar avatar, it might support strong body ownership and agency because:
- the real handle/seat/body motion matches the avatar,
- the avatar can be perceived as more “mine,”
- physical effort and virtual body feedback are tightly coupled.

Kocur et al. suggests that customized avatars may reduce perceived exertion and increase body ownership/identification during exercise.

### Boat-centered mode

The boat-centered mode emphasizes sport-realistic depiction and athletic rowing identity. It may benefit from:
- athletic avatar appearance,
- rower-specific avatar body/clothing,
- customization,
- avatar identification,
- wishful identification as “my fitter/rowing self.”

However, if visuomotor congruence is weaker due to transformed erg-to-oar mapping, the avatar appearance effect may depend on whether ownership/identification remain strong enough. This matches the paper’s claim that Proteus effects can fail when ownership/identification are weak.

## Strong thesis bridge

This paper supports the claim that avatar design is not a cosmetic detail in VR exercise. Avatar appearance and customization can change how hard exercise feels and can affect physiological responses under some conditions.

A possible bridge:

“Because avatar customization and athletic appearance can modulate perceived exertion and some physiological responses during VR exercise, avatar embodiment in XR rowing should be treated as part of the interaction design rather than as merely visual decoration.”

## Relevance to your avatar/customization pipeline

This paper is very useful for future product / outlook / customization discussion.

It provides support for:
- letting users customize avatars,
- creating athletic or idealized versions,
- using mirrors during customization,
- tuning body composition and clothing,
- considering wishful identification, not only exact self-similarity.

Important nuance:
The paper’s customized athletic avatar was not a fantasy superhero body. It was framed as a plausible future self after one year of healthy exercise and diet. That is useful for your rowing app because it fits a respectful sports/training context:
- “your fitter rower self,”
not
- “unrealistic superhero body.”

## Relation to Proteus effect

This paper is useful if you want a short Proteus effect subsection.

Key safe claim:
The Proteus effect may occur during VR exercise, but its effects are moderated by avatar ownership and identification and may be task-specific.

Use it to avoid over-simple claims like:
- “athletic avatars always improve performance,”
- “muscular avatars always reduce effort.”

Better claim:
- “athletic avatars can reduce perceived effort and influence physiological responses, but effects depend on avatar customization, ownership/identification, and exercise type.”

## Relation to embodiment theory

The paper explicitly connects:
- body ownership illusion,
- visuomotor synchrony,
- avatar identification,
- Proteus effect,
- VR exercise.

It is not a foundational RHI paper, but it is a good applied embodiment/exercise paper.

Use it after core theory papers:
- Kilteni / SoE,
- Kalckert & Ehrsson,
- Seinfeld & Müller,
- Waltemate,
- then Kocur et al. as applied VR exercise evidence.

## What not to overclaim

Do not claim customization always improves exercise outcomes. Effects were task-specific.

Do not claim athletic avatars improved all performance. The reaction wall task did not show significant performance effects, and biceps-curl HR was not significantly affected.

Do not claim general presence changed. Presence did not significantly differ between avatar conditions.

Do not claim the paper proves avatar customization improves rowing embodiment. It is VR exercise, not rowing.

Do not treat perceived exertion, heart rate, ownership, identification, and presence as the same construct. One of the paper’s strengths is that it separates them.

## Thesis-use priority

High priority for:
- VR exercise / exergame related work,
- avatar customization,
- Proteus effect during physical exertion,
- perceived exertion / heart rate measures,
- ownership and identification as moderators,
- future avatar customization system.

Medium priority for:
- product/app outlook,
- player-avatar identity,
- idealized athlete self-avatar.

Low priority for:
- rowing biomechanics,
- erg-vs-boat physical mismatch,
- core RHI/SoE definitions.

Suggested placement:
- related work subsection: “Avatar appearance and customization in VR exercise,”
- discussion of avatar realism / identification,
- future work: user customization and athlete-self avatars,
- limitations: participant-avatar match may moderate embodiment effects.

## Candidate thesis paragraph

“Recent VR-exercise research suggests that avatar appearance and customization can influence physical exertion. Kocur et al. found that athletic avatars reduced perceived exertion during weight holding and biceps curls, while customized avatars reduced perceived exertion during weight holding and increased biceps-curl performance. They further reported that athletic avatars reduced heart rate during weight holding only when the avatar had been customized. These findings suggest that avatar appearance effects during exercise depend not only on visual athleticism but also on the user’s ownership of and identification with the avatar. For XR rowing, this supports treating avatar design and potential customization as part of the embodiment and exercise experience rather than as a cosmetic afterthought.”

## Candidate short thesis sentence

“Avatar appearance effects in VR exercise appear to be moderated by ownership and identification: in Kocur et al.’s study, athletic avatars reduced heart rate during weight holding only when the avatar was customized.”

## Codex / agent note

Use this paper to support:
- avatar customization as future work,
- customized rower avatar pipeline,
- distinction between body ownership and avatar identification,
- perceived exertion and heart rate as possible secondary exercise measures,
- “athletic self” avatar framing.

Do not use it to justify:
- erg vs boat mechanics,
- feathering/squaring,
- physical rowing technique,
- core SoE definitions by itself.

Recommended terminology:
- “avatar customization,”
- “avatar identification,”
- “Proteus effect,”
- “perceived exertion,”
- “physiological response,”
- “task-specific avatar effects.”
