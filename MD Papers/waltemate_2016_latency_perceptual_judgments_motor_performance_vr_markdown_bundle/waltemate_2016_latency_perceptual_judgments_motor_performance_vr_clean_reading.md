# Waltemate et al. (2016) — The Impact of Latency on Perceptual Judgments and Motor Performance in Closed-loop Interaction in Virtual Reality

## Extraction notes

- Source PDF: 2016-latency.pdf

- Clean reading copy with page markers preserved.

- Light cleanup only; no interpretive notes mixed into source text.

- Verify exact quotations against the original PDF before thesis use.


---



<!-- page: 1 -->

The Impact of Latency on Perceptual Judgments and Motor Performance
in Closed-loop Interaction in Virtual Reality
Thomas Waltemate1
Irene Senna2
Felix H¨ulsmann1,3
Marieke Rohde4
Stefan Kopp3
Marc Ernst2
Mario Botsch1
1Computer Graphics Group, Bielefeld University, Germany
2Applied Cognitive Psychology, Ulm University, Germany
3Social Cognitive Systems, Bielefeld University, Germany
4AFFS Affective Signals GmbH, Berlin, Germany
Figure 1: Left: The basic virtual mirror scenario consists of an empty room and a simplistic mirror avatar. Right: The extended scenario
employed in the experiment, where the target movement is shown by a semi-transparent blue “ghost character”.
Abstract
Latency between a user’s movement and visual feedback is inevitable in every Virtual Reality application, as signal transmission and processing take time. Unfortunately, a high end-to-end
latency impairs perception and motor performance. While it is possible to reduce feedback delay to tens of milliseconds, these delays
will never completely vanish. Currently, there is a gap in literature
regarding the impact of feedback delays on perception and motor
performance as well as on their interplay in virtual environments
employing full-body avatars. With the present study at hand, we address this gap by performing a systematic investigation of different
levels of delay across a variety of perceptual and motor tasks during full-body action inside a Cave Automatic Virtual Environment.
We presented participants with their virtual mirror image, which
responded to their actions with feedback delays ranging from 45 to
350 ms. We measured the impact of these delays on motor performance, sense of agency, sense of body ownership and simultaneity
perception by means of psychophysical procedures. Furthermore,
we looked at interaction effects between these aspects to identify
possible dependencies. The results show that motor performance
and simultaneity perception are affected by latencies above 75 ms.
Although sense of agency and body ownership only decline at a
latency higher than 125 ms, and deteriorate for a latency greater
than 300 ms, they do not break down completely even at the highest
tested delay. Interestingly, participants perceptually infer the presence of delays more from their motor error in the task than from the
actual level of delay. Whether or not participants notice a delay in a
virtual environment might therefore depend on the motor task and
their performance rather than on the actual delay.
Keywords:
latency, simultaneity perception, body ownership,
sense of agency, full-body motion capture, virtual mirror
Concepts: •Computing methodologies →Virtual reality;
1
Introduction
Virtual Reality (VR) plays an essential role in various fields, such
as training of emergency situations, simulations, rehabilitation, or
motor learning. The success of VR applications is determined by
many factors, such as realism, ease of interaction, and responsiveness [Meehan et al. 2003]. Among these, one crucial factor is the
end-to-end latency: the delay between a user’s interaction and the
corresponding feedback presentation. This holds especially for applications in which users obtain real-time feedback of their action,
as is the case when they are presented with their own avatar. In setups presenting delayed visual feedback with respect to motor performance, high latencies influence perceived temporal coherence
of the scene, sense of agency, sense of ownership, as well as motor
performance [Franck et al. 2001; Longo and Haggard 2009; J¨org
et al. 2012; Imaizumi and Asai 2015]. If we had knowledge on
Permission to make digital or hard copies of all or part of this work for personal or classroom use is granted without fee provided that copies are not
made or distributed for profit or commercial advantage and that copies bear
this notice and the full citation on the first page. Copyrights for components
of this work owned by others than the author(s) must be honored. Abstracting with credit is permitted. To copy otherwise, or republish, to post on
servers or to redistribute to lists, requires prior specific permission and/or a
fee. Request permissions from permissions@acm.org. c⃝2016 Copyright
held by the owner/author(s). Publication rights licensed to ACM.
VRST ’16, November 02 - 04, 2016, Garching bei M¨unchen, Germany
ISBN: 978-1-4503-4491-3/16/11
DOI: http://dx.doi.org/10.1145/2993369.2993381



<!-- page: 2 -->

