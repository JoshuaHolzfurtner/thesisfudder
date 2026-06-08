# Thesis notes — Waltemate et al. (2016), “The Impact of Latency on Perceptual Judgments and Motor Performance in Closed-loop Interaction in Virtual Reality”

## Citation identity

Waltemate, T., Senna, I., Hülsmann, F., Rohde, M., Kopp, S., Ernst, M., & Botsch, M. (2016). The Impact of Latency on Perceptual Judgments and Motor Performance in Closed-loop Interaction in Virtual Reality. VRST ’16.

## What this paper is

This paper studies how visual feedback latency affects full-body VR interaction. Participants stood in a CAVE in front of a virtual mirror and saw a full-body mirror avatar. They followed a semi-transparent “ghost character” performing upper-body movements while the mirror avatar responded to their own motion with different delays.

Latency levels:
- 45 ms baseline
- 75 ms
- 125 ms
- 210 ms
- 350 ms

They measured:
- sense of agency
- sense of body ownership
- simultaneity perception
- motor performance accuracy

## Why it matters for the rowing/XR thesis

This is highly relevant because the rowing project depends on tight closed-loop feedback between the user’s real movement and the virtual avatar/oar/handle representation.

The paper gives a good empirical basis for saying:
- latency matters for both perceptual embodiment and motor performance
- motor performance may degrade before agency/ownership clearly collapses
- users may tolerate perceptible delays in agency/ownership judgments more than in simultaneity judgments
- task difficulty and motor errors influence whether users perceive delays

For your thesis, this supports treating latency not merely as an engineering nuisance but as an embodiment and performance variable.

## Core findings

### 1) Motor performance and simultaneity are sensitive earlier than agency/ownership

The paper reports that motor performance and simultaneity perception were affected by latencies above roughly 75 ms.

Agency and ownership only began clearly declining later, between roughly 125 ms and 210 ms, and did not fully break down even at the highest tested latency of 350 ms.

### 2) Agency and ownership are more tolerant than simultaneity

At 350 ms, simultaneity perception was very low, but participants still often reported agency and ownership.

This is useful because it shows that “I notice delay” and “I still feel this avatar is me / caused by me” are not identical judgments.

### 3) Performance accuracy predicted perceptual judgments better than delay alone

A very important nuance: participants seemed to infer delay partly from how well they performed. Poor motor performance made participants more likely to judge the feedback as non-simultaneous and to lose agency/ownership.

For rowing:
- if tracking errors or mapping mismatch reduce rowing task performance, the user may perceive worse latency/agency even if the actual system latency is unchanged
- conversely, clean predictable rowing motion may tolerate slightly more latency perceptually than chaotic high-error motion

### 4) Report latency in VR studies

The paper explicitly argues that VR latency should at least be reported, because it can be a source of side effects in embodiment and motor-performance studies.

This is relevant for your methods chapter.

## Thesis relevance

### Use for the technical methods chapter

This paper supports including:
- measured end-to-end latency
- tracking/mapping latency discussion
- the distinction between tracking delay, smoothing delay, rendering delay, and network delay
- why latency has to be controlled or at least documented

### Use for embodiment theory

It provides empirical support that ownership and agency are affected by delayed visual feedback, but with broad temporal tolerance under full-body action.

### Use for rowing/XR design

For an XR rowing app:
- visual avatar/oar feedback should be low-latency, especially for precise handle/seat timing
- delay can affect both technique performance and perceived embodiment
- feedback smoothness vs latency trade-offs should be handled carefully

## How it connects to your two modes

### Erg-centered mode

This mode should benefit strongly from low latency because it emphasizes precise visuomotor congruence:
- real handle and seat motion should feel tightly coupled to virtual handle/avatar motion
- excessive smoothing or delayed IK could damage the very thing this mode is designed to test

### Boat-centered mode

Latency may interact with the already-present mapping mismatch between real erg handle path and virtual oar/hand trajectory:
- a small representational mismatch may be tolerable if timing is tight
- timing delay plus spatial mismatch could compound the user’s sense that the avatar/oar is not “mine” or not under direct control

## What not to overclaim

Do not generalize the exact thresholds as universal. The authors emphasize that latency effects depend on display, movement, task, and performance.

Do not say agency/ownership are safe up to 350 ms in all VR systems. In this study they did not fully break down at 350 ms, but the task, avatar, CAVE setup, full-body mirror, and repeated judgments all matter.

Do not use this as the only latency source for HMD rowing. It used a CAVE and upper-body imitation task, not a headset rowing setup.

## Thesis-use priority

High priority for:
- latency as embodiment/performance variable
- methods reporting
- justification for measuring/controlling end-to-end latency
- distinguishing simultaneity, agency, ownership, and motor performance

Suggested placement:
- technical system/methods chapter
- embodiment-related work subsection on visuomotor synchrony and latency
- limitations section if latency or streaming is present in your setup

## Candidate thesis sentence

“Latency in closed-loop avatar feedback can affect motor performance and perceptual judgments differently. Waltemate et al. found that motor performance and simultaneity perception were already affected at lower delays, while agency and ownership declined later and did not fully collapse even at 350 ms. This suggests that XR rowing systems should report and control latency, especially when comparing visuomotor-congruent and representationally transformed rowing modes.”

Verify exact wording and page references against the source before final submission.
