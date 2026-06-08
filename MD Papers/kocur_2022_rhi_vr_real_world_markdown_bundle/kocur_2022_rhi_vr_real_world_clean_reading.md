# Clean reading text — Kocur et al. (2022)

Source: `VR Difference for Rubber Hand.pdf`

This is a lightly cleaned extraction for reading only. Page headings are retained; verify quotations against the PDF or raw page-marked file.

---

## Page 1

The Rubber Hand Illusion in Virtual Reality and the Real World -
Comparable but Different
Martin Kocur
martin.kocur@ur.de
University of Regensburg
Regensburg, Germany
Alexander Kalus
alexander.kalus@ur.de
University of Regensburg
Regensburg, Germany
Johanna Bogon
johanna.bogon@ur.de
University of Regensburg
Regensburg, Germany
Niels Henze
niels.henze@ur.de
University of Regensburg
Regensburg, Germany
Christian Wolff
christian.wolff@ur.de
University of Regensburg
Regensburg, Germany
Valentin Schwind
valentin.schwind@fb2.fra-uas.de
Frankfurt University of Applied
Sciences
Frankfurt, Germany
ABSTRACT
Feeling ownership of a virtual body is crucial for immersive experiences in VR. Knowledge about body ownership is mainly based on
rubber hand illusion (RHI) experiments in the real world. Watching
a rubber hand being stroked while one’s own hidden hand is synchronously stroked, humans experience the rubber hand as their
own hand and underestimate the distance between the rubber hand
and the real hand (proprioceptive drift). There is also evidence for a
decrease in hand temperature. Although the RHI has been induced
in VR, it is unknown whether effects in VR and the real world differ.
We conducted a RHI experiment with 24 participants in the real
world and in VR and found comparable effects in both environments. However, irrespective of the RHI, proprioceptive drift and
temperature differences varied between settings. Our findings validate the utilization of the RHI in VR to increase our understanding
of embodying virtual avatars.
CCS CONCEPTS
• Human-centered computing →Virtual reality.
KEYWORDS
rubber hand illusion, virtual reality, avatars, body ownership illusion, proprioceptive drift, disownership
ACM Reference Format:
Martin Kocur, Alexander Kalus, Johanna Bogon, Niels Henze, Christian
Wolff, and Valentin Schwind. 2022. The Rubber Hand Illusion in Virtual
Reality and the Real World - Comparable but Different. In 28th ACM Symposium on Virtual Reality Software and Technology (VRST ’22), November
29-December 1, 2022, Tsukuba, Japan. ACM, New York, NY, USA, 12 pages.
https://doi.org/10.1145/3562939.3565614
This work is licensed under a Creative Commons Attribution International
4.0 License.
VRST ’22, November 29-December 1, 2022, Tsukuba, Japan
© 2022 Copyright held by the owner/author(s).
ACM ISBN 978-1-4503-9889-3/22/11.
https://doi.org/10.1145/3562939.3565614
1 INTRODUCTION
Virtual reality (VR) enables users to experience a sense of ownership
of a virtual body—a phenomenon known as the body ownership illusion (BOI). Designers and researchers ofVR applications commonly
use avatars—the digital self-representation of the user—to provide
users with a virtual body in VR and create embodied experiences
(c.f., [34, 39]). Hence, the sense of having a virtual body in VR contributes to an enhanced and more realistic user experience [35, 67].
For this reason, understanding BOIs and the underlying mechanisms is important for the design of avatars and immersive VR
experiences. Our knowledge about body ownership is based on
the seminal RHI, which has evolved into a key instrument for investigating the embodiment of artificial limbs and significantly
contributed to a better understanding of human cognition and bodily awareness [52].
In 1998, Botvinick and Cohen [6] demonstrated that humans
can experience an artificial limb—a rubber hand —as if it was their
own hand. The RHI is a illusory sensation of embodying the rubber
hand and induced by multisensory conflicts. When the subjects’
real hand, which is hidden from view, and the rubber hand are
stroked at the same time while the subjects can see the rubber hand,
after some time they start to perceive the artifical limb as being
a part of their own body. As a result, subjects perceive the own
hand to be closer to the rubber hand. This phenomenon is known
as proprioceptive drift.
There is also empirical evidence that the RHI evokes physiological responses. Interestingly, Moseley et al. [47] revealed that when
participants experienced ownership of the rubber hand, the skin
temperature of the own hand decreased. As a drop in temperature
could also be found in neurological disorders, e.g., patients suffering from somatoparaphrenia have the feeling that their affected
limbs belong to someone else [75], the authors concluded that these
findings are associated with a disownership of the real hand. However, many other studies were not able to replicate these and other
related results using the RHI paradigm [8, 10, 16, 21, 42, 54, 58].
For this reason, effects on skin temperature caused by the RHI are
highly controversial [10].
The importance of the RHI is not limited to the understanding
of human perception. Understanding the RHI has implications for
the design of immersive virtual environments ( VEs) in general and
avatar creation in particular. Consequently, the knowledge from

## Page 2

VRST ’22, November 29-December 1, 2022, Tsukuba, Japan Kocur et al.
RHI experiments in the real world is transferred into VR to make
users experiencing ownership of virtual avatars [ 62]. For years,
designers and researchers have adopted the principles that govern
the induction of theRHI to induce BOIs in VR. Previous work found,
for example, that users feel ownership of virtual hands when they
see the virtual hands from a first-person perspective while both the
virtual and real limbs are synchronously stroked [63]. Although it
is known that users can even feel ownership of full-body avatars
in VR (e.g., [34, 37]), there is currently no empirical evidence that
the effects caused by ownership illusions in the real world are the
same as in virtual worlds.
A comparison between BOIs in both environments would validate that the principles that apply for BOIs in the real world translate to VR. Such a validation is important for designers and researchers of VR applications as it provides insights into whether
there are differences between virtual and real bodily illusions that
have to be considered during induction. For example, effects of
technological latency during stroking in VR or a decreased realism
of a VE can cause different degrees of BOIs compared to the real
world that have to be compensated by designers and researchers,
e.g., adapting induction procedures such as slower, longer, or firmer
stroking [52]. The RHI is a promising paradigm for this to explore
as it allows to induce an ownership illusion over a physical rubber
hand in the real word and it can be transferred into VR to create
the illusory sensation of embodying a virtual rubber hand.
In this paper, we conducted a study with 24 participants who experienced the RHI in the real world as well as in VR using a virtual
replica of the real environment. We found that the proprioceptive
drift was generally higher in VR compared to the real world. Our
results also revealed effects on the skin temperature of the own
hand. This implies that the RHI can induce temperature changes.
We discuss our findings in the light of theories on psychological
disownership of real body parts and provide implications for the
virtual embodiment of avatars in VR. This work evaluates an experimental setting to systematically induce the RHI in reality and
in VR and validates the utilization of the RHI in VR. Hence, we
show that researchers and designers can leverage VR technology
to perform classical RHI experiments to further study the cognitive
processes underlying BOIs.
2 RELATED WORK
Our work is based on a growing body of work demonstrating perceptual and physiological effects caused by the RHI. In this section,
we first provide an overview of RHIs and the effects on humans experiencing artificial limbs as their own. Afterwards, we summarize
previous work that cover RHIs in immersive virtual settings.
2.1 Rubber Hand Illusions
First demonstrations of an effect similar to the RHI were already
published in 1937 by Tastevin [68], who reported that people could
experience a plastic finger as their own finger, which was concealed
from view using a piece of cloth. After the seminalRHI from 1998 [6]
ignited the research interest in such perceptual illusions, many
researchers across various fields used such perceptual illusions to
learn about human cognition. There are some requirements that
have to be met to be able to induce the RHI [30].
Typically, researchers apply synchronous visuo-tactile stimulations creating a synchrony between the seen stroking of the rubber
hand and the felt stroking of the real hand (e.g., [2, 6, 72]). Slater
et al. [63], for example, used a soft ball attached to a wand to tap
and stroke the participants’ arm. Asynchronous stroking, however,
destroys the illusion, e.g., a temporal delay between stroking of
the rubber hand and real hand [ 52], as the brain is not able to
integrate the cues from different sensory modalities into a unified percept [23]. Kalckert and Ehrsson [26] applied synchronous
visuo-motor stimulations by enabling the participants to move
a finger of the rubber hand. This resulted in a visuo-motor synchrony so that participants felt their own finger movements and synchronously saw the finger of the rubber hand moving [11]. Kalckert
and Ehrsson [27] showed that the illusion is equally strong for tactile stimulations or active movements. Giummarra et al. [18] even
demonstrated that the mere observation of a rubber hand in an
anatomical plausible position and posture is sufficient to invoke the
RHI; however, the illusion can be enhanced through visuo-motor
contingencies [18]. Furthermore, Kilteni et al. [30] concluded that
it is necessary for the illusion to occur that the artificial limb has
to satisfy to some extent semantic constraints, e.g., it has to conform to humans’ anatomical structures [71]. Non-corporeal objects
that violate human anatomy such as checkerboards cannot create a
sense of embodiment [81].
Riemer et al . [52] provided a summary of sophisticated approaches that are used to quantify theRHI. Validated questionnaires
are a common method to assess the experiencedRHI. Different subscales and items, e.g., “it seemed like the rubber hand was my hand”
or“it seemed like the rubber hand belonged to me” [44], have been
used to measure the degree of the felt embodiment of the rubber
hand. Besides, perceptual responses such as the proprioceptive drift
were assessed during or immediately after the RHI [51, 72]. The
proprioceptive drift describes the illusory shift in location of the
own hand towards the rubber hand, so that participants perceive
their own hand being closer to the rubber hand. Further objective
measures for quantifying the RHI are physiological responses.
While various studies also used arousal-related metrics to assess
physiological reactions to a threatened rubber hand (see [ 13, 30,
52]), Moseley et al. [47] were the first demonstrating that embodying a rubber hand caused a drop in temperature in the real hand. The
authors argued that these findings indicate that a process of disembodiment of the real hand occurs during theRHI. Moseley et al. [46]
reported a possible explanation for this phenomenon and concluded
that the blood flow to the “disembodied” hand was reduced while
embodying the rubber hand. In line with these findings, Kammers
et al. [29] modulated the extent of the RHI by manipulating the
temperature of the participants’ hand. Cooling their hand increased
the strength of the RHI whereas warming decreased its strength.
Furthermore, Salomon et al. [56] induced a full-body illusion by
synchronously stroking the participants’ back and legs. Accordingly, the authors found a drop in skin temperature across different
body parts.
Another study found that the histamine reactivity of the own
hand was increased during the RHI, which is an indicator for a
decreased response of the immune system [5]. Folegatti et al. [16],
however, hypothesized that changes in skin temperature originate
from the visuo-proprioceptive conflict induced by the RHI instead

