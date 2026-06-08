# Kocur et al. (2025) — Customized Avatars and the Proteus Effect during Physical Exercise in VR

## Extraction notes

- Source PDF: 3706598.3713203-2.pdf

- Clean reading copy with page markers preserved.

- Light cleanup only; no interpretive notes mixed into source text.

- Verify exact quotations, statistics, and figure/table claims against the original PDF before thesis use.


---



<!-- page: 1 -->

.
.
Latest updates: hps://dl.acm.org/doi/10.1145/3706598.3713203
.
.
RESEARCH-ARTICLE
Investigating the Impact of Customized Avatars and the Proteus Eﬀect
during Physical Exercise in Virtual Reality
MARTIN KOCUR, University of Applied Sciences Upper Austria, School of Informatics,
Communications and Media, Hagenberg, Upper Austria, Austria
.
MELANIE KLOSS, University of Regensburg, Regensburg, Bayern, Germany
.
CHRISTOPH SCHAUFLER, University of Applied Sciences Upper Austria, School of
Informatics, Communications and Media, Hagenberg, Upper Austria, Austria
.
VALENTIN SCHWIND, Frankfurt University of Applied Sciences, Frankfurt am Main, Hessen,
Germany
.
NIELS HENZE, University of Regensburg, Regensburg, Bayern, Germany
.
.
.
Open Access Support provided by:
.
University of Applied Sciences Upper Austria, School of Informatics, Communications
and Media
.
University of Regensburg
.
Frankfurt University of Applied Sciences
.
PDF Download
3706598.3713203.pdf
01 February 2026
Total Citations: 5
Total Downloads: 2023
.
.
Published: 26 April 2025
.
.
Citation in BibTeX format
.
.
CHI 2025: CHI Conference on Human
Factors in Computing Systems
April 26 - May 1, 2025
Yokohama, Japan
.
.
Conference Sponsors:
SIGCHI
CHI '25: Proceedings of the 2025 CHI Conference on Human Factors in Computing Systems (April 2025)
hps://doi.org/10.1145/3706598.3713203
ISBN: 9798400713941
.



<!-- page: 2 -->

Investigating the Impact of Customized Avatars and the Proteus 
Effect during Physical Exercise in Virtual Reality 
Martin Kocur 
Digital Media Lab 
University of Applied Sciences Upper 
Austria 
Hagenberg, Austria 
martin.kocur@fh-hagenberg.at 
Melanie Kloss 
University of Regensburg 
Regensburg, Germany 
melanie.kloss@stud.uniregensburg.de 
Christoph Schaufler 
University of Applied Sciences Upper 
Austria 
Hagenberg, Austria 
christoph.schaufler@fh-hagenberg.at 
Valentin Schwind 
Frankfurt University of Applied 
Sciences 
Frankfurt am Main, Germany 
valentin.schwind@fb2.fra-uas.de 
Niels Henze 
University of Regensburg 
Regensburg, Germany 
nhenze@googlemail.com 
Abstract 
Virtual reality (VR) allows to embody avatars. Coined the Proteus 
effect, an avatar’s visual appearance can influence users’ behavior 
and perception. Recent work suggests that athletic avatars decrease 
perceptual and physiological responses during VR exercise. However, such effects can fail to occur when users do not experience 
avatar ownership and identification. While customized avatars increase body ownership and identification, it is unclear whether 
they improve the Proteus effect. We conducted a study with 24 
participants to determine the effects of athletic and non-athletic 
avatars that were either customized or randomly assigned. We developed a customization editor to allow creating customized avatars. 
We found that customized avatars reduced perceived exertion. We 
also found that athletic avatars decreased heart rate while holding 
weights, however, only when being customized. Results indicate 
that customized avatars can positively influence users during physical exertion. We discuss the utilization of avatar customization in 
VR exercise systems. 
CCS Concepts 
• Human-centered computing → Virtual reality; • Applied 
computing → Computer games. 
Keywords 
virtual reality, body ownership, Proteus effect, virtual embodiment, 
avatars, customization 
ACM Reference Format: 
Martin Kocur, Melanie Kloss, Christoph Schaufler, Valentin Schwind, and Niels 
Henze. 2025. Investigating the Impact of Customized Avatars and the Proteus Effect during Physical Exercise in Virtual Reality. In CHI Conference 
on Human Factors in Computing Systems (CHI ’25), April 26–May 01, 2025, 
This work is licensed under a Creative Commons Attribution 4.0 International License. 
CHI ’25, Yokohama, Japan 
© 2025 Copyright held by the owner/author(s). 
ACM ISBN 979-8-4007-1394-1/25/04 
https://doi.org/10.1145/3706598.3713203 
Yokohama, Japan. ACM, New York, NY, USA, 18 pages. https://doi.org/10. 
1145/3706598.3713203 
1 Introduction 
Physical inactivity has emerged as a global public health concern, 
contributing to various chronic diseases and overall deterioration 
of well-being [106]. Many people around the globe do not meet the 
recommended levels of physical activity and those who start exercising typically drop out within the first months [55, 59]. Leveraging 
immersive technology such as virtual reality (VR) has become a 
promising approach to tackle physical inactivity and increase exercise adherence [24, 110]. Therefore, immersive exercise systems 
and fitness applications received increased attention and aim to 
motivate people by eliciting enthusiasm during physical exertion 
and promoting a healthier lifestyle [40]. 
A crucial component of VR experiences is the avatar—the users’ 
digital self-representation. Modern VR technology allows users to 
experience the avatar as their own body resulting in a phenomenon 
commonly known as the body ownership illusion (BOI) [41, 47]. 
This illusory sensation of embodying a virtual avatar is typically 
induced using motion capture so that users’ motions are registered 
and transferred onto the avatar in real time [41, 90, 98]. When 
users move their limbs, the avatar’s equivalent limbs mimic this 
motion creating the perceptual illusion of having a foreign body. 
As VR allows displaying the avatar in all possible ways, the user 
can, therefore, embody all imaginable appearances with different 
characteristics than the own body [44]. 
Interestingly, previous work found that the avatars’ visual characteristics can change how users behave and perceive the surrounding environment [44, 108]. Yee and Bailenson [108] showed that 
users embodying attractive avatars behaved more confidently while 
talking to a confederate in VR. The authors termed this phenomenon the Proteus effect. This effect could also be evidenced during 
exergames. Peña and Kim [80] showed that users playing virtual 
tennis on a Wii Fit using a normal weight avatar were physically 
more active than when operating an avatar the authors dubbed 
obese. Similarly, Kocur et al. [48] revealed that muscular avatars 
can decrease the perception of effort during exercise in VR. As the 
perception of effort is a barrier to regular physical activity [65],



<!-- page: 3 -->

CHI ’25, April 26–May 01, 2025, Yokohama, Japan 
Kocur et al. 
these findings suggest that the avatars’ appearance can be leveraged to make more effective immersive fitness applications [44]. 
However, there is empirical evidence that the Proteus effect can 
also fail to occur when neglecting important moderators [5, 49, 74]. 
Kocur et al. [49] found that athletic avatars do not necessarily 
affect the perception of effort and heart rate responses positively 
while cycling in VR. The authors argue that the users had a reduced 
body ownership and identification with the avatars that made the 
Proteus effect fail to occur. This is in line with Praetorius and 
Görlich [81] who assumes that the magnitude of the Proteus effect 
and whether this phenomenon occurs at all depends on the extent of 
the experienced body ownership and how strong users can identify 
with the avatars [81]. Banakou et al. [5], for example, found that 
the Proteus effect is extinguished when the avatar do not move in 
synchrony due to a reduced sensation of body ownership. To avoid 
that an avatar’s effects fail to occur, it is important to find ways 
to increase the probability of successfully inducing the Proteus 
effect and amplify its magnitude by augmenting the sense of body 
ownership and identification with the avatars. 
Prior research showed the benefits of allowing users to customize 
their avatars such as enhanced body ownership sensations [67]. 
Birk et al. [13], for example, found that customized avatars can increase avatar identification and intrinsic motivation while playing 
an infinite runner on a non-immersive display. Koulouris et al. [56] 
revealed that customized avatars enhanced user identification and 
exercise performance while cycling in a VR exergame. While these 
findings suggest that customized avatars contribute to a higher 
sense of identification and embodiment, it is still unknown whether 
they also result in an amplified Proteus effect. If customized avatars 
can increase the Proteus effect resulting in enhanced exercise performance and reduced perceptual and physiological responses to 
physical effort, designers and developers could allow users to customize their avatars instead of assigning predefined ones to leverage 
the Proteus effect and create more effective fitness applications. 
In this paper, we conducted a study with 24 participants to determine the effects of avatars with two levels of athleticism that were 
either customized or randomly assigned. We measured the effects on 
participants’ perceptual and physiological responses as well as their 
physical performance. To allow users to customize their avatars, 
we developed a VR customization editor. Hence, users embodied 
athletic and non-athletic avatars that were either customized or 
randomly assigned while performing physically demanding tasks. 
We found that athletic avatars significantly reduced the heart while 
holding weights, however, only when being customized. We also 
show that the athletic as well as the customized avatars decreased 
the perception of effort. The findings indicate that avatar customization can positively affect users’ physical performance as well as 
perceptual and physiological responses during exercise. Results also 
suggest that avatar customization can augment the Proteus effect 
on physiological responses. We discuss our findings in the light of 
the Proteus effect and how they can be utilized for VR exercise and 
fitness applications. We also contribute with a VR customization 
editor that allows to create individualized avatars while embodying 
them. 
2 Related Work 
Our work builds on previous findings about the Proteus effect in 
physical settings and beyond. In the following, we first describe how 
users can experience the illusory sensation of embodying avatars. 
Afterward, we discuss work on the avatar customization and how 
it contributes to a closer avatar-user connection. Finally, we give 
an overview of the Proteus effect and its significant moderators. 
2.1 Body Ownership Illusions 
One remarkable capacity of the human brain lies in its ability to 
reconcile conflicting information from multiple senses, generating 
illusions that shape our perception of the world. This capability 
enables humans to interpret and experience their surroundings in 
ways that diverge from objective reality [41, 67]. 
Optical illusions fascinated humans since millenia. Aristotle already described that touching a small pea between two crossed fingers induced the tactile sensation of touching two different peas [2]. 
More recent perceptual illusions such as the Pinocchio illusion [58] 
or the popular rubber hand illusion (RHI) [17, 88] demonstrate how 
our brain can be tricked into perceiving other body parts or artificial limbs as our own. In the RHI, first demonstrated by Botvinick 
and Cohen [17], the act of simultaneously stroking one’s actual 
hand while observing a rubber hand causes humans to accept the 
artificial limb as part of their own body. This phenomenon has 
been explained by an integration of information from different 
senses during a single event. Our brain unifies the information into 
a cohesive perception [27, 33]. 
Despite apparent conflicts between visual input (seeing the rubber hand being stroked), tactile sensations (feeling the stroking on 
one’s actual hand), and proprioception (the awareness of the hand’s 
position), the brain adeptly resolves these conflicts. The result is a 
coherent and robust perceptual experience [28]. Consequently, the 
brain produces the illusion of ownership over artificial limbs, such 
as a rubber hand or even entire bodies, a phenomenon commonly 
referred to as the BOI [41, 98]. 
Petkova and Ehrsson [79], for example, showed that by applying 
visuo-tactile synchrony — a synchrony between touch and vision 
— the perception of a body swap can be induced. This induction 
method was also used to create the sensation of embodying an 
empty space resulting in an out-of-body experience [26]. While 
these illusions are just few of many examples that were induced 
in the real world [41], VR has become a promising technology to 
create the feeling of embodying a computer-generated body. 
VR enables the creation of perceptual experiences that are hardly 
feasible or even impossible to replicate in real-world environments. 
In VR, researchers can move beyond conventional visuo-tactile 
synchrony and explore alternative methods to induce bodily illusions. Utilizing tracking devices and advanced motion capture 
technologies, the movements of users can be accurately recorded 
and translated onto the virtual skeleton of an avatar, establishing a 
visuo-motor synchrony — a synchrony of movements between the 
physical body and the virtual representation. Sanchez-Vives et al. 
[93], for example, demonstrated the induction of a virtual RHI solely 
through visuo-motor synchrony, without the need for tactile stimulation. Participants in their experiment could move their actual 
hand and fingers, observing the virtual hand react synchronously.



<!-- page: 4 -->