which duration of latencies is still acceptable with respect to these
factors, we would be able to design systems that reduce the risk of
suffering from latency.
Even though numerous studies investigating the effects of feedback
delays in virtual environments have previously been conducted, no
clear picture has emerged.
While Held and Durlach [1991] report that delays as small as 60 ms significantly interfere with motor adaptation, others reported a threshold of 120 ms or 150 ms to
perceive latency (e.g., [Mauve et al. 2004; J¨org et al. 2012]). Furthermore, the impact of latency is often only considered with respect to one single factor (e.g., perception of simultaneity [Mania
et al. 2004; Raaen et al. 2014]). In other cases, only very simple tasks such as button pressing are examined without a focus on
VR [Kawabe et al. 2013; Rohde et al. 2014a]. Also, Rohde et al.
[2014b] found that feedback delays are processed differently in
predictable motor tasks as opposed to unpredictable motor tasks.
The effect of feedback delays is thus contingent on the display,
the movement performed, and on the perceptual or motor task (see
Section 2 for a review of the background literature). Most studies
to date have focused on just one task and one movement, which
makes it difficult to compare results from different studies and to
derive acceptable levels of delay in VR across applications.
We revisit the topic of visual feedback delays in VR using a more
encompassing approach. To this end, we use a virtual mirror scenario with full-body motion capture, as is employed in many virtual
reality experiments where monitoring the own movement of the full
body is important [Gonzalez-Franco et al. 2010; Lugrin et al. 2015;
de Kok et al. 2015; Samaraweera et al. 2015]. As our virtual environment we use a Cave Autonomous Virtual Environment (CAVE),
which is our preferred environment in the context of motor learning
in VR [Waltemate et al. 2015]. We use this system in the project ICSPACE1, which develops a virtual coaching system for motor learning. For such a system it is important to be able to monitor one’s
own body and to minimize the amount of disturbing hardware attached to the user while still providing an immersive experience. In
this context, a CAVE offers a good trade-off between the amount of
attached hardware and immersion. The virtual mirror image allows
to continuously monitor the own full-body movements.
Our study contributes to a better understanding of the effects of
feedback latencies on full-body closed-loop behavior. It combines
three important factors:
Plausibility: Our VR system provides an immersive, full-body virtual mirror image and allows for full-body motor learning of
complex tasks. Participants perform a motor task that requires
fast and precise movements of the whole upper body. Thus,
our study contributes to the development of VR environments
dedicated to motor learning, such as sports training, and will
hopefully be useful for the design of VR environments.
Temporal precision: Our CAVE is characterized by a low baseline end-to-end latency of 45 ms, which is particularly low for
an environment using full-body motion capturing. This allows us to evaluate our dependent variables using latencies
of 45 ms and higher. In the present study, we investigate a
range of delays, from 45 to 350 ms, which allows us to model
the perceptual responses as a continuous psychometric function of the feedback delay. Testing latencies as small as 45–
125 ms allows us to study the impact of even small feedback
delays in VR systems on perception and behavior. Exploring
high latencies allows us to identify the limits of the temporal
windows of perceived simultaneity, agency, and ownership in
VR while performing complex movements. This gives us the
1http://graphics.uni-bielefeld.de/research/icspace/
opportunity to compare our results on feedback delays in immersive VR with previous related work on visual feedback delays in simpler tasks and environments, such as button presses
and manual control interfaces (e.g., [Farrer et al. 2013; Rohde
et al. 2014a].
Range of measures: Apart from motor performance error, we
record
participants’
perceptual
judgments
(simultaneity,
agency, and body ownership) after performing movements in
our experimental setup. We test for interaction effects between these variables and pre-existing immersive tendencies.
This paradigm enables us to identify thresholds for tolerable delays in different domains of user performance and experience, to
compare these thresholds across measures and to identify interactions between measures. We hope that our study will be a useful
resource for the design of virtual environments and provides information about how transmission delays impair different aspects of
human perception and performance.
2
Related Work
In the physical world, causes and effects of an action are temporally contiguous. The human brain automatically compensates
for small and natural delays introduced by inconsistencies in neural propagation across signals in different modalities, and between
movement outputs and afferent signals. In VR setups and in computer games, the latency of the system always introduces further delay between motor commands and visual feedback [Stauffert et al.
2016]. While the brain tolerates small but perceivable delays, and
even temporally recalibrates to them [Rohde et al. 2014b; Yarrow
et al. 2013], larger delays might affect perception and behavior.
There is no golden rule specifying the highest acceptable latency
a system is allowed to have in order not to impair motor and perceptual performances. Studies involving different setups and sensorimotor tasks come to different conclusions when investigating
the perceptual threshold for delay detection. Users might be unaware of delays below 120 ms [Mauve et al. 2004], or below 150 ms
when controlling characters in computer games [J¨org et al. 2012].
Even delays around 200 ms between mouse movements and cursor
movements or between a button press and a visual stimulus might
go unnoticed [Raaen et al. 2014; Rohde et al. 2014a]. Although
the available body of literature suggests that participants might fail
to detect delays below 120–200 ms, other studies report that some
users are able to spot a latency as small as 50 ms in the context of
mouse-cursor movements [Raaen et al. 2014], and even a latency
of around 15 ms while using a Head-Mounted Display [Mania et al.
2004]. Moreover, when asked to detect changes of system latency
while wearing a Head-Mounted Display, users’ perceptual stability
across different virtual environments would require latencies below
16 ms [Ellis et al. 2004]
Delays between the execution of an action and its visual feedback can also impair two components of bodily self consciousness,
namely the sense of agency (i.e., the sense to have caused the action) and the sense of ownership over one’s body (i.e., the sense that
my body belongs to me) (e.g., [Gallagher 2000]). The emergence
of the sense of agency is though to be based on an internal forward model, which compares the predicted sensory consequences
of the motor commands with the actual sensory feedback [Wolpert
et al. 1995; Frith et al. 2000]. A mismatch between predicted and
observed feedback, as in the case of delayed feedback, can result in a loss of the sense of agency [Longo and Haggard 2009].
When this happens, people might even attribute the observed delayed feedback of their movement to an external cause [Farrer and
Frith 2002; Franck et al. 2001]. Although the sense of agency tends
to decrease with increasing delay between an action and its sensory



<!-- page: 3 -->

counterparts [Farrer et al. 2013; Imaizumi and Asai 2015], a certain amount of delay is acceptable for sense of agency to persist.
Literature suggests that, when observing a delayed image of one’s
own hand, people attribute the observed movements to the self even
at delays around 150 ms [Franck et al. 2001; Longo and Haggard
2009; Tsakiris et al. 2006; Tsakiris et al. 2010]. Above 100–150 ms,
perceived agency toward the delayed visual feedback of hand movements decreases [Franck et al. 2001], and does not emerge at delays
around 500 ms [Longo and Haggard 2009; Tsakiris et al. 2010].
However, when presented with visual flashes occurring after a voluntary button press, subjects report agency for flashes lagging even
up to around 500 ms [Rohde et al. 2014a]. It has been suggested
that body ownership might allow a narrower temporal window of
asynchrony than sense of agency, emerging with delays up to 100–
150 ms [Imaizumi and Asai 2015; Longo and Haggard 2009].
A perceivable delay between movements and their observed consequences does not only impair sense of ownership and agency,
but may also affect motor performance in 2D and 3D tasks (e.g.,
[Teather et al. 2009]). For instance, when controlling a character
in computer games, delays greater than 150 ms affect performance
[J¨org et al. 2012]. A latency of around 170 ms led to a longer time
necessary to complete a grasping task [Chung and So 1999]. In a
simple coordination task, the introduction of a 200 ms delay significantly increases the error rate [Gutwin 2001]. Similarly, in a tracking task, latencies of or above 110 ms dramatically increase the
error rate [Pavlovych and Stuerzlinger 2011]. A delay around 70–
75 ms has been found already effective in decreasing performance
in a VR reaching task [Ware and Balakrishnan 1994], and in tasks
which require moving a mouse cursor to a target [MacKenzie and
Ware 1993]. In a non-VR and low latency scenario with a Fitts’ law
style pointing task a latency of about 16 ms already seemed to have
an effect [Friston et al. 2016]. Samaraweera et al. [2013] showed
in an experiment using a HMD that inducing a latency of 225 ms
can change gait patterns. In another study they showed that latency
as well as using a virtual mirror can alter gait behavior by adding
200 ms of delay to the system latency to one half of the participants’
avatar [Samaraweera et al. 2015].
To summarize, these findings show that the impact of latency differs
in our four variables of interest—perceived latency, sense of agency,
sense of ownership, and motor performance—for different setups
and for different motor tasks.
3
Methods
3.1
Participants
Ten na¨ıve participants (4 males, mean age M = 23.2, standard deviation SD = 2.2, 9 right handed) with normal or corrected to normal vision took part in the study. Participants provided written informed consent and got paid for their participation. The study was
conducted in accordance with the Declaration of Helsinki, and had
ethical approval from our University’s ethics committee.
3.2
Apparatus
We conducted the experiments in a VR setup designed for full-body
motor learning of complex actions based on a two sided CAVE (Lshape, 3 m × 2.3 m for each side). Each wall was operated by two
projectors (Projection Design F35 WQ), which ran at 60 Hz. Each
of them had a resolution of 2100 × 1600 pixels. To separate the
images for both eyes, we used passive filters by INFITEC. All four
projectors were driven by a self-developed rendering engine running on a single computer to minimize latency. For each wall of
the CAVE, we used one NVIDIA Quadro K5000 graphics card.
The rendering engine, which ran at around 240 fps, received the
position and orientation of the participants’ glasses for perspective
adaptation as well as joint rotations of 19 joints and information on
limb lengths of the participants. We obtained this information by
using a passive marker-based full-body motion capture system by
OptiTrack. To attach the markers to participants, we used a partly
customized tight fitting marker suit consisting of a sleeveless shirt
and trousers. We attached markers to this suit or directly to the
participants’ skin depending on the desired marker position. The
motion capture setup consisted of ten Prime 13W cameras, which
proved to obtain latencies comparable to the commonly installed
VICON cameras [Waltemate et al. 2015].
Participants were placed inside a virtual room in front of a virtual
mirror. This mirror showed a reflection of the room itself as well
as a virtual avatar. This “mirror avatar” was scaled according to
the participants’ limb lengths and was animated according to the
participants’ motion in real time. Figure 1 (left) shows an example
of this setup.
The end-to-end latency between the participants’ movements and
the corresponding movements of the mirror avatar was increased
synthetically using a FIFO buffer holding back the motion data.
This buffer was filled with incoming motion capture frames, and as
soon as one of these frames was older than the desired latency offset, it was emitted and used to animate the mirror avatar. If multiple
frames satisfied this condition, the one closest to the desired latency
was used. We only delayed the mapping of the participants’ motion
onto the mirror avatar. The movement of the tracked glasses used
for perspective adaptation was not delayed.
3.2.1
Verifying latency
To determine the latency of our system itself and of our mechanism
to induce additional latency, we conducted end-to-end latency measurements. To this end, we used an extension of a well-established
latency measurement approach, as described in [Waltemate et al.
2015]: We equipped a test person with motion capture markers
and placed this person inside the CAVE. There, the person was instructed to move one arm up and down. This movement was then
mapped onto the mirror avatar. We recorded the person together
with the rendered mirror avatar using a consumer camera (Nikon 1
J4), which records 400 fps. In the resulting video, we measured the
delay between the person’s movement and the corresponding movement of the mirror avatar by frame counting. To reduce potential
errors (e.g., due to manual labeling), we averaged latency measurements over multiple trials. These measurements were performed
for the base latency as well as for the latencies that we manually induced during the experiment. We were able to obtain a mean for the
base latency of 44.9 ms (SD=6.1). The latencies induced manually
by our system were identical to the desired latencies.
The base latency of about 45 ms consists of the individual latencies
of the tracking cameras (∼4 ms according to manufacturer), of the
tracking software, the motion preprocessing (∼2 ms), the network
communication (∼1 ms), as well as rendering (∼4 ms at 240 fps),
display synchronization, and display hardware (∼19 ms according
to manufacturer). The known latencies add up to ∼30 ms, thus the
remaining ∼15 ms must be mainly due to display synchronization
and tracking software.
3.3
Procedure and Stimulus
First, participants filled in questionnaires for demographic data,
simulator sickness [Kennedy et al. 1993] and immersive tendencies [Witmer and Singer 1998]. Then they read the instructions for
the experiment. Afterwards, they put on the marker suit and per-



<!-- page: 4 -->

(a)
(b)
Figure 2: The participants’ avatar is grey (a), while it is not sufficiently close to the target posture of the ghost character (blue character) and green (b), when the posture is fitted sufficiently.
formed skeleton calibration in the CAVE. We did some refinement
of marker positions if necessary. Next, participants were presented
with the virtual mirror showing the mirror avatar (cf. Figure 1, left).
This scene was shown for about one minute to let participants familiarize themselves with the virtual mirror concept.
The following main part of the experiment consisted of multiple trials. In each trial, the mirror avatar was super-imposed with a second
character (blue, semi-transparent), which was scaled the same way
as the mirror avatar (cf. Figure 2(a)). This “ghost character” performed pre-recorded animations (cf. Figure 3). Participants were
instructed to simultaneously mimic the movements of the ghost
character, i.e., to move together with the ghost character. For all
frames in which the difference in posture between both characters
did not exceed a certain threshold (see Section 3.4.2), the mirror
avatar was colored green to give feedback on the accuracy of the
performance (cf. Figure 2(b)). During the trials, we systematically
introduced a delay in the movements of the mirror avatar. This
delay was varied between 45 and 350 ms on a logarithmic scale
and randomly set per trial. After each trial the virtual mirror was
disabled and turned white, and participants were asked three questions on perceptual judgments (cf. Section 3.4.1). The supplemental
video shows an example of one trial. After the main part of the experiment, participants filled in the simulator sickness questionnaire
again and took off the marker suit. In total the experiment took
about two hours.
We used five different pre-recorded animation sequences to animate
the ghost character (cf. Figure 3 and supplemental video). We limited these animations to upper body movements to keep the task
simple and avoid fatigue. Pilot experiments had shown that large
movements of the whole body including the legs (e.g., squat movement), are too exhausting for a long experiment as ours. Additionally, we noticed that lower body movements that involve lifting one
leg off the ground increase the risk of participants tumbling. The
same movement was always presented twice in a row per trial. The
movements varied in speed and trajectory and thus were not entirely predictable. This kind of movement was selected in order
to prevent participants from recurring to unwanted strategies while
performing the motor task. Indeed, individuals tend to modify their
performance in order to compensate for feedback delays either by
slowing down or by adopting a “move and wait” strategy [Ferrell
1965; Park and Kenyon 1999]. The latter consists of ignoring the
visual feedback while executing fast movements, and then waiting
to catch up with the visual feedback before continuing the task. By
forcing participants to execute fast movements with variable velocity and non-linear paths, we aimed to prevent such strategies [Rohde
et al. 2014b; Rohde and Ernst 2016]. Each animation lasted 5 s and
had the same starting posture (cf. Figure 3(a)). Before an animation
started, the ghost character remained in the starting posture for 1.5 s
to allow participants to take that posture. Thus, each trial lasted
6.5 s. As latency offsets we used 0, 30, 80, 165 and 305 ms. When
added to the baseline latency of the system, these offsets resulted in
end-to-end latencies of 45, 75, 125, 210 and 350 ms, respectively.
We decided to take also large latencies (> 125 ms) into account to
identify the perceptual limits of the sense of agency and body ownership, as pilot experiments had revealed that participants tolerate
larger delays when judging agency and ownership.
The experiment included 200 trials and ten practice trials. In the
practice trials each animation sequence was shown two consecutive
times with no additional latency. In the other 200 trials we randomized animations as well as latency offsets, while still making sure
to equally distribute the combinations of animation sequences and
latency offsets, so that each combination occurred equally often.
Therefore, each animation as well as each latency was presented 40
times. Since this results in a long time for participants to stand and
perform the movements (mean duration = 68 min (SD = 20)), we included a short break every 20 trials. These breaks were optional
and participants could continue with the experiment whenever they
wanted by touching a virtual box. Additionally, the mean accuracy
of the motor performance since the last break was shown to motivate participants.
3.4
Dependent Variables
3.4.1
Perceptual Judgments
After each of the 200 trials participants were asked the following
three questions in randomized order:
Agency judgment (AJ): Was the motion of the grey avatar the visual feedback to the movement you just performed?
Simultaneity judgment (SJ): Was the motion of the grey avatar
simultaneous to your movement?
Ownership judgment (OJ): Did you feel that the grey avatar belonged to you?
For agency judgment we instructed participants that the motion
performed by their avatar could either reflect their own movement
or some pre-recorded movement previously performed by them or
some previous participant. We introduced such a “cover story” to
provide participants with a reasonable alternative when attributing
the causality of the action [Rohde and Ernst 2016]. To avoid that
participants probe the system for agency (e.g., by making unexpected movements to test if the avatar follows), we instructed them
explicitly against such probing. We asked participants to answer
the questions according to how they felt and how they perceived
the movements of their avatar. The questions were visualized as
text inside the CAVE and were answered by touching virtual “Yes”
or “No” boxes. The fact that AJ, OJ and SJ were all yes/no tasks
allowed a direct comparison of the temporal windows of perceiving
agency, ownership, and simultaneity [Rohde et al. 2014a].
3.4.2
Motor Performance
The motor performance was determined by checking the posture
deviation of the participants’ avatar with the ghost character. For
each frame the distances of shoulder, elbow, and wrist joint of the
mirror avatar to the corresponding joints of the ghost character were



<!-- page: 5 -->

(a)
(b)
(c)
(d)
(e)
(f)
Figure 3: (a): Starting posture. (b)-(f): Turning point postures of the five animations used for the ghost character.
calculated and averaged. If that average distance was inside the error range of 12 cm, the participants’ posture was counted as sufficiently close and successful. The number of successful frames
divided by all rendered frames gave us the percentage of successful
postures in each trial.
4
Results
The first ten trials served as practice trials and were not included in
the analyses. For each participant we calculated the percentage of
“yes” responses in each perceptual task (i.e., AJ, OJ, SJ). The effect
of feedback delay on perceptual judgments and motor performance
was assessed separately for each task, by fitting the probability of
“yes” responses and the accuracy in the motor performance with a
generalized linear mixed model (GLMM, [Agresti 2002; Moscatelli
et al. 2012]). In such a model, the overall variance is divided into
a fixed and a random component [Agresti 2002]. The fixed component tests the effect of the independent variable (manipulated in the
experiment), while the random effect accounts for the heterogeneity
among different participants. Thus, the GLMM allows the analysis
of clustered categorical data, at the population and individual levels simultaneously [Moscatelli et al. 2012].
Here, feedback delay
(log-transformed) was the fixed effect, and subject identity was the
random effect (Model 1). A probit link function was applied. The
model parameters were estimated using Maximum Likelihood Estimation (MLE). The data was analyzed with MATLAB. The GLMM
analysis revealed a significant effect of feedback delay for all tasks
(all p < 0.001).
As shown in Figure 4, the higher the delay, the lower the probability
of responding “yes” in the perceptual judgment tasks, and the lower
the accuracy in motor performance (see also Table 1 for results for
each tested delay). In other words, sense of agency, ownership, and
perceived simultaneity decreased, and motor performance worsened, with increasing delay. Regarding the perceptual judgment
tasks (Figure 4(a)), the temporal window of perceived simultaneity
was narrower than those of perceived agency and ownership. Trials
with the minimum system delay (45 ms) were perceived as simultaneous 88 % of the times on average across participants. Perceived
simultaneity dramatically dropped with increasing delay: 49 % of
trials with 210 ms delay and only 12 % of trials presenting 350 ms
delay were perceived as simultaneous.
In contrast, although both perceived agency and ownership decreased significantly with increasing delay, they did not break down
even at the highest tested delay (350 ms). Indeed, while for minimum delay participants reported sense of agency in 96 % of the
trials and sense of ownership in 97 % of them, sense of agency and
ownership still occurred at 350 ms delay in 71.5 % and 62 % of the
trials, respectively. Responses in the OJ and AJ tasks were comparable, as shown by overlapping confidence intervals (CI, set at
95 % confidence level) for all tested delays between the two tasks
(see Figure 4(a) and Table 1). Motor performance gradually worsened with increasing delay, from 66 % of accuracy at 45 ms delay to 36 % at 350 ms (Figure 4(b) and Table 1).
Overall, performance in each of the four tasks did not differ between 45 and
75 ms delays, as shown by overlapping CI in each task between
those two delays. Motor performance significantly worsened between 75 ms (M = 64.8 %, CI = 58–71.6), and 125 ms (M = 61.4 %,
CI = 54.3–68.7; Wilcoxon signed-rank test, p = 0.009).
Similarly, perceived simultaneity showed a tendency to decrease between 75 ms (M = 87 %, CI = 83–90) and 125 ms (80 %, CI = 76–
84, Wilcoxon signed-rank test, p = 0.07). Conversely, perceived
agency and ownership started declining between 125 and 210 ms,
while they did not significantly differ between 75 ms and 125 ms
(agency, 75 ms: M = 94.8 %, CI = 92–96.7; 125 ms: M = 94 %,
CI = 91.2–96.1, Wilcoxon signed-rank test, p = 1; ownership,
75 ms: M = 95.5 %, CI = 93–97.3; 125 ms: M = 96.5 %, CI = 94–
98, Wilcoxon signed-rank test, p = 0.52).
With the minimum delay (i.e.,
45 ms),
motor performance
was more accurate in trials reported as simultaneous (accuracy, M = 67.3 %, SD = 11.9) than in those perceived as nonsimultaneous (M = 54.2 %, SD = 10.3), and in those for which
participants perceived agency (M = 66.5 % SD = 12.3) and ownership (M = 66.5 %, SD = 23) as compared to those that did not
elicit agency (M = 62 %, SD = 10.7 ) and ownership (M = 51.7 %,
SD = 10.5) feelings.
Given the positive association between the quality of the motor
performance and the successive perceptual judgements, we tested
a second model to assess whether the influence of motor performance in the task was significant. We fitted the probability of “yes”
responses in each task with a GLMM model with performance accuracy as fixed effect, and subject identity as random effect (Model
2). Results showed that motor performance accuracy predicts responses in all tasks (all p < 0.001). We compared the results of
Model 2 (i.e., the one with performance accuracy as a fixed effect)
with those of Model 1 (i.e., the one with feedback delay as a fixed
effect). The two models employ the same functions, and differ in
the predictors only. To select the model that better fits the data (i.e.,
the fixed effects that better explain the results), we compared the
two models using the Akaike Information Criterion (AIC, [Akaike
1973]). According to the AIC, Model 2 fitted the data better than
Model 1. This result suggests that, although both delay and motor performance accuracy affect perceptual judgments, participants
rely more on their own performance than on the delay itself when
estimating feedback simultaneity, sense of agency, and ownership.
However, we cannot exclude that the relationship between performance accuracy and subjective judgments might be mediated by a



<!-- page: 6 -->

45
100
150
200
250
300
350
0
1
Agency
Ownership
Simultaneity
Feedback delay (ms)
Proportion perceived ‘yes’
0.8
0.6
0.4
0.2
Perceptual judgments 
(a)
45
100
150
200
250
300
350
 
Feedback delay (ms)
Motor performance accuracy 
0
1
0.8
0.6
0.4
0.2
Motor performance
(b)
Figure 4: Psychometric functions for all tasks, obtained by pulling together the data from all participants. a) Perceptual judgments (agency,
ownership, simultaneity). b) Motor performance. Analyses were performed on the individual data from each participant, while aggregated
data are shown for illustrative purposes only. Error bars represent confidence intervals set at 95 %.
third latent variable, and further studies are necessary to better understand this issue.
To make sure that participants were not influenced or biased
because they were asked the same questions repeatedly in the
AJ/SJ/OJ tasks, we ran further analyses. For each perceptual task
we fitted the probability of “yes” responses with a GLMM with
feedback delay, trial number, and their interaction as fixed effects,
and subject identity as random effect (Model 3). The only significant fixed effect was that of the factor feedback delay (all p <
0.001), while trial number and the interaction of delay and trial
number were not significant (all p > 0.07). Moreover, a model
comparison according to the AIC favoured a model with a fixed effect only for the delay (Model 1) over more complex models with
also fixed effects of trial number or the interaction between trial
number and feedback delay (Model 3). These findings show that
participants did not alter their response strategy during the time of
the experimental session.
To assess whether individual differences in immersive tendencies
are related to individual differences in perceptual and motor tasks,
we calculated Pearson correlation between each item of the immersive tendencies questionnaire (ITQ) and the performance in each
task with minimum delay (i.e., 45 ms).
We found a significant
correlation between the item of the ITQ [“Do you easily become
deeply involved in movies or TV dramas?”] and sense of ownership (r = 0.66, p = 0.038), and between the same item and sense
of agency (r = 0.81, p = 0.005). Thus, participants who report to
be usually deeply involved in movies are the ones showing greater
sense of agency and ownership in the experimental task. Moreover
the item [“Do you ever become so involved in doing something
that you lose all track of time?”] was negatively correlated with
perceived simultaneity (r = -0.73 p = 0.01) and motor performance
(r = -0.65, p = 0.04). Thus, participants reporting a tendency to
lose track of time showed worse motor performance and a higher
tendency to report trials at 45 ms delay as non-simultaneous.
Finally, to test for the presence of motion sickness induced by our
system, we compared the responses to each item of the simulator
sickness questionnaire between the first and the second presentation
of the questionnaire using the Wilcoxon Signed rank test. Participants did not show motion sickness after taking part in the experiment (all p > 0.38).
5
Discussion
Previous research involving hand movement suggests that sense of
ownership might be more affected by delay than sense of agency
[Imaizumi and Asai 2015]. Here we found that even a delay as high
as 350 ms elicits both sense of agency and ownership. This result is
in line with recent findings suggesting that sense of agency toward
a moving hand might drive sense of ownership even toward the delayed image of the hand [Asai 2016]. Our findings suggest that
movements which are more complex than a simple button press, as
in the case of the full-body movements described in our study, induce a strong sense of ownership, even despite long delays in the
visual feedback. Notably the temporal structure of such a feedback
would be strongly correlated with participants’ motor performance.
Thus, participants might rely on correlation between the temporal
structure of the motor and visual signals to infer a common cause
(between motor actions and visual feedback), and a sense of agency,
ownership, and simultaneity. A recent computational model for
multisensory integration [Parise and Ernst 2016] suggests that people rely on such temporal correlation across different sensory signals when estimating simultaneity and common source.
Furthermore, results showed that motor performance accuracy predicts perceptual judgments even better than delays itself. Thus,
when motor performance is poor (i.e., in case of a mismatch between the desired outcome and the actual performance), participants tend to perceive the feedback as non-simultaneous, and to lose
sense of agency and ownership. In other words, a small delay tends
to be perceived as non-simultaneous in case of high performance errors, and higher delays might go undetected if motor performance
is accurate. This finding suggests that, in principle, the same delay
in a VR system might or might not impair perceptual judgments,
depending on the difficulty of the motor task. In case of a simple
motor task, leading to high performance accuracy, the delay might