## Page 3

The Rubber Hand Illusion in Virtual Reality and the Real World - Comparable but Different VRST ’22, November 29-December 1, 2022, Tsukuba, Japan
of a process of disownership. The authors did not use an artificial
limb such as a rubber hand but, instead, they shifted the position of
the real hand by 7.5 cm using prismatic goggles. By doing so, they
still slowed down tactile sensitivity and induced a proprioceptive
drift even if it was the own hand. On the contrary, Hohwy and
Paton [24] could show a decreased skin temperature using a rubber
hand which was co-located with the real hand..
Even if these intriguing findings suggest that the RHI can affect
unconscious and autonomic bodily functions such as thermoregulation, many researchers call such effects into question as they could
not be replicated in various other studies [9, 10, 20, 48, 54, 69]. As
such, de Haan et al. [10] and Rohde et al. [54] discussed potential
factors that confound effects on skin temperature during the RHI,
e.g., the speed, force and duration of stroking, lighting conditions,
and the characteristics of the experimenter. Hence, it still remains
unknown whether there is a causal relationship between the experienced embodiment of the rubber hand, the disownership of the
real hand, and the resulting effects on skin temperature.
2.2 Bodily Illusions in VR
Research from human-computer interaction (HCI) applies the knowledge from experiments inducing bodily illusions to create vivid
and effective VR experiences using virtual avatars [35, 38, 40, 41,
62]. Slater et al. [63] transferred the concept of the RHI into VR by
tapping and stroking the participants’ real arm using a soft ball and
accordingly displaying this tactile stimulation by a virtual soft ball
on a virtual arm rendered on a large display in front of the participants. The authors reported that the participants could experience
a sense of embodiment over the virtual arm.
Similar effects were revealed in another study where the authors
generated a virtual arm illusion [64]. Likewise, Yuan and Steed[80]
wondered whether theRHI can be induced by immersiveVR. In contrast to the “classical” RHI paradigm, the participants could move
their virtual arms while being embodied in a full-body avatar. The
embodiment of a full-body avatar with features and characteristics
that deviate from the users’ real physical body can evoke perceptual
and attitudinal changes [ 34, 36, 39, 79]. Thus, it is impossible to
isolate the effects caused by the limb ownership of one body part,
such as a virtual arm, from effects caused by the body ownership
of an entire body, which addresses the bodily self as a whole [7].
Another series of studies showed that users can embody virtual
hands with a reduced amount of fingers [33, 59], with a different
gender [60] as well as with a non-human appearance such as robot
hands [61]. As the authors wanted to create a natural and familiar
interaction with the VE, the participants’ arm and hand movements
were tracked using motion capture systems and transferred onto
the animation of the virtual hands. This is in line with Ma et al .
[45] or Ariza et al . [1], who also used hand tracking technology
to induce a virtual hand illusion. Hence, instead of a passive induction through visuo-tactile synchrony, the authors applied an
active induction through visuo-motor synchrony [57]. As bodily
illusions are modulated by visuo-tactile, visuo-motor and visuoproprioceptive cues [ 30], the type of stimulation influences the
experienced embodiment.
Similar to real world experiments, perceptual, behavioral and
physiological responses are used for quantifying the RHI [30]. Previous work found that users instinctively reacted to a virtual knife
stabbing the embodied virtual hand by moving the threatened hand
out of the way to avoid being injured [ 19]. Kocur et al. [33] also
showed emotional responses such as phantom pain when removing single fingers of the virtual hand. Tieri et al. [70] investigated
the hand temperature and showed that a first-person perspective
was sufficient to induce a limb ownership illusion of a virtual arm
with different appearances, e.g., anthropomorphic or wooden. The
authors found an increase in hand temperature for all types of arm
appearances. However, the increase was lower during the embodiment of the anthropomorphic virtual arm. These results suggest
that the effects on hand temperature are modulated by the vividness
of the ownership illusion.
In a review about bodily illusions, Braun et al . [7] concluded
that users can even experience a sense of ownership of full-body
avatars. Previous work induced a body ownership of avatars, for
example, with a different muscular [37] and athletic [34] appearance
or with a different age [3, 4, 39, 50]. Overall, in all these studies the
experimental design did not involve a control condition consisting
of an artificial arm illusion or even full-body illusion performed in
the real world, e.g., using a rubber hand or a mannequin [49].
2.3 Summary
The RHI can cause perceptual and physiological changes, such as an
elevated skin conductance response [13] or increased heart rate [65].
While some studies even revealed that the embodiment of a rubber
hand causes a drop in skin temperature of the own hand [ 24, 29,
47, 56, 73], others could not show such thermal reactions [9, 10, 20,
48, 54, 69]. Designers and researchers of VR applications apply the
knowledge gained from BOIs in the real world to induce ownership
of virtual avatars. However, a systematic comparison between the
effects caused by BOIs in the real world and BOIs in VR has not
been conducted yet.
3 METHOD
To find out whether the RHI induced in the real world differs from
a RHI in VR and compare the magnitude of effects between both
environments, we induced a RHI based on the experimental procedure by Moseley et al . [47] in both environments. We further
explored whether the RHI can cause skin temperature changes of
the own hand.
3.1 Study Design
We conducted a study using a within-subjects design with two
independent variables. To deteremine whether the effects of the
RHI induced in the real world differ from a RHI induced in VR, we
used the independent variable Environment with the two levels
real and VR. In the real condition, the RHI was conducted in the
real world whereas in the VR condition, the RHI was conducted in
VR using a virtual replica of the real environment (see Figure 1).
As previous work found that it is crucial that the real hand and the
rubber hand are touched at the same time to induce the RHI and
that temporal deviations between the seen and the felt touch stop
the illusion from occurring [30], we systematically manipulated the

## Page 4

VRST ’22, November 29-December 1, 2022, Tsukuba, Japan Kocur et al.
Figure 1: RHI performed in the real world and in VR (top), and the participants’ view of the real environment and the VE
(bottom). Participants saw the rubber hand being stroked while their real hands were hidden from view.
synchrony of the applied tactile and visual cues to modulate the
RHI. Hence, we used the independent variable Synchrony with
the two levels synchronous and asynchronous.
In the synchronous condition, we synchronously stroked the
participants’ real hand and the rubber hand in time and at the
correct position so that the participants saw and felt the stroking
congruently. In the asynchronous condition, we created a temporal
delay of approximately 5 s (duration of one stroke) between the
stroking on the rubber hand and the real hand by stroking both of
them alternately. This temporal delay between the visual perception
and the tactile perception of the stroking should prevent the illusion
from occurring [6, 15]. Hence, the asynchronous stimulation served
as a control condition allowing to control for effects caused by
the embodiment of the rubber hand. To reduce order effects, we
counterbalanced the order of the conditions employing all possible
permutations.
3.2 Measures
We took multiple measures to determine the effects of the independent variables. We assessed the proprioceptive drift and used aRHI
questionnaire [44] for quantifying the RHI. Additionally, we measured the skin temperature of both hands during the entire course
of each condition to analyze how the skin temperature evolves
across time. As handedness does not modulate the extent of the
RHI [66], we determined the right hand to be the stimulated hand,
which was stroked and hidden from view during the procedure.
The left hand was used as a control hand (unstimulated hand) and
was neither touched nor seen during the RHI procedure.
3.2.1 Proprioceptive Drift. We measured the proprioceptive drift,
which describes a shift of the stimulated hand’s perceived location
towards the rubber hand. A higher proprioceptive drift indicates
a stronger RHI [72]. To assess this illusory drift, we used the ruler
technique, which is a widely used strategy to quantify the proprioceptive drift [52]. After each condition, we placed a ruler above the
participants’ right hand (stimulated) and the rubber hand, which
were both hidden and could not be seen during the assessment
of the proprioceptive drift. For the RHI in VR, we used a virtual
ruler with the same scales as the physical ruler. We then asked the
participants to verbally indicate the number that is directly above
their own index finger.
3.2.2 RHI Questionnaire. We asked the participants to fill the RHI
questionnaire designed by Longo et al . [44] for quantifying the
experienced RHI. The questionnaire consists of seven-point Likert
items ranging from “strongly disagree” to “strongly agree”. The
items reflect five dimensions: embodiment of rubber hand , loss of
own hand, movement, affect and deafference. For the VR condition,
we changed the term “rubber hand” into “virtual rubber hand”. At
the end of the questionnaire, we added an additional item which
should explore whether the participants perceived any change in
skin temperature in the right hand (stimulated). Accordingly, we
used a seven-point Likert item ranging from “cooling” to “heating”.