Investigating the Impact of Customized Avatars and the Proteus Effect during Physical Exercise in Virtual Reality 
CHI ’25, April 26–May 01, 2025, Yokohama, Japan 
Since then, there have been numerous manifestations of full-body 
illusions demonstrating that users could even accept virtual bodies with visual attributes significantly divergent from their own 
physical selves. Examples included avatars that indicated having 
a different gender [96, 98] or body composition [30, 39, 53, 71], a 
much younger appearance [5], an older appearance [7], or even a 
different skin color [6, 31]. 
2.2 Avatar Identification 
Typically, game designers and researchers provide players with 
a virtual body using avatars — virtual characters that represent 
users in virtual worlds [8]. The term avatar is derived from the 
Hindu term “avatara” which refers to the descent of a deity on 
earth in terrestrial shapes [77]. According to Banks [8], in games 
users metaphorically descent into the virtual world by taking on 
digital bodies in terms of avatars. Hence, an avatar acts as the digital 
self-representation of players that is under their control during the 
game experience [44, 72]. 
Beside the perceived BOI, another important quality metric of 
the avatar experience is the sense of identification with the avatar. 
Van Looy et al. [102] postulates that avatar identification can be defined as a shift in self-perception that makes players consider their 
identity in the game as "I" and the virtual world as "where". Players, 
therefore, virtually turn into the avatar and experience in-game 
events as they were really happening to them [42]. In line with 
self-determination theory that is frequently used as a framework 
on how to design engaging games [13, 91], using avatars that players can identify with satisfies the need of relatedness, i.e., feeling 
connected to the avatar and others. Therefore, an increased avatar 
identification can result in a better overall game experience [10, 82], 
motivation [13], physical activity and arousal [85], as well as ingame performance [56, 84]. 
Van Looy et al. [102] subdivided avatar identification into three 
dimensions: similarity identification, wishful identification, and embodied presence. These dimensions are inspired by self-discrepancy 
theory [32] postulating that one’s self-concept consists of different 
components: the actual self (i.e., traits that an individual believes to 
possess), the ideal self (i.e., traits that an individual ideally wants 
to possess), and the ought self (i.e., traits that an individual believes they ought to possess). To achieve a high degree of avatar 
identification, these different selves need to be considered in the 
avatar design process. The more similar the avatar is to their player, 
the better they can identify with the avatar resulting in a stronger 
bond between both [20]. Similarity does not necessarily refer to the 
visual appearance only but also includes personality, attitudes, and 
beliefs [20, 102]. Wishful identification refers to the ideal version 
of oneself with attributes that are desirable and players would typically like to possess in the real world [99]. Previous work found 
that players who embodied idealized avatars were more satisfied 
and connected with their virtual characters [25, 37]. Similar to BOI, 
embodied presence refers to the sense of being present in the virtual 
world while being embodied in the avatar [102]. 
To foster identification with avatars in games and offer a more 
inclusive experience, many video games (particularly role-playing 
games) allow users to individually customize their avatar and express themselves [100]. In World of Warcraft [15], for example, 
players can choose the appearance, skills, and traits of their virtual 
characters. Another popular example is the open-world role-playing 
game Cyberpunk 2077 [18], where players can modify their avatar 
using an extensive and detailed customization editor. Prior research 
found that customized avatars enhance body ownership, identification, and the overall game experience [13, 87, 111]. Koulouris et al. 
[56] also showed that customized avatars reflecting a realistically 
better version of oneself improved physical performance while 
playing an exergame on a stationary bike. Interestingly, the authors 
showed that idealized avatars with characteristics that were nonachievable for the embodying users increased self-discrepancy resulting in deteriorating effects. While customization seems promising to increase body ownership and identification, the effects of 
customized avatars shown in previous work are not entirely understood. 
Overall, designers aim at inducing a strong sense of body ownership and avatar identification to create vivid and embodied experiences in games and virtual worlds [44]. The experience of body 
ownership is rather driven by cognitive mechanisms processed in 
a bottom-up manner, i.e., the fusion of single incoming sensory 
information across different modalities [3, 28]. Avatar identification arises when top-down concepts related to the avatar fit the 
self-concepts of the player. Hence, identification is mainly driven 
by top-down mechanisms based on prior knowledge and experiences, e.g., stereotypes [29, 104]. However, the precise mechanisms 
underlying BOIs and identification are yet not fully clarified and 
require further investigations. 
2.3 Proteus Effect 
The Proteus effect, as revealed by Yee and Bailenson [108], refers to 
the phenomenon where users’ perception and behavior in virtual 
environments are influenced by the appearance of their avatars. 
Yee and Bailenson [108] showed that users embodying attractive 
avatars exhibited increased confidence in social interactions compared to those with less attractive avatars. This effect stems from 
users associating stereotypical characteristics with their avatars’ 
appearance, subsequently leading to changes in behavior, attitude, 
and perception [11, 44, 83, 109]. 
One plausible explanation for the Proteus effect draws on selfperception theory, suggesting that individuals modify their behavior and attitudes based on their self-perception [9]. Users adapt their 
behavior and attitudes in response to the characteristics, stereotypes, and features associated with their avatars’ visual appearance. 
Numerous studies have demonstrated this phenomenon: olderlooking avatars influencing walking speed [86], muscular avatars 
enhancing physical performance [46, 48], and a sweaty appearance 
could affect perceived exertion [45]. 
Several studies point to avatars influencing users’ performance, 
with cognitive enhancements observed using an Einstein avatar [7, 
52]. Improved physical performance was demonstrated in scenarios such as typing and weightlifting, where avatars with specific 
attributes positively impacted users’ abilities [43, 46, 48]. Interestingly, the similarity between the user and avatar, rather than 
specific characteristics, has also been linked to enhanced physical 
activity [56, 69, 84].



<!-- page: 5 -->

CHI ’25, April 26–May 01, 2025, Yokohama, Japan 
Kocur et al. 
A recent study by Kocur et al. [49] showed that the Proteus effect 
can fail to occur when certain conditions are not met. In a VR experiment, athletic avatars could not affect perception of effort and heart 
rate responses while cycling an ergometer bike [49]. The authors 
argue that a reduced experienced embodiment and identification 
with the avatars are responsible for the absence of the Proteus effect. This is in line with Osimo et al. [74] who showed that avatars 
have a stronger cognitive influence when their move synchronously 
with the users’ motion compared to an asynchronous movement. 
Similarly, Banakou et al. [5] found that visuo-motor asynchrony 
can extinguish effects originated from the avatar’s appearance. For 
this reason, Kocur et al. [51] proposed to investigate embodiment 
time as a moderator of the Proteus effect, as previous work found 
that the longer one embodies foreign limbs the higher the degree 
of perceived body ownership [101]. In this vein, Navarro et al. [69] 
revealed that avatars displaying the users’ face have a stronger 
influence on users’ physical performance while running on a treadmill compared to avatars having a stranger’s face. While the results 
suggest that the Proteus effect could depend on the extent of avatar 
identification as well as experienced body ownership, a systematic 
investigation is still missing. 
2.4 Summary 
Previous research demonstrated a phenomenon known as the Proteus effect, which describes behavioral, perceptual, and attitudinal 
changes based on the avatars’ visual appearance. Research found 
that muscular and athletic avatars can improve physical performance during physically demanding tasks in VR. However, such 
effects can fail to occur when users experience a reduced sense of 
body ownership and identification with the avatar. While customizing avatars is known to increase body ownership and identification, 
it is still unknown whether customized avatars indeed augment 
the Proteus effect. Consequently, the impact of customized avatars 
on the Proteus effect and users’ perceptual and behavioral changes 
remains unclear. 
3 Method 
We conducted a study to examine the interplay between customized 
avatars and their athletic appearance. While previous work showed 
that generic athletic avatars can reduce physiological and perceptual responses [46, 48], we hypothesize that this effect can be enhanced when athletic avatars are customized instead of randomly 
assigned. We, therefore, aim to disentangle the perceptual and physiological effects of customized avatars and the effects of athletic 
avatars during physical exertion in VR. Consequently, participants 
embodied athletic and non-athletic avatars that were either customized by themselves or by another participant. Specifically, we 
explore how both customized and randomly assigned avatars, with 
either athletic or non-athletic appearances, affect physical performance, perceptual responses, and physiological reactions during 
exercise in VR. Additionally, body ownership, avatar identification, 
self-perceived fitness, and sense of presence are assessed to account 
for potential moderating factors [49, 81]. 
Based on the Proteus effect [46, 48, 109] and potential moderators 
such as body ownership and avatar identification [7, 81], the study 
therefore tested the following hypotheses: 
• Hypothesis 1 (H1): Athletic avatars reduce the perception 
of effort and physiological responses, and improve physical 
performance during physical exercise in VR. 
• Hypothesis 2 (H2): The effects of avatar customization and 
athleticism on perception of effort, physiological responses, 
and physical performance during physical exercise in VR interact. Specifically, we hypothesize that athletic avatars have 
a greater effect when being previously customized compared 
to randomly-assigned avatars. 
3.1 Study Design 
We investigate the effects of avatar customization and athleticism 
on physical performance as well as perceptual and physiological 
responses during exercise in VR. We conducted a study with two 
independent variables and followed the approach by Kocur et al. 
[48] by using a repeated-measures design to cancel out individual 
differences and reduce unsystematic variance. The first independent 
variable is Customization with the two levels customized and 
randomized. The second independent variable is Athleticism with 
two levels athletic and non-athletic. Participants therefore embodied 
customized and randomly assigned avatars with different levels of 
athleticism while performing physical exercises. To reduce order 
effects, we counterbalanced the order of the four conditions using 
a 4*4 Latin square. 
3.2 Measures 
We assessed the subjective perception of effort using the wellestablished Borg rating of perceived exertion (RPE) scale [16] while 
holding weights and performing biceps curls (see Fig. 1). We also 
continuously recorded the heart rate during the tasks and measured 
the physical performance by counting the number of curls. Another 
task was the reaction wall, where participants engaged in a reaction 
wall game that is frequently used as a playful way to train one’s 
agility, speed, and coordination in a range of domains [35, 38, 61]. 
In this task that took 45 seconds, we used the number of correct 
hits to operationalize physical performance. 
3.2.1 Perceived Exertion. We assessed the perceived exertion while 
participants were holding weights and during the biceps curls. The 
RPE scale was designed to increase linearly with exercise intensity and consists of 15 grades from 6 to 20. Every second grade 
is combined with a textual representation of the intensity, e.g. "7" 
stands for "very, very light" and "19" for "very, very hard" [16]. A 
rough estimation of the current heart rate can be calculated by 
multiplying each grade by 10, e.g., an intensity of 8 approximately 
matches a heart rate of 80. 
3.2.2 Heart Rate. The heart rate is frequently used as a valid predictor for one’s level of physical fitness [73]. We measured the HR 
using an optical HR monitor worn at the participant’s forearm (Polar OH1, Polar Electro, Finland). We continuously assessed the HR 
while participants were holding weights and performing biceps 
curls. 
3.2.3 Physical Performance. We assessed physical performance for 
the biceps curls and reaction wall game. For the biceps curls, we 
counted the number of curls throughout the duration of the task



<!-- page: 6 -->

