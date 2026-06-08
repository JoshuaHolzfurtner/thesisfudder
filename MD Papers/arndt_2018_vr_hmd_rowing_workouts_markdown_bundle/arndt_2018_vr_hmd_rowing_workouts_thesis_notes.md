# Thesis notes — Arndt 2018, “Using Virtual Reality and Head-Mounted Displays to Increase Performance in Rowing Workouts”

## Citation identity

Arndt, S., Perkis, A., & Voigt-Antons, J.-N. (2018). *Using Virtual Reality and Head-Mounted Displays to Increase Performance in Rowing Workouts*. In *MMSports’18: Proceedings of the 1st International Workshop on Multimedia Content Analysis in Sports* (pp. 45–50). ACM. https://doi.org/10.1145/3265845.3265848

## What this paper is

This is a short ACM workshop pilot study on indoor rowing in virtual reality.

The study places athletes on a stationary rowing machine, the Augletics Eight ergometer, and compares a regular indoor rowing workout with a rowing workout inside a head-mounted display. The VR scene was built in Unity and presented with an HTC Vive. The virtual environment showed a summer lake, distant mountains, a red scull, and oar/scull movement derived from rowing-machine parameters.

Participants completed 500 m in both conditions:
- a non-VR ergometer workout,
- a VR rowing workout with an HMD.

The sample was small: 16 participants, average age 23.4 years. Thirteen of them were experienced rowers, which makes this unusually relevant compared with many exergame studies that rely mostly on novices.

The paper measured:
- ergometer-derived technique metrics: consistency, movement, stroke length, recovery, rhythm,
- completion time,
- strokes per minute,
- breathing rate,
- flow / experience questionnaire ratings,
- SAM affect dimensions,
- motion sickness and quality of experience.

## Why it matters for the XR rowing thesis

This is one of the closest related-work papers for an XR rowing thesis because it is directly about HMD-based VR rowing on an ergometer.

It does not answer the exact thesis question, because it does not compare an erg-centered high-congruence avatar against a boat-centered sport-depiction avatar. However, it shows that the general design space already exists: rowing-machine data can drive an HMD-based virtual rowing scene, and such a scene can affect both objective rowing metrics and subjective experience.

For the thesis, the paper is useful as one member of a broader “immersion in virtual sport” cluster together with the cycling studies:
- Colombo et al. 2025: HMD + interaction can improve enjoyment, attention, presence, and preference in stationary cycling, without lowering RPE.
- Hibbs et al. 2024: low-screen Zwift-like cycling can be more favorable for some engagement/control dimensions than HMD VR, so immersion is not a simple ladder.
- Arndt et al. 2018: the same question appears directly in rowing, where VR may improve experience and some technique-related metrics, but may also reduce control and obscure feedback.

Together, these papers support a cautious claim: immersion is a relevant design variable in virtual sport, but it is not automatically beneficial in every dimension. The thesis can therefore investigate what kind of congruence or realism matters, instead of assuming that “more VR” is always better.

## Core findings / cheat sheet

- The VR condition produced slightly better objective rowing metrics than the non-VR condition.
  - Most relevant reported improvements were rhythm and recovery.
  - Breathing rate was lower in the VR condition.
  - Completion time was also different, but the authors caution that participants were instructed to focus on technique rather than time.

- The authors interpret rhythm and breathing as especially important.
  - They argue that VR may help improve the rhythmic pattern of rowing.
  - This matters because rhythm is central to rowing technique and team synchrony.

- Subjectively, VR changed the exercise experience.
  - Valence was higher in VR.
  - Transformation of time was higher in VR.
  - Autotelic experience was higher in VR.
  - Quality of experience and visual quality were also discussed positively.

- VR was not purely positive.
  - Participants reported less dominance / control in VR than in the non-VR workout.
  - Concentration on task was higher in the traditional workout.
  - Motion sickness was slightly higher in VR, although no participant had to quit and it was not reported as severe.

- Qualitative feedback strongly aligns with rowing-app design needs.
  - Participants wanted multiplayer.
  - They wanted racing against others.
  - Experienced rowers were especially interested in rowing in a virtual team boat and training synchrony.
  - Participants preferred plain speed indicators or red-line pacing over playful elements such as sharks.
  - They wanted more feedback in VR.
  - They suggested placing feedback between the legs, where rowers expect to look in real rowing.

## Relation to thesis concepts

### VR rowing / virtual sport

Very relevant. The paper is a direct prior example of HMD-based indoor rowing in a virtual on-water scene. It should be cited in the VR rowing related-work section.

### Immersion

Relevant, but not as a clean manipulation. The paper compares regular rowing with HMD VR rowing. It does not compare different degrees of immersion. Still, it shows that HMD-based immersion changes both subjective experience and some objective metrics.

### Action-outcome congruence

Relevant. Rowing-machine sensor data drove the virtual scene. The virtual boat/oars were linked to ergometer parameters, so the user’s physical rowing action had virtual consequences.

### Sport-action congruence

Relevant but limited. The VR condition visually placed the ergometer user into a lake/scull rowing scenario. This resembles the thesis’s boat-centered sport-depiction mode. However, the paper does not analyze whether virtual oar movement matched real handle movement, nor whether the sport depiction created embodiment or mismatch.

### Sense of agency / control

Useful. Participants felt less in control in VR, even though some technique metrics improved and the experience was more enjoyable. This is directly relevant to the thesis tradeoff: an immersive sport depiction can improve engagement while weakening perceived control or feedback.

### Flow / transformation of time

Useful. Participants reported stronger transformation of time in VR, suggesting that virtual rowing may make the workout feel more absorbing or less monotonous.