## Page 5

The Rubber Hand Illusion in Virtual Reality and the Real World - Comparable but Different VRST ’22, November 29-December 1, 2022, Tsukuba, Japan
In all conditions, the questionnaire was administered on a desktop
computer.
3.2.3 Skin Temperature. We continuously measured the participants’ skin temperature on their right and left hand to control
whether potential effects on skin temperature are limb-specific. If effects on the skin temperature originate from the embodiment of the
rubber hand, they should not occur on the unstimulated hand [47].
We therefore evaluated the time course of the temperature difference between the right hand (stimulated) and the left hand (unstimulated) across the entire stroking procedure. To calculate the temperature difference between both hands, we subtracted the temperature
on the left hand (unstimulated) from the temperature on the right
hand (stimulated): ∆𝑡 = t(stimulated hand) −t(unstimulated hand) .
A negative difference indicates a lower temperature in the right
hand (stimulated) than in the left hand (unstimulated). We therefore hypothesize that the negative difference between both hands
increase over time due to a decrease in temperature of the right
hand (stimulated). Additionally, we also analyzed the absolute skin
temperature of the right hand (stimulated) and the left hand (unstimulated) across time.
3.3 Apparatus
We employed the same apparatus as proposed by Kalus et al. [28].
We used two black cardboard boxes (45cm x 35cm x 23cm) with
cut holes placed on a table in front of the participants to hide
their hands (both the right and the left hand) during the RHI. The
male experimenter sat opposite the participants and used two common paintbrushes to stroke the rubber hand and the participants’
right hand. The experimenter also used in-ear headphones and a
metronome application running on a smartphone for pacing each
stroke.
As prior investigations found that seeing the experimenter during the stroking may influence the experience of touch [10, 17], we
used a window roller blind mounted on two wooden bars to avoid
that the participants could see the experimenter during the RHI.
Thus, the participants only saw the experimenter’s hand stroking
the rubber hand. A life-sized rubber model of a right human arm
(AFM-BLM Male flexible arms large hands medium arms, Hollands
Wondere Wereld vof, the Netherlands) was placed in front of the
participants in an anatomically plausible posture. The participants
wore a large black hairdressing cape to cover the forearm of the
rubber model and to ensure that the participants could not see their
own body parts during the RHI.
To measure the participants’ skin temperature, we used a professional thermometer module with a sampling rate of 10 Hz and
a resolution of 20 bit (TC-08 8-Channel USB Thermocouple Data
Acquisition Module, Omega Engineering, USA). We used four insulated T-thermocouples (Fast response insulated thermocouple
with connectors: 5SRTC-TT-TI-20-2M, Omega, USA) to assess the
skin temperature on each hand. To increase measurement accuracy
and compensate for a potential malfunction of a thermocouple, we
attached two thermocouples on the back of the right hand and
another two on the back of the left hand using a common adhesive
tape. To assess the proprioceptive drift, we used a printed paper
ruler (centimeter ruler for A3 paper, 80 cm) placed on a wooden
board. As the proprioceptive drift was measured four times in total
(once per condition), we used four rulers with different scales to
avoid biased answers caused by the recall of previous responses
and memory effects. Each ruler was only used once per experiment
and was randomly chosen for the conditions. Additionally, the experimenter used a USB foot switch to log UNIX timestamps for
determining the start and end of each condition.
To be able to compare the RHI conducted in the real world and
the RHI in VR, we designed a virtual replica of the real environment
with the identical experimental setup as in reality (see Figure 1).
We used the game engine Unity3D (v. 2019.2.1f1) to develop the
VR application. We designed a virtual rubber hand using a rubber
shader. We also designed a realistic virtual hand holding a paintbrush, which represented the experimenter’s hand stroking the
virtual rubber hand. To avoid tracking errors and reduce temporal deviations between the applied tactile and visual cues due to
the latency of the VR system, we created a stroking animation to
precisely simulate the stroking of the experimenter. A screen was
placed next to the experimenter displaying the participants’ view of
the VE. This allowed the experimenter to align the stroking of the
real hand to the stroking of the virtual hand in the VR condition.
We used an HTC Vive head-mounted display (HMD) (HTC Corporation, Tayuan, Taiwan) with a wide horizontal field of view
of 100° and a spatial resolution of 1080 × 1,200 pixels per eye. In
line with the real environment, their virtual body was covered by
a cloth-simulated cape. The VR application ran on a desktop PC
(MS-Windows 10, Intel i7-8750H, 16GB RAM, NVIDIA GeForce
GTX 1060 graphics card). The project files and the source code of
the VR prototype are available on github1.
3.4 Participants
We recruited 24 participants (14 male and 10 female) through our
university’s mailing list and public forums. Their age ranged from
19 to 29 years (M = 23.91 SD = 2.45). All of them had either normal
or corrected-to-normal vision. None of them reported any pain in
the upper limbs (shoulder, arm or hand region) before the study.
One participant was left-handed. Participants received course credits for participating in the study. They were informed that they
could withdraw or discontinue the experiment at any time without
penalty.
3.5 Procedure
After welcoming the participants, we explained the procedure of
the study. We then asked them to sign an informed consent form
and to complete the demographics questionnaire. Afterwards, the
participants sat at the table at a predefined position 37.5 cm from
the body’s midline (coronal plane) to the rubber hand. In the VR
condition, the experimenter helped the participants with putting on
the HMD, adjusted it to their head, and calibrated the inter-pupil
distance if necessary. Afterwards, the participants put their right
and left hand into the cardboard boxes to keep both hands out of
view.
The experimenter placed the hairdressing cape over the participants’ shoulders to cover their body and the forearm of the
rubber hand model. The experimenter then took a seat opposite
the participants and attached the thermocouples on both of their
1https://github.com/a-kalus/virtual_rhi

## Page 6

