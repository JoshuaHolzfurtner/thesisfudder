# Arndt 2018 — Using Virtual Reality and Head-Mounted Displays to Increase Performance in Rowing Workouts

## Extraction notes

- Source PDF: `3265845.3265848.pdf`

- Clean reading copy with page markers preserved.

- Light cleanup only; no interpretive notes mixed into source text.

- Verify exact quotations against the original PDF before thesis use.

- Tables and figures are especially important in this paper; verify metric values and p-values against the PDF before citing.


---



<!-- page: 1 -->

Using Virtual Reality and Head-Mounted Displays to Increase
Performance in Rowing Workouts
Sebastian Arndt
NTNU, Norwegian University of
Science and Technology
Trondheim, Norway
sebastian.arndt@ntnu.no
Andrew Perkis
NTNU, Norwegian University of
Science and Technology
Trondheim, Norway
andrew.perkis@ntnu.no
Jan-Niklas Voigt-Antons
Technische Universität Berlin
Berlin, Germany
jan-niklas.voigt-antons@tu-berlin.de
ABSTRACT
Technology is advancing rapidly in the domain of virtual reality, as
well as in using sensors to gather feedback from our body and the
environment we are interacting in. Combining these two technologies gives us the opportunity to create personalized and reactive
immersive environments. These environments can be used for training of dangerous situations (e.g. fire, crashes, etc) or to improve
skills with less distraction than regular natural environments would
offer. The pilot study described in this paper, puts an athlete rowing
on a stationary rowing machine into a virtual environment. The
virtual reality receives movement data from several sensors of the
rowing machine and displays those in the head-mounted display.
In addition, metrics on technique are derived from the sensor data
as well as physiological data. All this is used to investigate if and to
which extend VR improves the technical skills of an athlete, during
the complex sport of rowing. Furthermore, athletes are given subjective feedback about their performance comparing the standard
rowing workout with the workout using VR. First results indicate
improved performance of the workout and an enhanced experience
for the athlete in the VR condition.
ACM Reference Format:
Sebastian Arndt, Andrew Perkis, and Jan-Niklas Voigt-Antons. 2018. Using
Virtual Reality and Head-Mounted Displays to Increase Performance in
Rowing Workouts. In 1st International Workshop on Multimedia Content
Analysis in Sports (MMSports’18), October 26, 2018, Seoul, Republic of Korea.
ACM, New York, NY, USA, 6 pages. https://doi.org/10.1145/3265845.3265848
1
INTRODUCTION
The evolution of videogames has always focused on the task offering a more immersive experience, with better graphics, better
sound, better interaction, etc for the user. With the presentation of
Nintendo Wii, a new stage of videogames was created. The physical
activity while playing sport games was the added feature, and thus,
also the level of immersion in sports videogames was enhanced for
the users. It allowed the user to play with movement controllers
and it was the first console which brought the sports field to the
living room. After this, the Kinect appeared on the market which is
Permission to make digital or hard copies of all or part of this work for personal or
classroom use is granted without fee provided that copies are not made or distributed
for profit or commercial advantage and that copies bear this notice and the full citation
on the first page. Copyrights for components of this work owned by others than ACM
must be honored. Abstracting with credit is permitted. To copy otherwise, or republish,
to post on servers or to redistribute to lists, requires prior specific permission and/or a
fee. Request permissions from permissions@acm.org.
MMSports’18, October 26, 2018, Seoul, Republic of Korea
© 2018 Association for Computing Machinery.
ACM ISBN 978-1-4503-5981-8/18/10...$15.00
https://doi.org/10.1145/3265845.3265848
able to detect the body movements and interprets those movements
as input signals to control the videogame. Next, head-mounted displays (HMD) using virtual reality (VR) entered the market. These
devices bring the user the opportunity to get a 360-degree experience of the game they are playing. VR is also starting to be used
during sports workouts both by professionals and amateurs. On
the one hand, it gives the athlete the opportunity to replay certain
scenes of previous games. This can be especially interesting for
team sports (such as football, basketball, etc.). On the other hand, it
offers the possibility to perform entire training-sets in VR. This can
be used, in order to make monotonous indoor-workouts more fun,
or preparing the athlete for how the competition arena will look
like and let them perform there.
In the domain of sports and VR, so-called exergames put the focus on the gaming engine and thus rather have the goal to motivate
people to exercise. The fun and motivating part is more important
than the coaching on perfect technique or to perform optimal [2].
In addition, many approaches in VR sports try to simulate realistic
sports environment and are putting the focus on improving technique and add more realistic conditions for the athlete. However,
improving the fun during workout is also an important aspect here.
Appelbaum et al. [1] gives a review of sports vision training
using digital training techniques which is concentrating on teamsports and fast-paced sports. Mentioning that athletes rely greatly
on vision, and visual training for their sports such that they can
improve their performance using VR. In the review, three naturalistic sports training approaches are highlighted, one of them being
simulations to recreate the sporting environment in virtual reality.
While this is a growing market especially for amateurs, only very
limited research has been performed in this area which can show
an increase in performance.
Using virtual reality during monotonous indoor endurance workouts has become very popular with the rise of Zwift 1. Giving cyclist
and runners the opportunity to perform their workouts on stationary indoor bikes or treadmills online, while following a virtual
course and race against other athletes worldwide.
Neumann et al. [8] give an overview on using virtual reality
technology in endurance sports. Their conceptual framework for
applications in VR sports consists of four major factors: Task, User,
VR Environment, and Non-VR environmental factors. In their review, they highlight that most research so far has only been concentrating on the task, user, and VR-environment factors. The most
investigated task was cycling; running and rowing have only been
subject to a few studies. None of the studies they present used
1www.zwift.com
Session 2
MMSports’18, October 26, 2018, Seoul, Republic of Korea
45



