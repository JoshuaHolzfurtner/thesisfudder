# Thesis notes — Lamb (1989), “A kinematic comparison of ergometer and on-water rowing”

## Citation identity

Lamb, D. H. (1989). A kinematic comparison of ergometer and on-water rowing. *The American Journal of Sports Medicine*, 17(3), 367–373.

## What this paper is

This paper compares the kinematics of sweep rowing on-water with rowing on a rowing ergometer.

The study used 30 male candidates from the U.S. National Heavyweight Rowing Team selection camp. The rowers were filmed both:
- rowing on-water, and
- rowing on a Stanford rowing ergometer.

The paper digitized body joint positions from film and used a vector loop model to analyze the drive phase of the rowing stroke. The aim was to test whether ergometer rowing can validly simulate on-water rowing kinematics and to identify which body segments contribute most to total linear oar velocity.

## Why it matters for the XR rowing thesis

This is a high-value rowing-source anchor for the erg-vs-boat comparison.

Your thesis is built around a conflict:
- the erg-centered mode prioritizes direct mapping to the real erg handle/seat/body action,
- the boat-centered mode prioritizes a more on-water rowing depiction with virtual oars.

Lamb is directly about whether erg rowing resembles on-water rowing kinematically. The useful thesis-safe answer is nuanced:

- Ergometer and on-water rowing are broadly similar in the drive phase, especially in legs and trunk.
- Significant differences appear in arm motion at the beginning and end of the drive phase.
- Differences at the finish are linked to oar lifting / feathering actions that are essential on-water but not naturally exhibited on an ergometer.
- Therefore, the erg is a valid but incomplete simulator: good for many drive-phase kinematics, but less faithful for oar-specific arm/blade handling.

This is almost exactly the conceptual gap your boat mode is trying to visualize.

## Stroke-phase vocabulary

The paper defines the rowing stroke as:
- catch,
- drive phase,
- finish,
- recovery.

It states:
- catch: the oar is placed quickly in the water,
- drive: movement of the oar through the water,
- finish: the oar is withdrawn from the water,
- recovery: the oar moves through the air and is prepared to reenter the water.

This is useful for your glossary and for keeping rowing terminology clean.

## Study method / model

The paper used vector loop analysis and modeled rowing as two closed vector loops:
- lower-body loop,
- upper-body loop.

The digitized landmarks included:
- toe,
- ankle,
- knee,
- hip,
- shoulder,
- elbow,
- wrist,
- oar handle,
- head.

The hip joint was used as a representation of the seat position.

The main variables were five body-segment velocity contribution variables to total linear oar velocity:
- trunk component velocity,
- upper arm component velocity,
- lower arm component velocity,
- lower leg component velocity,
- upper leg component velocity.

It also examined:
- normalized relative seat velocity,
- normalized relative hand velocity.

## Core findings / cheat sheet

### 1) Ergometer rowing broadly simulated on-water rowing in the drive phase

The paper concludes that the hypothesis that ergometer rowing simulates on-water rowing was supported.

Important nuance:
This does not mean erg rowing and on-water rowing are identical. It means most drive-phase kinematic variables, especially legs and trunk, were similar enough to support ergometer-based kinematic testing.

### 2) Legs initiate the drive, but trunk contribution becomes dominant

The paper finds that the lower leg initiates the drive phase. Around 40–50% of the drive, the trunk contribution equals and then surpasses the lower-leg contribution.

It also concludes that the trunk segment is the major contributor to total linear oar velocity, even though the legs initiate the drive.

Thesis use:
This supports a more nuanced stroke model than “rowing is just legs” or “rowing is just arms.” For your avatar/IK, trunk and legs are not decorative; they are core to stroke representation.

### 3) Seat velocity dominates early drive; hand velocity dominates later drive

The paper reports that normalized relative seat velocity contributes more during the first 40% of the drive, while normalized relative hand velocity contributes more during the remaining 60%.

Thesis use:
This is useful for:
- stroke phase detection,
- handle/seat timing,
- mapping of seat vs hand movement,
- deciding which body segments should be emphasized at which part of the drive.

### 4) Significant differences occur mainly in arm motion

The statistically significant erg-vs-water differences were found in:
- upper arm component velocity,
- lower arm component velocity.

These differences occurred mainly:
- early in the drive,
- late in the drive / finish.

The paper treats these as minor relative to the larger leg/trunk contributions, but they matter for your thesis because the arm/oar mismatch is visually and experientially salient.

### 5) Early-drive arm differences are linked to oar slip / moving water fulcrum

The paper explains early drive differences by noting that the on-water oar has a nonstationary fulcrum because the blade slips in water, while the ergometer fulcrum is fixed/stationary.

Thesis use:
This directly supports the claim that the ergometer interface cannot fully reproduce on-water oar mechanics, even if gross body kinematics are similar.

### 6) Finish differences are linked to feathering / lifting the oar

The paper states that end-of-drive arm differences may result from reduced tendency to “feather” or lift the oar at the finish in ergometer rowing, which is essential in on-water rowing.

This is very important for your virtual oar / IK / feathering-squaring angle:
- feathering is not random rowing nerd detail,
- it appears in a classic erg-vs-water biomechanics comparison as one of the differences between erg and on-water rowing,
- it supports your idea that boat mode should represent oar-specific actions even if the real erg cannot physically enforce them.

## Relation to the thesis modes

### Erg-centered mode