VRST ’22, November 29-December 1, 2022, Tsukuba, Japan Kocur et al.
0
2
4
6
8
10
12
real VR
prop. drift in cm
0
1
2
3
4
real VR
embodiment
0
1
2
3
real VR
loss of own hand
0
1
2
real VR
movement
0
1
2
3
4
5
real VR
affect
0
2
4
6
8
10
12
real VR
proprioceptive drift (cm)
synchrony synchronous asynchronous
Figure 2: Mean values of the proprioceptive drift (cm) and the dimensions of the RHI questionnaire embodiment, loss of
own hand, movement, and affect for the RHI performed in the real world and in VR. The error bars show the 95% confidence
interval.
hands using tape. The experimenter precisely positioned the participants’ hands at a fixed location marked with tape strips on the
table. The participants were asked to keep their hands still during
the procedure. The tip of the right index finger was 22.5 cm from
the rubber hand’s tip of the index finger. This distance conforms to
the mean of distances used in a series of studies by Moseley et al.
[47]. Before a trial started, the roller blind was lowered to ensure
that the participants could not see the experimenter except for the
hand stroking the rubber hand.
The experimenter started the conditions by pressing the foot
switch and beginning to stroke. Each stroke started from the wrist
along the index finger to the finger tip resulting in a stroking
distance of ~15 cm. In line with current recommendations about
stroking velocity [52], we used a velocity of ~3 cm/s so that each
stroke lasted ~5 s. After a stroke, the experimenter immediately
repositioned the brushes at the wrist and started the next stroke. In
the VR condition, a stroking animation was displayed so that the
experimenter only stroked the real hand aligned to the animation.
After three minutes of stroking per condition, the proprioceptive
drift was assessed. Therefore, the roller blind was rolled up and the
ruler attached on a wooden board was placed above the participants’
right hand as well as the rubber hand. We asked the participants
to verbally indicate the number that is directly above their own
index finger. In the VR condition, the experimenter triggered an
event using the HTC Vive controller, which simulated the realworld setting by automatically rolling up the virtual roller blind
and placing the virtual ruler at the same position in the VE.
The experimenter then removed the thermocouples, and helped
the participants with taking off the hairdressing cape and theHMD.
Afterwards, the participants completed the RHI questionnaire on a
desktop computer. This procedure is repeated for each condition.
The study took approximately 60 minutes per participant in total.
4 RESULTS
Our measures consist of parametric data. We used Shapiro-Wilk
tests to determine the assumption of normal distribution of the
proprioceptive drift and the scores of the RHI questionnaire (all
𝑝 > .05). As skin temperature is normally distributed across the
population, we also assume a normal distribution of the skin temperature data.
4.1 Proprioceptive Drift
A 2(Environment:real vs. VR) x 2( Synchrony: synchronous vs.
asynchronous) ANOVA revealed a significant main effect of Environment, 𝐹(1,23)= 14.426, 𝑝 < .001, η2𝑝 = .385, on the proprioceptive drift. Participants showed a generally larger proprioceptive drift in VR compared to the real environment (10.2cm vs.
7.6cm). There was also a significant main effect of Synchrony,
𝐹(1,23) = 6.591, 𝑝 = .017, η2𝑝 = .222, indicating a higher proprioceptive drift in the synchronous conditions compared to the
asynchronous conditions (9.7 cm vs. 8.1 cm). However, there was
no significant interaction effect of Environment ×Synchrony,
𝐹(1,23)= .139, 𝑝 = .712, η2𝑝 = .006. The non-significant interaction
effect Environment ×Synchrony revealed by the ANOVA does
not automatically confirm the hypothesis that the difference in
proprioceptive drift between the synchronous condition and the
asynchronous condition is comparable between environments.
To quantify the comparability of the effects between VR and
the real world, we calculated a Bayesian t-test on the differences
between the proprioceptive drift in the synchronous condition and
the asynchronous condition (∆PropDrift = PropDrift𝑠𝑦𝑛𝑐 −PropDrift𝑎𝑠𝑦𝑛𝑐 ) for both settings [77]. This revealed a Bayes factor of
𝐵𝐹01 = 4.371, indicating that the data is 4.37 times more likely
under the null hypothesis postulating identical RHI effects on proprioceptive drift for VR and the real environment (∆PropDrift𝑉 𝑅
= ∆PropDrift𝑟𝑒𝑎𝑙 ) than under the alternative hypothesis that postulates different effects (∆PropDrift𝑉 𝑅≠ ∆PropDrift𝑟𝑒𝑎𝑙 ). Figure 2
depicts the mean ratings of the proprioceptive drift.
4.2 RHI Questionnaire
We performed 2(Environment:real vs. VR) x 2(Synchrony: synchronous vs. asynchronous) ANOVAs on each dimension of the RHI
questionnaire. Figure 2 shows the mean ratings for the dimensions
embodiment,loss of own hand , movement, and affect.
We did not find any significant effect of Environment on the
dimensions of the RHI questionnaire (all 𝑝 > .05). However, we
found a significant effect of Synchrony on the dimensions embodiment of the rubber hand , 𝐹(1,23)= 43.443, 𝑝 < .001, η2𝑝 = .653,
loss of own hand , 𝐹(1,23)= 9.224, 𝑝 = .005, η2𝑝 = .286, movement,
𝐹(1,23)= 7.951, 𝑝 = .009, η2𝑝 = .256, and affect, 𝐹(1,23)= 21.371,
𝑝 < .001, η2𝑝 = .481. We did not find any significant interaction

## Page 7

The Rubber Hand Illusion in Virtual Reality and the Real World - Comparable but Different VRST ’22, November 29-December 1, 2022, Tsukuba, Japan
real VR
0.5 1 1.5 2 2.5 3 0.5 1 1.5 2 2.5 3
−0.3
−0.2
−0.1
0.0
0.1
time (minutes)
Δ t = t(stimulated) − t(unstimulated) in °C
synchrony synchronous asynchronous
Figure 3: Average temperature difference ( ∆𝑡) between the right (stimulated) and left hand (unstimulated) per 30 seconds during
the RHI in the real world and in VR for synchronous and asynchronous stroking. The error bars show the standard error.
effect Environment ×Synchrony on the dimensions of the RHI
questionnaire. The calculated Bayes factor showed anectodal to
moderate evidence (𝐵𝐹01 >= 2.162 and 𝐵𝐹01 <= 4.589) that the
data is more likely under the null hypothesis postulating identical
RHI effects on the dimensions of the RHI questionnaire for VR and
the real environment. Figure 2 depicts the average proprioceptive
drift and the mean ratings of the RHI questionnaire.
4.2.1 Correlation Analysis of the Proprioceptive Drift and the Dimensions of the RHI Questionnaire. To test whether there is a relationship between the proprioceptive drift and the experienced
embodiment of the rubber hand, we performed a Pearson’s correlation analysis of the dimensions of the RHI questionnaire and
the proprioceptive drift in the synchronous conditions. We did not
find a significant relationship between proprioceptive drift and
the dimensions embodiment of the rubber hand , loss of own hand ,
movement and deafference of the RHI questionnaire (all 𝑝 > .05).
However, there was a significant positive correlation between the
proprioceptive drift and the dimensionaffect, 𝑟(46)= .333, 𝑝 = .020.
4.3 Skin Temperature
As previous work found that a drop in skin temperature was caused
by the embodiment of the rubber hand and, thereby, only occurred
in the stimulated hand and not in the unstimulated hand [47], we
evaluated the time course of the temperature difference between
the right hand (stimulated) and the left hand (unstimulated) across
the entire stroking procedure (see Figure 3). Additionally, we analyzed the absolute skin temperature of the right (stimulated) and left
hand (unstimulated) across time (see Figure 4). In line with Moseley
et al. [47], we calculated 30-second time intervals and included the
factor TIME with six levels in the statistical analyses. Hence, we
performed 2(Environment:real vs. VR) x 2(Synchrony: synchronous vs. asynchronous) x 6(Time: 0.5 vs 1 vs 1.5 vs 2 vs 2.5 vs 3)
ANOVAs to analyze the skin temperature across time.
4.3.1 Skin Temperature Difference between Both Hands. We did
not find a significant main effect of Environment, 𝐹(1,23)= .581,
𝑝 = .453, η2𝑝 = .024, of Synchrony, 𝐹(1,23) = .704, 𝑝 = .409,
η2𝑝 = .029 and of Time, 𝐹(5,115)= 2.074, 𝑝 = .073, η2𝑝 = .082. However, we found a significant interaction effect ofSynchrony ×Time,
𝐹(5,115)= 4.829, 𝑝 < .001, η2𝑝 = .173, indicating that the skin
temperature differences between both hands over the course of
time depended on the synchrony of stroking. We did not find interaction effects of Environment ×Synchrony, 𝐹(1,23)= .048,
𝑝 = .827, η2𝑝 = .002, of Environment ×Time, 𝐹(5,115)= .185, 𝑝 =
.967, η2𝑝 = .007, as well as of Environment ×Synchrony ×Time,
𝐹(5,115)= .360, 𝑝 = .874, η2𝑝 = .015. Bonferroni-corrected post-hoc
comparisons revealed significant differences between the skin temperature difference in synchronous condition in the first 30 seconds
and the synchronous condition in the third (last) minute (𝑝 < .001).
All other pairwise comparison were not significant (𝑝 > .05).
4.3.2 Absolute Skin Temperature. To analyze the absolute skin
temperature, we additionally included the factor Hand into the
statistical analysis. There was no significant main effect of Environment, 𝐹(1,23)= .021, 𝑝 = .885, η2𝑝 = .000, of Synchrony,
𝐹(1,23)= .0.204, 𝑝 = .655, η2𝑝 = .008, and of Hand, 𝐹(1,23)= .347,
𝑝 = .561, η2𝑝 = .014. However, we found a significant main effect of Time on the absolute skin temperature, 𝐹(5,115)= 27.835,
𝑝 < .001, η2𝑝 = .547. There was also an interaction effect of Environment ×Time, 𝐹(5,115)= 2.666, 𝑝 = .025, η2𝑝 = .103. We
also found an interaction effect of Synchrony ×Hand ×Time,
𝐹(5,115)= 4.829, 𝑝 < .001, η2𝑝 = .173. Other interaction effects
were not significant (all 𝑝 > .05).
4.3.3 Correlation Analysis of the Proprioceptive Drift, the Skin Temperature Difference, and the RHI Questionnaire. We performed a
Pearson’s correlation analysis of all measures to test whether there
is a relationship between the propriceptive drift and the skin temperature, as well as theRHI questionnaire and the skin temperature
in the last minute (the third minute) in the synchronous conditions.
However, we did not find a significant relationship between the
measures (all 𝑝 > .05).

## Page 8