<!-- page: 2 -->

HMD as the display for the virtual environment. Furthermore, it
gets obvious that most studies rather use novice users to the sports,
as compared to experienced.
Very recent work from Shepherd et al. [11] uses HMD while
athletes cycle in a virtual velodrome. The non-elite cyclists evaluate
their experience during cycling in the VR. The study results showed
an increase in behavioural fidelity as well as in performance which
is including the concept of presence. The studies of [10] and [5] used
rowing and head-mounted displays. Where [10] investigated the
impact of a virtual environment in a single-player rowing exergame.
As virtual environments a CAVE environment was compared to a
HMD. Different feedback mechanisms to motivate people to row
at a certain pace. And [5] shows how VR and the opportunity to
talk to the opponent influences the performance of the athlete in a
multi-player exergame.
Previous studies have shown that bringing athletes into a virtual
reality scenario, their performance in terms of covered distance /
power output increases. This was shown in different endurance
sports such as rowing [3], running on a treadmill [9], or cycling [7].
All these three studies and most studies in the current literature are
focussing on performance improvement (based on time, power, etc)
and/or increase of mood and not on improving technique using VR
systems.
Only little work has been done on the focus on comparing technique when work out in standard mode versus virtual reality. Sigrist
et al. [12] investigated how different feedback mechanisms and the
congruency of them can improve technique when rowing on a
trunk-arm. Visual feedback was given in the sense of showing
the trajectory of an optimal stroke and the comparison of the participants stroke. In addition, auditory and haptic feedback was
evaluated. The results suggest that congruent audiovisual feedback
provides the best feedback for learning of the movement. The visual
feedback in this study was projected on the wall.
In this paper, we present a study within indoor-rowing. Where
we explore how the VR environment presented in a head-mounted
display unit is affecting the performance and the experience of
athletes over a regular indoor-workout.
2
METHODS
2.1
Hardware
In the experiment, we used a rowing machine, Augletics Eight2,
from Augletics 2. The ergo-meter is equipped with several sensors
which in addition to standard rowing machines is capturing movement of the sledge and the handlebars. Furthermore, the machine
provides with information about the power on each stroke, duration of the stroke, recovery slide, strokes per minute, etc. Using
these objective measures, different metrics on rowing technique are
being derived. Feedback on these metrics is given on the display
of the rowing machine itself 1b. The derived metrics are consistency, movement, stroke length, recovery, rhythm (see Table 1).
Each metric reaches values between 1 and 100, where 1 is very poor
performance and 100 perfect.
An API provides parameters such as stoke force and speed via
an HTTP connection. Two oars and a scull are modelled by a linear
2www.augletics.de
Metric
Description
Stroke length
Stretch further! Roll forward until your
shins are in a vertical position
Recovery
Try to roll forward slowly and steadily.
This put less strain on your joints
Rhythm
Pull handle quickly towards your chest
then roll slowly forward. A good
rhythm is 20 strokes per minute
Consistency
Try to make every stroke like the last
one, using the same amount of strength
and the same technique
Movement
Extend your arms first, then move your
upper body forward and only then begin to bend your knees and roll forward
Table 1: Metrics from the ergo-meter provided by Augletics.
interpolation between the ergometer parameters and the game object positions. The resistance of the ergometer was set to a medium
value (5 out of 10), to avoid rapid fatigue of users. Unity project was
used for the visualization of the virtual environment (a summer
lake surrounded by distant mountains and a red scull). Very realistic haptic feedback was provided by using the ergo handles in the
real world. For displaying the virtual world scenario, a HTC Vive
set was used. Participants were wearing the headset during the
workout. The controllers were placed next to the rowing machine,
to indicate to the VR system the location and orientation of the
ergometer. The controllers were not moved during the sessions.
In addition to the sensors on the machine, the participants wore
a belt around their chest to measure the breathing rate during
exercise. The breathing rate from the Sweetzpot 3 breathing sensor
was read every 50 m.
2.2
Experimental Design
Participants filled in a demographic questionnaire in the beginning.
Afterwards, they performed a warm-up/baseline phase, in which
they were rowing 500m, in both, the non-VR and VR setup, in order
to get accustomed to the rowing machine and the VR environment.
During the non-VR setup, participants saw all the available feedback
including the metrics regarding their technique. In the VR-case, the
only feedback they received was passing a distance indicator-line
every 50m. The warm-up session was followed by the two test
conditions.
During the experiment, two conditions were tested. (1) A regular workout on the ergo-meter where participants only saw the
distance covered as feedback during their workout. (2) A workout
on the ergo-meter in the virtual environment. Here, participants
were wearing the HTC Vive headset (Fig. 1a), and were put on an
artificial lake to row (Fig. 1b). The feedback that was provided in the
second scenario was distance markers every 50m besides the steady
movement on the lake depending on the force applied to the oars.
During both sessions, the participants needed to cover a distance
of 500m rowing on the machine. The order of VR vs non-VR was
3www.sweetzpot.com
Session 2
MMSports’18, October 26, 2018, Seoul, Republic of Korea
46