Investigating the Impact of Customized Avatars and the Proteus Effect during Physical Exercise in Virtual Reality 
CHI ’25, April 26–May 01, 2025, Yokohama, Japan 
Figure 1: User wearing a motion capture suit (left), the VR customization editor (top middle), the athletic avatars while holding 
weights (top right) and performing biceps curls (bottom middle) in front of a virtual mirror, and a non-athletic avatar during 
the reaction wall game (bottom right). 
(30 seconds). For the reaction wall game, we counted the number 
of hits throughout the duration of the task (45 seconds). 
3.3 Control Measures 
To account for potential moderating factors [49, 81], a set of subjective measures were taken. We assessed the sense of presence 
using Item G5 of the Igroup Presence Questionnaire (IPQ) ("In 
the computer generated world I had a sense of "being there) [94]. 
Self-assessment of personal fitness was obtained through the SelfPerceived Fitness Questionnaire (SPF) [23], and the degree of avatar 
embodiment was assessed using the Body Representation Questionnaire (BRQ) [7]. Furthermore, identification with the avatar 
was measured using the Player Identification Scale (PIS) [102]. 
3.3.1 Body Ownership. Body ownership refers to the sense of perceptually "inhabiting" an avatar. It describes how much users feel 
that the avatar is an extension of their own body or self in the 
virtual space [41, 97]. To quantify the induced body ownership, we 
used the BRQ [7] with the single-item subscales vrbody ("I felt that 
the virtual body I saw when looking down at myself was my own 
body"), mirror ("I felt that the virtual body I saw when looking at 
myself in the mirror was my own body"), features ("I felt that the 
virtual body resembled my own real body in terms of shape, skin 
tone or other visual features"), twobodies ("I felt as if I had two 
bodies"), and agency ("I felt that the movements of the virtual body 
were caused by my own movements"). 
3.3.2 Self-Perceived Fitness. Self-assessment of personal fitness 
was obtained through the SPF [23]. This questionnaire uses the 
subscales (scores range from 1 to 13) fitness, strength, body composition, endurance, and flexibility (see Table 1). We surveyed participants using the SPF before the VR experiment to determine 
how fit they perceived themselves, which served as the baseline. In 
addition, we also asked the participants to complete the SPF after 
completing the tasks while still embodying the respective avatar 
condition to learn how fit they perceived themselves during avatar 
embodiment. Fig. 8 shows the average Δ SPF total score indicating 
the resemblance of the avatars’ perceived fitness and participants’ 
actual perceived fitness. 
3.3.3 Avatar Identification. While the concepts of body ownership and avatar identification are related, they involve distinct 
psychological and experiential processes. Avatar identification is 
the psychological process of connecting with or seeing the avatar 
as a representation of oneself. It describes how much an individual 
identifies with the avatar in terms of personality, values, goals, or 
narrative [13, 102]. In line with previous work [81], we also assessed 
the sense of identification with the avatar using the PIS [102]. This 
scale consists of the subdimensions embodied presence, similarity 
identification, and wishful identification. 
3.3.4 Presence. In line with previous work [48, 86, 92], we determined how present participants felt in the virtual environment. As 
Schwind et al. [95] suggested that the IPQ [94] questionnaire best 
reflects the construct of presence, we used the item G1 "general 
presence" using a 7-point Likert scale.



<!-- page: 7 -->

CHI ’25, April 26–May 01, 2025, Yokohama, Japan 
Kocur et al. 
3.4 Tasks 
We used three different tasks using isometric (i.e., holding weights) 
and isotonic exercises (i.e., biceps curls), and exercises that rely 
on agility and coordination (i.e., reaction wall) to cover a broad 
range of different physical abilities. Building on prior research in 
sports physiology [14, 103] and avatar studies [46, 48], we aimed 
to minimize unsystematic variance by controlling the task order 
across conditions: reaction wall, biceps curls, and holding weights. 
While randomizing the task order would minimize order effects but 
instead introduce random variability, a fixed sequence ensured that 
any order effects, such as fatigue accumulation, were systematic 
and equally distributed across avatar conditions. This enables better 
control over their influence on the results [103]. 
3.4.1 Reaction Wall Task. The reaction wall is frequently used as a 
playful way to train one’s agility, speed, and coordination in a range 
of domains [35, 38, 61]. In this task, participants were standing in 
front of a virtual wall consisting of a total of 16 fields that can light 
up. Once the participant initiated the game with the start button, 
one field lit up in red. Upon touching that field, another randomly 
selected field lit up. The game lasted for a total of 45 seconds, and 
the objective was to touch as many fields as possible within this 
time frame. The task required the participant to move quickly and 
coordinate their movements. We used the number of correct fields 
hit to operationalize physical performance in this task. 
3.4.2 Biceps Curls. In the second task, participants had to perform 
biceps curls following the approach proposed by the American Alliance for Health, Physical Education, Recreation and Dance Functional Fitness Test [89]. The fitness test is suitable for all fitness 
levels and can be conducted without adjusting weights for each 
participant. Consequently, participants performed as many curls as 
possible in 30 seconds using 2 kg dumbbells. They were instructed 
to perform the curls only as fast as they could while still adhering 
to a correct execution. The exercise was explained before the experiment, and proper posture and execution were practiced with test 
weights. The experimenter observed the execution and corrected if 
necessary by verbal instructions. During the execution, participants 
maintained an upright posture with feet shoulder-width apart, holding the dumbbells at the sides of the body with slightly bent arms. 
Without moving the upper arms, the forearms were maximally bent 
upward over the elbow joint. The arms were then brought back 
to the starting position in a controlled manner [21]. We counted 
the number of curls to operationalize physical performance in this 
task. 
3.4.3 Holding Weights. According to a standardized procedure [1, 
68], participants held one weight of 1kg in each hand for 60 seconds 
in a position at 90 degrees of shoulder abduction in the scapular 
plane (see Fig. 1). During the task, participants were presented 
with the RPE scale using a virtual panel, which remained visible 
throughout the entire task. At the 20th, 40th, and 55th seconds, a 
red border appeared around the panel, and the participant verbally 
indicated their perceived effort by stating a number on the scale. 
3.5 Participants 
We recruited 24 participants (12 female and 12 male) through the 
mailing list of our institution and social networks. One additional 
Female (N=12) 
Male (N=12) 
Scales of the SPF (min=1,max=13) 
M 
SD 
M 
SD 
Fitness 
7.75 
2.26 
6.75 
2.52 
Strength 
8.00 
2.04 
8.33 
1.49 
Body Composition 
7.75 
1.28 
7.41 
1.97 
Endurance 
7.08 
2.19 
7.66 
1.92 
Flexibility 
7.91 
1.24 
7.75 
1.95 
Table 1: Means (M) and standard deviations (SD) of the subscales of the SPF questionnaire by Delignières et al. [23] showing how participants assessed their personal fitness level. 
participant (female) was only recruited to create the first set of 
customized avatars without taking part in the main study. Hence, 
the following information only refer to the 24 participants. Their 
age ranged from 20 to 34 years (𝑀 = 26.13, 𝑆𝐷 = 3.58). Twentytwo participants were right-handed, and two were left-handed. 
Regarding the VR experience, 82.6% of the participants indicated 
they had no prior experience with VR, and 17.4% reported playing 
VR games a few times a year. To assess the participants’ level of 
fitness, we used the SPF questionnaire by Delignières et al. [23] as 
part of the demographics (see Table 1). 
39.1% of the participants reported never playing computer games, 
26.1% played a few times a year, 8.7% played a few times a month, 
13% played a few times a week, and 13% played daily. Seventeen 
participants wore contact lenses of had no visual impairment. Seven 
participants wore glasses. Four participants mentioned having previous upper extremity injuries, but all participants were healthy 
and pain-free at the time of the study. The body mass index (BMI) 
was within the normal range for 17 participants, ranging from 23.0 
to 23.9. One participant had a low BMI of 17.9. Five participants had 
a slightly elevated BMI between 25.6 and 28.3, and one participant 
had an elevated BMI with a value of 32. 
Participants were compensated with credit points for their study 
course. They were informed that they could withdraw or discontinue the experiment at any time without penalty. 
3.6 Apparatus 
We used an HTC Vive Pro HMD with a wireless adapter to allow 
participants moving freely within the VR area (see Fig. 1). The integrated Vive chaperone system rendered virtual lines when users 
approached the space boundaries preventing them to go beyond 
the defined VR area. The HMD has a wide horizontal field-of-view 
of 110◦ and a spatial resolution of 1440 × 1600 pixels per eye displayed at 90 fps. Participants perceived the virtual body and the 
surrounding environment from first-person perspective. 
We induced body ownership and agency by visuomotor synchrony. Participants’ real movements were captured with Optitrack 
motion capturing1 and transferred onto the virtual skeleton of the 
avatar. To track participants’ full-body motion, we employed a 
marker-based OptiTrack motion tracking system with twelve cameras (eight PRIME 13 and four PRIME 13W) and the Motive software 
(v. 2.1). The motion tracking software ran on a dedicated PC with 
Windows 10, Intel i7-8700, 26GB RAM, and a NVIDIA GeForce GTX 
1https://optitrack.com/



<!-- page: 8 -->

Investigating the Impact of Customized Avatars and the Proteus Effect during Physical Exercise in Virtual Reality 
CHI ’25, April 26–May 01, 2025, Yokohama, Japan 
1080 graphics card. We calibrated the OptiTrack system according 
to the manufacturer’s specification. 
Participants had to wear black marker suits (Optitrack Motion 
Capture Suit Classic2) available in different sizes (S, M, and L) with 
49 passive markers. The OptiTrack system tracked participants’ 
skeleton with 240 fps and was synchronized with the HMD’s head 
tracking to avoid interference. Using UDP multicast the skeletons 
were streamed through a local 1000 Mbit network connection via 
the NatNet protocol to the PC (Windows 10, Intel i7-8750H, 16GB 
RAM, NVIDIA GeForce GTX 1060 graphics card) that ran the VR 
application and rendered the 3D scene. 
3.6.1 Avatars. We used the Standard Genesis 8.1 Basic Male and 
Genesis 8.1 Basic Female characters from the 3D suite of DAZ Studio 4.20 as the basis for all avatars3 . The bodies and clothing of the 
avatars can be adjusted using morph targets, e.g, body fat, muscularity, height, etc. For detailed facial adjustments, we used the DAZ 
extension 200 Plus Head and Face Morphs for Genesis 8 Male and 
Female4 . The avatars and clothing were additionally post-processed 
in Blender 3.05 , to align the morph targets of the clothes and bodies. 
To achieve better skin textures, the PreIntegratedSkinShader V2.06 
was applied to the models. Various hairstyles were used from the 
Daz suite, and additional hairstyles were exported from various 
Mixamo7 avatars. 
3.6.2 VR Customization Editor. To compare the effects of customized avatars with avatars that were randomly assigned, an 
avatar creator was needed. Thus, we developed a customization editor that enables to adjust the avatar’s appearance based on certain 
parameters, e.g., clothes, facial features, hair, and body composition. To ensure a high degree of body ownership, we developed 
the VR customization editor using Unity (v. 2020.3.21f1) to allow 
participants to customize their avatars while embodying them (see 
Fig. 1). Participants initially embodied a standard avatar fitting 
the specified gender which could be modified through a menu in 
the virtual space. There were two panels representing the user interface. The left panel allowed participants to navigate through 
categories that could be altered, e.g., body, face, or hair. In the right 
panel, individual parameters could be adjusted in detail. Navigation and control were done using 3D buttons and sliders, activated 
through virtual touch. All changes were transferred in real-time to 
the embodied avatar. In the virtual space, there were three mirrors 
allowing participants to view themselves from all angles. 
We followed the approach by Koulouris et al. [56] to determine 
the avatars’ characteristics that could be modified. During avatar 
creation, participants could choose from a total of 16 face templates, 
which could then be adjusted in detail. There were 20 facial details 
(eyes, eyebrows, nose, mouth, face shape) that could be customized. 
For the body, there were a total of 13 editing options regarding the 
2https://optitrack.com/products/motion-capture-suits/
3https://www.daz3d.com/
4https://www.daz3d.com/200-plus-head-and-face-morphs-bundle-for-genesis-8female-s-and-male-s 
5https://www.blender.org/
6https://assetstore.unity.com/packages/vfx/shaders/pre-integrated-skin-shader7238 
7https://www.mixamo.com/ 
categories muscularity, body fat, and height. The level of muscularity and body fat could be adjusted using morph targets89 (ranging from 0 to 100%) that controlled the extent of fitness, weight, 
muscularity, body fat, fitness details such as definition, and the 
overall body mass. Participants could therefore extensively design 
the avatars’ athleticism using sliders in the customization editor 
that controlled the morph targets’ values. To reduce complexity 
and ensure realistic proportions, the morph targets controlled the 
entire body and not specific body parts. Fig. 2 shows examples of 
customized baseline, athletic, and non-athletic avatars. 
An essential aspect of avatar creation was enabling adjustments 
to easily recognizable features such as hair, clothing, and body 
shape to facilitate identification with the avatar [25]. Therefore, 
participants could choose from 10 hairstyles (ranging from short to 
long as well as tied hair), different clothing items ranging from short 
to long attire with 5 types of pants (shorts, jeans, joggers, loose 
pants, leggings), 4 types of upper part clothing (tank top, jogging 
sweater, t-shirt, sweatshirt), and three types of shoes (unisex sneakers, basketball shoes, and casual everyday-shoes.) All items’ colors 
as well as the colors of skin, hair, and eyes could be customized. 
First, participants were instructed to create an avatar that should 
best represent themselves and resemble the real appearance and 
their body shape as closely as possible. Based on this avatar, an 
athletic and non-athletic version were created and later embodied 
during the physical tasks (see Fig. 2). 
3.7 Procedure 
After arrival, we explained the study’s procedure. Afterward, participants read and signed an informed consent form. Following that, 
a demographic questionnaire was filled out on a desktop computer, 
along with a questionnaire assessing their own fitness. The experimenter asked the participants if they were right- or left-handed, 
as the device for measuring heart rate was attached to the nondominant arm. 
Participants were briefed on the tasks and the RPE scale. The 
holding weight exercise and biceps curls were explained, and proper 
posture and execution were practiced with test weights. Afterwards, 
the user interface of the VR customization editor was explained. 
Participants then put on the motion capture suit, donned the VR 
headset, and adjusted its size fitting to their head. Once clothing 
and the headset were in place, participants performed a T-pose to 
calibrate the skeleton for the avatars. 
The VR customization editor was launched and participants initially embodied a neutral base avatar corresponding to their stated 
gender. Alongside the user interface for avatar creation and mirrors, 
there was also a panel with instructions and a timer. Participants 
had a maximum of 20 minutes to create an avatar that best matched 
their real appearance. Starting from this avatar, they could create 
an athletic version with the instruction "Create an avatar that is 
a representation of your appearance after 1 year having a healthy 
and active lifestyle with regular exercise and a healthy diet," and a 
non-athletic version with the instruction "Create an avatar that is a 
representation of your appearance after 1 year having an unhealthy 
and inactive lifestyle with no exercise and an unhealthy diet". In 
8https://www.daz3d.com/massive-morphs-for-genesis-8-male
9https://www.daz3d.com/massive-morphs-for-genesis-8-female-s



<!-- page: 9 -->

CHI ’25, April 26–May 01, 2025, Yokohama, Japan 
Kocur et al. 
Figure 2: Examples of avatars with the baseline, athletic, and non-athletic version (from left to right). Participants had 
a maximum of 20 minutes to create an avatar that best matched their real appearance while doing sports. Starting from 
this avatar, they had additional five minutes to create an athletic version with the instruction "Create an avatar that is a 
representation of your appearance after 1 year having a healthy and active lifestyle with regular exercise and a healthy diet," 
and a non-athletic version with the instruction "Create an avatar that is a representation of your appearance after 1 year having 
an unhealthy and inactive lifestyle with no exercise and an unhealthy diet". Participants could customize a range of options 
ranging from different faces and facial details, body compositions using categories such as muscularity, body fat, and height, as 
well as different hair and sports clothes from long to short attire (see section 3.6.2) 
total, participants had five minutes for creating the athletic and 
non-athletic versions. 
After avatar creation, participants embodied the athletic and 
non-athletic avatars during the physical tasks. As we aimed to 
increase external validity, we did not use one generic avatar as the 
randomized avatar for all participants. Instead, they were assigned 
two avatars (one was athletic, one was non-athletic) created by the 
preceding participant. Thus, each participant embodied a total of 
four avatars. As the first participant also required two avatars that 
were not customized, an additional participant was recruited only 
for customizing an athletic and non-athletic avatar. 
To allow the participant to become familiar with the virtual environment and the respective avatar condition, we included a short 
adaptation phase where participants could perceive themselves in 
a virtual mirror. Once ready, the participants could start the reaction wall game by pressing a virtual button. After 45 seconds, a 
notification appeared indicating that the task was completed. The 
experimenter paused the VR application and the screen faded to 
black. The experimenter then handed over the dumbbells to the 
participants and restarted the VR application to start the bicep 
curls task. The participants were asked if they were ready, and with 
a verbal signal from the experimenter, the task started. After 25 
seconds, the RPE scale lit up in red, and the participant stated a 
number representing their perceived effort. The task concluded 
after 30 seconds, and a scale for weight assessment appeared. 
Participants rated the perceived weight on the scale verbally from 
0 (light) to 6 (heavy). Afterwards, the VR application was paused 
and the experimenter then handed dumbbells to the participant for 
the weight-holding task. After restarting the VR application, the 
experiment used a verbal signal to start the weight holding task. 
The participants were asked to hold the weights for 60 seconds 
and provide their perceived effort using the RPE scale after 20, 40, 
and 55 seconds. Following that, the weight of the dumbbell was 
subjectively assessed from 0 (light) to 6 (heavy). The experimenter 
removed the dumbbells and the participants were asked to complete 
the questionnaires in VR, i.e., BRQ, IPQ, PIS, and SPF. In line with 
Kocur et al. [46], we leveraged the time for completing the questionnaires as a resting period taking about 3 minutes per participant to 
reduce the heart rate before the next condition. Afterwards, the first 
condition was finished and the participant received a new avatar, 
repeating the procedure. 
Once the tasks with all avatars were completed, participants 
could remove the VR headset and the motion capture suite. Finally, 
they filled out a questionnaire regarding their experience with 
the avatars and the experiment. Participants were debriefed and 
received credit points for their study course and as well as sweets 
for their participation. The entire study lasted approximately 90 
minutes in total, with approximately 60 minutes spent in the virtual 
world. 
4 Results 
Our measures consisted of both parametric and non-parametric 
data. We conducted Shapiro-Wilk tests to assess normality for the 
perception of effort, physical performance, and all questionnaire



<!-- page: 10 -->

Investigating the Impact of Customized Avatars and the Proteus Effect during Physical Exercise in Virtual Reality 
CHI ’25, April 26–May 01, 2025, Yokohama, Japan 
12 
13 
customized 
randomized 
perceived exertion 
holding weights 
10.0 
10.5 
11.0 
11.5 
12.0 
customized 
randomized 
perceived exertion 
biceps curls 
Figure 3: Average perceived exertion score while holding weights (left) and while performing biceps curls (right). Participants 
had a significantly lower perceived exertion while holding weights when embodying the customized avatar and the athletic 
avatar. Similarly, participants also had a significantly lower perception of effort while performing biceps curls when embodying 
the athletic avatar. The error bars represent the standard error of the means. 
scores. For hypothesis testing involving non-parametric data, we 
used the Aligned Rank Transform (ART) package for R by Wobbrock et al. [107] to perform an ART analysis of variance (ANOVA). 
All analyses were performed at the participant level with the subject as a random factor. Table 3 shows a summary of the inferential 
statistics per measure and task. 
To analyze the effects on perceived effort, we conducted a 2 × 2 
repeated measures analysis of variance (RM-ANOVA) with Customization (customized, randomized) and Athleticism (athletic, 
non-athletic) as within-subject factors. The dependent variable was 
perceived exertion, measured on the RPE scale, ranging from 6 
to 20. We used the same analysis framework for evaluating selfperceived fitness, avatar identification, experienced illusion of 
body ownership (IBO), and sense of presence. For the analysis of 
heart rate (HR) during the biceps curls, we conducted a 2 × 2 × 6 
RM-ANOVA with Customization (customized, randomized), Athleticism (athletic, non-athletic), and Time (after 5, 10, 15, 20, 25, 
30 seconds) as within-subject factors. HR data were aggregated in 
5-second intervals. In the analysis of HR while holding weights, 
Time included 12 levels, corresponding to measurements every 5 
seconds for 60 seconds. The dependent variable was HR, measured 
in beats per minute (BPM). 
4.1 Perceived Exertion 
We performed statistical analyses to find out the effects of Avatar 
and Customization on the perception of effort for the tasks holding 
weights and biceps curls. 
4.1.1 Holding Weights. A 2 × 2 RM-ANOVA revealed a significant 
main effect of Athleticism, 𝐹 (1, 23) = 4.663, 𝑝 = .041, 𝜂2 
𝑝= .169, 
and Customization, 𝐹 (1, 23) = 5.812, 𝑝 = .024, 𝜂2 
𝑝= .202, on perceived exertion during weight holding tasks. However, the interaction between Customization and Athleticism was not significant, 
𝐹 (1, 23) = 2.545, 𝑝 = .124, 𝜂2 
𝑝= .100. Participants reported lower 
perceived effort when embodied in athletic avatars compared to 
non-athletic avatars and in customized avatars compared to randomized ones. Hence, we confirm H1 indicating that athletic avatars 
could reduce perception of effort. In addition, we also found that 
customization could also reduce perception of effort. 
4.1.2 Biceps Curls. Similarly, a 2 × 2 RM-ANOVA for biceps curls 
revealed a significant effect of Athleticism, 𝐹 (1, 23) = 10.599, 
𝑝 = .003, 𝜂2 
𝑝= .315, but no significant effect of Customization, 
𝐹 (1, 23) = 0.576, 𝑝 = .455, 𝜂2 
𝑝= .024. There was also no significant 
interaction between Customization and Athleticism, 𝐹 (1, 23) = 
1.501, 𝑝 = .233, 𝜂2 
𝑝= .061. Participants reported lower perceived 
exertion during biceps curls when embodied in athletic avatars 
compared to non-athletic avatars (see Fig. 3). Hence, these findings 
again confirm H1. 
4.1.3 Correlation Analysis. To test whether there is a relationship 
between the perception of effort and the participants’ self-perceived 
fitness (baseline, i.e., evaluated before avatar embodiment), we 
performed Pearson’s correlation analyses of the total SPF score and 
the perception of effort while holding weights and during biceps 
curls. There was a significant negative correlation between the 
perception of effort and the self-perceived fitness while holding 
weights, 𝑟 (94) = −0.295, 𝑝 = .003. We also found a significant 
negative correlation between the perception of effort and the selfperceived fitness during biceps curls, 𝑟 (94) = −0.435, 𝑝 < .001. The 
negative correlation indicates that a higher self-perceived fitness 
tended to result in a lower perception of effort for both tasks. 
4.2 Heart Rate 
As we continuously recorded the HR while participants were holding the weights and performing the biceps curls, we report the 
inferential statistics per task. For both tasks, HR was determined 
every second over the duration of the task (60 seconds for holding 
weights and 30 seconds for biceps curls). The recorded data were 
then aggregated into 5-second intervals for both tasks, resulting in 
12 aggregate HR values per participant for holding weights and 6 
values for biceps curls. To control for individual differences in resting HR and eliminate potential confounding factors, we normalized 
the HR data by centering it at zero for each participant (subtracting 
the initial HR value from subsequent values). As previous work



<!-- page: 11 -->

CHI ’25, April 26–May 01, 2025, Yokohama, Japan 
Kocur et al. 
customized 
randomized 
5 10 15 20 25 30 35 40 45 50 55 60 
5 10 15 20 25 30 35 40 45 50 55 60 
0 
5 
10 
time in seconds 
heart rate in bpm 
holding weights 
customized 
randomized 
5 
10 
15 
20 
25 
30 
5 
10 
15 
20 
25 
30 
0.0 
2.5 
5.0 
7.5 
10.0 
12.5 
time in seconds 
heart rate in bpm 
biceps curls 
Figure 4: Average normalized heart rate centered at zero while holding weights (left) and performing biceps curls (right). 
Participants had a significantly reduced heart rate while holding weights when embodying the athletic avatar, however, when 
the avatar was previously customized. The error bars show the standard error of the means. 
suggest that the Proteus effect is time-dependent [46], this allowed 
us to investigate how HR evolved over time and explore whether 
the effects caused by the independent variables differently evolve 
across time. 
4.2.1 Holding Weights. A 2 × 2 × 12 RM-ANOVA was conducted 
to analyze the effects of Customization, Athleticism, and Time 
on the normalized HR while holding weights. The analysis revealed 
no significant main effect of Customization, 𝐹 (1, 23) = 0.311, 
𝑝 = .583, 𝜂2 
𝑝= .013. However, there was a significant main effect 
of Athleticism, 𝐹 (1, 23) = 4.374, 𝑝 = .048, 𝜂2 
𝑝= .160, indicating 
that participants had a lower HR when embodying athletic avatars 
compared to non-athletic avatars. A significant main effect of Time 
was also observed, 𝐹 (1.71, 39.33) = 29.814, 𝑝 < .001, 𝜂2 
𝑝= .565, as 
well as a significant two-way interaction between Customization 
and Athleticism, 𝐹 (1, 23) = 5.214, 𝑝 = .032, 𝜂2 
𝑝= .185. Furthermore, a significant three-way interaction between Customization, 
Athleticism, and Time, 𝐹 (1.99, 45.82) = 3.471, 𝑝 = .040, 𝜂2 
𝑝= .131, 
was found. All other interactions were non-significant (all 𝑝 > .05). 
These results confirm H1 indicating that participants experienced a lower HR over time when embodying athletic avatars. In 
addition, H2 is also confirmed as the analysis showed a significant 
interaction effect of Customization and Athleticism indicating 
that the effects caused by the avatars’ athleticism depended on if 
the avatars were being previously customized (see Fig. 4). 
4.2.2 Biceps Curls. A 2 × 2 × 6 RM-ANOVA was conducted to 
analyze the effects of Customization, Athleticism, and Time 
on the normalized HR during biceps curls. The analysis revealed 
no significant main effect of Customization, 𝐹 (1, 23) = 0.366, 
𝑝 = .551, 𝜂2 
𝑝= .016, or Athleticism, 𝐹 (1, 23) = 3.125, 𝑝 = .090, 
𝜂2 
𝑝= .120. However, there was a significant main effect of Time, 
𝐹 (1.67, 38.40) = 74.028, 𝑝 < .001, 𝜂2 
𝑝= .763, indicating a strong 
effect of time on HR during the task. All interaction effects were 
non-significant (all 𝑝 > .05). These results suggest that participants’ 
HR during biceps curls was significantly influenced by the passage 
of time but was not affected by the athletic appearance or the 
customization of the avatars (see Fig. 4). Consequently, H1 and 
H2 cannot be confirmed for biceps curls suggesting that avatars’ 
physiological effects are task-specific. 
4.2.3 Correlation Analysis. To test whether there is a relationship between the heart rate responses and the participants’ selfperceived fitness (baseline, i.e., evaluated before avatar embodiment), we performed Pearson’s correlation analyses of the total 
SPF score and the heart rate while holding weights and during 
biceps curls. There was a significant negative correlation between 
the heart rate and the self-perceived fitness while holding weights, 
𝑟 (94) = −0.224, 𝑝 = .029. We also found a significant negative correlation between the heart rate and the self-perceived fitness during 
biceps curls, 𝑟 (94) = −0.240, 𝑝 = .019. The negative correlation 
indicates that a higher self-perceived fitness tended to result in a 
lower heart rate for both tasks. 
4.3 Physical Performance 
A 2 × 2 RM-ANOVA was conducted to analyze the effects of Customization and Athleticism on the number of hits during the 
reaction wall game. The analysis showed no significant main effect of Customization, 𝐹 (1, 23) = 4.103, 𝑝 = .055, 𝜂2 
𝑝= .151, or 
Athleticism, 𝐹 (1, 23) = 3.332, 𝑝 = .081, 𝜂2 
𝑝= .127. There was 
also no significant interaction between Customization and Athleticism, 𝐹 (1, 23) = 2.490, 𝑝 = .128, 𝜂2 
𝑝= .098. A 2 × 2 ART 
ANOVA was performed to analyze the number of biceps curls. 
The analysis revealed a significant main effect of Customization, 
𝐹 (1, 23) = 5.806, 𝑝 = .024, 𝜂2 
𝑝= .200, indicating that participants 
executed more biceps curls while embodying customized avatars 
compared to randomized ones. However, there was no significant 
effect of Athleticism, 𝐹 (1, 23) = 3.575, 𝑝 = .071, 𝜂2 
𝑝= .130, and 
no significant interaction between Customization and Athleticism, 𝐹 (1, 23) = 0.020, 𝑝 = .887, 𝜂2 
𝑝< .001. These results suggest 
that participants performed more biceps curls when embodying 
customized avatars, regardless of their athleticism. Figure 5 shows 
the number of hits and biceps curls across the conditions. Hence, 
H1 and H2 cannot be confirmed for the amount of biceps curls and 
number of hits during the reaction wall game.



<!-- page: 12 -->

Investigating the Impact of Customized Avatars and the Proteus Effect during Physical Exercise in Virtual Reality 
CHI ’25, April 26–May 01, 2025, Yokohama, Japan 
48 
50 
52 
54 
56 
customized 
randomized 
number of hits 
reaction wall 
16 
17 
18 
customized 
randomized 
number of curls 
biceps curls 
Figure 5: Mean number of hits for the reaction wall game (left) and the number of biceps curls (right). Participants performed 
significantly more biceps curls when embodying customized avatars, regardless of their athleticism. The error bars show the 
standard error of the means. 
4.3.1 Correlation Analysis. To test whether there is a relationship between the physical performance and the participants’ selfperceived fitness (baseline, i.e., evaluated before avatar embodiment), we performed Pearson’s correlation analyses of the total 
SPF score and the performance during the reaction wall game 
and biceps curls. There was no significant correlation between 
the performance and the self-perceived fitness during biceps curls, 
𝑟 (94) = −0.025, 𝑝 = .810. We also did find not a significant correlation between the performance and the self-perceived fitness during 
the reaction wall game, 𝑟 (94) = −0.107, 𝑝 = .287. 
4.4 Control Measures 
In the following, we report the statistical results of each control 
measure that was used to account for potential moderators proposed by previous work [49, 81]. The summary of the statistical 
analysis of each control measure can be found in Table 2. 
4.4.1 Body Ownership. We performed 2 × 2 ART RM-ANOVAs on 
each dimension of the BRQ (vrbody, twobodies, mirror, features, and 
agency) to analyze the effects of Customization, Athleticism, and 
their interaction. The results indicate that participants experienced 
higher body ownership when embodying the customized avatars 
compared to the randomized ones, as well as when embodying 
the athletic avatars compared to the non-athletic avatars. Figure 6 
shows the average scores for each dimension of the BRQ across 
conditions. 
4.4.2 Avatar Identification. We conducted 2 × 2 ART RM-ANOVAs 
on each dimension of the PIS (embodied presence, similarity identification, and wishful identification) to analyze the effects of Customization and Athleticism. The results suggest that participants 
experienced a higher sense of identification with the customized 
avatars compared to the randomized ones, as well as with the athletic avatars compared to the non-athletic ones. Figure 7 shows the 
average scores of each dimension of the PIS for each condition. 
4.4.3 Self-Perceived Fitness. We conducted a 2 × 2 RM-ANOVA on 
the total score of the SPF to analyze the effects of Customization 
and Athleticism. The results suggest that participants perceived 
higher fitness when embodying customized and athletic avatars, 
but this was independent of any interaction between customization 
and athleticism. Figure 8 shows the average overall scores of selfperceived fitness across conditions relative to participants’ actual 
perceived fitness. 
4.4.4 Presence. We conducted a 2 × 2 ART RM-ANOVA to analyze 
the effects of Customization and Athleticism on the general 
presence measured by the IPQ. The results indicate that participants 
did not experience a significant difference in their sense of presence 
while embodying the respective avatars. Figure 8 shows the average 
overall presence scores per condition. 
5 Discussion 
The quantitative results of our study revealed that customized and 
athletic avatars can decrease the perception of effort while exercising in VR. Participants had a lower perception of effort while 
holding weights when embodying the customized avatars compared to the randomly assigned ones. In line with previous work on 
the Proteus effect [46, 48], we also showed that participants had a 
lower perceived exertion when embodying the athletic avatar compared to the non-athletic version. As indicated by the significant 
Customization × Athleticism interaction, our results even show 
that athletic avatars reduced the heart rate over time while holding weights, however, only when being customized. This implies 
that customizing avatars can influence the effects by an avatar’s 
athleticism on physiological responses to physical effort. In addition, participants executed more biceps curls while embodying the 
customized compared to the randomized avatars. 
Considering the Proteus effect, we could show that participants 
had a lower perception of effort while embodying athletic avatars 
during biceps curls and when holding weights. While not significant, we can observe the trend that the impact of athletic avatars 
on perceived exertion appear larger when the avatars were customized (see Fig. 3). In line with the perception of effort, we could 
show a dependency between customization and athleticism on 
heart rate while holding weights (see Fig. 4). We would expect 
that the customized athletic avatars resulted in the best while the 
customized non-athletic avatars in the worst performance as well 
as perceptual and physiological responses. We, however, found



<!-- page: 13 -->

CHI ’25, April 26–May 01, 2025, Yokohama, Japan 
Kocur et al. 
Customization 
Athleticism 
Customization × Athleticism 
Questionnaire Items 
𝑭 (1, 23) 
p 
𝜼 2 
𝒑 
𝑭 (1, 23) 
p 
𝜼 2 
𝒑 
𝑭 (1, 23) 
p 
𝜼 2 
𝒑 
BRQ: vrbody 
11.478 
.002 
.33 
6.609 
.017 
.22 
5.789 
.025 
.20 
BRQ: twobodies 
.482 
.494 
.02 
.043 
.837 
.002 
.549 
.466 
.02 
BRQ: mirror 
8.330 
.008 
.27 
11.996 
.002 
.34 
4.289 
.049 
.16 
BRQ: features 
16.796 
<.001 
.42 
29.820 
<.001 
.56 
4.196 
.052 
.15 
BRQ: agency 
.033 
.858 
.001 
4.648 
.042 
.17 
2.090 
.161 
.08 
PIS: embodied presence 
32.402 
<.001 
.58 
18.451 
<.001 
.45 
8.887 
.007 
.28 
PIS: similarity identification 
36.296 
<.001 
.61 
48.181 
<.001 
.68 
20.644 
<.001 
.47 
PIS: wishful identification 
13.590 
.001 
.37 
178.379 
<.001 
.89 
38.454 
<.001 
.63 
SPF: total score 
8.204 
.009 
.263 
7.501 
.012 
.246 
0.657 
.420 
.03 
IPQ: general presence 
1.712 
.203 
.07 
0.177 
.677 
.007 
3.096 
.091 
.12 
Table 2: Inferential statistics for all control measures assessing body ownership (BRQ), avatar identification (PIS), self-perceived 
fitness (SPF), and presence (IPQ). 
that customization influences the most measures irrespective of 
the avatars’ athleticism. Consequently, our findings suggest that 
whether customization increases avatars’ effects could depend on 
the task at hand. Holding weights is an isometric exercise, while 
biceps curls are an isotonic exercise, and these different types of 
exercises may have varying susceptibility to the Proteus effect. Understanding how the effectiveness of the Proteus effect changes 
across different types of tasks is a promising direction for future 
research. 
We rule out effects of fatigue and exhaustion as an causal explanation for the variance in physiological and perceptual responses 
between the avatars. We employed a repeated-measures design to 
minimize unsystematic variance arising from individual differences. 
To mitigate order effects, we counterbalanced the conditions across 
participants. Furthermore, task durations were controlled and held 
consistent across participants to ensure that all participants had an 
equal amount of time for each task. As participants completed the 
same sequence of tasks regardless of the avatar they embodied, any 
fatigue experienced would affect each avatar condition systematically. Thus, the significant differences in heart rate and perceptual 
responses we observed cannot be attributed to fatigue, as such 
effects would not explain the variation between avatar conditions. 
Furthermore, we also ensured that the participants had a workload that was within the aerobic threshold of 75% maximum HR [76] 
per avatar condition by using physical tasks with a light to moderate intensity to minimize effects of fatigue and avoid the lactate 
turn point [46, 76]. This is also represented by participants’ perceived exertion that ranged from 10 to 13 which is considered light 
to moderate [16] (see Fig. 3). Hence, our findings indicate that, although later tasks (e.g., holding weights) or conditions may have 
led to higher levels of exhaustion, the effects of the avatars were 
sufficiently robust to remain detectable. 
5.1 Perception of Effort and Physical 
Performance 
In line with previous findings [46, 48], we found that an avatar’s 
appearance can affect the perception of effort during physically 
demanding tasks. Customized avatars resulted in a generally lower 
perception of effort compared to randomly assigned ones. While 
previous work found that an avatar’s level of athleticism [46, 48] or 
the sweaty appearance [45] has an effect on perceptual responses, 
our findings show that customization has also an effect while exercising in VR. 
In contrast to the assumption that customizing avatars could 
increase the Proteus effect, we could not find a higher perception 
of effort when embodying customized avatars with a non-athletic 
appearance compared to randomly assigned ones when holding 
weights. We assume that customizing an avatar that reflects the 
user irrespective of the athleticism increases attachment and motivation. Hence, we hypothesize that participants were more attached 
to the outcome and their performance regarding the perception 
of effort when embodying customized avatars and, in turn, rated 
lower scores than when embodying the randomly assigned avatars. 
These findings are in line with the subjective ratings of experienced 
embodiment and user identification showing higher similarity and 
embodied presence ratings (see Fig. 7) and generally higher embodiment scores across dimensions (see Fig. 6). 
Previous work found that muscular avatars can increase physical 
performance in terms of a higher grip strength [48]. While we also 
found effects of athletic avatars, they could not be observed for 
all tasks (see Table 3). Kocur et al. [50], for example, argued that 
the Proteus effect occurs for a range of activities such as virtually 
rowing. Our study, however, adds that for some tasks avatars’ effects seem to be more effective than for others. While previous 
work revealed that the Proteus effect is avatar-specific, e.g., users 
tend not to behave in line with undesired attributes such as narcissism [36], our work suggests that the Proteus effect can also be 
task-specific. Hence, future studies should investigate what tasks 
benefit more or less from the avatars’ appearance to learn more 
about the phenomenon’s effectivity and its utilization. 
In addition, we show that customized avatars can also improve 
performance in terms of a higher numbers of biceps curls. As customized avatars can positively influence users across different physically demanding tasks, we recommend enabling users to customize 
avatars in immersive fitness applications. While customization options in popular exergames, e.g., RingFit [70], are still limited [22],



<!-- page: 14 -->

Investigating the Impact of Customized Avatars and the Proteus Effect during Physical Exercise in Virtual Reality 
CHI ’25, April 26–May 01, 2025, Yokohama, Japan 
1 
2 
3 
4 
5 
6 
customized randomized 
vrbody 
1 
2 
3 
4 
5 
6 
customized randomized 
mirror
1 
2 
3 
4 
5 
6 
customized randomized 
features 
1 
2 
3 
4 
5 
6 
customized randomized 
agency 
1 
2 
3 
4 
5 
6 
customized randomized 
twobodies 
Figure 6: Mean BRQ questionnaire scores for each subdimension (vrbody, mirror, features, agency, and twobodies). Error bars 
show the standard error of the means. 
1 
2 
3 
4 
5 
6 
customized randomized 
embodied presence 
1 
2 
3 
4 
5 
6 
customized randomized 
similarity 
1 
2 
3 
4 
5 
6 
customized randomized 
wishful 
Figure 7: Mean PIS questionnaire scores for each subdimension (embodied presence, similarity identification, and wishful 
identification). Error bars show the standard error of the means. 
future work should further investigate how more extensive customization features and also the level of athleticism can contribute 
to a lower perception of effort. 
While previous work has already shown that customized avatars 
can improve motivation [12] and performance in exergames [22, 56, 
60], our work is the first that systematically disentangled the effects 
caused by customization and the Proteus effect. The effects of customization suggest that the Proteus effect may thus operate through 
mechanisms of self-identification and perceived control, rather than 
just mimicking the avatar’s characteristics. Hence, this supports 
the notion that perceptual and behavioral changes are triggered by 
changes in self-perception [9] rather than priming effects [4, 83]. 
This shifts the focus from the avatar’s external traits to the user’s internal connection with the avatar [11]. Users’ perceptual responses 
and performance is therefore closely tied to the psychological connection with their avatar rather than just its visual attributes. This 
suggests that instead of solely focusing on traits such as athleticism 
and muscularity, future work should explore to leverage traits that 
resonate with users’ self-concept and increase the psychological 
connection with the avatar [34], e.g., using 3D-scanned avatars 
that align with users’ physical appearance [105]. This is in line 
with Clark [19], who argues that stereotypical appearances can 
be effective, however, could further reinforce stereotypical thinking. The main effect of customization regardless of the avatars’ 
athleticism suggests that designers could consider focusing on useravatar similarity instead of only stereotypical appearances such as 
athleticism. 
−1.0 
−0.5 
0.0 
0.5 
1.0 
customized randomized 
Δ perceived fitness = avatar − real body 
4.0 
4.5 
5.0 
5.5 
6.0 
customized 
randomized 
presence 
Figure 8: Left: Average Δ self-perceived fitness scores of each 
subdimension (fitness, strength, body composition, flexibility, endurance) showing the resemblance of the avatars’ perceived fitness and participants’ actual perceived fitness (positive = avatar is perceived more fit, 0 = equal perceived fitness 
of avatars and participants, negative = avatar is perceived 
less fit). Right: average score of the general presence of the 
IPQ (right). Error bars show the standard error of the means. 
▶ Customized avatars can reduce the perception of effort 
and improve physical performance irrespective of the avatars’ 
athleticism.



<!-- page: 15 -->

CHI ’25, April 26–May 01, 2025, Yokohama, Japan 
Kocur et al. 
5.2 Heart Rate 
Kocur et al. [46] showed that athletic avatars reduced heart rate 
while cycling an ergometer in VR. We extend previous work by 
showing that athletic avatars reduced heart rate responses while 
holding weights, however, only when being customized. Previous 
work explained that the effects on heart rate could originate from 
the different levels of experienced embodiment and identification 
rather than from the visual athleticism of avatars [46, 50]. Accordingly, Navarro et al. [69] also showed that user-avatar similarity 
influenced cardiac frequency while walking on a treadmill. As we 
found that the experienced embodiment and identification is higher 
on average for the customized avatars compared to the randomly 
assigned ones, our results suggest that body ownership and avatar 
identification augmented the effects caused by the avatars’ appearance. Accordingly, participants perceived the customized athletic 
avatars as more fit than the randomized athletic avatars relative 
to their actual fitness level (see Fig. 8). This indicates that avatars 
that were personally created by users were attributed with higher 
physical abilities than randomized ones and can, therefore, explain 
the effects caused by customization. Consistent with the ratings of 
wishful identification (see Fig. 7), participants created a more idealized version of themselves when customizing the athletic avatar, 
indicating a successful manipulation check. These findings imply 
that customizing avatars with idealized physical characteristics 
can augment the physiological effects originating from the Proteus 
effect due to the avatars’ athletic appearance. Besides, correlation 
analyses suggest that a higher self-perceived fitness resulted in a 
lower reduced heart rate. Future work could systematically analyze 
how metrics that objectively quantify participants’ athleticism, e.g., 
using a cooper test to determine physical fitness [64], influence the 
Proteus effect. 
Interestingly, the descriptive statistics suggest that the heart rate 
while embodying athletic avatars is higher compared to non-athletic 
avatars during biceps curls. In line with Kocur and Schwind [54], we 
assume that avatars do not directly control physiological measures 
such as heart rate, but induce a behavioral change and depend 
on the physiological activity. In our study, avatars increased heart 
rate when power and speed are required (e.g., while performing 
biceps curls) and decrease heart rate when endurance is required 
(e.g., while holding weights), suggesting a cognitive mapping and 
an underlying mechanism that controls body functions via motor 
control (e.g., through breathing) [54]. 
In a different context, Slater et al. [97] revealed that participants who embodied an avatar from a third-person perspective 
had a lower heart rate response to a virtual threat compared to a 
first-person perspective. Furthermore, it seems also plausible that 
avatars with visual attributes that fundamentally differ from the 
real self can also influence physiological responses due to novelty 
effects [57]. As the randomly assigned avatars were created by other 
participants with characteristics deviating from the self, embodying them could create a novel and interesting experience raising 
the heart rate. Hence, we assume that customization is the driving 
factor for physiological responses due to avatar embodiment. 
▶ Athletic avatars can reduce heart rate responses while holding weights, however, only when being customized. 
5.3 Design Considerations 
Our findings consolidate previous work [46, 48, 50, 78] indicating that designers and researchers of VR exercise applications can 
use athletic avatars to improve participants’ perception of effort. 
Athletic avatars can be effective in fitness-oriented applications, 
where embodying a muscular, capable character aligns with the 
physical effort and achievement goals of the application. As the 
perception of effort is a barrier to regular physical activity [66], 
making exercise feel less intense without changing the actual intensity can contribute to more effective exergames [65]. Hence, 
athletic avatars can inspire players to push themselves further due 
to a reduced perceived exertion by reinforcing a sense of athleticism 
and competence [62, 63]. 
Our study also revealed that physiological effects caused by 
the Proteus effect can be enhanced using customized avatars with 
an athletic appearance. However, we found that the heart rate 
responses could only be influenced while holding weights — an 
isometric exercise involving the static contraction of a muscle without any active repetitive movement. While Kocur et al. [46] revealed that utilizing an avatar’s athleticism can be advantageous 
for users while cycling, we show that when athleticism and customization are combined during isometric exercises, the exercise 
benefits can be even more impactful. A lower heart rate response 
can help prevent premature fatigue and enhance exercise enjoyment, potentially making it easier for users to adhere to long-term 
fitness routines [66]. For beginners, for example, reducing heart 
rate responses can lower the risk of overexertion, ensuring safety 
and comfort, and make exercise a more appealing and mentally 
beneficial experience [16, 75]. 
Besides utilization, it is important to know how an avatar’s 
appearance affect the basal HR from a research perspective. If psychophysiological effects due to the embodiment of athletic and customized avatars occur, the avatar, therefore, has to be considered in 
the experimental design process. While more research is required 
to better understand avatars’ effects with a broader range of activities, we propose to consider customization options in immersive 
exergames or fitness applications to enhance avatar identification 
and embodiment, with the goal to augment the Proteus effect. 
5.4 Limitations and Future Work 
Even though our immersive customization editor was equipped 
with many options to personalize the avatars, commercial customization editors offer more options for individualization. While 
the results indicate that our options were sufficient to induce different degrees of body ownership and identification, they do not 
encompass the full range of possible avatar customization, e.g., to 
study behavioral traits or more nuanced personality traits. 
Additionally, the study focused solely on short-term physiological and perceptual responses during exercise in VR. The long-term 
effects of using customized avatars, including potential behavioral 
changes or sustained modifications in physical activity levels, were



<!-- page: 16 -->

Investigating the Impact of Customized Avatars and the Proteus Effect during Physical Exercise in Virtual Reality 
CHI ’25, April 26–May 01, 2025, Yokohama, Japan 
Measures 
Tasks 
Customization 
Athleticism 
Customization × Athleticism 
𝐹 (1, 23) 
p 
𝜂2 
𝑝 
𝐹 (1, 23) 
p 
𝜂2 
𝑝 
𝐹 (1, 23) 
p 
𝜂2 
𝑝 
Perceived Effort 
Holding Weights 
5.812 
.024 
.202 
4.663 
.041 
.169 
2.545 
.124 
.100 
Biceps Curls 
0.576 
.455 
.024 
10.599 
.003 
.315 
1.501 
.233 
.061 
Heart Rate 
Holding Weights 
0.311 
.583 
.013 
4.374 
.048 
.160 
5.214 
.032 
.185 
Biceps Curls 
0.366 
.551 
.016 
3.125 
.090 
.120 
0.423 
.522 
.018 
Performance 
Biceps Curls 
5.806 
.024 
.200 
3.575 
.071 
.130 
0.020 
.887 
<.001 
Reaction Wall 
4.103 
.055 
.151 
3.332 
.081 
.127 
2.490 
.128 
.098 
Table 3: Summary of the inferential statistics providing p-values and the corresponding effect sizes (𝜂2 
𝑝 ) for each measure and 
task. Building on prior research, we hypothesized that athletic avatars would lead to a reduced perception of effort [45, 48] and 
lower heart rate responses [46, 50] (H1). Additionally, we hypothesized an interaction effect between customization and avatar 
athleticism on the measures due to body ownership and avatar identification as moderators of the Proteus effect [7, 46, 81](H2). 
We confirm H1 for the perception of effort during holding weights and biceps curls, as well as for the heart rate while holding 
weights. We also confirm H2 for heart rate responses while holding weights. 
not assessed. Future research should explore these long-term impacts to provide a more comprehensive understanding of how 
avatar customization can be optimized for VR exercise applications. In addition, a more diverse participant pool with different 
characteristics, e.g., different levels of athleticism, could provide 
valuable insights into possible moderators of the Proteus effect. 
Furthermore, we focused on avatars with realistically enhanced 
abilities, e.g., after one year of a healthy diet. However, our study 
did not investigate how customizing avatars with super abilities, 
e.g., Superman, influence perceptual and physiological responses. 
Our findings indicate that customizing avatars can influence 
the heart rate while exercising. On the one hand, a reduced heart 
rate can be interpreted as positive when considering it as a physiological reaction to a decreased perception of effort. In this case, 
using customization options in VR exercise applications can be 
seen as beneficial for players. However, an elevated heart could 
also be interpreted as positive when considering it as a measure 
for physical activity [69]. In this case, randomly assigned avatars 
could cause participants to be more physically active, burn more 
calories, and put more effort into the task even if at an unconscious 
level. As both options appear plausible, future work should further 
investigate physiological changes caused by avatars during physically demanding activities to derive conclusive guidelines how to 
utilize avatar customization and the Proteus effect for VR exercise 
systems. 
Another potential limitation is the consistency of the observed 
effects of avatars’ athleticism and customization across different 
tasks. While we could demonstrate significant effects for some tasks, 
such as reduced heart rate caused by athletic avatars for holding 
weights but not for biceps curls, these effects were not observed 
uniformly across all task types. These findings may indicate a potential lack of generalizability of the Proteus effect suggesting that 
the influence of avatar athleticism and customization may depend 
on specific task characteristics. While we aimed to explore different 
physical tasks to cover a broad range of physical abilities, i.e., a 
reaction time task (reaction wall game), an isometric task (holding 
weights) as well as an isotonic task (biceps curls), there is still a 
range of activities that need to be analyzed to learn about the generalization of the Proteus effect. These findings emphasize the need 
for further research to explore the underlying mechanisms driving 
these task-specific effects and to better understand how the Proteus 
effect can consistently influence performance and perception across 
a broader range of activities [50]. 
The experiment and the tasks introduced some accumulation 
of fatigue due to physical activity. Hence, the effects caused by 
customization or avatar athleticism could be influenced by the task 
sequence. It is therefore still unclear if and how the Proteus effect 
is affected by the physical workload users are experiencing during 
avatar embodiment. Consequently, future work could systematically explore the robustness and effect size of avatars’ effects at 
different levels of exhaustion and fatigue. 
6 Conclusion 
In this paper, we investigate the effects of customized and randomly assigned avatars on users’ physical performance as well as 
perceptual and physiological responses during physically demanding tasks in VR. We developed an immersive VR customization 
editor allowing to create individualized avatars while embodying 
them. We then conducted a controlled experiment with 24 participants who played a reaction wall task, performed biceps curls, and 
held weights while embodying athletic or non-athletic avatars that 
were either customized or randomly assigned. We found that embodying athletic avatars resulted in lower heart rates while holding 
weights, however, only when they were customized. Additionally, 
customized and athletic avatars resulted in a lower perception of 
effort while holding weights. In addition, customized avatars increased the number of performed curls irrespective of the avatars’ 
athleticism. 
Overall, we showed that customized avatars can positively affect 
users’ perception of effort, heart rate, and physical performance 
to physical effort. We also replicated findings from previous work 
indicating that athletic avatars can decrease perception of effort 
during physically demanding tasks. Hence, our paper extends prior



<!-- page: 17 -->

CHI ’25, April 26–May 01, 2025, Yokohama, Japan 
Kocur et al. 
research about the Proteus effect by showing that not only athletic 
avatars but also customized avatars can be beneficial for users’ 
physical performance while exercising. In addition, results also 
indicate that customizing avatars can increase the Proteus effect on 
physiological responses while holding weights. While we could find 
the Proteus effect for some tasks, e.g., a reduced heart rate caused 
by athletic avatars for holding weights but not for biceps curls, 
our results may suggest a lack of generalizability of the Proteus 
effect indicating that this phenomenon depends on the task. This 
contradicts prior research postulating that avatars’ effects during 
physical activity translate to a range of activities and adds a new 
perspective on the Proteus effect and its effectivity for certain tasks. 
Future studies can build upon our work to explore further aspects 
such as long-term effects or behavioral changes across different 
activities to deepen our understanding of avatars’ effects. 
References 
[1] Lars L. Andersen, Christoffer H. Andersen, Ole S. Mortensen, Otto M. Poulsen, 
Inger Birthe T. Bjørnlund, and Mette K. Zebis. 2010. Muscle Activation and 
Perceived Loading During Rehabilitation Exercises: Comparison of Dumbbells 
and Elastic Resistance. Physical Therapy 90, 4 (04 2010), 538–549. 
https: 
//doi.org/10.2522/ptj.20090167 
[2] Jonathan Barnes Aristotle et al. 1984. The complete works of Aristotle. Vol. 2. 
Princeton University Press Princeton. 
[3] K. Carrie Armel and V. S. Ramachandran. 2003. Projecting sensations to external 
objects: evidence from skin conductance response. Proceedings of the Royal 
Society of London. Series B: Biological Sciences 270, 1523 (2003), 1499–1506. https: 
//doi.org/10.1098/rspb.2003.2364 
[4] Erin Ash. 2016. Priming or Proteus Effect? Examining the Effects of Avatar 
Race on In-Game Behavior and Post-Play Aggressive Cognition and Affect in 
Video Games. Games and Culture 11, 4 (2016), 422–440. https://doi.org/10.1177/ 
1555412014568870 
[5] Domna Banakou, Raphaela Groten, and Mel Slater. 2013. Illusory ownership of 
a virtual child body causes overestimation of object sizes and implicit attitude 
changes. Proceedings of the National Academy of Sciences 110, 31 (2013), 12846– 
12851. https://doi.org/10.1073/pnas.1306779110 
[6] Domna Banakou, Parasuram D Hanumanthu, and Mel Slater. 2016. Virtual embodiment of white people in a black virtual body leads to a sustained reduction 
in their implicit racial bias. Frontiers in human neuroscience (2016), 601. 
[7] Domna Banakou, Sameer Kishore, and Mel Slater. 2018. Virtually Being Einstein 
Results in an Improvement in Cognitive Task Performance and a Decrease in Age 
Bias. Frontiers in Psychology 9 (2018). https://doi.org/10.3389/fpsyg.2018.00917 
[8] J. Banks. 2018. Avatar, Assembled: The Social and Technical Anatomy of Digital 
Bodies. Peter Lang Publishing, Incorporated. https://books.google.de/books? 
id=VPlbtAEACAAJ 
[9] Daryl J. Bem. 1972. Self-Perception Theory. Advances in Experimental Social 
Psychology 6 (1972), 1–62. https://doi.org/10.1016/S0065-2601(08)60024-6 
[10] Katherine Bessière, A. Fleming Seay, and Sara Kiesler. 2007. The Ideal Elf: 
Identity Exploration in World of Warcraft. CyberPsychology & Behavior 10, 4 
(2007), 530–535. https://doi.org/10.1089/cpb.2007.9994 PMID: 17711361. 
[11] David Beyea, Rabindra (Robby) Ratan, Yiming (Skylar) Lei, Hanjie Liu, Gabriel E. 
Hales, and Chaeyun Lim. 2023. A New Meta-Analysis of the Proteus Effect: 
Studies in VR Find Stronger Effect Sizes. PRESENCE: Virtual and Augmented 
Reality (07 2023), 1–30. https://doi.org/10.1162/pres_a_00392 
[12] Max V. Birk. 2018. Investigating avatar customization as a motivational design strategy for improving engagement with technology-enabled services for 
health. Phd Thesis 4 Research NOT TU/e / Graduation NOT TU/e). University 
of Saskatchewan. 
[13] Max V. Birk, Cheralyn Atkins, Jason T. Bowey, and Regan L. Mandryk. 2016. 
Fostering Intrinsic Motivation through Avatar Identification in Digital Games. In 
Proceedings of the 2016 CHI Conference on Human Factors in Computing Systems 
(San Jose, California, USA) (CHI ’16). Association for Computing Machinery, 
New York, NY, USA, 2982–2995. https://doi.org/10.1145/2858036.2858062 
[14] D Bishop and M Spencer. 2004. Determinants of repeated-sprint ability in welltrained team-sport athletes and endurance-trained athletes. J Sports Med Phys 
Fitness 44, 1 (March 2004), 1–7. 
[15] Blizzard Entertainment. 2004. World of Warcraft. Game [PC]. Blizzard Entertainment, Irvine, USA. 
[16] GA Borg. 1982. Psychophysical bases of perceived exertion. Medicine and science 
in sports and exercise 14, 5 (1982), 377—381. http://europepmc.org/abstract/ 
MED/7154893 
[17] Matthew Botvinick and Jonathan Cohen. 1998. Rubber Hands ’Feel’ Touch that 
Eyes See. Nature 391, 6669 (1998), 756. https://doi.org/10.1038/35784 
[18] CD Projekt RED. 2020. Cyberpunk 2077. Game [PC, Xbox, PS]. CD Projekt, 
Warsaw, Poland. 
[19] Oliver James Clark. 2020. How To Kill A Greek God - A Review, Critique, and 
Meta-Analysis of 14 years of Proteus Effect Research. PsyArXiv (2020), 1–62. 
https://doi.org/10.31234/osf.io/9rbcs 
[20] Jonathan Cohen. 2001. Defining Identification: A Theoretical Look at the Identification of Audiences With Media Characters. Mass Communication and Society 
4, 3 (2001), 245–264. https://doi.org/10.1207/S15327825MCS0403_01 
[21] Giuseppe Coratella, Gianpaolo Tornatore, Stefano Longo, Nicholas Toninelli, 
Riccardo Padovan, Fabio Esposito, and Emiliano Cè. 2023. Biceps Brachii and 
Brachioradialis Excitation in Biceps Curl Exercise: Different Handgrips, Different 
Synergy. Sports 11, 3 (2023). https://doi.org/10.3390/sports11030064 
[22] Sara Czerwonka, Adrian Alvarez, and Victoria McArthur. 2021. One Ring Fit to 
Rule Them All? An Analysis of Avatar Bodies and Customization in Exergames. 
Frontiers in Psychology 12 (2021). https://doi.org/10.3389/fpsyg.2021.695258 
[23] D. Delignières, A. Marcellini, J. Brisswalter, and P. Legros. 1994. Self-Perception 
of Fitness and Personality Traits. Perceptual and Motor Skills 78, 3 (1994), 843–851. 
https://doi.org/10.1177/003151259407800333 PMID: 8084701. 
[24] Lars Donath, Roland Rössler, and Oliver Faude. 2016. Effects of Virtual Reality 
Training (Exergaming) Compared to Alternative Exercise Training and Passive 
Control on Standing Balance and Functional Mobility in Healthy CommunityDwelling Seniors: A Meta-Analytical Review. Sports Medicine 46 (2016), 1293– 
1309. Issue 9. https://doi.org/10.1007/s40279-016-0485-1 
[25] Nicolas Ducheneaut, Ming-Hui Wen, Nicholas Yee, and Greg Wadley. 2009. 
Body and Mind: A Study of Avatar Personalization in Three Virtual Worlds. In 
Proceedings of the SIGCHI Conference on Human Factors in Computing Systems 
(Boston, MA, USA) (CHI ’09). Association for Computing Machinery, New York, 
NY, USA, 1151–1160. https://doi.org/10.1145/1518701.1518877 
[26] H. Henrik Ehrsson. 2007. The Experimental Induction of Out-of-Body Experiences. Science 317, 5841 (2007), 1048–1048. https://doi.org/10.1126/science. 
1142175 
[27] Marc O Ernst and Martin S Banks. 2002. Humans Integrate Visual and Haptic 
Information in a Statistically Optimal Fashion. Nature 415, 6870 (2002), 429–433. 
https://doi.org/10.1038/415429a 
[28] Marc O. Ernst and Heinrich H. Bülthoff. 2004. Merging the senses into a robust 
percept. Trends in Cognitive Sciences 8, 4 (2004), 162–169. https://doi.org/10. 
1016/j.tics.2004.02.002 
[29] Susan T Fiske, Amy J C Cuddy, Peter Glick, and Jun Xu. 2002. A model of (often 
mixed) stereotype content: competence and warmth respectively follow from 
perceived status and competition. Journal of personality and social psychology 
82, 6 (2002), 878–902. https://doi.org/10.1037/0022-3514.82.6.878 
[30] David Halbhuber, Martin Kocur, Alexander Kalus, Kevin Angermeyer, Valentin 
Schwind, and Niels Henze. 2023. Understanding the Effects of Perceived Avatar 
Appearance on Latency Sensitivity in Full-Body Motion-Tracked Virtual Reality. 
In Proceedings of Mensch Und Computer 2023 (Rapperswil, Switzerland) (MuC 
’23). Association for Computing Machinery, New York, NY, USA, 1–15. https: 
//doi.org/10.1145/3603555.3603580 
[31] Beatrice S. Hasler, Bernhard Spanlang, and Mel Slater. 2017. Virtual Race 
Transformation Reverses Racial Ingroup Bias. PLoS ONE 12, 4 (2017), 1–20. 
https://doi.org/10.1371/journal.pone.0174965 
[32] E. T. Higgins. 1987. Self-discrepancy: A theory relating self and affect. Psychological Review 94, 3 (1987), 319–340. https://doi.org/10.1037/0033-295X.94.3.319 
[33] J. M. Hillis, M. O. Ernst, M. S. Banks, and M. S. Landy. 2002. Combining Sensory 
Information: Mandatory Fusion Within, but Not Between, Senses. Science 298, 
5598 (2002), 1627–1630. https://doi.org/10.1126/science.1075396 
[34] Katherine Isbister. 2006. Better Game Characters by Design: A Psychological 
Approach. Morgan Kaufmann Publishers Inc., San Francisco, CA, USA. 
[35] Mads Møller Jensen, Majken Kirkegaard Rasmussen, and Kaj Grønbæk. 2014. 
Design Sensitivities for Interactive Sport-Training Games. In Proceedings of 
the 2014 Conference on Designing Interactive Systems (Vancouver, BC, Canada) 
(DIS ’14). Association for Computing Machinery, New York, NY, USA, 685–694. 
https://doi.org/10.1145/2598510.2598560 
[36] Sun Joo (Grace) Ahn Jessica McCain and W. Keith Campbell. 2018. Is Desirability of the Trait a Boundary Condition of the Proteus Effect? A Pilot Study. Communication Research Reports 35, 5 (2018), 445–455. 
https: 
//doi.org/10.1080/08824096.2018.1531212 
[37] Seung-A Annie Jin. 2010. “I Feel More Connected to the Physically Ideal Mini Me 
than the Mirror-Image Mini Me”: Theoretical Implications of the “Malleable Self” 
for Speculations on the Effects of Avatar Creation on Avatar–Self Connection 
in Wii. Cyberpsychology, Behavior, and Social Networking 13, 5 (2010), 567–570. 
https://doi.org/10.1089/cyber.2009.0243 PMID: 20950182. 
[38] Raine Kajastila, Leo Holsti, and Perttu Hämäläinen. 2016. The Augmented 
Climbing Wall: High-Exertion Proximity Interaction on a Wall-Sized Interactive 
Surface. In Proceedings of the 2016 CHI Conference on Human Factors in Computing 
Systems (San Jose, California, USA) (CHI ’16). Association for Computing Machinery, New York, NY, USA, 758–769. https://doi.org/10.1145/2858036.2858450



<!-- page: 18 -->

Investigating the Impact of Customized Avatars and the Proteus Effect during Physical Exercise in Virtual Reality 
CHI ’25, April 26–May 01, 2025, Yokohama, Japan 
[39] Alexander Kalus, Martin Kocur, Johannes Klein, Manuel Mayer, and Niels Henze. 
2023. PumpVR: Rendering the Weight of Objects and Avatars through Liquid 
Mass Transfer in Virtual Reality. In Proceedings of the 2023 CHI Conference on 
Human Factors in Computing Systems (Hamburg, Germany) (CHI ’23). Association for Computing Machinery, New York, NY, USA, Article 263, 13 pages. 
https://doi.org/10.1145/3544548.3581172 
[40] Maximus D. Kaos, Ryan E. Rhodes, Perttu Hämäläinen, and T.C. Nicholas Graham. 2019. Social Play in an Exergame: How the Need to Belong Predicts 
Adherence. In Proceedings of the 2019 CHI Conference on Human Factors in Computing Systems (Glasgow, Scotland Uk) (CHI ’19). Association for Computing 
Machinery, New York, NY, USA, 1–13. https://doi.org/10.1145/3290605.3300660 
[41] Konstantina Kilteni, Antonella Maselli, Konrad P. Kording, and Mel Slater. 2015. 
Over my fake body: Body ownership illusions for studying the multisensory 
basis of own-body perception. Frontiers in Human Neuroscience 9, MAR (2015). 
https://doi.org/10.3389/fnhum.2015.00141 
[42] Christoph Klimmt, Dorothée Hefner, and Peter Vorderer. 2009. The video 
game experience as "true" identification: A theory of enjoyable alterations of 
players’ self-perception. Communication Theory 19, 4 (2009), 351–373. https: 
//doi.org/10.1111/j.1468-2885.2009.01347.x 
[43] Pascal Knierim, Valentin Schwind, Anna Maria Feit, Florian Nieuwenhuizen, and 
Niels Henze. 2018. Physical Keyboards in Virtual Reality: Analysis of Typing 
Performance and Effects of Avatar Hands, In Proceedings of the 2018 CHI 
Conference on Human Factors in Computing Systems (2018-04-21). Proceedings 
of the 2018 CHI Conference on Human Factors in Computing Systems. https: 
//doi.org/10.1145/3173574.3173919 
[44] Martin Kocur. 2022. Utilizing the Proteus Effect to Improve Performance Using 
Avatars in Virtual Reality. https://epub.uni-regensburg.de/52677/ 
[45] Martin Kocur, Johanna Bogon, Manuel Mayer, Miriam Witte, Amelie Karber, 
Niels Henze, and Valentin Schwind. 2022. Sweating Avatars Decrease Perceived 
Exertion and Increase Perceived Endurance while Cycling in Virtual Reality. 
In Proceedings of the 28th ACM Symposium on Virtual Reality Software and 
Technology (Tsukuba, Japan) (VRST ’22). Association for Computing Machinery, 
New York, NY, USA, Article 29, 12 pages. https://doi.org/10.1145/3562939. 
3565628 
[46] Martin Kocur, Florian Habler, Valentin Schwind, Paweł W. Woźniak, Christian 
Wolff, and Niels Henze. 2021. Physiological and Perceptual Responses to Athletic Avatars While Cycling in Virtual Reality. In Proceedings of the 2021 CHI 
Conference on Human Factors in Computing Systems (Yokohama, Japan) (CHI 
’21). Association for Computing Machinery, New York, NY, USA, Article 519, 
18 pages. https://doi.org/10.1145/3411764.3445160 
[47] Martin Kocur, Alexander Kalus, Johanna Bogon, Niels Henze, Christian Wolff, 
and Valentin Schwind. 2022. The Rubber Hand Illusion in Virtual Reality and 
the Real World - Comparable but Different. In Proceedings of the 28th ACM 
Symposium on Virtual Reality Software and Technology (Tsukuba, Japan) (VRST 
’22). Association for Computing Machinery, New York, NY, USA, Article 31, 
12 pages. https://doi.org/10.1145/3562939.3565614 
[48] Martin Kocur, Melanie Kloss, Valentin Schwind, Christian Wolff, and Niels 
Henze. 2020. Flexing Muscles in Virtual Reality: Effects of Avatars’ Muscular 
Appearance on Physical Performance. In Proceedings of the Annual Symposium 
on Computer-Human Interaction in Play (Virtual Event, Canada) (CHI PLAY ’20). 
Association for Computing Machinery, New York, NY, USA, 193–205. https: 
//doi.org/10.1145/3410404.3414261 
[49] Martin Kocur, Manuel Mayer, Amelie Karber, Miriam Witte, Niels Henze, and 
Johanna Bogon. 2023. The Absence of Athletic Avatars’ Effects on Physiological 
and Perceptual Responses While Cycling in Virtual Reality. In Proceedings of 
the 22nd International Conference on Mobile and Ubiquitous Multimedia (Vienna, 
Austria) (MUM ’23). Association for Computing Machinery, New York, NY, USA, 
366–376. https://doi.org/10.1145/3626705.3627769 
[50] Martin Kocur, Thomas Noack, Valentin Schwind, Johanna Bogon, and Niels 
Henze. 2024. Physiological and Perceptual Effects of Avatars’ Muscularity 
while Rowing in Virtual Reality. In Proceedings of Mensch Und Computer 2024 
(Karlsruhe, Germany) (MuC ’24). Association for Computing Machinery, New 
York, NY, USA, 44–52. https://doi.org/10.1145/3670653.3670654 
[51] Martin Kocur, Daniel Roth, and Valentin Schwind. 2020. Towards an Investigation of Embodiment Time in Virtual Reality. In Mensch und Computer 2020 -
Workshopband, Christian Hansen, Andreas Nürnberger, and Bernhard Preim 
(Eds.). Gesellschaft für Informatik e.V., Bonn. https://doi.org/10.18420/muc2020ws134-339 
[52] Martin Kocur, Philipp Schauhuber, Valentin Schwind, Christian Wolff, and 
Niels Henze. 2020. The Effects of Self- and External Perception of Avatars 
on Cognitive Task Performance in Virtual Reality. In 26th ACM Symposium 
on Virtual Reality Software and Technology (Virtual Event, Canada) (VRST ’20). 
Association for Computing Machinery, New York, NY, USA, Article 27, 11 pages. 
https://doi.org/10.1145/3385956.3418969 
[53] Martin Kocur and Valentin Schwind. 2024. Investigating the Proteus Effect on 
Physiological Responses While Resting in VR. Mensch und Computer 2024 -
Workshopband. https://doi.org/10.18420/muc2024-mci-ws06-215 
[54] Martin Kocur and Valentin Schwind. 2024. Investigating the Proteus Effect on 
Physiological Responses While Resting in VR. Mensch und Computer 2024 -
Workshopband. https://doi.org/10.18420/muc2024-mci-ws06-215 
[55] Harold W Kohl, Cora Lynn Craig, Estelle Victoria Lambert, Shigeru Inoue, 
Jasem Ramadan Alkandari, Grit Leetongin, and Sonja Kahlmeier. 2012. The 
pandemic of physical inactivity: global action for public health. The Lancet 380 
(7 2012), 294–305. Issue 9838. https://doi.org/10.1016/S0140-6736(12)60898-8 
doi: 10.1016/S0140-6736(12)60898-8. 
[56] Jordan Koulouris, Zoe Jeffery, James Best, Eamonn O’Neill, and Christof Lutteroth. 2020. Me vs. Super(Wo)Man: Effects of Customization and Identification 
in a VR Exergame. In Proceedings of the 2020 CHI Conference on Human Factors 
in Computing Systems (Honolulu, HI, USA) (CHI ’20). Association for Computing 
Machinery, New York, NY, USA, 1–17. https://doi.org/10.1145/3313831.3376661 
[57] A. Krekhov, S. Cmentowski, and J. Krüger. 2019. The Illusion of Animal Body 
Ownership and Its Potential for Virtual Reality Games. In 2019 IEEE Conference 
on Games (CoG). 1–8. https://doi.org/10.1109/CIG.2019.8848005 
[58] James R. Lackner. 1988. Some Proprioceptive Influences on the Perceptual 
Representation of Body Shape and Orientation. Brain 111, 2 (04 1988), 281–297. 
https://doi.org/10.1093/brain/111.2.281 
[59] I-Min Lee, Eric J Shiroma, Felipe Lobelo, Pekka Puska, Steven N Blair, and Peter T 
Katzmarzyk. 2012. Effect of physical inactivity on major non-communicable 
diseases worldwide: an analysis of burden of disease and life expectancy. The 
Lancet 380 (7 2012), 219–229. Issue 9838. https://doi.org/10.1016/S0140-6736(12) 
61031-9 doi: 10.1016/S0140-6736(12)61031-9. 
[60] Myungchul Lee, Donghyun Kim, Myungho Lee, and Kyunghun Han. 2024. 
Impact of Customized Content in 3D Virtual Reality Motionless Imagery Exercise through Avatar on Emotional Well-Being, Cognition, and Physiological 
Response. Applied Sciences 14, 7 (2024). https://doi.org/10.3390/app14072724 
[61] Mats Liljedahl, Stefan Lindberg, and Jan Berg. 2005. Digiwall: An Interactive 
Climbing Wall. In Proceedings of the 2005 ACM SIGCHI International Conference 
on Advances in Computer Entertainment Technology (Valencia, Spain) (ACE ’05). 
Association for Computing Machinery, New York, NY, USA, 225–228. https: 
//doi.org/10.1145/1178477.1178513 
[62] Jih-Hsuan Tammy Lin and Dai-Yun Wu. 2021. Exercising With Embodied 
Young Avatars: How Young vs. Older Avatars in Virtual Reality Affect Perceived 
Exertion and Physical Activity Among Male and Female Elderly Individuals. 
Frontiers in psychology 12 (2021). https://doi.org/10.3389/fpsyg.2021.693545 
[63] Jih-Hsuan Tammy Lin, Dai-Yun Wu, and Ji-Wei Yang. 2021. Exercising With 
a Six Pack in Virtual Reality: Examining the Proteus Effect of Avatar Body 
Shape and Sex on Self-Efficacy for Core-Muscle Exercise, Self-Concept of Body 
Shape, and Actual Physical Activity. Frontiers in psychology 12 (2021). https: 
//doi.org/10.3389/fpsyg.2021.693543 
[64] Michael G. Maksud and Kenneth D. Coutts. 1971. Application of the Cooper 
Twelve-Minute Run-Walk Test to Young Males. Research Quarterly. American 
Association for Health, Physical Education and Recreation 42, 1 (1971), 54–59. 
https://doi.org/10.1080/10671188.1971.10615035 
[65] Samuele Marcora. 2016. Can Doping be a Good Thing? Using Psychoactive 
Drugs to Facilitate Physical Activity Behaviour. Sports Medicine 46 (2016), 1–5. 
Issue 1. https://doi.org/10.1007/s40279-015-0412-x 
[66] Samuele Maria Marcora and Walter Staiano. 2010. The limit to exercise tolerance 
in humans: mind over muscle? European Journal of Applied Physiology 109, 4 
(2010), 763–770. https://doi.org/10.1007/s00421-010-1418-6 
[67] Antonella Maselli and Mel Slater. 2013. The building blocks of the full body 
ownership illusion. Frontiers in Human Neuroscience 7 (2013). https://doi.org/ 
10.3389/fnhum.2013.00083 
[68] Natalie L Myers, Jenny L Toonstra, Jacob S Smith, Cooper A Padgett, and Tim L 
Uhl. 2015. Sustained isometric shoulder contraction on muscular strength and 
endurance: A randomized clinical trial. Int J Sports Phys Ther 10, 7 (2015), 
1015–1025. 
[69] Jessica Navarro, Jorge Peña, Ausias Cebolla, and Rosa Baños. 2020. Can Avatar 
Appearance Influence Physical Activity? User-Avatar Similarity and Proteus 
Effects on Cardiac Frequency and Step Counts. Health Communication (2020), 
1–8. https://doi.org/10.1080/10410236.2020.1834194 
[70] Nintendo EPD. 2019. Ring Fit Adventure. Nintendo Switch. Nintendo, Kyoto, 
Japan. 
[71] Jean-Marie Normand, Elias Giannopoulos, Bernhard Spanlang, and Mel Slater. 
2011. Multisensory Stimulation Can Induce an Illusion of Larger Belly Size in 
Immersive Virtual Reality. PLoS ONE 6, 1 (2011), 1–11. https://doi.org/10.1371/ 
journal.pone.0016128 
[72] Kristine L Nowak and Jesse Fox. 2018. Avatars and computer-mediated communication: a review of the definitions, uses, and effects of digital representations. 
Review of Communication Research 6 (2018), 30–53. https://doi.org/10.12840/ 
issn.2255-4165.2018.06.01.015 
[73] Karin Olsson, Jane Salier Eriksson, Hans Rosdahl, and Peter Schantz. 2020. Are 
heart rate methods based on ergometer cycling and level treadmill walking 
interchangeable? PLOS ONE 15, 8 (08 2020), 1–18. https://doi.org/10.1371/ 
journal.pone.0237388 
[74] Sofia Adelaide Osimo, Rodrigo Pizarro, Bernhard Spanlang, and Mel Slater. 
2015. Conversations between self and self as Sigmund Freud - A virtual body



<!-- page: 19 -->

CHI ’25, April 26–May 01, 2025, Yokohama, Japan 
Kocur et al. 
ownership paradigm for self counselling. Scientific Reports 5 (2015), 1–14. https: 
//doi.org/10.1038/srep13899 
[75] Benjamin Pageaux. 2014. The Psychobiological Model of Endurance Performance: An Effort-Based Decision-Making Theory to Explain Self-Paced 
Endurance Performance. Sports Medicine 44, 9 (01 Sep 2014), 1319–1320. 
https://doi.org/10.1007/s40279-014-0198-2 
[76] Sung Wook Park, Michael Brenneman, William H Cooke, Alberto Cordova, and 
Donovan Fogt. 2014. Determination of Anaerobic Threshold by Heart Rate or 
Heart Rate Variability using Discontinuous Cycle Ergometry. Int J Exerc Sci 7, 1 
(Jan. 2014), 45–53. https://pmc.ncbi.nlm.nih.gov/articles/PMC4831896/. 
[77] G. Parrinder. 1997. Avatar and Incarnation: The Divine in Human Form in the 
World’s Religions. Oneworld Publications. https://books.google.de/books?id= 
VkV5AAAAMAAJ 
[78] Jorge Peña, Jeffrey T. Hancock, and Nicholas A. Merola. 2009. The priming 
effects of avatars in virtual settings. Communication Research 36, 6 (2009), 
838–856. https://doi.org/10.1177/0093650209346802 
[79] Valeria I. Petkova and H. Henrik Ehrsson. 2008. If I were You: Perceptual Illusion 
of Body Swapping. PLoS ONE 3, 12 (2008), 1–9. https://doi.org/10.1371/journal. 
pone.0003832 
[80] Jorge Peña and Eunice Kim. 2014. Increasing exergame physical activity through 
self and opponent avatar appearance. Computers in Human Behavior 41 (2014), 
262–267. https://doi.org/10.1016/j.chb.2014.09.038 
[81] Anna Samira Praetorius and Daniel Görlich. 2020. How Avatars Influence User 
Behavior: A Review on the Proteus Effect in Virtual Environments and Video 
Games. In Proceedings of the 15th International Conference on the Foundations of 
Digital Games (Bugibba, Malta) (FDG ’20). Association for Computing Machinery, 
New York, NY, USA, Article 49, 9 pages. https://doi.org/10.1145/3402942.3403019 
[82] Andrew K. Przybylski, Netta Weinstein, Kou Murayama, Martin F. Lynch, and 
Richard M. Ryan. 2012. The Ideal Self at Play: The Appeal of Video Games 
That Let You Be All You Can Be. Psychological Science 23, 1 (2012), 69–76. 
https://doi.org/10.1177/0956797611418676 PMID: 22173739. 
[83] Rabindra Ratan, David Beyea, Benjamin J. Li, and Luis Graciano. 2019. Avatar 
characteristics induce users’ behavioral conformity with small-to-medium effect 
sizes: a meta-analysis of the proteus effect. Media Psychology 3269 (2019). 
https://doi.org/10.1080/15213269.2019.1623698 
[84] Rabindra Ratan and Young June Sah. 2015. Leveling up on stereotype threat: 
The role of avatar customization and avatar embodiment. Computers in Human 
Behavior 50 (2015), 367–374. https://doi.org/10.1016/j.chb.2015.04.010 
[85] Rabindra A Ratan and Michael Dawson. 2015. When Mii Is Me: A Psychophysiological Examination of Avatar Self-Relevance. Communication Research 43, 8 
(2015), 1065–1093. https://doi.org/10.1177/0093650215570652 
[86] René Reinhard, Khyati Girish Shah, Corinna A. Faust-Christmann, and Thomas 
Lachmann. 2020. Acting your avatar’s age: effects of virtual reality avatar 
embodiment on real life walking speed. Media Psychology 23, 2 (2020), 293–315. 
https://doi.org/10.1080/15213269.2019.1598435 
[87] Minjin MJ Rheu, Rabindra Ratan, Young June Sah, Leticia Cherchiglia, and 
Tom Day. 2022. Jogging in Your Avatar’s Footsteps: The Effects of Avatar 
Customization and Control Intuitiveness. Frontiers in Virtual Reality 3 (2022). 
https://doi.org/10.3389/frvir.2022.873689 
[88] Martin Riemer, Jörg Trojan, Marta Beauchamp, and Xaver Fuchs. 2019. The 
rubber hand universe: On the impact of methodological differences in the rubber 
hand illusion. Neuroscience & Biobehavioral Reviews 104 (2019), 268–280. https: 
//doi.org/10.1016/j.neubiorev.2019.07.008 
[89] Roberta E. Rikli and C. Jessie Jones. 2012. Development and Validation of 
Criterion-Referenced Clinically Relevant Fitness Standards for Maintaining 
Physical Independence in Later Years. The Gerontologist 53, 2 (05 2012), 255–267. 
https://doi.org/10.1093/geront/gns071 
[90] Daniel Roth and Marc Erich Latoschik. 2020. Construction of the Virtual Embodiment Questionnaire (VEQ). IEEE Transactions on Visualization and Computer 
Graphics 26, 12 (2020), 3546–3556. https://doi.org/10.1109/TVCG.2020.3023603 
[91] Richard M. Ryan, C. Scott Rigby, and Andrew Przybylski. 2006. The Motivational 
Pull of Video Games: A Self-Determination Theory Approach. Motivation and 
Emotion 30, 4 (01 Dec 2006), 344–360. https://doi.org/10.1007/s11031-006-9051-8 
[92] Nouran Sadek, Passant Elagroudy, Ali Khalil, and Slim Abdennadher. 2022. The 
Superhero Pose: Enhancing Physical Performance in Exergames by Embodying 
Celebrity Avatars in Virtual Reality. In Nordic Human-Computer Interaction 
Conference (Aarhus, Denmark) (NordiCHI ’22). Association for Computing Machinery, New York, NY, USA, Article 1, 11 pages. 
https://doi.org/10.1145/ 
3546155.3546707 
[93] Maria V. Sanchez-Vives, Bernhard Spanlang, Antonio Frisoli, Massimo Bergamasco, and Mel Slater. 2010. Virtual hand illusion induced by visuomotor correlations. PLoS ONE 5, 4 (2010), 1–6. https://doi.org/10.1371/journal.pone.0010381 
[94] Thomas Schubert. 2003. The sense of presence in virtual environments: A 
three-component scale measuring spatial presence, involvement, and realness. 
Zeitschrift für Medienpsychologie 15 (04 2003), 69–71. https://doi.org/10.1026/ 
/1617-6383.15.2.69 
[95] Valentin Schwind, Pascal Knierim, Nico Haas, and Niels Henze. 2019. Using 
presence questionnaires in virtual reality. Proceedings of the 2019 CHI Conference 
on Human Factors in Computing Systems (2019), 1–12. https://doi.org/10.1145/ 
3290605.3300590 
[96] Valentin Schwind, Pascal Knierim, Cagri Tasci, Patrick Franczak, Nico Haas, 
and Niels Henze. 2017. "These Are Not My Hands!": Effect of Gender on the 
Perception of Avatar Hands in Virtual Reality. In Proceedings of the 2017 CHI 
Conference on Human Factors in Computing Systems (Denver, Colorado, USA) 
(CHI ’17). ACM, New York, NY, USA, 1577–1582. https://doi.org/10.1145/3025453. 
3025602 Honorable Mention Award. 
[97] Mel Slater, Daniel Pérez Marcos, Henrik Ehrsson, and Maria Sanchez-Vives. 
2008. Towards a Digital Body: The Virtual Arm Illusion. Frontiers in Human 
Neuroscience 2 (2008), 1–8. https://doi.org/10.3389/neuro.09.006.2008 
[98] Mel Slater, Bernhard Spanlang, Maria V. Sanchez-Vives, and Olaf Blanke. 2010. 
First Person Experience of Body Transfer in Virtual Reality. PLoS ONE 5, 5 
(2010), 1–9. https://doi.org/10.1371/journal.pone.0010564 
[99] Alistair Raymond Bryce Soutter and Michael Hitchens. 2016. The relationship 
between character identification and flow state within video games. Computers 
in Human Behavior 55 (2016), 1030–1038. https://doi.org/10.1016/j.chb.2015.11. 
012 
[100] T. L. Taylor. 2002. Living Digitally: Embodiment in Virtual Worlds. Springer 
London, London, 40–62. https://doi.org/10.1007/978-1-4471-0277-9_3 
[101] Manos Tsakiris and Patrick Haggard. 2005. The Rubber Hand Illusion Revisited: 
Visuotactile Integration and Self-attribution. Journal of Experimental Psychology: 
Human Perception and Performance 31, 1 (2005), 80–91. https://doi.org/10.1037/ 
0096-1523.31.1.80 
[102] Jan Van Looy, Cédric Courtois, and Melanie De Vocht. 2010. Player Identification in Online Games: Validation of a Scale for Measuring Identification in 
MMORPGs. In Proceedings of the 3rd International Conference on Fun and Games 
(Leuven, Belgium) (Fun and Games ’10). Association for Computing Machinery, 
New York, NY, USA, 126–134. https://doi.org/10.1145/1823818.1823832 
[103] J. P. Verma. 2018. Repeated Measures Design for Enhancing Precision in Sports 
Research. John Wiley & Sons, Ltd, 1–22. https://doi.org/10.1002/9781118445112. 
stat07960 
[104] Rolf von Eckartsberg. 1989. The Social Psychology of Person Perception and 
the Experience of Valued Relationships. Springer US, Boston, MA, 137–154. 
https://doi.org/10.1007/978-1-4615-6989-3_9 
[105] Stephan Wenninger, Jascha Achenbach, Andrea Bartl, Marc Erich Latoschik, 
and Mario Botsch. 2020. Realistic Virtual Humans from Smartphone Videos. 
In Proceedings of the 26th ACM Symposium on Virtual Reality Software and 
Technology (Virtual Event, Canada) (VRST ’20). Association for Computing 
Machinery, New York, NY, USA, Article 29, 11 pages. https://doi.org/10.1145/ 
3385956.3418940 
[106] WHO. 2022. Physical activity. https://www.who.int/news-room/fact-sheets/ 
detail/physical-activity. 
[107] Jacob O. Wobbrock, Leah Findlater, Darren Gergle, and James J. Higgins. 2011. 
The Aligned Rank Transform for Nonparametric Factorial Analyses Using Only 
Anova Procedures. In Proceedings of the 2011 CHI Conference on Human Factors 
in Computing Systems (Vancouver, BC, Canada) (CHI ’11). ACM, New York, NY, 
USA, 143–146. https://doi.org/10.1145/1978942.1978963 
[108] Nick Yee and Jeremy Bailenson. 2007. The Proteus Effect: The Effect of Transformed Self-representation on Behavior. Human Communication Research 33, 3 
(2007), 271–290. https://doi.org/10.1111/j.1468-2958.2007.00299.x 
[109] Nick Yee and Jeremy N. Bailenson. 2009. The difference between being and 
seeing: The relative contribution of self-perception and priming to behavioral 
changes via digital self-representation. Media Psychology 12, 2 (2009), 195–209. 
https://doi.org/10.1080/15213260902849943 
[110] Hsin-Yen Yen and Huei-Ling Chiu. 2021. Virtual Reality Exergames for Improving Older Adults’ Cognition and Depression: A Systematic Review and MetaAnalysis of Randomized Control Trials. Journal of the American Medical Directors 
Association 22, 5 (2021), 995–1002. https://doi.org/10.1016/j.jamda.2021.03.009 
[111] Sukkyung You, Euikyung Kim, and Donguk Lee. 2017. Virtually Real: Exploring 
Avatar Identification in Game Addiction Among Massively Multiplayer Online 
Role-Playing Games (MMORPG) Players. Games and Culture 12, 1 (2017), 56–71. 
https://doi.org/10.1177/1555412015581087