VRST ’22, November 29-December 1, 2022, Tsukuba, Japan Kocur et al.
real VR
synchronousasynchronous
0.5 1 1.5 2 2.5 3 0.5 1 1.5 2 2.5 3
33.2
33.6
34.0
33.2
33.6
34.0
time (minutes)
temperature in °C
left hand (unstimulated)right hand (stimulated)
Figure 4: Average temperature per 30 seconds during the RHI in the real world and in VR for synchronous and asynchronous
stroking for the left (unstimulated) and right hand (stimulated), respectively. The error bars show the standard error.
5 DISCUSSION
As predicted for both environments, participants had a higher proprioceptive drift during synchronous stroking compared to asynchronous stroking. In VR, the proprioceptive drift was generally
higher compared to the real world. As indicated by questionnaire
ratings, we found that the participants experienced a stronger RHI
during synchronous stroking in both environments.
Our results also revealed that the RHI affected the skin temperature of the own hands. Even if the skin temperature of both hands
increased in all conditions, the interaction between synchrony
and time indicates that skin temperature difference between right
(stimulated) and left (unstimulated) hand increasingly diverge from
each other over time due to synchronous stroking (see Figure 3).
Hence, there was a lower increase in skin temperature of the stimulated hand during synchronous stroking compared to the increase
in skin temperature of the unstimulated hand.
5.1 Physical RHI vs Virtual RHI
We found systematic effects of the RHI performed in the real world
and in VR on the proprioceptive drift and the questionnaire ratings.
In line with findings from RHI experiments (e.g., [14, 72, 78]), we
found a significant higher proprioceptive drift as well as significant higher scores for each dimension of the RHI questionnaire
during synchronous stroking compared to asynchronous stroking.
However, the proprioceptive drift was generally higher in the RHI
conducted in VR compared to the real world.
This is not necessarily an implicit indicator for a higher degree
of ownership of the virtual rubber hand in VR. Instead, other factors such as a reduced field of view due to the HMD or a different
depth perception inVR could be responsible for such effects [25, 76].
This assumption may be supported by the fact that we could not
find significant differences between the effects of both environments on the ratings of the RHI questionnaire. We also did not
find any correlation between the perceived embodiment assessed
by questionnaire ratings and the proprioceptive drift. This is not
surprising as previous investigations found that both measures are
not necessarily related to each other due to different underlying
mechanisms [53, 74].
When being immersed in VR, not only is the user’s hand “replaced” by the virtual rubber hand but the entire body by the virtual
body. In other words, inVR the participants did not only experience
a limb ownership illusion of the rubber hand but also a full-body
ownership illusion of the virtual body. This is in line with Llobera
et al. [42], who postulated that when participants enter the VR and
perceive a VE from a first-person perspective, the virtual body substitutes the entire real body. Even if we covered the real and virtual
body by a hairdressing cape to minimize all identity cues to ensure a
high concordance between the real world and VR, small deviations
between the own body and virtual self can activate the illusion
of embodiment. As we asked about the distance between the real
hand and the virtual rubber hand to assess the proprioceptive drift,
the position of the real hand, which is a part of the virtual body in
VR, can already be misperceived resulting in a higher proprioceptive drift. Future studies should investigate whether multisensory
asynchrony, e.g., caused by latency, breaks the illusion on full-body
level or only on limb ownership.
For the proprioceptive drift and the ratings of the RHI questionnaire, we could not find an interaction effect of the environment
in which the RHI was performed and the synchrony of stroking.
However, this does not automatically confirm that the difference in
proprioceptive drift and the dimensions of the RHI questionnaire
between the synchronous condition and the asynchronous condition
is comparable between environments. The calculated Bayes factors,

## Page 9

The Rubber Hand Illusion in Virtual Reality and the Real World - Comparable but Different VRST ’22, November 29-December 1, 2022, Tsukuba, Japan
however, showed anectodal to moderate evidence (𝐵𝐹01 >= 2.162
and 𝐵𝐹01 <= 4.589) that the data is more likely under the null
hypothesis postulating identical RHI effects on the proprioceptive
drift and the dimensions of the RHI questionnaire. Hence, our findings suggest that VR technology can be leveraged to create RHIs
and increase our understanding of embodying virtual avatars.
5.2 Effects on Skin Temperature
To explain the effects on skin temperature caused by the RHI, we
refer to Moseley et al . [47] who revealed that the RHI causes a
decrease in skin temperature of the own hand. Notably, the skin
temperature of other body parts were unaffected, i.e., the other hand
and the feet did not cool. This suggests that the effects depended
on the illusion of ownership of the rubber hand.
Moseley et al. [46] introduced the concept of the cortical body
matrix to explain the effects of bodily illusions. When the real and
the rubber hand are stroked synchronously, the neural areas associated with the space occupied by the rubber hand increase their
activity starting to incorporate it into the own body schema, which
in turn results in the sensation of the rubber hand being a part of the
actual body. On the contrary, the neural areas associated with the
space around the real hand decrease their activity, which in turn decreases the extent to which the real hand is “owned” and eventually,
results in reduced homeostatic controls, e.g., thermoregulation.
As parts of the cortical body matrix has connections with parts
in the brain that regulate autonomic functions, the authors assume
that the blood flow to the “disowned” hand is reduced causing a drop
in skin temperature. These explanations are in line with Barnsley
et al. [5], who showed that participants had an increased histamine
reactivity in the stimulated hand during the RHI. As an elevated
histamine reactivity is associated with a decreased response of the
immune system resulting in a reduced metabolism of histamine,
the authors concluded that the stimulated hand during the RHI is
treated as when it has been “rejected” [5].
In contrast to Moseley et al . [47], however, it is important to
note that we did not induce a cooling of the stimulated hand in
a sense that the skin temperature at the end was lower than at
the beginning of the RHI. Instead, we found a constant increase
in skin temperature of both hands regardless of the vividness of
the experienced RHI (see Figure 4). This seemed to be the “normal”
physiological response in our experiment. However, our results
show that the temperature of the stimulated and unstimulated
hand increasingly diverge across time during synchronous stroking
(see Figure 3 and 4). During asynchronous stroking, such effects
did not occur. We therefore assume that RHI decreased the skin
temperature of the stimulated hand in a sense that it attenuated the
“normal” increase in skin temperature that occurred in this situation
under those circumstances. Although our laboratory is temperaturecontrolled, the environmental temperature directly around and
within the experimental area could also possibly increase affecting
the participants’ skin temperature. Furthermore, we cannot dismiss
thermal reactions caused by social contact through the touch of the
experimenter [10, 22, 54].
As we could not find a correlation between the skin temperature
differences and the ratings of the RHI questionnaire as well as the
proprioceptive drift, we cannot conclude that the embodiment of
the physical or virtual rubber hand was responsible for a decreased
temperature of the stimulated hand. In accordance to Folegatti et al.
[16], we therefore cannot dismiss that changes in skin temperature
were caused by the perceptual conflict that is created during the
RHI, i.e. the mismatch between the felt and seen tactile cues [16].
5.3 Implications and Future Work
Due to our findings, we argue that the RHI can be transferred into
VR resulting in similar and comparable effects. As VR serves an
extended design space, it is possible to produce experiences that
are hardly feasible or impossible to create in the real world. Virtual
rubber hands, for example, with a reduced amount of fingers [33, 59],
with a burning skin [12], or with a supernatural length [31] can be
easily designed in a VE allowing a high degree of control over the
experimental variables.
Regarding the effects on the skin temperature, it is important to
consider this phenomenon when creating embodiedVR experiences.
Researchers have to know how limb ownership illusions influence
the basal skin temperature as such effects may confound physiological measurements, e.g., the skin conductance response [43]. As the
human body’s temperature regulation processes involve thermal
signals from the skin [55], the activity of sweat glands therefore
partially depends on the skin temperature [43].
Such effects may also be explained within the theoretical framework of the Proteus effect that describes behavioral, perceptual, and
attitudinal changes caused by an avatar’s stereotypical visual appearance [32, 34, 37, 79]. The embodiment of a virtual hand whose
rubbery appearance is associated with artificiality and inanimateness may potentially could cause participants to move their hand
less in terms of micromovements than they would with a vital and
lifelike hand resulting in a drop in skin temperature. This can be
addressed in future work.
6 CONCLUSION
In this paper, we compared the RHI in the real world with a RHI in
VR. We conducted a study with 24 participants who experienced
the RHI in the real world and in VR. The proprioceptive drift as
well as the ratings of the RHI questionnaire were higher during
synchronous stroking compared to asynchronous stroking in both
environments. Equivalent tests using the Bayes factor revealed
that the differences between the effects on the proprioceptive drift
and the ratings of the RHI questionnaire caused by synchronous
stroking and asynchronous stroking were more likely identical
for both environments. These findings imply that the RHI causes
similar and comparable effects in both environments. Hence, this
work validates that the RHI can be leveraged in VR to increase our
understanding of BOIs and the virtual embodiment of avatars.
We also found that the RHI affected the skin temperature of the
real hands. Even if the skin temperature of both hands increased,
the skin temperature of the right hand (stimulated) and the left hand
(unstimulated) increasingly diverge from each other across time
during synchronous stroking. These insights extend our knowledge
about the consequences of limb ownership illusions for the own
body and illustrate the psychophysiological impact of embodying
virtual limbs on users.

## Page 10