<!-- page: 3 -->

(a) Rower on ergo-meter using VR
(b) Screenshot of VR
Figure 1
randomized between participants. The breathing rate was noted
every 50m, and was averaged afterwards over the session.
After each of the two sessions, participants were asked to fill
in the Activity Flow Scale questionnaire, to asses their level of
immersion, flow and satisfaction with the rowing experience. In
addition, participants reported on their emotional state after the
exercise on a 9-point-SAM [6] questionnaire, which contained the
dimensions of valence, arousal, and dominance.
2.3
Questionnaires
After welcoming the participants, and let them read the instructions
of the experiments, a demographic questionnaire was completed by
each participant. Here, age and gender was retrieved first, followed
by how many hours per week participants train on average and
how often per week they exercise. Next, they answered how much
experiences they have in rowing and in the use of VR technologies,
such as HMD, Cave environment, etc.
After each test condition, participants filled out the Activity Flow
State Scale (AFSS) questionnaire [4], with 24 items using four questions for each of the eight factors; which are: actions and awareness
merging; clear goals; concentration on task at hand; unambiguous
feedback; challenge-skill balance; transformation of time; sense of
control; loss of self-conscious; autotelic experience. For analysis, the
four questions for each of the factors were averaged. In addition to
the AFSS, questions concerning the participants perceived level of
motion-sickness, the quality of the overall experience with the test
condition were asked for, and in case of the VR condition judging
the visual quality. All questions were rated on a five-point Likert
scale (Results were afterwards transferred as -2=’Strongly Disagree’,
-1=’Disagree’, 0=’Neutral’, 1=’Agree’, 2=’Strongly Agree’).
Furthermore, a 9-point-SAM scale was deployed, after each condition asking for the level of valence, arousal, and dominance during
each condition.
3
RESULTS
16 participants (5male, 11female) took part in the study with an
average age of 23.4 years. 13 of them stated to be experienced rowers, while the other 3 were non-regular rowers. Except for one
participant all subjects are very involved in training, and stated to
train 9.4 hours per week in average.
3.1
Objective Data
Table 2 shows the results of the objective metrics provided by the
ergo-meter manufacturer as well as the value for breath per minute,
taken from the breathing sensor, during both conditions. The results
show marginal improvements on most of the statistics.
The objective measures taken during the experiment and the
metrics derived based on those, show that values are generally
slightly higher for the VR scenario than for the non-VR scenario.
With the exception for the breathing rate which is slightly smaller.
The biggest difference being in Rhythm, followed by Recovery. A
paired t-test comparing VR and non-VR condition for the collected
data reveals a significant differences between the two scenarios (VR
vs non-VR) for consistency (p=0.1), recovery (p=0.09), and rhythm
(r ≤0.01). Furthermore, the average breathing rate for the non-VR
condition was slightly higher as for the VR case, also showing a
significant difference (r ≤0.01).
Correlations calculated between the different metrics show a
strong correlation (r ≥0.7) between Breath and Strokes/Min, Breath
and Rhythm, Stroke Length and Rhythm and Stroke Length and
Movement can be seen. As well as a moderate correlation (r ≥0.5)
between Breath and Movement, Breath and Stroke Length, Breath
and Recovery, Consistency and Time and Rhythm and Strokes/Min
(see Table 4).
3.2
Subjective Data
Subjective data was gathered after each session on the 24-item
Activity-Flow-Scale questionnaire. Results of questions for each
participants were averaged over the four questions for each category. This questionnaire was extended by questions towards the
entire experience of the workout and in case for the VR-case by the
evaluation of the visual quality.
Table 3 shows the averaged data from the questionnaire filled in
after each of the conditions.
Transformation of Time (TT) gave the biggest difference between
both conditions, showing that participants lost their sense of time
more during the VR workout as compared to the standard workout.
Valence ratings were higher for the VR case than the non-VR case,
the same absolute difference was observed for the dominance ratings with the difference that participants felt less in control in the
VR condition compared to the non-VR case. The autotelic experience
was also rated significantly higher for the VR condition compared
to the standard workout. People were reporting on a slightly elevated level of motion sickness for the VR case than for the non-VR
case. However, no participant needed to quit the session nor was it
reported to be uncomfortable.
Session 2
MMSports’18, October 26, 2018, Seoul, Republic of Korea
47