<!-- page: 7 -->

Delay
Agency
Ownership
Simultaneity
Motor performance
45 ms
96 %
97.25 %
88 %
66.1 %
(93.6–97.7 %)
(95.5–98.8 %)
(84.4–91 %)
(59.6–72.6 %)
75 ms
94.8 %
95.5 %
86.75 %
64.83 %
(92–96.7 %)
(93–97.3 %)
(83–90 %)
(58–71.6 %)
125 ms
94 %
96.5 %
80.25 %
61.5 %
(91.2–96.1 %)
(94–98 %)
(76–84 %)
(54.3–68.7 %)
210 ms
86.5 %
90 %
49.25 %
51.83 %
(82.8–89.7 %)
(86.6–92.8 %)
(44.35–54.3 %)
(44.7–58.9 %)
350 ms
71.5 %
62 %
12.25 %
36 %
(66.8–75.9 %)
(57–66.8 %)
(9.2–15.9 %)
(30.4–41.6 %)
Table 1: The table depicts the mean percentage of “yes” answers for agency, ownership, and simultaneity judgments as well as mean
percentage of the successful postures for motor performance for each delay. The confidence intervals (lower limit–upper limit), set at 95 %,
are listed beneath their corresponding mean value.
go unnoticed. In case of more complex tasks, leading to higher
chances of performance errors, delays will exert a stronger impact
on perceived agency, ownership, and simultaneity. This might explain why in previous studies recurring to button press [Rohde et al.
2014a], participants were unaware even of long delays: a simple
motor performance requiring only a button press would not lead to
error signals related to the motor performance, and this in turn reduces the probability of detecting the delay. For the same reason,
trained users (for instance, experts in a certain sport), performing a
motor task better than novices in a sport scenario, might be perceptually less affected by delays than novices. Previous studies have
shown that people are not particularly accurate in detecting delays
in sensorimotor tasks: delays up to around 200–250 ms can even
go unnoticed, and in some cases participants might report agency
also for events preceding the action [Rohde et al. 2014a]. Here we
show that the quality of the motor performance strongly influences
perceptual decisions.
6
Conclusion
In our study, we used a novel paradigm employing VR and psychophysical procedures to investigate how delays between an action
and its visual feedback affect perception and motor performance.
In particular, we assessed the impact of latency on perceived simultaneity, sense of agency, ownership, as well as motor performance
during the execution of full-body movements in front of a virtual
mirror. Considering the large variability in the literature concerning a possible threshold for visual delays to be detected and affect
behavior, we systematically assessed the effect of delays on motor performance and perceptual judgments in the same setup, and
in the same experimental session. To this end, we parametrically
varied the delay of the visual feedback between 45 ms (i.e., the latency intrinsic in the system) and 350 ms, while participants on each
trial performed both a motor task and perceptual judgments on the
delayed feedback. Results showed that, although inducing delay
increasingly affects perceptual judgments and motor performance,
incrementing the delay from 45 to 75 ms had no significant impact
on participants’ performance in the four tasks. Delays above 75 ms
worsen motor performance and influence simultaneity perception,
while they do not affect perceived agency and ownership, which
significantly start declining only later, between 125 ms and 210 ms.
Interestingly, the temporal windows of perceived agency and ownership are much broader than the one of perceived simultaneity:
while at the highest tested delay (i.e., 350 ms) visual feedback is
hardly perceived as simultaneous, perceived agency and ownership
are not disrupted, although significantly reduced. Thus, participants
tolerated perceptible delays when reporting agency and ownership
toward their avatar’s movements. These findings are in line with
studies investigating the temporal window of agency and simultaneity [Farrer et al. 2013; Rohde et al. 2014a] when participants
judged whether a visual event presented on a screen was caused
by their button press and whether it was simultaneous. Here we
show that this also holds true in the case of complex upper-body
movements. Moreover, we found that individual differences in immersive tendencies modulate sensitivity to delays, sense of agency,
and ownership, as well as motor performance.
In conclusion, our study extends our understanding of the effect
of feedback delays on perceptual and motor tasks. While previous
studies mainly involved manual tasks, we focused on more complex movements involving the entire upper body. Since we always
tracked and visualized the whole body in an immersive environment
employing a virtual mirror, we assume that our findings transfer
from upper-body to full-body movements, but this has to be examined in future studies. Moreover, our study introduced a systematic investigation of the interplay between perceived simultaneity,
agency, and ownership in virtual environments, while previous research has mainly focused on a subset of these phenomena. The
present findings contribute to a deeper understanding of what information people rely on when making perceptual decisions about
agency, ownership, and simultaneity. Furthermore, it contributes
to fill a gap in the literature regarding which delay might be considered acceptable for VR systems for motor learning of complex
tasks involving full-body movements. While smaller delays might
not appreciably affect perception, they might still impair motor performance.
In general, this work stresses the importance of latency for fullbody interaction in virtual environments. While latency is often
neglected or at least put in second place, we argue that the latency
of a VR system used for a specific study should at least be reported.
Moreover, the effect of latency should be taken into consideration
as the source of possible side effects.
7
Future Work
In future work we would like to examine the influence of jitter in
the latency on motor performance, simultaneity perception, sense
of ownership, and sense of agency. As we concentrated on upperbody movements in the present study we would like to investigate
whether the findings of this work also hold true for interaction involving complex movements of the full body. Moreover, we would
like to investigate the impact of appearance on sense of embodi-