VRST ’22, November 29-December 1, 2022, Tsukuba, Japan Kocur et al.
REFERENCES
[1] Oscar Ariza, Jann Freiwald, Nadine Laage, Michaela Feist, Mariam Salloum, Gerd
Bruder, and Frank Steinicke. 2016. Inducing Body-Transfer Illusions in VR by
Providing Brief Phases of Visual-Tactile Stimulation. In Proceedings of the 2016
Symposium on Spatial User Interaction (Tokyo, Japan) (SUI ’16). Association for
Computing Machinery, New York, NY, USA, 61–68. https://doi.org/10.1145/
2983310.2985760
[2] Carrie Armel and Vilayanur S. Ramachandran. 2003. Projecting sensations to external objects: evidence from skin conductance response.
Proceedings of the Royal Society of London. Series B: Biological Sciences
270, 1523 (2003), 1499–1506. https://doi.org/10.1098/rspb.2003.2364
arXiv:https://royalsocietypublishing.org/doi/pdf/10.1098/rspb.2003.2364
[3] Domna Banakou, Raphaela Groten, and Mel Slater. 2013. Illusory ownership of
a virtual child body causes overestimation of object sizes and implicit attitude
changes. Proceedings of the National Academy of Sciences of the United States of
America 110, 31 (2013), 12846–12851. https://doi.org/10.1073/pnas.1306779110
[4] Domna Banakou, Sameer Kishore, and Mel Slater. 2018. Virtually being Einstein
results in an improvement in cognitive task performance and a decrease in age
bias. Frontiers in Psychology 9, JUN (2018). https://doi.org/10.3389/fpsyg.2018.
00917
[5] N. Barnsley, J.H. McAuley, R. Mohan, A. Dey, P. Thomas, and G.L. Moseley. 2011.
The rubber hand illusion increases histamine reactivity in the real arm. Current
Biology 21, 23 (2011), R945–R946. https://doi.org/10.1016/j.cub.2011.10.039
[6] Matthew Botvinick and Jonathan Cohen. 1998. Rubber hands ‘feel’ touch that
eyes see. Nature 391, 6669 (1998), 756. https://doi.org/10.1038/35784
[7] Niclas Braun, Stefan Debener, Nadine Spychala, Edith Bongartz, Peter Sörös,
Helge H. O. Müller, and Alexandra Philipsen. 2018. The Senses of Agency and
Ownership: A Review. Frontiers in Psychology 9 (2018), 535. https://doi.org/10.
3389/fpsyg.2018.00535
[8] Jennifer L. Campos, Graziella El-Khechen Richandi, Babak Taati, and Behrang
Keshavarz. 2018. The Rubber Hand Illusion in Healthy Younger and Older Adults.
Multisensory Research 31, 6 (2018), 537 – 555. https://doi.org/10.1163/2213480800002614
[9] Nicole David, Francesca Fiori, and Salvatore M Aglioti. 2014. Susceptibility to
the rubber hand illusion does not tell the whole body-awareness story. Cognitive,
Affective, & Behavioral Neuroscience 14, 1 (2014), 297–306. https://doi.org/10.
3758/s13415-013-0190-6
[10] Alyanne M. de Haan, Haike E. Van Stralen, Miranda Smit, Anouk Keizer, Stefan
Van der Stigchel, and H. Chris Dijkerman. 2017. No consistent cooling of the
real hand in the rubber hand illusion. Acta Psychologica 179 (2017), 68–77.
https://doi.org/10.1016/j.actpsy.2017.07.003
[11] Timothy Dummer, Alexandra Picot-Annand, Tristan Neal, and Chris Moore.
2009. Movement and the Rubber Hand Illusion. Perception 38, 2 (2009), 271–
280. https://doi.org/10.1068/p5921 arXiv:https://doi.org/10.1068/p5921 PMID:
19400435.
[12] Daniel Eckhoff, Cecilia Li-Tsang, Gladys Cheing, Alvaro Cassinelli, and Christian
Sandor. 2021. Investigation of Microcirculatory Effects of Experiencing Burning
Hands in Augmented Reality. In 2021 IEEE Conference on Virtual Reality and 3D
User Interfaces Abstracts and Workshops (VRW) . 569–570. https://doi.org/10.1109/
VRW52623.2021.00167
[13] H. Henrik Ehrsson, Katja Wiech, Nikolaus Weiskopf, Raymond J. Dolan, and
Richard E. Passingham. 2007. Threatening a rubber hand that you feel is yours
elicits a cortical anxiety response. Proceedings of the National Academy of Sciences
104, 23 (2007), 9828–9833. https://doi.org/10.1073/pnas.0610011104
[14] Roberto Erro, Angela Marotta, and Mirta Fiorio. 2020. Proprioceptive drift is
affected by the intermanual distance rather than the distance from the body’s
midline in the rubber hand illusion. Attention, Perception, & Psychophysics 82, 8
(2020), 4084–4095. https://doi.org/10.3758/s13414-020-02119-7
[15] Roberto Erro, Angela Marotta, Michele Tinazzi, Elena Frera, and Mirta Fiorio.
2018. Judging the position of the artificial hand induces a “visual” drift towards
the real one during the rubber hand illusion. Scientific Reports 8, 1 (2018), 2531.
https://doi.org/10.1038/s41598-018-20551-6
[16] Alessia Folegatti, Frédérique de Vignemont, Francesco Pavani, Yves Rossetti,
and Alessandro Farnè. 2009. Losing One’s Hand: Visual-Proprioceptive Conflict
Affects Touch Perception. PLOS ONE 4, 9 (09 2009), 1–9. https://doi.org/10.1371/
journal.pone.0006920
[17] Martina Fusaro, Matteo P Lisi, Gaetano Tieri, and Salvatore Maria Aglioti. 2021.
Heterosexual, gay, and lesbian people’s reactivity to virtual caresses on their
embodied avatars’ taboo zones. Scientific Reports 11, 1 (2021), 2221. https:
//doi.org/10.1038/s41598-021-81168-w
[18] Melita J Giummarra, Nellie Georgiou-Karistianis, Mike E R Nicholls, Stephen J
Gibson, and John L Bradshaw. 2010. The Phantom in the Mirror: A Modified
Rubber-Hand Illusion in Amputees and Normals. Perception 39, 1 (2010), 103–
118. https://doi.org/10.1068/p6519 arXiv:https://doi.org/10.1068/p6519 PMID:
20301851.
[19] Mar González-Franco, Tabitha C Peck, Antoni Rodríguez-Fornells, and Mel Slater.
2014. A threat to a virtual hand elicits motor cortex activation. Experimental
Brain Research 232, 3 (2014), 875–887. https://doi.org/10.1007/s00221-013-3800-1
[20] Delphine Grynberg and Olga Pollatos. 2015. Alexithymia modulates the experience of the rubber hand illusion. Frontiers in Human Neuroscience 9 (2015), 357.
https://doi.org/10.3389/fnhum.2015.00357
[21] Arvid Guterstam, Valeria I. Petkova, and H. Henrik Ehrsson. 2011. The Illusion
of Owning a Third Arm. PLOS ONE 6, 2 (02 2011), 1–11. https://doi.org/10.1371/
journal.pone.0017208
[22] Amanda C Hahn, Ross D Whitehead, Marion Albrecht, Carmen E Lefevre, and
David I Perrett. 2012. Hot or not? Thermal reactions to social contact. Biology
letters 8, 5 (oct 2012), 864–867. https://doi.org/10.1098/rsbl.2012.0338
[23] J. M. Hillis, M. O. Ernst, M. S. Banks, and M. S. Landy. 2002. Combining
Sensory Information: Mandatory Fusion Within, but Not Between, Senses.
Science 298, 5598 (2002), 1627–1630. https://doi.org/10.1126/science.1075396
arXiv:https://science.sciencemag.org/content/298/5598/1627.full.pdf
[24] Jakob Hohwy and Bryan Paton. 2010. Explaining Away the Body: Experiences
of Supernaturally Caused Touch and Touch on Non-Hand Objects within the
Rubber Hand Illusion. PLOS ONE 5, 2 (02 2010), 1–10. https://doi.org/10.1371/
journal.pone.0009416
[25] Xu Jin, Jason Meneely, and Nam-Kyu Park. 2022. Virtual Reality Versus RealWorld Space: Comparing Perceptions of Brightness, Glare, Spaciousness, and
Visual Acuity. Journal of Interior Design 47, 2 (2022), 31–50. https://doi.org/10.
1111/joid.12209 arXiv:https://onlinelibrary.wiley.com/doi/pdf/10.1111/joid.12209
[26] Andreas Kalckert and H Ehrsson. 2012. Moving a Rubber Hand that Feels Like
Your Own: A Dissociation of Ownership and Agency. Frontiers in Human Neuroscience 6 (2012), 40. https://doi.org/10.3389/fnhum.2012.00040
[27] Andreas Kalckert and H. Henrik Ehrsson. 2014. The moving rubber hand illusion
revisited: Comparing movements and visuotactile stimulation to induce illusory
ownership. Consciousness and Cognition 26 (2014), 117–132. https://doi.org/10.
1016/j.concog.2014.02.003
[28] Alexander Kalus, Martin Kocur, Niels Henze, Johanna Bogon, and Valentin
Schwind. 2022. How to Induce a Physical and Virtual Rubber Hand Illusion.
In Mensch und Computer 2022 - Tagungsband , Bastian Pfleging, Kathrin Gerling, and Sven Mayer (Eds.). ACM, New York, 572–575. https://doi.org/10.1145/
3543758.3547512
[29] Marjolein P.M. Kammers, Katy Rose, and Patrick Haggard. 2011. Feeling numb:
Temperature, but not thermal pain, modulates feeling of body ownership. Neuropsychologia 49, 5 (2011), 1316–1321. https://doi.org/10.1016/j.neuropsychologia.
2011.02.039
[30] Konstantina Kilteni, Antonella Maselli, Konrad P. Kording, and Mel Slater. 2015.
Over my fake body: body ownership illusions for studying the multisensory
basis of own-body perception. Frontiers in Human Neuroscience 9 (2015), 141.
https://doi.org/10.3389/fnhum.2015.00141
[31] Konstantina Kilteni, Jean-Marie Normand, Maria V. Sanchez-Vives, and Mel Slater.
2012. Extending Body Space in Immersive Virtual Reality: A Very Long Arm
Illusion. PLOS ONE 7, 7 (07 2012), 1–15. https://doi.org/10.1371/journal.pone.
0040867
[32] Martin Kocur. 2022. Utilizing the Proteus Effect to Improve Performance Using
Avatars in Virtual Reality . Ph.D. Dissertation. Regensburg, Germany. https:
//doi.org/10.5283/epub.52677
[33] Martin Kocur, Sarah Graf, and Valentin Schwind. 2020. The Impact of Missing
Fingers in Virtual Reality. In 26th ACM Symposium on Virtual Reality Software
and Technology (Virtual Event, Canada) (VRST ’20) . Association for Computing
Machinery, New York, NY, USA, Article 4, 5 pages. https://doi.org/10.1145/
3385956.3418973
[34] Martin Kocur, Florian Habler, Valentin Schwind, Paweł W. Wozniak, Christian
Wolff, and Niels Henze. 2021. Physiological and Perceptual Responses to Athletic
Avatars While Cycling in Virtual Reality. InProceedings of the 2021 CHI Conference
on Human Factors in Computing Systems (Yokohama, Japan)(CHI ’21). Association
for Computing Machinery, New York, NY, USA, Article 519, 18 pages. https:
//doi.org/10.1145/3411764.3445160
[35] Martin Kocur, Niels Henze, and Valentin Schwind. 2021. The Extent of the Proteus
Effect as a Behavioral Measure for Assessing User Experience in Virtual Reality.
In CHI 2021 - Workshop on Evaluating User Experiences in Mixed Reality . 1–3.
https://doi.org/10.5283/epub.45543
[36] Martin Kocur, Niels Henze, and Valentin Schwind. 2021. Towards an Investigation
of Avatars’ Sweat Effects during Physical Exertion in Virtual Reality. In Mensch
und Computer 2021 - Workshopband , Carolin Wienrich, Philipp Wintersberger,
and Benjamin Weyers (Eds.). Gesellschaft für Informatik e.V., Bonn. https:
//doi.org/10.18420/muc2021-mci-ws16-261
[37] Martin Kocur, Melanie Kloss, Valentin Schwind, Christian Wolff, and Niels Henze.
2020. Flexing Muscles in Virtual Reality: Effects of Avatars’ Muscular Appearance
on Physical Performance. In Proceedings of the Annual Symposium on ComputerHuman Interaction in Play . Association for Computing Machinery, New York, NY,
USA, 193–205. https://doi.org/10.1145/3410404.3414261
[38] Martin Kocur, Daniel Roth, and Valentin Schwind. 2020. Towards an Investigation of Embodiment Time in Virtual Reality. In Mensch und Computer 2020
- Workshopband, Christian Hansen, Andreas Nürnberger, and Bernhard Preim
(Eds.). Gesellschaft für Informatik e.V., Bonn. https://doi.org/10.18420/muc2020-