### Feedback design

Highly relevant. Participants wanted more feedback in VR and suggested a rower-appropriate feedback location between the legs. This directly supports diegetic rowing-monitor or SpeedCoach-style UI design.

### Multiplayer / synchrony

Highly relevant for future-work and product framing. Experienced rowers asked for rowing in a team boat and synchrony training, which overlaps strongly with the thesis/project direction.

### Cybersickness / discomfort

Moderately relevant. Motion sickness was higher in VR but not severe. Use cautiously as small-pilot evidence only.

## How it maps to my thesis modes

### Erg-centered mode

The paper supports the feasibility of using real rowing-machine sensor data to drive virtual movement. It also shows that ergometer-derived metrics can be used to evaluate technical aspects such as rhythm, recovery, consistency, movement, and stroke length.

However, the paper does not seem to implement or evaluate a high-congruence avatar where the virtual handle, hands, seat, and body are spatially aligned with the real erg. It should not be used as proof for the erg-centered embodiment mode.

### Boat-centered mode

The paper is closer to the boat-centered / sport-depiction side. The user rows on an ergometer but is visually placed into a virtual lake/scull environment. This makes it a useful precedent for transforming indoor rowing into an on-water virtual rowing scene.

However, the paper does not explicitly address the key mismatch that my thesis cares about: the difference between the real erg handle trajectory and the virtual oar/boat action. That gap is exactly where the present thesis can contribute.

### Core tradeoff

The paper contributes a practical example of the tradeoff between immersive sport depiction and control/feedback.

VR made the rowing experience more enjoyable and time-absorbing and may have improved some rhythm-related metrics. But participants also felt less in control and wanted more rowing-specific feedback. This supports the thesis claim that VR rowing design cannot simply maximize visual immersion; it must preserve technical feedback, action-outcome clarity, and perceived control.

## What not to overclaim

- Do not claim that VR rowing is proven to improve rowing performance in general.
- Do not claim that HMD rowing is better than non-VR rowing.
- Do not claim that this paper proves embodiment, body ownership, or self-location.
- Do not claim that virtual oars became embodied tools.
- Do not claim that the paper proves boat-centered VR is better than erg-centered VR.
- Do not claim that all rowers prefer VR rowing.
- Do not treat the technique improvements as strong evidence; this was a small pilot study with 16 participants and short 500 m sessions.
- Be careful with the statistics: some p-values are reported as significant at p = 0.10, which is exploratory at best and not conventionally significant.
- Do not overread the qualitative feedback as systematic survey evidence; it was informal feedback gathered after the experiment.

## Thesis-use priority

High priority for:
- VR rowing related work,
- HMD rowing on an ergometer,
- indoor rowing transformed into an on-water virtual scene,
- experienced rower feedback,
- rhythm/recovery/technique metrics,
- feedback placement in VR rowing,
- multiplayer/team/synchrony motivation,
- critical framing of VR rowing limitations.

Medium priority for:
- immersion and engagement,
- flow / transformation of time,
- action-outcome congruence,
- sport-action congruence,
- enjoyment and motivation,
- cybersickness / control tradeoff.

Low priority for:
- formal embodiment theory,
- body ownership,
- self-location,
- avatar morphology,
- precise visuomotor congruence,
- proof of erg-centered vs boat-centered superiority.

Suggested placement:
- Related Work: VR rowing and exergames.
- Related Work: virtual sport systems and immersion.
- System / Prototype: design rationale for feedback placement and multiplayer/synchrony.
- Discussion: VR rowing is promising but not automatically superior; feedback and control remain important.
- Future Work: multiplayer, team boats, synchrony training, rower-specific UI.

## Candidate thesis paragraph

Arndt et al. provide a directly relevant example of HMD-based VR rowing on an ergometer. In their pilot study, participants completed 500 m workouts in a standard ergometer condition and in a VR lake/scull environment driven by ergometer sensor data. The VR condition showed small improvements in several technique-related metrics, particularly rhythm and recovery, and participants reported a more enjoyable and time-absorbing experience. However, participants also felt less in control and noted that the VR condition provided too little feedback. The study therefore supports the relevance of immersive rowing environments, but also illustrates that VR rowing must balance sport depiction with rower-specific feedback, control, and technical clarity.

## Candidate short thesis sentence

Arndt et al.’s VR rowing pilot suggests that HMD-based rowing can improve experience and affect technique-related metrics, but also highlights that immersive rowing environments may reduce perceived control and obscure feedback important to experienced rowers.

## Codex / agent note

Use this paper as a core VR-rowing related-work source, but keep claims cautious. It is highly relevant because it is directly about HMD-based rowing on an ergometer, but it is still a small pilot study. The best use is not to “prove VR rowing,” but to show that prior work has already identified the same design tensions: immersion and enjoyment may improve, rhythm may change, but experienced rowers still need clear, rowing-specific feedback and control.

Preserve the following ideas:
- HMD rowing on ergometer.
- Augletics sensor data driving virtual lake/scull scene.
- rhythm/recovery improvements as exploratory findings.
- higher transformation of time / autotelic experience / valence in VR.
- less control and less technical concentration in VR.
- qualitative requests for multiplayer, team rowing, synchrony, opponent avatars, red-line pacing, and feedback between the legs.

Use this in the “trifecta” with Colombo 2025 and Hibbs 2024:
- Colombo = HMD + interaction can improve subjective experience in cycling.
- Hibbs = screen-based Zwift-like systems can be strong and sometimes better tolerated.
- Arndt = the same immersion/control/feedback question exists directly in rowing.

Do not use it as direct evidence for embodiment or the erg-centered vs boat-centered comparison.