<!-- page: 8 -->

ment in the virtual mirror scenario. To this end, we will employ
3D-scanning to create high-quality avatars of participants, so that
we can confront them with a more realistic virtual mirror image.
Acknowledgements
This research was supported by the Cluster of Excellence Cognitive
Interaction Technology CITEC (EXC 277) at Bielefeld University,
which is funded by the German Research Foundation (DFG).
References
AGRESTI, A. 2002. Categorical Data Analysis. Wiley Series in
Probability and Statistics. Wiley.
AKAIKE, H. 1973. Information theory and an extension of the
maximum likelihood principle. In Proc. of Second International
Symposium on Information Theory, 267–281.
ASAI, T. 2016. Agency elicits body-ownership: proprioceptive
drift toward a synchronously acting external proxy. Experimental brain research 234, 5, 1163–1174.
CHUNG, K., AND SO, R. H. 1999. Effects of hand movement
lag on discrete manual control tasks in virtual environements.
In Proceedings of the Human Factors and Ergonomics Society
Annual Meeting, vol. 43, SAGE Publications, 1210–1213.
DE KOK, I., HOUGH, J., H ¨ULSMANN, F., BOTSCH, M.,
SCHLANGEN, D., AND KOPP, S. 2015. A multimodal system
for real-time action instruction in motor skill learning. In Proc.
of International Conference on Multimodal Interaction, ACM,
355–362.
ELLIS, S. R., MANIA, K., ADELSTEIN, B. D., AND HILL, M. I.
2004. Generalizeability of latency detection in a variety of virtual environments. In Proceedings of the Human Factors and Ergonomics Society Annual Meeting, vol. 48, SAGE Publications,
2632–2636.
FARRER, C., AND FRITH, C. 2002. Experiencing oneself vs another person as being the cause of an action: The neural correlates of the experience of agency. NeuroImage 15, 3, 596–603.
FARRER, C., VALENTIN, G., AND HUP, J. 2013. The time windows of the sense of agency. Consciousness and Cognition 22,
4, 1431–1441.
FERRELL, W. R. 1965. Remote manipulation with transmission
delay. IEEE Transactions on Human Factors in Electronics, 1,
24–32.
FRANCK, N., FARRER, C., GEORGIEFF, N., MARIE-CARDINE,
M., DALRY, J., D’AMATO, T., AND JEANNEROD, M. 2001.
Defective recognition of one’s own actions in patients with
schizophrenia. American Journal of Psychiatry 158, 3, 454–459.
FRISTON, S., KARLSTR ¨OM, P., AND STEED, A. 2016. The effects
of low latency on pointing and steering tasks. IEEE transactions
on visualization and computer graphics 22, 5, 1605–1615.
FRITH, C. D., BLAKEMORE, AND WOLPERT, D. M. 2000. Abnormalities in the awareness and control of action. Philosophical
Transactions of the Royal Society of London B: Biological Sciences 355, 1404, 1771–1788.
GALLAGHER, S. 2000. Philosophical conceptions of the self: implications for cognitive science. Trends in Cognitive Sciences 4,
1, 14–21.
GONZALEZ-FRANCO, M., PEREZ-MARCOS, D., SPANLANG, B.,
AND SLATER, M. 2010. The contribution of real-time mirror
reflections of motor actions on virtual body ownership in an immersive virtual environment.
In Proceedings of IEEE Virtual
Reality, 111–114.
GUTWIN, C. 2001. The effects of network delays on group work
in real-time groupware. In Proc. Seventh European Conference
on Computer-Supported Cooperative Work, Springer, 299–318.
HELD, R., AND DURLACH, N. 1991. Telepresence, time delay
and adaptation. In Pictorial communication in virtual and real
environments. 232–246.
IMAIZUMI, S., AND ASAI, T.
2015.
Dissociation of agency
and body ownership following visuomotor temporal recalibration. Frontiers in Integrative Neuroscience 9, 35.
J ¨ORG, S., NORMOYLE, A., AND SAFONOVA, A.
2012.
How
responsiveness affects players’ perception in digital games. In
Proceedings of the ACM Symposium on Applied Perception, 33–
38.
KAWABE, T., ROSEBOOM, W., AND NISHIDA, S. 2013. The sense
of agency is action–effect causality perception based on crossmodal grouping. Proceedings of the Royal Society of London B:
Biological Sciences 280, 1763.
KENNEDY, R. S., LANE, N. E., BERBAUM, K. S., AND LILIENTHAL, M. G. 1993. Simulator sickness questionnaire: An enhanced method for quantifying simulator sickness. The international journal of aviation psychology 3, 3, 203–220.
LONGO, M. R., AND HAGGARD, P. 2009. Sense of agency primes
manual motor responses. Perception 38, 1, 69–78.
LUGRIN, J.-L., LANDECK, M., AND LATOSCHIK, M. E. 2015.
Avatar embodiment realism and virtual fitness training. In Proceedings of IEEE Virtual Reality, 225–226.
MACKENZIE, I. S., AND WARE, C. 1993. Lag as a determinant
of human performance in interactive systems. In Proceedings of
the INTERACT’93 and CHI’93 conference on Human factors in
computing systems, ACM, 488–493.
MANIA, K., ADELSTEIN, B. D., ELLIS, S. R., AND HILL, M. I.
2004. Perceptual sensitivity to head tracking latency in virtual
environments with varying degrees of scene complexity. In Proc.
of the 1st Symposium on Applied Perception in Graphics and
Visualization, ACM, 39–47.
MAUVE, M., VOGEL, J., HILT, V., AND EFFELSBERG, W. 2004.
Local-lag and timewarp: providing consistency for replicated
continuous applications. IEEE Transactions on Multimedia 6,
1, 47–57.
MEEHAN, M., RAZZAQUE, S., WHITTON, M. C., AND BROOKS,
F. P. 2003. Effect of latency on presence in stressful virtual
environments. In Proceedings of IEEE Virtual Reality, 141–148.
MOSCATELLI, A., MEZZETTI, M., AND LACQUANITI, F. 2012.
Modeling psychophysical data at the population-level: the generalized linear mixed model. Journal of Vision 12, 11, 26–26.
PARISE, C. V., AND ERNST, M. O. 2016. Correlation detection
as a general mechanism for multisensory integration.
Nature
communications 7.
PARK, K. S., AND KENYON, R. V.
1999. Effects of network
characteristics on human performance in a collaborative virtual
environment. In Proceedings of IEEE Virtual Reality, 104–111.