## Page 11

The Rubber Hand Illusion in Virtual Reality and the Real World - Comparable but Different VRST ’22, November 29-December 1, 2022, Tsukuba, Japan
ws134-339
[39] Martin Kocur, Philipp Schauhuber, Valentin Schwind, Christian Wolff, and Niels
Henze. 2020. The Effects of Self- and External Perception of Avatars on Cognitive
Task Performance in Virtual Reality. In 26th ACM Symposium on Virtual Reality
Software and Technology (Virtual Event, Canada) (VRST ’20) . Association for
Computing Machinery, New York, NY, USA, Article 27, 11 pages. https://doi.
org/10.1145/3385956.3418969
[40] Martin Kocur, Valentin Schwind, and Niels Henze. 2019. Utilizing the Proteus
Effect to Improve Interactions using Full-Body Avatars in Virtual Reality. In
Mensch und Computer 2019 - Workshopband . Gesellschaft für Informatik e.V.,
Bonn. https://doi.org/10.18420/muc2019-ws-584
[41] Martin Kocur, Jessica Sehrt, Valentin Schwind, and Niels Henze. 2022. Designing
Interactive Avatars for Mixed Reality Applications. In Tutorial at Mensch und
Computer (MuC’22) . https://doi.org/10.18420/muc2022-mci-tut03-408
[42] Joan Llobera, M. V. Sanchez-Vives, and Mel Slater. 2013. The relationship between virtual body ownership and temperature sensitivity. Journal of The Royal
Society Interface 10, 85 (2013), 20130300. https://doi.org/10.1098/rsif.2013.0300
arXiv:https://royalsocietypublishing.org/doi/pdf/10.1098/rsif.2013.0300
[43] T. Lobstein and J. Cort. 1978. The relationship between skin temperature and skin
conductance activity: Indications of genetic and fitness determinants. Biological
Psychology 7, 1 (1978), 139–143. https://doi.org/10.1016/0301-0511(78)90046-7
[44] Matthew R. Longo, Friederike Schüür, Marjolein P.M. Kammers, Manos Tsakiris,
and Patrick Haggard. 2008. What is embodiment? A psychometric approach.
Cognition 107, 3 (2008), 978–998. https://doi.org/10.1016/j.cognition.2007.12.004
[45] Ke Ma, Dominique P Lippelt, and Bernhard Hommel. 2017. Creating Virtual-hand
and Virtual-face Illusions to Investigate Self-representation. Journal of visualized
experiments : JoVE 121 (mar 2017), 54784. https://doi.org/10.3791/54784
[46] G. Lorimer Moseley, Alberto Gallace, and Charles Spence. 2012. Bodily illusions
in health and disease: Physiological and clinical perspectives and the concept
of a cortical ’body matrix’. Neuroscience and Biobehavioral Reviews 36, 1 (2012),
34–46. https://doi.org/10.1016/j.neubiorev.2011.03.013
[47] G. Lorimer Moseley, Nick Olthof, Annemeike Venema, Sanneke Don, Marijke Wijers, Alberto Gallace, and Charles Spence. 2008. Psychologically
induced cooling of a specific body part caused by the illusory ownership
of an artificial counterpart. Proceedings of the National Academy of Sciences 105, 35 (2008), 13169–13173. https://doi.org/10.1073/pnas.0803768105
arXiv:https://www.pnas.org/content/105/35/13169.full.pdf
[48] Bryan Paton, Jakob Hohwy, and Peter G Enticott. 2012. The Rubber Hand
Illusion Reveals Proprioceptive and Sensorimotor Differences in Autism Spectrum
Disorders. Journal of Autism and Developmental Disorders 42, 9 (2012), 1870–1883.
https://doi.org/10.1007/s10803-011-1430-7
[49] Valeria I. Petkova and H. Henrik Ehrsson. 2008. If I Were You: Perceptual Illusion
of Body Swapping. PLOS ONE 3, 12 (12 2008), 1–9. https://doi.org/10.1371/
journal.pone.0003832
[50] René Reinhard, Khyati Girish Shah, and Corinna A Faust-Christmann. 2019.
Acting Your Avatar ’ s Age : Effects of Virtual Reality Avatar Embodiment on
Real Life Walking Speed. Media Psychology 0, 0 (2019), 1–23. https://doi.org/10.
1080/15213269.2019.1598435
[51] Martin Riemer, Florian Bublatzky, Jörg Trojan, and Georg W. Alpers. 2015. Defensive activation during the rubber hand illusion: Ownership versus proprioceptive
drift. Biological Psychology 109 (2015), 86–92. https://doi.org/10.1016/j.biopsycho.
2015.04.011
[52] Martin Riemer, Jörg Trojan, Marta Beauchamp, and Xaver Fuchs. 2019. The
rubber hand universe: On the impact of methodological differences in the rubber
hand illusion. Neuroscience & Biobehavioral Reviews 104 (2019), 268–280. https:
//doi.org/10.1016/j.neubiorev.2019.07.008
[53] Marieke Rohde, Massimiliano Di Luca, and Marc O Ernst. 2011. The Rubber Hand
Illusion: feeling of ownership and proprioceptive drift do not go hand in hand.
PloS one 6, 6 (2011), e21659–e21659. https://doi.org/10.1371/journal.pone.0021659
[54] Marieke Rohde, Andrew Wold, Hans-Otto Karnath, and Marc O. Ernst. 2013. The
Human Touch: Skin Temperature during the Rubber Hand Illusion in Manual
and Automated Stroking Procedures. PLOS ONE 8, 11 (11 2013), null. https:
//doi.org/10.1371/journal.pone.0080688
[55] A A Romanovsky. 2014. Skin temperature: its role in thermoregulation. Acta
physiologica (Oxford, England) 210, 3 (mar 2014), 498–507. https://doi.org/10.
1111/apha.12231
[56] Roy Salomon, Melanie Lim, Christian Pfeiffer, Roger Gassert, and Olaf Blanke.
2013. Full body illusion is associated with widespread skin temperature reduction.
Frontiers in Behavioral Neuroscience 7 (2013), 65. https://doi.org/10.3389/fnbeh.
2013.00065
[57] Maria V. Sanchez-Vives, Bernhard Spanlang, Antonio Frisoli, Massimo Bergamasco, and Mel Slater. 2010. Virtual Hand Illusion Induced by Visuomotor Correlations. PLOS ONE 5, 4 (04 2010), 1–6. https://doi.org/10.1371/journal.pone.0010381
[58] Simone Schütz-Bosbach, Peggy Tausche, and Carmen Weiss. 2009. Roughness
perception during the rubber hand illusion. Brain and cognition 70, 1 (jun 2009),
136–144. https://doi.org/10.1016/j.bandc.2009.01.006
[59] Valentin Schwind, Pascal Knierim, Lewis Chuang, and Niels Henze. 2017."Where’s
Pinky?": The Effects of a Reduced Number of Fingers in Virtual Reality . Association
for Computing Machinery, New York, NY, USA, 507–515. https://doi.org/10.
1145/3116595.3116596
[60] Valentin Schwind, Pascal Knierim, Cagri Tasci, Patrick Franczak, Nico Haas, and
Niels Henze. 2017. "These Are Not My Hands!": Effect of Gender on the Perception
of Avatar Hands in Virtual Reality . Association for Computing Machinery, New
York, NY, USA, 1577–1582. https://doi.org/10.1145/3025453.3025602
[61] Valentin Schwind, Lorraine Lin, Massimiliano Di Luca, Sophie Jörg, and James
Hillis. 2018. Touch with Foreign Hands: The Effect of Virtual Hand Appearance
on Visual-Haptic Integration. In Proceedings of the 15th ACM Symposium on
Applied Perception (Vancouver, British Columbia, Canada) (SAP ’18) . Association
for Computing Machinery, New York, NY, USA, Article 9, 8 pages. https://doi.
org/10.1145/3225153.3225158
[62] Sofia Seinfeld, Tiare Feuchtner, Antonella Maselli, and Jörg Müller. 2020. User
Representations in Human-Computer Interaction. Human–Computer Interaction
(feb 2020), 1–39. https://doi.org/10.1080/07370024.2020.1724790
[63] Mel Slater, Daniel Perez-Marcos, H. Henrik Ehrsson, and Maria V. Sanchez-Vives.
2008. Towards a digital body: The virtual arm illusion. Frontiers in Human
Neuroscience 2, AUG (2008), 1–8. https://doi.org/10.3389/neuro.09.006.2008
[64] Mel Slater, Daniel Pérez Marcos, Henrik Ehrsson, and Maria Sanchez-Vives. 2009.
Inducing illusory ownership of a virtual body. Frontiers in Neuroscience 3 (2009),
29. https://doi.org/10.3389/neuro.01.029.2009
[65] Mel Slater, Bernhard Spanlang, Maria V. Sanchez-Vives, and Olaf Blanke. 2010.
First Person Experience of Body Transfer in Virtual Reality. PLOS ONE 5, 5 (05
2010), 1–9. https://doi.org/10.1371/journal.pone.0010564
[66] M. Smit, D. I. Kooistra, I. J. M. van der Ham, and H. C. Dijkerman. 2017. Laterality
and body ownership: Effect of handedness on experience of the rubber hand
illusion. Laterality 22, 6 (2017), 703–724. https://doi.org/10.1080/1357650X.2016.
1273940 arXiv:https://doi.org/10.1080/1357650X.2016.1273940 PMID: 28041532.
[67] Anthony Steed, Ye Pan, Fiona Zisch, and William Steptoe. 2016. The impact of a
self-avatar on cognitive load in immersive virtual reality. In 2016 IEEE Virtual
Reality (VR) . 67–76. https://doi.org/10.1109/VR.2016.7504689
[68] J Tastevin. 1937. En partant de l’expérience d’Aristote les déplacements artificiels
des parties du corps ne sont pas suivis par le sentiment de ces parties ni par
les sensations qu’on peut y produire. [Starting from Aristotle’s experiment the
artificial displacements of parts of the body are not followed by feeling in these
parts or by the sensations which can be produced there.]. L’Encéphale: Revue de
psychiatrie clinique biologique et thérapeutique 32 (1937), 57–158.
[69] Katharine N. Thakkar, Heathman S. Nichols, Lindsey G. McIntosh, and Sohee
Park. 2011. Disturbances in Body Ownership in Schizophrenia: Evidence from the
Rubber Hand Illusion and Case Study of a Spontaneous Out-of-Body Experience.
PLOS ONE 6, 10 (10 2011), 1–9. https://doi.org/10.1371/journal.pone.0027089
[70] Gaetano Tieri, Annamaria Gioia, Michele Scandola, Enea F. Pavone, and Salvatore M. Aglioti. 2017. Visual appearance of a virtual upper limb modulates the temperature of the real hand: a thermal imaging study in Immersive Virtual Reality. European Journal of Neuroscience 45, 9 (2017), 1141–1151.
https://doi.org/10.1111/ejn.13545
[71] Manos Tsakiris, Lewis Carpenter, Dafydd James, and Aikaterini Fotopoulou. 2010.
Hands only illusion: multisensory integration elicits sense of ownership for body
parts but not for non-corporeal objects. Experimental brain research 204, 3 (jul
2010), 343–352. https://doi.org/10.1007/s00221-009-2039-3
[72] Manos Tsakiris and Patrick Haggard. 2005. The rubber hand illusion revisited:
Visuotactile integration and self-attribution. Journal of Experimental Psychology:
Human Perception and Performance 31, 1 (2005), 80–91. https://doi.org/10.1037/
0096-1523.31.1.80
[73] Manos Tsakiris, Ana Tajadura Jiménez, and Marcello Costantini. 2011. Just a
heartbeat away from one’s body: interoceptive sensitivity predicts malleability of body-representations. Proceedings of the Royal Society B: Biological
Sciences 278, 1717 (2011), 2470–2476. https://doi.org/10.1098/rspb.2010.2547
arXiv:https://royalsocietypublishing.org/doi/pdf/10.1098/rspb.2010.2547
[74] Haike E. van Stralen, Martine J.E. van Zandvoort, Sylco S. Hoppenbrouwers,
Lidewij M.G. Vissers, L. Jaap Kappelle, and H. Chris Dijkerman. 2014. Affective
touch modulates the rubber hand illusion. Cognition 131, 1 (2014), 147–158.
https://doi.org/10.1016/j.cognition.2013.11.020
[75] Haike E van Stralen, Martine J E van Zandvoort, L Jaap Kappelle, and H Chris
Dijkerman. 2013. The Rubber Hand Illusion in a Patient with Hand Disownership. Perception 42, 9 (2013), 991–993. https://doi.org/10.1068/p7583
arXiv:https://doi.org/10.1068/p7583 PMID: 24386718.
[76] Cyril Vienne, Stéphane Masfrand, Christophe Bourdin, and Jean-Louis Vercher.
2020. Depth Perception in Virtual Reality Systems: Effect of Screen Distance,
Environment Richness and Display Factors. IEEE Access 8 (2020), 29099–29110.
https://doi.org/10.1109/ACCESS.2020.2972122
[77] Eric-Jan Wagenmakers, Jonathon Love, Maarten Marsman, Tahira Jamil, Alexander Ly, Josine Verhagen, Ravi Selker, Quentin F Gronau, Damian Dropmann,
Bruno Boutin, Frans Meerhoff, Patrick Knight, Akash Raj, Erik-Jan van Kesteren,
Johnny van Doorn, Martin Šmíra, Sacha Epskamp, Alexander Etz, Dora Matzke,
Tim de Jong, Don van den Bergh, Alexandra Sarafoglou, Helen Steingroever,
Koen Derks, Jeffrey N Rouder, and Richard D Morey. 2018. Bayesian inference