<!-- page: 4 -->

Breaths/min
Consistency
Movement
Stroke Length
Recovery
Rhythm
Time (s)
Strokes/min
VR
19.25
85.28
85.26
97.92
75.89
79.41
137.75
23.63
Non-VR
20.41
84.36
83.36
97.14
72.63
73.98
135.69
22.73
Delta
-1.15
0.92
1.89
0.78
3.26
5.44
2.06
0.90
T-Test
≤0.01**
0.10*
0.10
0.40
0.09*
≤0.01**
≤0.01**
0.43
Table 2: Average over all subjects of recorded objective data for the VR and Non-VR condition. Delta is the difference between
VR and Non-VR, T-Test shows the p-values of the T-Test between the two conditions. Consistency, Movement, Stroke Length,
Recovery and Rhythm are metrics taken from the ergo-meter.
SAM1
SAM2
SAM3
MAA
CG
CO
UF
TT
CN
SC
AE
MS
EX
QoE
VQ
VR
7.56
4.63
6.44
0.88
0.25
0.29
0.03
0.54
0.50
1.40
1.00
1.34
1.13
1.25
0.63
Non-VR
6.50
4.00
7.06
0.96
0.36
0.46
0.41
-0.17
0.66
1.33
0.42
1.78
0.88
0.81
0.00
Delta
1.06
0.63
-0.63
-0.08
-0.11
-0.17
-0.38
0.71
-0.16
0.06
0.58
-0.44
0.25
0.44
0.63
T-Test
≤0.01**
0.14
0.15
0.62
0.27
0.01*
0.11
≤0.01**
0.53
0.66
≤0.01**
0.07*
0.10
0.09*
0.03*
Table 3: Average over all subjects of recorded subjective data for the VR and Non-VR condition. Delta is the difference between VR and Non-VR, T-Test shows the p-values of the T-Test between the two conditions. SAM1=valence;
SAM2=arousal; SAM3=dominance; MAA=merging actions and awareness; CG=clear goals; CO=Concentration on task at hand;
UF=unambiguous feedback; CS = challenge skill balance; TT=Transformation of time; CN=Sense of Control; SC=loss of selfconscious; AE = atotelic experience; MS=Motion sickness; EX=Experience; QoE=Quality of Experience; VQ = Visual Quality
Breaths/min
Consistency
Movement
Stroke Length
Recovery
Rhythm
Time
Strokes/Min
Breath
-0.13
-0.61**
-0.51*
0.64***
-0.74***
-0.35
0.85***
Consistency
0.62
-0.10
-0.25
-0.02
-0.13
0.62**
-0.15
Movement
0.01**
0.71
0.81***
-0.39
0.87***
-0.22
-0.40
Stroke Length
0.05*
0.35
0.01***
-0.28
0.74***
-0.36
-0.40
Recovery
0.01***
0.95
0.14
0.3
-0.37
-0.24
0.36
Rhythm
0.01***
0.62
0.01***
0.01***
0.16
-0.18
-0.60**
Time
0.18
0.01**
0.42
0.17
0.37
0.5
-0.40
Strokes/Min
0.01***
0.58
0.12
0.12
0.17
0.01**
0.13
Table 4: Results of Pearsons correlation between the different metrics. Lower left diagonal shows p-values of the correlation,
upper right shows correlation values. ***indicates correlations with p values lower 0.01; ** correlations lower 0.05; *correlations
lower than 0.1.
A T-Test was calculated comparing both conditions and yields
significant results for ’Transformation of time’ (r ≤0.01), the
valence scale by the SAM questionnaire (r ≤0.01), ’Autotelic Experience’ (r ≤0.01), ’Concentration on Task-at-Hand’ (p=0.01),
’Motion Sickness’ (p=0.07), ’Quality of Experience’ (p=0.09) were
significant.
Correlations calculated for the subjective data shows strong correlation (r ≥0.7) between Valence and Autotelic experience, and
moderate correlations (r ≥0.5) for Dominance and Unambiguous
feedback, Dominance and Sense of Control, Sense of Control and Unambiguous Feedback, Valence and Quality of Experience, and Quality
of Experience and Autotelic experience.
3.3
Combined Data
Investigating relationships between the subjective data and the
objectively extracted metrics indicates only a few weak (r ≥0.3)
but significant (r ≤0.1)correlations between the different data; such
as Unambiguous feedback and Stroke Length, Transformation of time
and Stroke Length, Arousal and Rhythm, Rhythm and Unambiguous
feedback, Loss of self-conscious and Rhythm, Motion sickness and
Strokes/Min, and Strokes/Min and Visual Quality.
3.4
Qualitative Data
After the experiment some participants gave informal feedback of
things to improve the system. This was not a planned part of the
experiment, but contains helpful information for further development and research in this area. The main feedback here was that a
multiplayer mode would be desirable. Here two different versions
are of interest: race against others; and to row in a team. Especially
the latter one is interesting for experienced rowers, as synchrony
between the rowers in one boat is one of the main challenges in
team rowing. Having the chance to row in a virtual team boat
and work on the synchrony of the row would be a very beneficial
training especially during winter.
Rowing against others in a multiplayer game would especially
be fun and motivating when having avatars of the opponents. In
Session 2
MMSports’18, October 26, 2018, Seoul, Republic of Korea
48