<!-- page: 9 -->

PAVLOVYCH, A., AND STUERZLINGER, W.
2011. Target following performance in the presence of latency, jitter, and signal
dropouts. In Proceedings of Graphics Interface, 33–40.
RAAEN, K., EG, R., AND GRIWODZ, C. 2014. Can gamers detect
cloud delay?
In Proceedings of the 13th Annual Workshop on
Network and Systems Support for Games, IEEE Press.
ROHDE, M., AND ERNST, M. O. 2016. Time, agency, and sensory
feedback delays during action. Current Opinion in Behavioral
Sciences 8, 193–199.
ROHDE, M., SCHELLER, M., AND ERNST, M. O. 2014. Effects
can precede their cause in the sense of agency. Neuropsychologia
65, 191–196.
ROHDE, M., VAN DAM, L. C., AND ERNST, M. O. 2014. Predictability is necessary for closed-loop visual feedback delay
adaptation. Journal of Vision 14, 3, 1–23.
SAMARAWEERA, G., GUO, R., AND QUARLES, J. 2013. Latency
and avatars in virtual environments and the effects on gait for
persons with mobility impairments. In IEEE Symposium on 3D
User Interfaces, IEEE, 23–30.
SAMARAWEERA, G., PERDOMO, A., AND QUARLES, J. 2015.
Applying latency to half of a self-avatar’s body to change real
walking patterns. In Proceedings of IEEE Virtual Reality, 89–
96.
STAUFFERT, J. P., NIEBLING, F., AND LATOSCHIK, M. E. 2016.
Reducing application-stage latencies of interprocess communication techniques for real-time interactive systems. In Proceedings of IEEE Virtual Reality, 287–288.
TEATHER, R. J., PAVLOVYCH, A., STUERZLINGER, W., AND
MACKENZIE, I. S. 2009. Effects of tracking technology, latency, and spatial jitter on object movement. In Proceedings of
IEEE Symposium on 3D User Interfaces, 43–50.
TSAKIRIS, M., PRABHU, G., AND HAGGARD, P. 2006. Having
a body versus moving your body: How agency structures bodyownership. Consciousness and cognition 15, 2, 423–432.
TSAKIRIS, M., LONGO, M. R., AND HAGGARD, P. 2010. Having
a body versus moving your body: neural signatures of agency
and body-ownership. Neuropsychologia 48, 9, 2740–2749.
WALTEMATE, T., H ¨ULSMANN, F., PFEIFFER, T., KOPP, S., AND
BOTSCH, M. 2015. Realizing a low-latency virtual reality environment for motor learning. In Proc. of ACM Symposium on
Virtual Reality Software and Technology, 139–147.
WARE, C., AND BALAKRISHNAN, R. 1994. Reaching for objects in VR displays: lag and frame rate. ACM Transactions on
Computer-Human Interaction 1, 4, 331–356.
WITMER, B. G., AND SINGER, M. J. 1998. Measuring presence
in virtual environments: A presence questionnaire. Presence:
Teleoperators and virtual environments 7, 3, 225–240.
WOLPERT, D. M., GHAHRAMANI, Z., AND JORDAN, M. I. 1995.
An internal model for sensorimotor integration. Science 269,
5232, 1880–1882.
YARROW, K., SVERDRUP-STUELAND, I., ROSEBOOM, W., AND
ARNOLD, D. H.
2013.
Sensorimotor temporal recalibration
within and across limbs. Journal of Experimental Psychology:
Human Perception and Performance 39, 6, 1678–1689.