## Page 12

VRST ’22, November 29-December 1, 2022, Tsukuba, Japan Kocur et al.
for psychology. Part II: Example applications with JASP. Psychonomic Bulletin &
Review 25, 1 (2018), 58–76. https://doi.org/10.3758/s13423-017-1323-7
[78] Andrew Wold, Jakub Limanowski, Henrik Walter, and Felix Blankenburg. 2014.
Proprioceptive drift in the rubber hand illusion is intensified following 1 Hz
TMS of the left EBA. Frontiers in Human Neuroscience 8 (2014), 390. https:
//doi.org/10.3389/fnhum.2014.00390
[79] Nick Yee and Jeremy Bailenson. 2007. The Proteus Effect: The Effect of Transformed Self-representation on Behavior. Human Communication Research 33, 3
(2007), 271–290. https://doi.org/10.1111/j.1468-2958.2007.00299.x
[80] Ye Yuan and Anthony Steed. 2010. Is the rubber hand illusion induced by immersive virtual reality?. In 2010 IEEE Virtual Reality Conference (VR) . 95–102.
https://doi.org/10.1109/VR.2010.5444807
[81] Regine Zopf, Greg Savage, and Mark A. Williams. 2010. Crossmodal congruency
measures of lateral distance effects on the rubber hand illusion.Neuropsychologia
48, 3 (2010), 713–725. https://doi.org/10.1016/j.neuropsychologia.2009.10.028
The Sense of Body.