Lamb supports the erg-centered mode because:
- legs and trunk kinematics are broadly similar between erg and water rowing during the drive,
- ergometer-based kinematic measures may be valid for training/selection contexts,
- direct handle/seat mapping preserves important physical timing and body-motion cues.

Thesis angle:
The erg-centered mode is not “less rowing.” It preserves key drive-phase kinematics and physical constraints.

### Boat-centered mode

Lamb supports the boat-centered mode because:
- ergometer rowing differs at the arms during early and late drive,
- on-water rowing involves oar slip, moving fulcrum, oar lifting, and feathering,
- these oar-specific details are not naturally present on a standard erg.

Thesis angle:
The boat-centered mode can be framed as visually restoring rowing-specific oar/blade mechanics that the erg abstracts away.

### Central thesis tension

The paper gives a perfect evidence base for the thesis dilemma:

The ergometer is similar enough to on-water rowing to be a meaningful rowing simulator, but different enough in oar/arm/blade-specific mechanics that a realistic virtual boat/oar depiction introduces a real representational tradeoff.

## Feathering / squaring relevance

This paper explicitly mentions feathering at the finish.

It does not deeply explain the whole feather/square cycle, but it says that reduced tendency to feather or lift the oar at the finish in ergometer rowing may explain differences in arm motion. It also states that, for practical purposes, ergometer rowing should emphasize feathering the oar or hyperextending the wrists at the finish.

Thesis use:
This is a strong source for saying:
- oar/blade handling matters,
- erg rowing may omit or reduce these actions,
- virtual oar representation can add sport-specific detail.

Do not overbuild the claim:
This paper does not test virtual feathering, embodiment, or IK. It only supports that feathering/lifting is a meaningful difference between on-water and ergometer rowing.

## Relation to Rauter et al. (2013)

Rauter et al.:
- high-fidelity rowing simulator,
- skill transfer,
- haptic oar-water interaction,
- oar handling metrics such as catch slip, blade depth, oar angles.

Lamb:
- classic kinematic comparison of erg vs on-water,
- supports erg similarity for drive phase,
- identifies arm/oar/finish differences.

Together:
- Lamb supports the erg as a valid partial simulator.
- Rauter supports the importance of oar-water/oar-handling fidelity.
- Your thesis sits between these: real erg action with optional virtual boat/oar depiction.

## What not to overclaim

Do not claim Lamb proves all ergometers are identical to on-water rowing. It used a specific Stanford rowing ergometer and sweep rowing context.

Do not claim the whole stroke is equivalent. The analysis focuses on the drive phase, not the full recovery and not detailed blade work throughout the complete cycle.

Do not ignore that significant arm differences were found. These are precisely relevant for your boat/oar visualization.

Do not claim feathering/squaring was fully analyzed as a separate dependent variable. It is mentioned as an interpretation of finish differences.

Do not treat the trunk-finding as a universal coaching slogan without context. The study says legs initiate the drive, trunk contribution becomes dominant later, and trunk contributes strongly to total linear oar velocity.

## Thesis-use priority

High priority for:
- erg vs on-water biomechanics,
- justification of erg-centered condition,
- justification of boat-mode oar/arm mismatch,
- stroke-phase glossary,
- feathering/finish relevance,
- handle/seat timing discussion.

Medium priority for:
- form-analysis appendix,
- avatar/IK body-segment timing,
- future biomechanical evaluation.

Low priority for:
- embodiment theory,
- presence,
- Proteus/avatar customization.

Suggested placement:
- related work: rowing biomechanics and ergometer validity,
- system/prototype rationale: why handle/seat tracking is meaningful,
- design dilemma: why boat depiction introduces a mismatch,
- appendix: technical rowing variables / stroke phase model.

## Candidate thesis paragraph

“Classic biomechanical work supports treating ergometer rowing as a meaningful but incomplete simulator of on-water rowing. Lamb compared on-water sweep rowing with rowing on a Stanford ergometer and found broadly similar drive-phase kinematics for the legs and trunk, supporting the use of ergometer-based kinematic measures. However, significant differences appeared in the upper and lower arm components at the beginning and end of the drive. Lamb attributed early-drive differences partly to oar slip and the nonstationary water fulcrum, and finish differences partly to the reduced tendency to feather or lift the oar on an ergometer. This is directly relevant for XR rowing: an erg-centered representation can preserve important drive-phase body and seat/handle congruence, while a boat-centered representation can visually restore oar-specific actions that the ergometer abstracts away.”

## Candidate short thesis sentence

“Ergometer rowing can approximate on-water drive-phase kinematics, especially for the legs and trunk, but classic kinematic comparisons still identify arm and finish-phase differences related to oar slip and feathering, which supports treating virtual oar depiction as a meaningful design dimension rather than pure visual decoration.”

## Codex / agent note

Use this paper to support:
- stroke phase glossary,
- erg-vs-water difference claims,
- why handle/seat tracking matters,
- why oar/arm representation and feathering are not optional trivia,
- why the two thesis modes are a real tradeoff.

Do not use this paper to support:
- embodiment theory,
- avatar ownership,
- presence,
- modern VR exercise effects.

Implementation-relevant takeaways:
- seat/hip motion dominates early drive,
- hand motion dominates later drive,
- legs initiate drive,
- trunk contribution becomes major mid-to-late drive,
- arm differences at catch/finish are the most erg-vs-water salient,
- virtual oar/feathering logic belongs especially near finish/release.