<!-- page: 5 -->

SAM1
SAM2
SAM3
MAA
CG
CO
UF
TT
CN
SC
AE
MS
EX
QoE
VQ
SAM1
0.03
0.36**
-0.01
-0.01
-0.04
0.11
0.37**
0.09
-0.07
0.81***
0.17
0.08
0.70***
0.43**
SAM2
0.89
-0.17
-0.18
-0.05
0.27
-0.16
-0.21
-0.23
-0.20
-0.01
-0.45***
0.04
0.09
0.02
SAM3
0.04**
0.35
0.28
0.30*
-0.10
0.63***
-0.18
0.65***
-0.10
0.27
0.36
-0.09
0.38**
0.41**
MAA
0.97
0.33
0.13
-0.08
-0.30*
0.41**
0.06
0.44**
0.07
0.08
0.08
0.28
-0.16
0.08
CG
0.96
0.8
0.09*
0.67
0.30
0.00
-0.16
-0.01
-0.11
0.06
0.09
-0.11
0.02
-0.06
CO
0.84
0.13
0.59
0.09*
0.1
-0.31*
-0.22
-0.18
-0.06
0.05
0.00
-0.18
-0.02
-0.06
UF
0.56
0.39
0.01***
0.02**
0.98
0.08*
-0.20
0.62***
0.15
0.09
0.30*
-0.03
0.26
0.30
TT
0.04**
0.25
0.32
0.75
0.38
0.22
0.28
-0.21
0.18
0.41**
-0.10
0.17
0.07
0.01
CN
0.62
0.21
0.01***
0.01**
0.94
0.31
0.01***
0.25
0.04
0.20
0.31*
-0.13
0.05
0.43**
SC
0.69
0.27
0.57
0.7
0.55
0.75
0.42
0.34
0.84
0.13
0.11
0.39**
0.13
0.18
AE
0.01***
0.94
0.13
0.66
0.74
0.77
0.63
0.02**
0.28
0.48
0.09
0.21
0.63***
0.48***
MS
0.37
0.01***
0.04
0.65
0.63
0.98
0.1*
0.58
0.09*
0.55
0.62
-0.02
0.29
0.26
EX
0.68
0.84
0.63
0.13
0.56
0.33
0.86
0.36
0.48
0.03**
0.25
0.91
0.04
0.00
QoE
0.01***
0.62
0.03**
0.37
0.9
0.9
0.16
0.7
0.8
0.47
0.01***
0.11
0.83
0.46***
VQ
0.02**
0.91
0.02**
0.68
0.73
0.73
0.98
0.97
0.01**
0.32
0.01***
0.16
1
0.01***
Table 5: Results of Pearsons correlation between the different subjective scores. Lower left diagonal shows p-values of the
correlation, upper right shows correlation values. ***indicates correlations with p values lower 0.01; ** correlations lower 0.05;
*correlations lower than 0.1.
Breaths/min
Consistency
Movement
Stroke Length
Recovery
Rhythm
Average
Time
Strokes/Min
Q1
-0.09
0.19
-0.03
-0.17
0.20
0.18
0.16
0.28
0.11
Q2
-0.23
-0.12
0.34*
0.36*
-0.20
0.36**
0.31*
-0.24
-0.11
Q3
0.05
0.24
-0.06
-0.16
-0.13
-0.11
-0.16
0.18
0.12
MAA
0.12
0.17
0.05
-0.27
-0.20
-0.08
-0.14
0.23
0.20
CG
-0.04
0.07
0.03
0.02
-0.16
-0.02
-0.07
-0.05
0.08
CO
0.23
-0.10
0.07
0.13
0.24
0.02
0.19
-0.25
0.17
UF
0.28
0.14
-0.35*
-0.36**
-0.04
-0.37**
-0.43**
-0.09
0.29
TT
0.13
-0.07
-0.24
-0.40**
0.09
-0.06
-0.18
0.13
0.30*
CN
0.18
0.20
-0.20
-0.20
-0.07
-0.33*
-0.32*
0.10
0.35*
SC
0.12
0.02
-0.26
-0.26
0.17
-0.40**
-0.29
-0.17
0.15
AE
0.06
0.28
-0.07
-0.18
0.30*
0.05
0.13
-0.01
0.39**
MS
-0.11
-0.05
-0.14
-0.16
-0.14
-0.02
-0.19
0.19
-0.02
EX
-0.27
0.34*
0.21
-0.05
-0.09
0.24
0.18
0.09
-0.23
QoE
-0.18
0.01
0.10
0.03
0.00
0.23
0.16
-0.08
0.05
VQ
0.07
0.22
-0.16
-0.07
0.02
-0.21
-0.18
0.11
0.36**
Table 6: Results of Pearsons correlation between the different metrics. Table shows correlation values between the subjective
scores and the objective metrics. ***indicates correlations with p values lower 0.01; ** correlations lower 0.05; *correlations
lower than 0.1.
addition, participants were saying that otherwise they would prefer
to have a simple red line following them, to keep a certain speed
compared to more playful elements such as following sharks or
similar. Having a plain speed indicator for experienced athletes is
also in line with previous research [10].
Participants were mentioning that currently there is too little
feedback in the VR condition. They suggested that the optimal place
for feedback would be the virtual place between the legs. The same
position where they also get feedback during outdoor rowing.
4
DISCUSSION AND CONCLUSION
The objective results above indicate that athletes perform slightly
better with regard to technical aspects in the VR-condition compared to the traditional workout. Though also the performance
data such as completion time show a significant difference. We
will disregard this for the further analysis as participants were instructed to concentrate on technique rather than on time. Indicating
that an improvement of time may be a by-product of an improved
technique or just putting unknowingly more effort into one of the
conditions.
Rhythm and Breath were the two metrics that improved the
most in the VR case compared to the non-VR case. Also, the strong
Session 2
MMSports’18, October 26, 2018, Seoul, Republic of Korea
49



<!-- page: 6 -->

correlation between these two metrics implies that VR helps to
improve the rhythmic pattern which is essential when it comes to
rowing.
When it comes to the objective metrics provided by the ergometer, it offers two different operating modes for the feedback,
normal and advanced. In our study we used the normal mode. In
case of experienced athletes this may not be the ideal setting. In
future studies it would be best considering to change to advanced
mode when performing the experiment with experienced rowers.
In this mode, the metrics are more rigorous, which may be more appropriate for experienced rowers. This change may result in larger
differences between the two conditions concerning the technique
metrics.
On the subjective scores, participants reported on a different experience between the two scenarios. The scale Concentration on the
task shows a higher score for the traditional workout. During this
condition athletes obviously have fewer distraction and therefore
can concentrate much more on the technical aspects of the workout.
However, although participants report to be less concentrated on
the task per-se, the technique metrics increased. Here, especially
the ones related to the rhythmic movement exertion. The fact that
participants enjoyed the VR experience more than the non-VR (valence score increased), also may be in line with them reporting to
have a higher score on loose sense of time. Due to the distraction of
the VR, they lost easier track of time. This could be an important
point why people may use increasingly indoor workouts enriched
by virtual environments. The reported emotional feedback from
the questionnaires shows also an increase in the arousal score, but
athletes felt less in control of the rowing experience (dominance)
for the VR case than the traditional condition. They also scored
higher for the autotelic experience.
From the results we can in general conclude that there is a difference when working out in VR versus a standard workout. This was
only a first study to investigate possible effects. In this experiment,
we concentrated rather on technique of the rower, and not so much
on the best performance time-wise. Future studies could investigate how VR is affecting the rowers performance when working on
more exhausting zones during the workout. Also, what effects in VR
would be improving the rower and their experience? Working out
in a more social context such as rowing versus friends or opponents
could be interesting to investigate. Thus varying the non-VR environmental factors could give interesting insights. An other aspect
is to investigate the different demands non-experienced rowers vs
experienced rowers would have on such a VR rowing system.
5
ACKNOWLEDGEMENTS
The authors would like to thank Ricard Vivo Monero for conducting
the study, as well as thanking the team at the Quality and Usability
Lab at TU Berlin for helping to create the virtual environment.
Thanks goes also to Sweetzpot for providing with the breathing
sensor.
REFERENCES
[1] L Gregory Appelbaum and Graham Erickson. 2016. Sports vision training: A
review of the state-of-the-art in digital training techniques. International Review
of Sport and Exercise Psychology (2016), 1–30.
[2] Kristoffer Hagen, Konstantinos Chorianopoulos, Alf Inge Wang, Letizia Jaccheri,
and Stian Weie. 2016. Gameplay as exercise. In Proceedings of the 2016 CHI
Conference Extended Abstracts on Human Factors in Computing Systems. ACM,
1872–1878.
[3] Charles P Hoffmann, Alessandro Filippeschi, Emanuele Ruffaldi, and Benoit G
Bardy. 2014. Energy management using virtual reality improves 2000-m rowing
performance. Journal of sports sciences 32, 6 (2014), 501–509.
[4] Susan A Jackson and Herbert W Marsh. 1996. Development and validation of a
scale to measure optimal experience: The Flow State Scale. Journal of sport and
exercise psychology 18, 1 (1996), 17–35.
[5] Tanja Kojic, Jan-Niklas Voigt-Antons, Lukas Tetzlaff, Bruno Kortowski, Uliana
Sirotina, and Sebastian Möller. 2018. Influence of Virtual Environments and Conversations on User Engagement During Multiplayer Exergames. In Proceedings
of Conference on Quality of Multimedia Experience (QoMEX 2018). IEEE.
[6] Peter J Lang, Margaret M Bradley, and Bruce N Cuthbert. 1997. International
affective picture system (IAPS): Technical manual and affective ratings. NIMH
Center for the Study of Emotion and Attention (1997), 39–58.
[7] Fabien D Legrand, Philippe M Joly, William M Bertucci, Mickael A SoudainPineau, and Julie Marcel. 2011. Interactive-virtual reality (IVR) exercise: An
examination of in-task and pre-to-post exercise affective changes. Journal of
Applied Sport Psychology 23, 1 (2011), 65–75.
[8] David L Neumann, Robyn L Moffitt, Patrick R Thomas, Kylie Loveday, David P
Watling, Chantal L Lombard, Simona Antonova, and Michael A Tremeer. 2017. A
systematic review of the application of interactive virtual reality to sport. Virtual
Reality (2017), 1–16.
[9] Mateus Nunes, Luciana Nedel, and Valter Roesler. 2014. Motivating people to
perform better in exergames: Competition in virtual environments. In Proceedings
of the 29th Annual ACM Symposium on Applied Computing. ACM, 970–975.
[10] Steven Schmidt, Patrick Ehrenbrink, Benjamin Weiss, Jan-Niklas Voigt-Antons,
Tanja Kojic, Andrew Johnstony, and Sebastian Möller. 2018. Impact of Virtual
Environments on Motivation and Engagement During Exergames. In Proceedings
of Conference on Quality of Multimedia Experience (QoMEX 2018). IEEE.
[11] Jonathan Shepherd, Lewis Carter, Gert-Jan Pepping, and Leigh-Ellen Potter. 2018.
Towards an Operational Framework for Designing Training Based Sports Virtual
Reality Performance Simulators. In Multidisciplinary Digital Publishing Institute
Proceedings, Vol. 2. 214.
[12] Roland Sigrist, Georg Rauter, Laura Marchal-Crespo, Robert Riener, and Peter
Wolf. 2015. Sonification and haptic feedback in addition to visual feedback
enhances complex motor task learning. Experimental brain research 233, 3 (2015),
909–925.
Session 2
MMSports’18, October 26, 2018, Seoul, Republic of Korea
50
