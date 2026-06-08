# Mottelson et al. (2023) - A Systematic Review and Meta-analysis of the Effectiveness of Body Ownership Illusions in Virtual Reality

## Extraction notes
- Source PDF: `Body Ownership illusions.pdf`
- Article: Aske Mottelson, Andreea Muresan, Kasper Hornbaek, Guido Makransky (2023)
- Venue: ACM Transactions on Computer-Human Interaction, 30(5), Article 76
- DOI: 10.1145/3590767
- Page markers are preserved as HTML comments.
- This raw file keeps page text in fenced blocks to reduce accidental mixing between source text and interpretation.
- Verify exact quotations against the original PDF before thesis use.

---


<!-- page: 1 / 42 -->

```text
A Systematic Review and Meta-analysis of the Effectiveness
of Body Ownership Illusions in Virtual Reality


ASKE MOTTELSON, Department of Digital Design, IT University of Copenhagen
ANDREEA MURESAN and KASPER HORNBÆK, Department of Computer Science, University of
Copenhagen
GUIDO MAKRANSKY, Department of Psychology, University of Copenhagen


Body ownership illusions (BOIs) occur when participants experience that their actual body is replaced by a
body shown in virtual reality (VR). Based on a systematic review of the cumulative evidence on BOIs from
111 research articles published in 2010 to 2021, this article summarizes the findings of empirical studies of   76
BOIs. Following the PRISMA guidelines, the review points to diverse experimental practices for inducing
and measuring body ownership. The two major components of embodiment measurement, body ownership
and agency, are examined. The embodiment of virtual avatars generally leads to modest body ownership and
slightly higher agency. We also find that BOI research lacks statistical power and standardization across tasks,
measurement instruments, and analysis approaches. Furthermore, the reviewed studies showed a lack of
clarity in fundamental terminology, constructs, and theoretical underpinnings. These issues restrict scientific
advances on the major components of BOIs, and together impede scientific rigor and theory-building.

CCS Concepts: • Human-centered computing →Virtual reality; User studies; • General and reference
→Surveys and overviews;

Additional Key Words and Phrases: Virtual reality, embodiment, body ownership illusions, systematic review,
meta-analysis

ACM Reference format:
Aske Mottelson, Andreea Muresan, Kasper Hornbæk, and Guido Makransky. 2023. A Systematic Review and
Meta-analysis of the Effectiveness of Body Ownership Illusions in Virtual Reality. ACM Trans. Comput.-Hum.
Interact. 30, 5, Article 76 (September 2023), 42 pages.
https://doi.org/10.1145/3590767


SUMMARY

This systematic review provides a comprehensive assessment of the effects of virtual body manip-
ulations on the experience of owning a virtual body. It presents data from 111 articles with 4,925
participants. The original empirical virtual reality (VR) studies had human participants wear


This research received support from the University of Copenhagen’s Data+ pool, under the project “Quantifying Body
Ownership in Virtual Reality”.
Authors’ addresses: A. Mottelson, Department of Digital Design, IT University of Copenhagen, Rued Langgaards Vej 7,
Copenhagen S DK-2300, Denmark; email: asmo@itu.dk; A. Muresan and K. Hornbæk, Department of Computer Science,
University of Copenhagen, Sigurdsgade 40, Copenhagen N, Denmark; emails: {aam, kash}@di.ku.dk; G. Makransky, Depart-
ment of Psychology, University of Copenhagen, Øster Farimagsgade 2A, Copenhagen K, Denmark; email: gm@psy.ku.dk.
Permission to make digital or hard copies of all or part of this work for personal or classroom use is granted without fee
provided that copies are not made or distributed for profit or commercial advantage and that copies bear this notice and
the full citation on the first page. Copyrights for components of this work owned by others than the author(s) must be
honored. Abstracting with credit is permitted. To copy otherwise, or republish, to post on servers or to redistribute to lists,
requires prior specific permission and/or a fee. Request permissions from permissions@acm.org.
© 2023 Copyright held by the owner/author(s). Publication rights licensed to ACM.
1073-0516/2023/09-ART76 $15.00
https://doi.org/10.1145/3590767


     ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 2 / 42 -->

```text
76:2                                                                        A. Mottelson et al.


head-mounted displays (HMDs), in which a virtual avatar replaced their own body. Reported
measures of embodiment were collected for analysis. The study presents (i) a first comparison of
virtual body replacements on embodiment, (ii) a disentanglement of collection and analysis of sub-
jective embodiment measures, (iii) a field-wide comparison of normalized embodiment constructs,
(iv) exploratory analyses of the factors important for embodiment, and (v) a synthesis of practical
experimental procedures. Results indicated that manipulation of visuo-motor synchrony renders
the largest effect for body ownership (д = 1.09), but that a congruence of appearance, perspective,
visuo-tactile stimuli, and abstraction of the avatar are also effective manipulations. We find that
BOI studies mostly employ non-validated embodiment measures, and that specific embodiment
constructs and questionnaire items originate from the Rubber Hand Illusion (RHI). We also ob-
serve that BOI studies typically have low power, with several conditions accompanied by a modest
number of participants. Of the two main components of embodiment, body ownership and agency,
agency is generally reported to be higher than body ownership (i.e., participants report higher con-
trol of their virtual bodies compared to the belief that the virtual bodies are theirs). Furthermore,
the heterogeneity in effects on agency due to experimental manipulation are substantially higher
for agency than for body ownership (I 2 = 79% vs. I 2 = 17%).
  Our data suggest that tactile congruence compared to visual congruence between the physical
body and the virtual avatar leads to lower body ownership (ΔBodyOwnership = −0.56), yet greater
agency (ΔAдency = 0.66).
  We observe a correlation between the time spent in VR and the agency scores reported, r (32) =
0.31, but less so for body ownership, r (55) = 0.02. We did not find a strong correlation between
participants’ gender and body ownership, comparing ratio of gender with effect sizes, r (75) = 0.10.
Female participants, on a 7-point scale, on average report 0.16 higher body ownership and 0.58
lower agency, compared to male participants. We also find that the presence of virtual mirrors
(д = 0.67) has a limited to negative effect on body ownership compared to studies without any
mirror (д = 0.78). Finally, our review synthesizes the practicalities of conducting BOI studies, such
as the time spent during the phase of embodiment (M = 190 s, SD = 146), the use of questionnaires,
and the experimental designs (58% of studies use a within-participant design); based on these
observations, we suggest ways to improve the science of BOIs.

1  INTRODUCTION
Scientific curiosity in multiple disciplines has long been fueled by the question of how the body
shapes the mind. Influential theories of body–mind connections have been developed in philoso-
phy [44, 117], biology [32], neuroscience [13], and psychology [98]. A central question that these
theories have grappled with is what it takes for someone to experience something as their body,
so-called embodiment. The challenge is that, on the one hand, it is phenomenologically clear that
we experience our body in a particular manner and not just like any other object in the world [110].
Furthermore, the experience of our body is closely related to our experience of the self [25, 45]; it
is, for example, generally not possible to misidentify a part of your body as belonging to someone
else. On the other hand, spelling out what it takes for something to be experienced as embodied
has proven difficult.
  One approach to this question is to separate dimensions of embodiment. Gallagher [43] sug-
gested that the sense of having a body covers at least two separate dimensions. One part is the
feeling of controlling one’s movements; this is largely based on motor control, and hence top-down.
Another part is the feeling that one’s body is the source of sensations; this is largely about inte-
gration of sensory input into a sense of ownership. Moreover, it has long been recognized that the
experience of the location of the self is malleable. For instance, some patients with brain damage
experience seeing a duplicate of their body away from their real body [17]. This suggests that the


ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 3 / 42 -->

```text
Body Ownership Illusions in VR                                                             76:3


position of one’s self in the world is also a component of embodiment. A general model of the
dimensions of embodiment is due to de Vignemont [30], who separated ownership (“this is my
body”) from agency (“it is me who acts”) and self-location (“it is me who is here”). Among these
dimensions, body ownership has received the most attention, perhaps because it has received the
most theoretical work [34] and because it was early and strikingly manipulated in experimental
paradigms [113].
  One such experimental paradigm is the RHI. Botvinick and Cohen [21] showed how synchro-
nous stroking of the hidden hand of a participant and the rubber hand elicited reports of the
rubber hand being experienced as real, while asynchronous strokes did not produce an equiva-
lent response. The RHI is a commonly employed experimental paradigm. The experimental setup,
however, has strict limits for further developing the understanding of body–mind links, due to
constraints the physical rubber hand enforce. To counter the constraints of the RHI, researchers
have used VR technology to study body–mind links. This is achieved through an experimental
procedure where participants experience their body replaced by a virtual body. The real body of
the participant is tracked and its virtual replacement is rendered in real time via an HMD. Usually,
the experience of owning a virtual body creates an illusion that the virtual body is indeed your
body. This has been called the body ownership illusion (BOI).
  Researchers in psychology, neuroscience, and human-computer interaction have explored nu-
merous variants of the BOI. Empirical studies of such variants commonly compare the experience
of embodying a virtual body through consistent sensory information with the experience of incon-
sistent sensory information intended to break the embodiment illusion. Early studies manipulated
the congruence of visual and/or tactile information so that the sensory information (visual, tactile)
received was either synchronous or asynchronous with the virtual rendering (e.g., [165]). Later,
this has been supplemented with creative studies of the cognitive effects of being in a body with
amputations [76], in the body of a child [5], or being an out-group member [137].
  BOIs have numerous applications beyond the study of the relationship between the body and
the mind. Embodying a virtual avatar is an effective paradigm for designing engaging VR interven-
tions that change people’s attitudes and behavior [108, 137]. For instance, a reduction in implicit
racial bias has been found after exposure to an immersive body illusion experience [6, 137]. Sim-
ilarly, a reduction in age bias has been reported following the embodiment of an old avatar [7].
In recent health research, the embodiment of an old avatar was also shown to be effective in an
intervention designed to increase intentions to vaccinate [122, 178]. Virtual embodiment is also an
emerging technology to support motor learning and rehabilitation [54, 62, 176]. Moreover, a large
randomized controlled trial showed that BOIs are effective in the treatment of fear of heights [40].
As consumer-oriented VR equipment is increasingly being adopted, a host of social applications
have emerged (e.g., VRChat,1 Mozilla Hubs,2 Horizon Worlds,3 and Spatial4). These applications of-
fer a variety of social interactions based on embodiment [153]. Finally, the use of full-body tracked
avatars is becoming prominent for commercial VR games (e.g., Guardians,5 and Ready Player Me6).
These applications and studies collectively show the breadth of use cases for BOIs in embodiment
research, health interventions, training, treatment of mental health disorders, communication, and
games.


1vrchat.com.
2hubs.mozilla.com.
3oculus.com/horizon-worlds.
4spatial.io.
5virtualage.io.
6readyplayer.me.


     ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 4 / 42 -->

```text
76:4                                                                        A. Mottelson et al.


   Despite the work just mentioned, an overview of how these variations in virtual bodies actually
influence body ownership is lacking. Thus, we do not know which conflicting sensory information
reduces body ownership, nor by how much. The benefits of understanding such influences are
several:

  — It helps understand which effects are robust. For instance, it has been claimed that embodi-
     ment suffers when experiencing the body in a third-person (3PP) compared to a first-person
      (1PP) perspective; data have been presented that confirms [85] and rejects this assertion [37].
     Our analyses supports that perspective has a strong effect on body ownership and agency.
  — It helps HCI researchers design new virtual experiences and bodies. Work on body-based
      user interfaces is to a large extent informed by understanding the mechanisms involved in
     body ownership [169].
  — It establishes best practices for measuring and collecting data on illusions of body ownership.
      This, in turn, can help researchers standardize measures and perform robust experiments.
  — It identifies future research directions, including understanding the benefits of mirrors in
      establishing body ownership, the influence of gender on agency, and the impact of facial
      animations on feeling embodied in an avatar.

   In BOI research, the analysis of dependent measures is conducted to uncover differences
attributable to a successful BOI (i.e., by showing effects that are not present when the illusion is
broken). In this work, we refer to the experimental condition of owning a virtual body through
consistent sensory information as embodiment, and, conversely, to the experimental conditions
of conflicting sensory information as disembodiment. Understanding the difference between these
is the key to understanding the mechanisms involved in body ownership. This understanding
of disembodiment should not be confused with research on the disownership of limbs [71] (i.e.,
“leaving one’s own body”).
  The purpose of this article is to review illusions of body ownership in VR. Our goal is to conduct
a systematic review of how body ownership is affected by the manipulation of the virtual body. At
the same time, we wish to quantify how well different manipulations affect body ownership. Con-
sequently, we note the type of embodiment and disembodiment implemented, and we quantify the
effects of cross studies of experiencing ownership of particular bodies by comparing embodiment
and disembodiment conditions. Finally, based on the review and meta-analysis, we discuss what
we still need to understand about body ownership in VR.

2 BACKGROUND AND RELATED WORK

Due to advances in consumer-oriented VR technology (such as HTC and Oculus devices) and
body-tracking equipment (from Leap Motion, Oculus, and others), it has become easier to perform
research in this field, resulting in a steady increase in publications on embodiment in VR across the
last decade (2010–2012: 7 articles, 2013–2015: 24 articles, 2016–2018: 43 articles, and 2019–2021: 41
articles). The host of new studies is coupled with many complex decisions in experimental work,
and as such, the increasing publication rate has diverged research practices. So far, these practices
have not been the subject of a systematic review.
  BOI research involves many practical and technical decisions. Researchers will have to decide on
apparatus, sensory stimuli, experimental design, and visual instruments to employ, to name a few.
So far, only anecdotal evidence describes the relative importance of these decisions, both impeding
progress in experimental practices and building field-wide theory. It is additionally unclear to
what extent experimental procedures, such as the presence of mirrors and the duration of the
embodiment induction, influence experimental findings.



ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 5 / 42 -->

```text
Body Ownership Illusions in VR                                                             76:5


  This article presents a systematic review and meta-analysis whereby we summarize empirical
findings across the field of BOI research, synthesize a reliable understanding of virtual embodi-
ment’s effect, and cultivate guidelines for future research in this domain.
  Several earlier reviews have addressed the topic of illusory experiences in VR (e.g., [47]). Some
reviews have specifically addressed BOIs [18, 77, 108, 164, 176], covering such aspects of BOIs as
how to induce body ownership experimentally [164, 167], why BOIs are induced [77], the effects
of BOIs on social cognition [108], and their applications in healthcare [115, 176] and therapy [18].
  More than a decade ago, Slater et al. [164] reviewed evidence from three of their experiments
that showcased the feasibility and impact of various techniques for illusory body ownership. The
authors showed how the ownership of a virtual limb can be induced by means of visuo-tactile
stimulation, visual-motor synchrony, and to some extent through a brain-computer interface. As
an early report of successful body ownership induction using computer equipment (i.e., a data
glove and a projection-based VR) the reported evidence is a cornerstone in the development of
BOI practices. Since then, many studies have been conducted with inspiration taken from the
reported studies.
   Later, Kilteni et al. [77] examined known experimental illusory body ownership procedures,
with or without the aid of computer equipment. Following a synthesis of effective apparatus and
experimental methodology, they distilled the principles for triggering BOIs. As a comprehensive
review of theories, practices, and evidence from experimental findings from illusions of body own-
ership, the work of Kilteni et al. [77] began an important discussion of how and why BOIs are
induced, integrating contemporary embodiment frameworks.
  Focusing specifically on the social cognitive effects of illusory body ownership, Maister et al.
[108] reviewed recent evidence on the role of embodiment in implicit social bias. The authors
posited that illusory ownership of an out-group individual (i.e., with respect to gender, age, or
race) can reduce implicit biases against said group. The review highlighted recent findings related
to embodying avatars with a skin color that differs from that of the participant and the subsequent
impact on attitudes, thus documenting an important social psychological application of BOIs.
  The replacement of bodies in VR is both an effective and flexible manipulation. As an illustra-
tion of the flexibility of BOIs, Won et al. [187] wondered if and how participants would experience
being a bat; for instance by controlling wings with one’s arms. Through two studies, the authors
found that virtual bodies can significantly differ from those of the participant, even if non-human,
suggesting an adaptive body schema. Studies that explore this phenomenon have successfully in-
vestigated experiences of missing or altered limbs [78, 81].
  The reviews above provide clear information on practical recommendations, theoretical ac-
counts, and recent evidence in BOI research. However, large-scale comparisons, and importantly,
meta-analytical estimations of evidence across many BOI studies remain unexplored, beyond
specific applications of BOIs (e.g, healthcare [18, 115, 176]). Consequently, no clear evidence-based
guidelines have been developed for BOI studies. The scientific literature also lacks comparisons
of the effects of commonly used experimental manipulations for studies concerning embodiment
in VR.

3  OBJECTIVES
The concept of body ownership is the most prominent dimension of embodiment and central for
conducting empirical investigations of how the body shapes the mind [77]. A thorough understand-
ing of the theoretical and practical limitations of body ownership is fundamental to improve VR
interfaces [63], with applications for, among other things, entertainment, education, and clinical
purposes [12, 97, 109].



     ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 6 / 42 -->

```text
76:6                                                                        A. Mottelson et al.


  To our knowledge, no prior meta-analytical review of VR and BOIs exists, despite the need for
it, as outlined above. Therefore, we set out to conduct a systematic review and meta-analysis, with
the following five objectives:

   (1) to identify the most effective experimental manipulations for inducing body ownership;
   (2) to investigate the practices employed for measuring subjective embodiment, by examining
      the origins, constructs, items, and statistical treatment of the questionnaires used;
   (3) to describe the fundamental embodiment constructs and estimate their mean scores;
   (4) to identify other factors affecting the strength of the BOI (including gender of participants,
      duration of induction, presence of mirrors); and
   (5) to present commonly employed induction procedures, and study designs related to BOIs,
     with the resulting synthesis serving as a resource to guide future research.


4 METHODS
4.1  Eligibility Criteria and Data Sources

We searched the academic databases ACM Digital Library (727 results), PubMed (19 results), Sci-
enceDirect (633 results), and IEEE Xplore (367 results). We furthermore searched the Frontiers
databases (63 results). These were chosen based on breadth of research areas (computer science,
engineering, health sciences, and general science), and based on recommendations by Gusenbauer
and Haddaway [53] (i.e., principal sources).
  We limited the scope of the search to only include research on BOI in VR, and hence not illu-
sions for mixed reality (MR) technology such as augmented reality (AR). AR renders virtual
computer generated graphics on top of the real world, and hence participants can see their physi-
cal bodies. Although this technology also supports body illusions (e.g., arm extensions [38]), it is
a fundamentally different experience in VR. Illusions in AR have their own set of challenges and
opportunities, which is why findings are not directly comparable with findings from VR.

4.2  Article Identification and Selection
Figure 1 shows a PRISMA-style flowchart for the article selection process [119, 131]. BOI research is
cross-disciplinary. The disparate publication traditions within the contributing fields—principally,
social scientists’ preference for journal publications and technical fields’ preference for conference
proceedings—led us to consider both journals, in such areas as psychology and behavioral science,
and proceedings from conferences in computer science and engineering.
  We searched the relevant research databases (query: (“VIRTUAL  REALITY”)  AND  (“BODY
OWNERSHIP” OR “EMBODIMENT” OR “SELF  PRESENCE”)) across the title, abstract, and full text of
articles written in English published in 2010 through 2022 and identified 1,774 unique articles. We
designed the query to inclusively target all VR research that dealt with embodiment, taking into
consideration that the concepts of body ownership, embodiment, and self presence are sometimes
used interchangeably. Then, we scanned the articles and included those that met the following
criteria:

  — representing original research (this criterion excludes systematic reviews, posters, and
      commentaries),
  — used an HMD (this excludes projection-based VR, smartphone VR, CAVEs, and other less
     immersive media),
  — describing an empirical study with healthy human participants,
  — presenting work in which participants had a human avatar (this excludes work using
     non-humanoid avatars, mannequins and 360-degree video), and
  — measuring some form of embodiment (e.g., body ownership or agency).

ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 7 / 42 -->

```text
Body Ownership Illusions in VR                                                             76:7





 Fig. 1. A PRISMA-style flowchart of the selection of studies for the systematic review and meta-analysis.


  In all, 289 articles appeared to meet these criteria. After reading their full text, we excluded 178
for ultimately not adhering to them. Consequently, the review presented here covers 111 articles,
spanning 11 years of BOI research (see Table 1).
  Our meta-analysis, in turn, included the 92 articles in the corpus that (i) include reporting on
virtual embodiment with a standard avatar (a control condition) and that (ii) report descriptive
statistics for embodiment (e.g., mean, standard deviation, median, or interquartile range) or con-
tain box plots or bar charts from which these can be extracted. Of these, 61 articles experimentally
manipulate embodiment as an independent variable  (e.g., through manipulating appearance,
abstraction, or perspective of the avatar), enabling comparisons of effect sizes across experimental
manipulations.




     ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 8 / 42 -->

```text
76:8                                                                        A. Mottelson et al.



                                                       0.5]
                                         0.9]      1.6]      1.9]                     0.9]                0.7] 3.8] 0.8] 1.0]      0.6]      0.9] 2.7]           1.0] 4.9] 1.9] 3.7]                     1.8] 0.9]      1.8] 2.4]                                                      ownershipCI]                                [−0.9;                                                                                                                                                                                                                                                                                                                                                                                                                                                                    (Continued)                             effect                             [95%           [−0.4;        [−0.2;       [0.6;                             [−0.2;                      [−0.4; [2.0; [−0.1; [−0.1;        [−0.5;        [−0.3; [1.1;               [−0.5; [2.1; [0.2; [1.1;                          [0.7; [−0.3;       [0.5; [1.0;                                Estimates of bodyд    .2   .7 −0.2 1.3          .4        .2 2.9 .4 .4   .0   .3 1.9     .2 3.5 1.1 2.4                1.2 .3    1.2 1.7

                                                                                                                                                      (1.7)                             Agency  estimation(SD)M           (1.4)0.5       (1.6)1.8 (1.4)1.8       (2.3)1.3 (1.5)1.8 (1.9)1.0                                (1.8)1.2          −0.3       (1.8)2.6       (1.4)1.2 (1.5)1.8 (1.3)1.8              (0.7)1.2       (1.3)1.5 (1.4)2.0 (2.1)2.2 (1.7)1.5       (1.0)2.2 (1.4)1.2             (0.8)2.2

                                                                                                          (2.0) (2.4)                                (1.7)                                             (3.0)                                                   (1.6)       (1.6) (1.4) (1.8) (1.6) (1.5) (1.9)                    (2.1) (1.5) (1.0) (1.2) (1.8)              (1.8)       (1.8) (1.5) (2.2) (1.0)       (1.2) (2.1) (0.7) (1.4) (2.1) (2.4)       (1.2) (2.3) (2.1) (1.9) (1.1)     Sample               (SD)              Body  ownership  estimationM       0.4    1.0 1.0 0.8 1.8 1.0 0.8     −1.1 −0.2 0.1 1.2 1.4 1.6 0.4 −0.3    1.5    0.8 1.8 0.6 0.8 −0.8 1.0 0.8 1.1 1.2 1.3 1.1    1.5 0.5 1.0 1.3 1.4
     Entire
  the                                                                                      Incongruency               Abstract                Visuo-motor   Visuo-tactile   Visuo-motor                                                                    Visuo-tactile                                Displace  Displace   Visuo-motor   Perspective                   Visuo-tactile                Perspective  Displace                              Perspective   Visuo-tactile   Visuo-tactile   Visuo-motor                                                         Visuo-motor  Abstract               Appearance  Visuo-motor     Across
                                                      Inductionsec. 60        300 120    300 300 360        300    660            240        180 180   6 150 30        300    180 120 300   20    300      Analysis
   Meta                             Mirror No No Yes Yes Yes Yes Yes Yes Yes No No Yes Yes Yes No No No No Yes Yes No Yes No Yes No Yes Yes No No Yes No Yes No Yes Yes No No Yes
  and
                                                                               Perspective  1PP 1PP 1PP 1PP 1PP 1PP 1PP 1PP 1PP 1PP 1PP 1PP 1PP 1PP 1PP 1PP 1PP  1PP/3PP 1PP  1PP/3PP 3PP  1PP/3PP 1PP 1PP  1PP/3PP  1PP/3PP 1PP 1PP 1PP 1PP 1PP 1PP 3PP 1PP 1PP 1PP 1PP 1PP     Review
                                                                                                                                                                                                              Wide5             3D
                                                   VR920 SX111 SX111 SX111 SX111 SX111    DK2              SX111 SX111       SX111    DK2 SX111    DK2 SX60              SX111 DK2 SX111 Labs              SX111    DK2    DK2            CV1        Systematic                                                                  Rift                     Rift      Rift Rift      Rift Rift      Rift           Rift           Rift                Rift Viewer Rift                Rift                                    Vive iWear nVisor nVisor nVisor nVisor nVisor Vive      Vive         nVisor nVisor         nVisor                nVisor                nVisor      Vive nVisor         nVisor           Vive nVisor HMZ-T1                Vive Vive Vive  the               HMD  HTC Vuzix NVIS NVIS NVIS NVIS NVIS HTC Oculus HTC    VisuaStimDigital NVIS NVIS Oculus NVIS Oculus Oculus NVIS Oculus Oculus Nvis Oculus HTC NVIS Oculus NVIS  Fakespace Oculus HTC NVIS Sony Oculus  Virtual Oculus HTC HTC HTC Oculus
  for
                 M/F   13/5 17/21 112/75 21/23 18/18 21/25 0/90 30/0 0/16 34/30 9/16 10/21 4/8 0/32 7/17 15/4 15/29 15/16 21/19 40/8 45/34 0/43 12/4 16/16 12/24 32/0 10/10 20/16 8/8 0/20 21/19 0/32 20/16 35/26 30/10 6/14 7/17 20/22       Variables                      Gender
                                                Subjects Total 18 38 187 44 36 46 90 30 16 65 25 31 12 32 24 19 44 31 40 48 79 43 16 32 36 32 20 36 16 20 40 32 36 61 40 20 24 42
       Collected  1.                                  Studies 1 1 2 1 1 2 2 1 1 1 1 1 1 1 1 1 1 1 1 1 2 1 1 1 1 1 1 1 1 1 3 1 2 2 1 1 1 1
    Table                   Year   2019 2016 2014 2014 2017 2013 2016 2018 2018 2020 2014 2016 2013 2017 2019 2018 2019 2019 2020 2017 2013 2014 2018 2014 2018 2020 2010 2017 2019 2018 2015 2017 2013 2018 2017 2018 2018 2020
                                                                                                                                                                                   [56]                                                                                     [14]                                                                                                                   [26]                                                                                                                                                                [49]                                                                                                                                       [31]                                                                                                                                       al.                                  [4]                                                                                                                                                                     [50]                                                                                                                                                 [39]                                                                al.                                                                                                                                  [46]                                                                                      al.                                                                                          et                                                                                                                        al.                                                                                [11]                                  al.                                      [8]                                          [9]                                                                                                                           al.                                                         et                                                                                                 al.                                                                                et                                                                                                                                       Rosa                       et                              [3]                                                                 et                                                                   la                                           et [16]                                                                                                                                                      [41]                                                                                                                                                                                                  [61]                                                                                  et [51]                                                                                                                                                                              [52]                                                                                                                                                                                                                         Müller                                                                                                                             [28]                                             [5]                                                 [6]                                                     [7]                                                                                                                                            [37]                                                                           [10]                              al.                                                                                                    [22]                                                                                                         [23]                                                                                               [20]                                                                            Slater                                                                                   Slater                                                                   de                                                                    al.                           [2]                                                                                                                                                           [42]                                                                                                                al.                                                                                                                                                                                             [58]                                                                                                                                                  al.                                                                                                                               al.                                                                                                                                   al.                    et                                                                                              al.                                             al.                                                 al.                                                     al.                                                                                                              [24]                                                                                                         al.                                                                                                                        [27]                                                                                                                                            Kaufman                                                        al.                                                                           al.                                                                               al.                                             et                                                                       al.                                                                                                                                                                                        [57]                                                                                                             and                                                                                                                                                                                                                           [66]                                                                                                                                                                                                            [68]                                                                                                                                                                                                                 [69]                                                                                                                                                                                                                      [67]                                                                           et                           al.                                                                                     et                                                                                       et                                                                                                                    al.                                                                                                                                              al.                                                                                                 et [65]                                                              et                                      and                                          and                              et                                 et                                   et                                                                                                     and                                                                      et                                      et                                                                                  al.                                                                                          al.                                                  et                                                    et                                                et                                                                                                                                          al.                                                                                                                                                                    al.                                                                                                                                                         al.                                                                                                                                                             al.                                                                                                                                                                 al.                                                                                                                                                                                                                                   Debarba                  et                                                            and                                                                             et                                                                                               et                                                                                                                                                     al.                                                       et                                                            et                                                                                            et                                                                                                             et                                                                                                      et                                                                                                         et                                                                                                           et
                                                                                                    et                                                  Article    Abtahi  Alimardani    Aymerich-Franch  Banakou  Banakou  Banakou  Banakou  Banakou  Barberia Barbot    Bekrater-Bodmann  Bergstrøm  Borland  Bourdin  Bourdin Bovet    Brugada-Ramentol Burin  Christofi Galvan  Dobricki  Falconer  Feuchtner  Friedman Fusaro    Gonzalez-Liencres    González-Franco  Grechuta  Grechuta     Hamilton-Giachritsis Hara Hasler  Heydrich Jun Jung Jung Jung Jung




ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 9 / 42 -->

```text
Body Ownership Illusions in VR                                                             76:9



                                                    0.6]
                                          0.9] 1.0]           0.6] 1.9]      2.2]      0.8] 1.8] 3.2] 4.7] 0.7] 1.1] 1.6]      2.0]           0.6]           1.1] 1.8]           1.1] 0.3]      1.0]           1.7] 0.9] 2.1]                                                                                                                                                                                                         1.4]                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               (Continued)                                                              ownershipCI]                      [−1.1;                                  effect                                [95%        [−0.1; [−0.1;               [−0.6; [0.9;       [0.6;        [−0.6; [0.2; [1.6; [2.4; [−0.6; [−0.1; [−0.0;       [0.4;               [−0.6;               [−0.8; [0.5;               [−0.3; [−0.1;        [−0.5;       [0.1; [0.4; [−0.3; [0.3;                                        Estimates of bodyд   .4 .5 −0.2   .0 1.4    1.4   .1 1.0 2.4 3.6 .1 .5 .8    1.2     .0     .1 1.1     .4 .1   .2   .8 1.0 .3 1.2

                                                           (1.9)                                                                     (1.6)                                  Agency  estimation(SD)M         (0.8)2.4 −0.2                                (2.0)2.3       (2.2)1.6 (2.0)0.8 (1.1)2.2 (1.0)2.3 −0.7                                (1.4)2.1 (1.9)1.1                          (1.8)0.0              (1.7)1.7                          (1.4)1.3       (1.6)2.0

                                                           (1.6) (2.3)                                                               (1.4)                                      (2.7)                                                         (2.8)                          (SD)        (1.9)                    (1.9) (1.5)       (2.0)       (1.9) (1.5) (1.9) (1.0)       (1.9) (2.0)       (1.4) (1.7) (2.5)       (1.1) (1.8) (1.6) (1.9) (1.8) (1.5) (2.7) (2.1)              (1.9) (1.8) (1.6) (1.6) (1.6)                  Body  ownership  estimationM     0.6 −0.3 −0.5    0.0 1.2    1.1    0.8 1.2 1.0 1.9 −0.3 0.5 0.7    1.4 0.5 1.1 −0.2 1.7 0.8 1.2 1.0 0.0 1.0 0.4 0.3     −0.6 0.8 0.5 1.4 1.2 1.0
                                                                                                 Incongruency                Visuo-motor   Visuo-motor   Visuo-tactile             Invisible   Visuo-motor               Appearance                Visuo-motor   Perspective   Visuo-motor   Visuo-motor  Invisible  Abstract   Visuo-motor               Appearance                        Invisible                              Visuo-motor   Perspective                              Visuo-motor  Appearance                Visuo-motor                Visuo-motor  Abstract  Abstract  Visuo-motor
                                                              Inductionsec.             60   30 60            300        120 120 300        300     60 30 10        120 60    300 150 240   30 300
                                                 Mirror No Yes No No Yes Yes Yes Yes Yes Yes Yes Yes No No No Yes No No No No Yes Yes No No No No No No Yes Yes No No Yes No No Yes Yes

                                                  ±ϕ
             Continued                                                                                         Perspective 1PP 1PP 1PP 1PP 1PP 1PP 1PP 1PP 1PP 1PP 1PP  1PP/3PP 3PP  1PP/3PP 1PP 1PP 1PP  eye-height 1PP 1PP 1PP 1PP 1PP 1PP  1PP/3PP  1PP/3PP  1PP/3PP 1PP 1PP 1PP 1PP 3PP 1PP 1PP 1PP 1PP 1PP
   1.
       Table                         60                                                                                                                                                                         Wide5                                                                                                             SX111 SX111                                                                 SX111 SX111                                                                         DK2                                                                                                                                                                  DK2                            DK2    DK2                                                                                DK2                                                  DK2                                                                            Pro                                                                                        Pro                                                                                                                          SX60                          SX111 SX111 SX111 SX111 DK2                               Labs    Pro                                     Rift Rift Rift                zSight Rift                          Rift      Rift Rift           Rift Rift                               Rift Rift       Quest Rift Rift           Rift      Rift                                                                              nVisor nVisor           Vive Vive Vive nVisor nVisor      Vive           Vive nVisor           Vive Vive nVisor nVisor nVisor nVisor           Vive                Vive           Vive
                        HMD Oculus Oculus Oculus NVIS NVIS  Sensics Oculus HTC HTC HTC NVIS NVIS Oculus HTC Oculus Oculus HTC Nvis Oculus Oculus HTC HTC NVIS NVIS NVIS NVIS Oculus Oculus HTC Oculus Oculus Oculus HTC  Fakespace Oculus HTC Oculus
                                         GenderM/F 10/12 9/25 0/59 36/14 17/19 20/20 16/24 32/0 15/15 12/12 13/19 8/20 50/0 51/3 20/23 9/11 23/3 27/27 14/1 12/8 24/0 26/49 0/30 0/24 39/33 12/22 24/0 44/15 47/41 255/20 12/4 6/9 60/0 22/0 11/11 63/28 22/0
                                                       Subjects Total 22 34 59 50 36 40 40 32 30 24 32 28 50 54 43 20 26 54 15 20 24 75 30 24 72 34 24 59 88 282 16 15 60 22 22 91 22
                                                         Studies 1 1 1 1 1 1 1 1 1 1 2 1 3 3 1 1 2 1 1 1 1 1 1 1 3 3 1 2 3 1 1 1 1 1 1 1 2

                                Year 2019 2020 2016 2012 2013 2016 2020 2020 2020 2021 2015 2016 2018 2020 2017 2017 2020 2011 2016 2019 2019 2018 2013 2015 2013 2014 2018 2020 2017 2021 2020 2018 2020 2011 2019 2020 2015
                                                                                                                                                                                                                            [120]
                                                                                                                                                                                                   [113] [114]                                          [73]                                                                                       [86]                                                                                            [85]                                                                                                                                                                                                                                  [122]                                                                                                                [91]                                                                                                                                                                                                                                                           [126]                                                                                                                                                                                                                [116]                                                                                                                                                                                                                                                                                                                    Hornbæk                                al.                                     [72]                                                                                                                                                                                       [112]                                                                                                                                                                                             [111]                                                                 al.                                                                     al.                                                                                                                                                                                                                                         [123]                                                                                                                                        al.                                                                                                                                                                                                                                                                 [128]                                                                                                                                                                                                                                                                        [129]                                                                                                                                                              [100]                                                                                                                                                                                                                                                     [125]                                                                                    al.                                                    [79]                                                         [75]                                                              [76]                                                                                                                                                                                 [104]                                                                                                                                                       al.                                                                                                 [87]                                                                                                      [88]                                                                                                                          [96]                                                                                                                                                                                                                                                                              [130]                                                                                                                             al.                                                                                                                                                                                                                                           Slater                                                                                                                                                                                                                                                  Slater                                                                        [84]                                                                             [83]                                                                                  [82]                                                                                                                                                                           [103]                     et [74]                                                                                                           [89]                                                                                                                                                                                                                                               [124]                            al.                                                                                                                                                                                                                      [118]                                           et                                              et                                                                                                                                    and                                                                                           et                                                                                                              al.                                                                                                                  al.                                                                                                                                            al.                                                                   [80]                                                                                                                                                          al.                                                                                                                                                              al.                                                                                                    et                                                                                                                                                   al.                                                                                   et                                       al.                                           al.                                               al.                                                                                                          al.                                                                         al.                                                                            al.                                                                                           al.                                                                                                                                                                  al.                                                        et [93]                                   al.                                                                                                                                                                    [101]                                                      al.                                                          al.                                                             al.                                                                                                      al.                   et                                                                                al.                                                                                                                                               al.                                                                                                                                al.                                                                                                                               Jörg                                                                         et                                                                            et                                                                                             et                                                                                                                     and                                                                                                                         and                                                                                                       et                                                                                                         et                                                                                                  et                          et                             et                               et                                                                       et                                                  al.                                                et                                                   et                                                             et                                                                                                            et                        et                                    et                                      et                                         et                                                                                        al.                                                                    et                                                                                                   al.                                                     et                                                                                                et                                                                                      et
                                  et                                                          et                                                                                               and                                                                  et                                                         Article  Karnath  Keenaghan Keizer  Kilteni  Kilteni  Kilteni Kim Kocur Kocur Kocur  Kokkinara  Kokkinara Kondo Kondo Kong  Latoschik Lee Leyrer Lin Lin Lopez Lugrin  Martini  Martini  Maselli  Maselli  Medeiros Mine  Mottelson  Mottelson  Nataraj Nesti Neyret  Normand Ogawa Ogawa Osimo




     ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 10 / 42 -->

```text
76:10                                                                       A. Mottelson et al.



                                                                                                                         0.5]
                                          1.1]                                                                                                                                                  1.4]      1.8]           1.1]                                                                                                 1.5]                1.1]                                                              1.0]           1.0]      2.0]                                                                                                                                                                                                        0.9] 1.8]      0.5]      estimates                                                         1.3]                                                                                                                                                                                       1.5]                                                                                            1.6]                                              ownershipCI]                                                                                                                                                                            [−0.6;      0.8]                        effect                         [95%                  [−0.4;              [0.3; [−0.4;               [−0.4;       [1.1; [0.2; [0.6;                      [−0.1;              [0.1;               [−0.9;       [0.6;               [−0.1;          [0.3;                  [−0.1; [1.0;        [−0.4;                        Estimates of bodyд       .4     .8 .3     .3    1.5 .9 1.1        .5 −0.0   .4     .3    1.2     .5    .9       .4 1.4   .1                                                                                                                                                                                                                                                                                        agency
                                                                                                                                            and
                                                                                                                         (1.6)                        Agency  estimation(SD)M                 (2.0)0.2                    (2.0)0.1       (1.2)1.2              (2.5)1.0 (2.9)0.0 −0.6                          (1.8)0.6 (1.3)2.0       (2.3)1.5 (1.4)1.1       (1.7)1.0       (1.2)1.5                       (1.3)1.8                 (1.6)1.1 (1.0)1.8 (0.6)1.6 (1.6)1.7                                                                                                                                                                                                                                                                                                                                                                                                                                    ownership
                                                    (2.0)              (1.7) (2.0)                                                               (2.4)                                                                               (1.0)    (1.7)              (1.5)                    (SD)          (1.7)                                      (1.7) (1.7)       (2.1) (2.9) (1.6)                          (1.8) (1.3) (1.6) (2.3) (1.6) (2.7) (1.7) (1.7) (2.3)       (1.6)                          (3.3) (1.7)       (0.7) (1.9)  body           Body  ownership  estimationM       1.5 −0.5          −0.7 −0.1    0.0 0.4    1.5 0.8 1.4               −0.6 0.2 1.0 1.0 0.7 0.6 0.7 0.7 0.8 1.0    1.8        −0.1   −0.3 1.2 0.5 −0.1 1.1 1.2
                                                                                                                                            The
                                                                                                                                                                                                                                                                                                                                                                                                                                    variable.                                                                            Incongruency                                Appearance                                   Visuo-tactile   Visuo-motor                              Visuo-motor            Abstract   Perspective   Visuo-motor                                                   Visuo-tactile   Visuo-motor            Abstract                              Visuo-motor                Visuo-motor                              Visuo-motor                       Perspective                                    Visuo-motor   Perspective               Appearance
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  independent                                              Inductionsec.  180 300 180 180 240    480        180        270 60   900  40   30    120        30        120    600   300    20 40 456
                                                                                             an
                                      Mirror  Yes Yes Yes Yes No No No No No No No No No No   Yes  Yes No No No No No No Yes Yes No Yes No No No   Yes  Yes No Yes Yes No No as
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   embodiment Continued                                                     Perspective  1PP 1PP 1PP 1PP 1PP 3PP 1PP 1PP 1PP 3PP 1PP 1PP  1PP/3PP 1PP   1PP  1PP 3PP 1PP 1PP 1PP 1PP 1PP  1PP/3PP 1PP 3PP 1PP 1PP 1PP 1PP  eye-height  chest-height 1PP 1PP 1PP  1PP/3PP  1PP/3PP 1PP

1.                            3D                                                                                                          Wide5                                                                                                                                                        manipulate                                                                                                SX111Table                    CV1 SX111        CV1       SX111 DK2                                                      Pro                                                                 DK2 S    CV1     3D        Pro           Labs    DK2 DK2 CV1                   DK2 Pro Pro Pro
                                                                                                                                        Rift Rift                                                                                                                                                                                                   Rift                                Rift                                                    Rift Viewer                                                                                                                                                            Rift Rift Rift Rift                                                                   Rift                                                                                             nVisor                                                                        Vive nVisor                                                                                                                                                       Vive                                                       nVisor Vive Vive                                                                                                                                                                                Vive   Vive   Vive                                                                                                                                                                                                        Vive Vive Vive Vive    studies                                                                                  Rift Rift Rift Rift Rift HMD0 Vive Viewer Vive Vive VIVE
                                                                                                                                            all                   HMD    Oculus NVIS HTC HTC Oculus  Virtual NVIS Oculus HTC NVIS Oculus Oculus Oculus Oculus Oculus FOVE HTC Real HTC HTC HTC Oculus Oculus  Fakespace HTC Oculus Oculus Oculus Oculus HTC   HTC  HTC Oculus HTC HTC HTC HTC                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                condition.
                                                                                                                                            Not
                               GenderM/F    13/27 0/60 0/64 63/62 16/17 47/34 0/32 11/9 33/18 30/0 14/4 20/30 5/12 13/32     63/105    20/20 14/8 39/29 9/22 30/44 6/4 12/7 24/0 28/30 0/27 0/34 0/30 48/48 24/0    12/13    14/15 5/27 8/25 0/56 13/12 21/21    agency.                                                                                                                                                                                                                                                                                                                                                                                                                                                synchrony
                                         Subjects Total 40 60 64 125 33 81 32 20 51 30 18 50 17 45   168  40 22 68 31 74 10 19 24 58 27 34 30 96 24  25  29 32 33 56 25 42 or                                                                                                                                                                                                                                                                                                                                                                                                                                    ownership   visuo-motor
                                            Studies 1 1 1 1 1 3 1 1 1 1 1 1 1 1 3 1 1 3 1 1 1 1 1 1 1 1 1 4 1 1 1 1 1 1 1 1      the                                                                                                                                                                                           body
                         Year   2020 2013 2018 2020 2018 2013 2014 2019 2018 2013 2019 2016 2021 2020   2020   2019 2013 2020 2020 2020 2019 2019 2010 2019 2019 2017 2021 2019 2017   2019   2018 2017 2021 2021 2019 2020
                                                                                                                                                                                                                                                                                                                                       measure  represent                                                                                          [144]
                                                                                                                                                                                                         [170]                                        and                                                                                                                                                                          [181]                                                                                                                         al.                                                                                                                                                              [160]                                                                                                                                                                                                                     [172]                                                                                                                                  [154]                                                                                                                                                3],                                                                                                                                                                                                                                                                                                                                       studies                                                                                                                                                                                                                                     [177]                                                                 [139]                                                                                                [145]                                                                                                                                           [155]                                                                             [142]                                                                                                                                                                                                                                              [182]                                                                                                                                         al.                                                                                                                                               Kaufmann                                                                                                                                            all                                                                                                            [147]                                                                                et [171]                                                                                                                                                                                                   [166]                                                                                                                  [148]                                                                                                                                                                           Neff                                       al.                                                                                                                                                 [156]                                                                                                                                                       [157]                                              al.                                                                                                                                                                                      [−3;                                                                                                                                               al.                                                                                                      [146]                                                                                            et                                                                                                                                                                                             Müller                                        [132]                                                                                                                         [149]                                                                                                                                                                                                                                                                             [189]                          et [141]                                                                 al.                                                                                                                            al.                                                                                                                     al.                               et [143]                                                                                       al.                                                                                                                                                                                      [165]                                                                                                                                                                                             [162]                                                                                           al.                                                                                                                                                                                                                                                          [185]                                                                     Pia                                                                                                                   Slater                                                                                                                                                                                [190]                                                      and                                                                                               et [184]                                                                                                to                                                                                                                                                                                                                                                                 [186]                                                                                                                                and [173]                                              [137]                                                    [134]                                                           [136]                                                                                                                                            not                                                             al.                                                                                                                                                                    [161]                                           al.                                                                                                                                                                                                                                                                                                                                                    Liarokapis                                                                                                                                           Gamer                                           et                                                                                   et                        al.                                                                              et                                                  al.                                                                                                                                                                                                                                          Latoschik                                                                        al.                                                                                                                                                                                                                                                                       [188]                                                                                                                                                                 al.                                                                                                                                                   al.                                                          et                                                             et                                                                                                             al.                                                                                                                 al.                                                                                               and                                                                                                                                                      al.                                                                                                          al.                                                                                                                                                                                       Veer                                         et                            et                                                                                                                                                          al.                                                                                                                                    al.                            al.                               al.                                   al.                                                                                                  al.                et                                 et                                                                     and                                                et                                                         and                                                                                                            et                                                                                                  et                                                                                                                                                              al.                                                                         et                                                                           et                                                                                                    et                                                                                                      and                                                                      et                                                                                   and                                                                                                       et                                                                                        et                                                                              and                  et                     et                       et                                                                                                                                                                                           that                                                                  et                                                                                                                                         der                                                                                                         et                                                                                                                                                                                                                                                                                                scaled                                            Article    Patané Peck Peck Peck   Perepelkina  Pfeiffer  Piryankova  Pittera  Podkosova Pomes  Porssut  Pritchard Pyasik Pyasik   Roth   Rubo  Salomon  Schwind  Seinfeld Shin Škola Škola Slater Slater  Spanlang    Tajadura-Jiménez  Tambone  Toothman Tran   van       Waltemate Weeth Weijs Wolf Wu Zhang                                                                                                                                                                                           Note are



ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 11 / 42 -->

```text
Body Ownership Illusions in VR                                                           76:11


4.3  The Source Data and Materials

Each article that met the eligibility criteria underwent manual extraction of relevant variables.
Due to the triviality of the task, three individuals collectively sourced data without overlap. We
collected the following information:

  Study design, procedures, and methods. Number of studies, number of participants (by study and
by gender), type of VR headset, completeness of body ownership (full body, arm(s), or hand(s)),
perspective, presence/absence of a mirror, manipulation of embodiment (visual synchrony, tactile
synchrony, an abstract body, etc.), induction duration, study design, and objective measurements
of embodiment.

  The subjective measurements. Reference to the questionnaire(s) employed, number of questions,
number of constructs, scale (min., max., and delta), statistical analysis, and reliability.

  Meta-analysis. Type  of disembodiment, number  of  participants  for each  condition, and
condition-specific descriptive statistics for each subjective embodiment variable.

4.4  Measurements
In addition to reviewing the data obtained in the aforementioned manner, we conducted meta-
analyses involving four constructs recurrently applied for measurements in BOI studies: agency,
body ownership, mirror body, and two bodies. The specific wording of questions is often adapted
to the experiment’s context and hence differs across samples. Likewise, the scales employed vary,
although measurements are commonly collected with a 7-point Likert scale ([−3; 3] or [1; 7] is
typical, though some studies use [1; 5] or [1; 100]).

4.5  Effect Sizes
Effect sizes facilitate comparison between studies, help estimate the required sample size for future
studies, and aid in assessing the importance of experimental findings [1].
  We report Hedges’ д, since it is less biased with small sample sizes than Cohen’s d [59]. We
computed effect sizes from means, standard deviations, and sample sizes using the R function
esc::esc_mean_sd [107], with per-condition sample sizes considered (we assumed an even distri-
bution of participants when the authors did not report group-specific sample sizes).
  Most BOI studies feature a baseline control condition, in which the participant experiences an
adult humanoid avatar matched to gender in first-person perspective (1PP) with visuo-motor syn-
chrony. This enables comparison with a condition wherein participants experience a body with
some form of disembodiment (e.g., appearance, feature, or perspective changes or incongruence of
visual/tactile cues). Therefore, the effect sizes reported from the meta-analysis represent the mag-
nitude of the difference in the dependent variables between the given study’s embodiment and dis-
embodiment conditions. The employed statistical practice is furthermore described in Appendix A.

5  RESULTS
The cumulative evidence from our review supports the hypothesis that manipulations to virtual
avatars influence subjective ratings of embodiment, the central aspect of BOIs (see the summary in
Table 1). A detailed analysis of publication bias can be found in the Appendix B; weight-function
modeling and funnel plot analyses did not uncover evidence for systematic publication bias.

5.1  Effects of Avatar Manipulation
The most fundamental aspect of virtual embodiment, body ownership, are collected from both
baseline and body-manipulation conditions in 61 articles in the sample; similarly, 35 studies


     ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 12 / 42 -->

```text
76:12                                                                       A. Mottelson et al.


manipulating avatars have reported subjective agency scores. We use these scores to compare the
effectiveness of experimental manipulations.

   5.1.1  On Body Ownership. Body ownership measurements are reported in 61 of the articles.
These reports enable field-wide comparisons of embodiment and disembodiment effect sizes, re-
spectively. The effects for body ownership are grouped by type of disembodiment (see Figure 2).
Due to the modest sample size, we did not compute the mean weighted effect sizes for studies ma-
nipulating avatar placement. Across all disembodiment manipulations, the largest effect on subjec-
tive body ownership emerged for visuo-motor asynchrony;д = 1.1, 95% CI [0.83; 1.35]. Perspective
(i.e., first- or third-person perspective; д = 0.88), abstraction (i.e., use of a non-humanoid avatar;
д = 0.72), and visuo-tactile asynchrony (i.e., incongruence between visual and tactile stimulation;
д = 0.68) similarly manifested consistent effects on body ownership. Interestingly, “embodying” an
invisible avatar showed consistent null effects on body ownership, д = 0.07, 95% CI [−0.02; 0.16],
providing evidence that incongruence in sensory stimuli diminishes the sense of body ownership
while absence of stimuli does not. These meta-analytical findings are important for weighing the
relative importance of the various components of multi-sensory integration, and they may have
implications for future experiment design in BOI research.

   5.1.2  On Agency. Figure 3 shows the effect sizes of avatar manipulation on agency, for indi-
vidual studies and in the aggregate. Visuo-motor asynchrony proved to be the most influential
manipulation, with a mean effect size of д = 1.54, 95% CI [0.93; 2.2]. No other types of avatar
manipulation showed large effects on agency. It follows that congruence of vision appears as the
most prominent stimulus in BOIs.
  However, embodying an abstract avatar consistently showed some effect on agency (д = 0.49),
demonstrating that, across the board, embodying non-humanoid avatars (such as robots, primitive
shapes, wooden bodies, or mannequins) reduced both body ownership and agency from the levels
seen in control conditions.
  Furthermore, perspective showed as an effective manipulation on agency д = .89. Tactile asyn-
chrony also had effect (д = 0.66) on agency. Thus, congruence of tactile stimulation affects body
ownership and agency to similar degrees. The effect of avatar appearance (e.g., facial features,
clothing, and skin color) on agency, relative to body ownership, is limited д =  0.19, 95% CI
[0.05; 0.32].
   In line with the effects of avatar manipulation on body ownership, the data for invisible avatars
suggest null effects on agency.


5.2  Subjective Measurement of Embodiment in VR
BOI studies often employ questionnaires to measure the subjective embodiment of virtual bodies.
These vary in the number of constructs and items, the scale’s number of steps and its minimum
and maximum values, and analysis approach. To investigate the field’s subjective measurement
practices, we collected data related to embodiment questionnaires across BOI studies. For each
article, we collected

  — any references to the embodiment questionnaire(s) employed;
  — the number of constructs and number of items used; and
  — the scale’s minimum, maximum, and number of steps.

Ad hoc questionnaires are commonly used, sometimes as a sub-set or super-set of pre-existing
questionnaires’ items. Of the 111 articles included in the review, 26 employ unique embodiment
measurements. In comparison, 90 articles directly employ previous embodiment measures.


ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 13 / 42 -->

```text
Body Ownership Illusions in VR                                                           76:13





Fig. 2. Body ownership effect sizes, grouped by embodiment manipulation, where error bars denote the 95%
CI and red diamonds depict the weighted means of means with a 95% CI of means (omitted for “Displace”
because of sparsity and high variance).




     ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 14 / 42 -->

```text
76:14                                                                       A. Mottelson et al.





Fig. 3. Agency effect sizes, by embodiment manipulation, where error bars denote the 95% CI and red di-
amonds depict the weighted means of means with a 95% CI of means (omitted for “Displace” because of
sparsity and high variance).





ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 15 / 42 -->

```text
Body Ownership Illusions in VR                                                           76:15


  In some cases, the references cited for the embodiment measurements point to other studies,
with the resulting “chains” of references to embodiment questionnaires ultimately pointing to
original research rather than to psychometric instruments.
  Due to mixed practices with respect to subjective embodiment instruments, we noted when ques-
tionnaires were adapted, overlapped, and/or were identifiable from their references or wordings,
so that we collected the most complete set of data possible. Finally, only 12 of the articles address
the reliability of subjective measurements (e.g., by Cronbach α). This limitation makes conclusive
estimations difficult; however, isolated articles report low or even negative reliability [129, 136],
while other report high α values for embodiment constructs above 0.9 [67, 93].
  The data suggest six commonly employed questionnaires for subjective embodiment, summa-
rized in Table 2. In Table 2, we also report Cronbach’s α for some of the commonly employed
embodiment questionnaires using the data reported in their original studies, and find acceptable,
yet not unambiguous levels (i.e., α-values in the range of 0.78–0.85). It is evident that the prac-
tices of measuring subjective embodiment vary greatly. Most importantly, few of these practices
have been formally validated, and the questionnaires utilized have, for the most part, been devel-
oped for purposes other than VR research (often for the RHI). The six most commonly employed
measurements are summarized in Appendix C.

5.3  Terminological Confusion
Eighteen articles report body ownership as the only subjective measurement of embodiment. Some-
times, the assessment of body ownership involves only a single item (e.g., [111, 112, 137]). Other-
times, it involves the application of an elaborate questionnaire with many questions, including
constructs often considered to represent agency or self-location. Hence, VR research sometimes
uses the notions of body ownership and embodiment interchangeably. In the embodiment liter-
ature, a specific question may refer to various named constructs; a case in point is the use of
the question “[...] did you feel as if the virtual right arm was your own right arm?” referred to
measuring both the “level of ownership” [23, 111] and the “embodiment level” [112]. Also preva-
lent are combined constructs, such as “embodiment” [172] or “body ownership and agency” [28].
Furthermore, researchers often collect multiple body ownership measurements—for instance, by
asking about the body seen upon looking down (often called “me down”), on looking in a mirror
(or “mirror body”), and more generally (“my body”). Additionally, material for constructs similar
to embodiment gets collected in BOI studies, such as “self presence.” For this, researchers (e.g.,
[4]) use a 15-item presence instrument with such questions as “To what extent did you feel that
the avatar’s body was your own body?” Arguably, this touches on the same aspects of bodily
self-consciousness as body ownership. Similarly, Dobricki and de la Rosa [31] suggested the three
sub-scales “self-identification”, “spatial presence”, and “agency” for measuring “Conscious Full-
body Self-perception”. Finally, the wealth of detailed neuropsychological accounts of embodiment
related to limb ownership, agency, and body ownership [35, 55, 70, 102, 174, 175] does not provide
an easily accessible vocabulary for VR researchers. This shortcoming makes scientific output diffi-
cult to compare and often raises validity concerns, thus creating what Ekkekakis and Russell [36]
characterized as a “terminological Gordian knot” when documenting disparate measurements of
affect in health-behavior research.

5.4  Consistency Checks

In addition to direct embodiment constructs, the control questions often used in embodiment
questionnaires as consistency checks are of interest. For instance, six of nine questions in the
original RHI study were control items; only three questions being expected to show differences
across conditions. A review by Gonzalez-Franco and Peck [48] reports that 60% of the studies


     ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 16 / 42 -->

```text
76:16                                                                       A. Mottelson et al.


               α - - -  0.85A -  0.80C    -  -       0.78D




                                   =                                                                                                                                     Citations   4748     1416    929  648  174  264           111      990    91                    0.75.                                   α
                                                    Three)                                                                                                                                                                                                               yields
                                                                                                                                                                                                                                                     condition)                                                             (Bottom           *                                                                                                                                                                                                                                                                                                       Error(P/sync))                     +    sync)                                          trial)                   touch)                                                   twobodies                                                                                                                          ∼sync         *                                                                                    sync                                             ∼condition)                                      and
                     *                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             Error(P/latency))                                                                                                                                                                   question)                  *                                    condition,                                                                      condition,                                                                                                                                                                                                                                                     ordered=T)                                                                           movement* +                                                                                                                         Questionnaires                                                                                                                                                                                     ordered=T                                                     features                                                                                                                                                                                                                  ∼component                                                                                           ∼sync ∼sync)                          BOI                                ∼condition)                                3,                                                                                                                                                                                                                                                                                                    ∼latency               R                                                      %/%                                                                                                                                                                                                                                                                                                                       Including                                                                                                                                                                                                                                                                                                                                                                                                                                  ∼perspective                                           other                                                                                                     (Q+2)                                                                                         Psuedo     t.test(Q      aov(score  t.test(Q      aov(score           friedman.test(Q,          polr(factor(Q,               wilcox.test(PCA_factor                                                         friedman.test(Q,        polr(factor( )     aov(var                                                                                                                                                                                                                                                                                                                                                                                                                                      constructs.                          and                                                                                                                                                                                                                                                                       mirror).
                                           Six),                                                                          Order    random             sequential        random       sequential       sequential    random    -                   sequential           random             and                                   (Top                                                                                                                                                                                                                                                                                   embodiment                                                                                                                                                                                                                                                                                                         (Q1–Q5).                                                                                                                                                                                                                                      (vrbody                                                                                                                                                    Validation No   No    Yes No No NoB       No    No      Yes                                         other                                                                                                                                                    used                                                                                                                                          used        for
                                                                                                                                                    were                                                                                                                                          were                                                                                                                         Questionnaires                                                                                                                                                                                                                                                                                                                   reported                                                                                                                                                                             items                          BOI                    Min./max./delta    −3/3/7       −3/3/7       −3/3/7    −3/3/7    −3/3/7    −3/3/7                  1/7/7             0/10/11         1/7/7                                                                                                                                                                                                                                                                                                                                              ownership  values                                                                                                        Two
                                                                          Items 9 7   10 4 5 25    1  8    12                                  [135]. body                                                    Common                                                                                                          2022.                                                                                                               for  identical                                                                                                                                                                                                                                                                                                                       material.
                                   Most                                                                31,                    Items                                                                                                                                                    Constructs 9 7 3 4 5 6    1  8  3                                                                                                                                                                                                                                      Almost
                          the                                              22                 of                                                                     70,               December                                         Gonzalez-Franco  GitHub.  paper.                                      14                                                  48,    of                    supplementary                                                                                                           and     the               N 10    14,    131 30 44  N/A       30    24      50,    as                                                                                                                                               Peck  author’s in                                                               α.  paper’s                                                                                               Description                                                                                              video               child      speaking    avatar           arm            avatar           avatar             Scholar     the                                                                                                                                                                                                                                                                                                                   reported                                                                                                        Concept  RHI   VR    RHI  BOI  BOI VR       VR    VR    VR         in by firston                                                                                                         2018                                                                                                                  Cronbach’s                                                                                                                                                                             found  presented found  items),                                                             Summary                                                                                                                               Google                                                                   as                                                                                                                                from                                                                                                                                          data later data                 2.            1998     2007                   2014    Peck,                                     2020                                                                                                                                                                                                (four                                                                                                are                                                                           al.,                   and                                                                                                                    participants.                                                                                           2013                                                                                                                                                                                                                                                                           validity from study from                                                                                                                                                                            Slater,                     2013                                           Table                  Cohen,                                      et     2008                                                                                                                                       2010      of                                                                                           al.,                                                                                                                                                                                                                                                                                                                                                                              Latoschik,           counts                                                 and              al., et  and                     al.,                                                              et        al.,                                                                                                                                                                                                                                                                                                                                                         ownership                                          et                       et      and    number            internal
                               =  =                                                                                                                                                                                  Authors/year      Botvinick                Lenggenhager      Longo     Banakou     Banakou           Gonzalez-Franco                         Martini            Slater        Roth                               N  Citation α AComputed BValidation CComputed DFor



ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 17 / 42 -->

```text
Body Ownership Illusions in VR                                                           76:17


examined use such control questions (not to be confused with control of avatar actions or agency).
The number and type of control questions in BOI studies vary, as does the approach to any
analysis conducted. In 23 studies, the “two bodies” construct (e.g., “I felt as if I had two bodies”)
is measured and reported.
   Practices of employing control questions as a consistency check in embodiment questionnaires
lack uniformity. Control items originally developed for this purpose are commonly included with-
out any analysis of consistency; they function merely as “filler items.” Researchers seldom actively
hypothesize about or test for consistency across conditions. Furthermore, some studies even use
control questions as part of the embodiment metric; for instance, Peck et al. [137] suggested com-
puting body ownership as (MyBody + 6 −NotMe)/2.
   Practices related to control questions are inconsistent in general, as exemplified by influential
works, with Petkova and Ehrsson [140] and Banakou and Slater [8] suggesting the use of “Features”
as a consistency check (i.e., “I felt that my virtual body resembled my own (real) body in terms
of shape, skin tone, or other visual features”). More recent research has most often employed this
construct directly as a sub-dimension of embodiment [48] despite its original intention.
  Taking into account the use of control items in RHIs, Riemer et al. [152] emphasized that “empir-
ical support justifying this practice is lacking”. More recently, Lush et al. [106] suggested that the
use of control questions in embodiment research exacerbates the risks of demand characteristics.
Indeed, our review shows that, while control questions are commonplace in BOI settings, there is
great disparity in their use, a lack of clear hypotheses, and inconsistency of approach (they may be
treated as dependent variables or filler items). Finally, this general state of affairs may introduce
threats to the statistical validity.
  Notwithstanding the questionable approach to control questions, the most commonly employed
embodiment-connected control question, on “two bodies,” does not seem affected by experimental
manipulations of disembodiment (д = −0.06, 95% CI [−0.24; 0.12]). The mean response across
means for all control conditions is M = −1.02, SD = 0.68 (range: −3 to 3), showing that participants,
as expected, in fact do not experience two bodies when embodied in one.

5.5  All Roads Lead to Rubber Hands

Following the path of references for embodiment questionnaires leads to the embodiment ques-
tions associated with the RHI (see Figure 4). For instance, Patané et al. [133] stated that their items
addressing the level of subjective ownership over one’s virtual body are adaptations of Banakou
et al. [6] and Banakou et al. [7]’s work; both publications address the questions considered by
Banakou and Slater [8], who, in turn, referenced Botvinick and Cohen [21] as inspiration. Although
this observation itself is harmless, two concerns arise. First, the fundamental principle behind all
subjective embodiment measurements in VR research is, by transitive relationship, based on the
RHI, an experiment paradigm popularized well before modern advances in VR BOIs. While the
RHI and the BOI phenomena are inherently related, the questions, constructs, and analyses devel-
oped specifically for the latter’s analogue setup have never been validated for the fundamentally
different medium of the digital domain, which features greater immersion, presence, and visuo-
motor synchrony. Second, the practices seem to illustrate collective confusion surrounding both
the origin of the measurements and the corresponding analyses. The chains of references make
convergence to similar practices difficult, and junior researchers may find it especially hard to
unearth the relevant resources for conducting solid empirical research.

5.6  Subjective Embodiment Scores

The corpus of reports on BOI studies measures many dependent variables related to embodiment.
In our presentation of results, constructs with high similarity are matched to allow for field-wide


     ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 18 / 42 -->

```text
76:18                                                                       A. Mottelson et al.





Fig. 4. A diagram connecting each study in the survey to other articles referencing the subjective embod-
iment scale employed, such that the lines’ and circles’ size denote the number of references (number of
references in parentheses). The colors differentiate between publishers.

comparison. Among the most commonly employed notions and terms are (i) body ownership,
(ii) agency, (iii) mirror body, and (iv) two bodies. Numerous other constructs were measured in the
studies surveyed, among them “other person,” yet these show limited application (with 10 or fewer
occurrences in the corpus). See Table 3 for an overview. The constructs reported vary slightly in the
name used (e.g., “VRBody” and “MyBody”) and in the specific wording of the measurement items.
  Research into BOIs typically employs a control condition and a body-manipulation condition,
for a two-by-two design, with independent variables such as embodiment (e.g., skin color) and
disembodiment (e.g., related to the synchronicity of movements or tactile feedback). This type
of work advances our understanding of bodily self-awareness through estimating the differences
in embodiment responses across conditions. In designing such studies, researchers will often ask
themselves what range of embodiment scores they could expect the participants to report.
  Figure 5 shows the distribution of the study-specific embodiment-response means. It raises sev-
eral interesting points. First, the ratings for agency are higher (M = 1.39, SD = 0.83) than those
for body ownership (M = 0.80, SD = 0.67), on average. This finding is unsurprising when one
considers that agency involves one’s control of actions and does not require humanoid bodily prop-
erties. Second, average body ownership is fairly modest across “embodiment” conditions—that is,
conditions in which participants experience a body with visual congruence from 1PP. Therefore,
researchers should expect absolute mean body ownership ranges between 0.1 and 1.4 (on a scale


ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 19 / 42 -->

```text
Body Ownership Illusions in VR                                                           76:19


               Table 3. Commonly Employed Subjective Metrics for Embodiment in BOIs

   Construct         Similar variables                 Example questions

   Body ownership   VR Body, My Body, Own Body,       How much did you feel that the virtual body you saw when you
                      Sense of Ownership, Virtual            looked down at yourself was your own body?
                    Body Ownership, Self presence,
                Me Down, Avatar Acceptance,                I felt as if the virtual body were my body
                           Self Identification, Embodiment,
                                          How much do you feel like your avatar is an extension of your body
                    Embodied Avatar, Embodied presence


   Agency             Control, Sense of Agency,                      I felt that the movements of the virtual body were caused by my
                Own Agency, My Movements,        own movements
                       Control Move
                                                                                            I felt that if I moved my real body (arms, hands, legs), the virtual
                                                       one would also move accordingly

    Mirror body      Me Mirror                                           I felt that the virtual body I saw when looking at myself in the mirror
                                                    was my own body

                                          How much did you feel that the virtual body you were looking at
                                                                   in the mirror was your own (real) body?





Fig. 5. A summary of four commonly measured constructs across all BOI studies for baseline conditions,
involving (parts of) an adult human avatar in visuo-motor synchrony, where mean values are represented by
horizontal lines in which each dot denotes the estimated mean from one study scaled to [−3; 3].


from −3 to 3) for avatars with sensor congruency in BOI studies. This finding implies great po-
tential for technical contributions that improve BOI-research (e.g., related to visual and tracking
fidelity, kinematics algorithms, and 3D modeling) in addition to research avenues whereby exper-
iments pinpoint techniques that improve the sense of embodiment with virtual avatars.

5.7  Criticism of Subjective Embodiment Measures
More than a decade ago, Slater and colleagues identified methodological challenges with subjective
embodiment measurements [163], later noting that “questionnaires in this area are problematic
unless supported by behavioral or physiological evidence” [165]. Our review shows that only about
half of BOI studies include such physiological evidence, most commonly galvanic skin response


     ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 20 / 42 -->

```text
76:20                                                                       A. Mottelson et al.


to a threat (e.g., the appearance of a saw), heart-rate variability, and proprioceptive drift of limbs
(for a full list of the objective measurements, see Table 4). While such measures might complicate
study procedures, and, especially for physiological measures, are seldom available with off-the-
shelf VR equipment, the collection can significantly increase validity of findings. To this end Table 4
can serve as an inspiration for VR embodiment studies considering an expansion of dependent
measures beyond subjective.
   In light of a significant difference in non-illusion questions between synchrony conditions, Slater
et al. [163] stressed the importance of the issues accompanying questionnaires, underlining that
“over-reliance on questionnaires is methodologically dubious.” Because of their applicability to
most experimental setups, subjective measures continue to dominate measurement of embodi-
ment. To this end, being terminologically accurate and applying standardized tools and analysis
techniques is of high importance to the validity of measurements; which unfortunately is often
not the case in BOI research.


5.8  Correlations with Subjective Embodiment

The subjective embodiment scores demonstrate correlation to numerous measurements. We iden-
tified correlations of dependent variables related to embodiment scores’ for subjective, cognitive,
motor-function, and physiological measurements (see Table 4).
  Many of the physiological outcomes in particular—such as skin response to a threat and various
heart-rate responses—are often treated as evidence for embodiment, whereas subjective, cognitive,
and motor-function outcomes (apart from drift) are commonly regarded as the exploratory part
of a study. Still, examples of objective cognitive measures taken as direct evidence for dimensions
of embodiment do exist (e.g., Libet’s clock [99] for measuring sense of agency in VR [15], or the
mental ball task to measure implicit self-location [94]).
   Analysis of embodiment correlations together show the host of attitudes and behaviors con-
nected with subjective embodiment of virtual bodies. Empirical support for embodiment correlates
has been shown repeatedly with regard to (age-, race-, and gender-) biases, size estimations (for
objects and bodies), and empathy. Since most of these correlations have been reported only once,
we refrain from estimating mean effect sizes across categories. Note that many of the reports do
not demonstrate causal relations to embodiment, but rather demonstrate relations to embodiment
specific virtual bodies (e.g., affect of embodying a smile or frowning avatar [65]). Because of the
limited studies for each measurement, the data is too scarce to conduct meta-analytical estimations
of the correlations.


5.9  Mirrors
Mirrors give the participant an opportunity to see their bodies in first-person perspective; hence,
they are relevant primarily for full-body illusions. About half of the studies surveyed used mirrors
in the induction procedure. Of these, half (N = 27) examined body ownership with reference to
the body seen in the mirror—“mirror body.” The latter representation shows a strong correlation
with more general body ownership (i.e., “my body”), with Pearson’s r (14) = 0.96, p < 0.0001.
Furthermore, as Figure 5 attests, these constructs’ distributions are highly similar, reflecting that
the two constructs probably measure the same thing.
  Our data suggest that the presence of a mirror might impinge on the size of the resulting effect
for body ownership. Studies without a mirror yielded a weighted mean effect size ofд = 0.78, while
the effect was smaller in those with a mirror present, at д = 0.67. It should, however, be noted that
studies with mirrors present might reflect task designs that incorporate activity to body parts that
without the presence of a virtual mirror would be out of sight.


ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 21 / 42 -->

```text
Body Ownership Illusions in VR                                                           76:21


    Table 4. Correlation of Subjective Embodiment to Subjective, Cognitive, Motoric, and Physiological
                                     Measurements

   Subjective measurement    Studies

   Age bias                   Banakou et al. [7]
    Racial bias                  Aymerich-Franch et al. [4], Hasler et al. [58], Patané et al. [133], Peck et al. [137]
   Health decisions              Mottelson et al. [122], Tambone et al. [171]
   Gender bias                 Lopez et al. [103], Peck et al. [136]
   Math confidence             Peck et al. [136]
    Self-criticism                 Falconer et al. [37]
   Bodily awareness            Bergstrøm et al. [16]
   Empathy                    Barbot and Kaufman [11], Christofiet al. [28], Hamilton-Giachritsis et al. [56], Patané et al. [133]
    Perception of risk             Shin et al. [161]
    Social-interaction quality      Latoschik et al. [91]
    Guilt, Regret                Friedman et al. [41]
    Social anxiety               Aymerich-Franch et al. [4]
    Attitudes to life change        Barberia et al. [10]
    Fear of death                Bourdin et al. [22]
    Affect                       Jun et al. [65], Osimo et al. [130]
    Feelings of vulnerability       Gonzalez-Liencres et al. [49]
   Presence                 Kim et al. [80], Schwind et al. [157]
   Pain                     Weeth et al. [184]
   Human-likeness              Latoschik et al. [91]
   User experience         Wu et al. [188]
   Cognitive measurement     Studies

   Navigation                  Medeiros et al. [116]
   Cognitive performance       Banakou et al. [7], Bergstrøm et al. [16], Latoschik et al. [91]
   Cognitive load              Kocur et al. [84]
    Size estimation             Banakou et al. [5], Jung et al. [67], Keizer et al. [74], Kokkinara et al. [86], Leyrer et al. [96], Normand et al.
                                      [126], Ogawa et al. [128], Piryankova et al. [142], Tajadura-Jiménez et al. [170]
    Localization                van der Veer et al. [177]
   Weight perception           Wolf et al. [186]
   Reaction time              Banakou et al. [5]
   Learning of motor imagery    Alimardani et al. [3]
   Delegation of electric shocks   Neyret et al. [125]
   Body-change recognition      Peck et al. [136]
   Motoric measurement      Studies

   Reach                      Bourdin et al. [23], Nataraj et al. [123]
   Movements                  Burin et al. [27], Rubo and Gamer [155]
   Mimicry                     Hasler et al. [58]
    Vection                       Nesti et al. [124]
    Collision avoidance           González-Franco et al. [50], Ogawa et al. [129]
   Drumming                      Kilteni et al. [75]
    Drift                      Hara et al. [57], Kondo et al. [87], Perepelkina et al. [139], Pomes and Slater [145], Pyasik et al. [149]
   Kinematics                   Perepelkina et al. [139]
   Motor performance           Grechuta et al. [51], Kocur et al. [82, 83], Seinfeld and Müller [160]
   Throughput                 Peck et al. [134], Tran et al. [173]
   Grip strength               Kocur et al. [83]
   Speaking                  Banakou and Slater [8], Tajadura-Jiménez et al. [170]
   Physiological               Studies
   measurement

   ERD                         Škola et al. [190]
  HR                         Bergstrøm et al. [16], Slater et al. [162]
  HRV                       Bergstrøm et al. [16], Slater et al. [162]
  HRD                          Maselli and Slater [113], Slater et al. [165]
   MEPs                           Kilteni et al. [76]
   ERPs                       Spanlang et al. [166]
   GSR                       Galvan Debarba et al. [46], Gonzalez-Liencres et al. [49], Grechuta et al. [51]
   SCR                         Fusaro et al. [42], Pyasik and Pia [148], Tambone et al. [171], Weeth et al. [184], Weijs et al. [185]
  EMG                       Bourdin et al. [23]
   Skin temperature            Salomon et al. [156]

 ERD = event-related desynchronization, HR = heart rate, HRV = heart-rate variability, HRD = heart-rate deceleration,
 MEPs = motor evoked potentials, ERPs = event-related brain potentials, GSR = galvanic skin response, SCR = skin
  conductance reactivity, and EMG = electromyography.





     ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 22 / 42 -->

```text
76:22                                                                       A. Mottelson et al.


5.10  Effects of Gender

VR studies with only one gender of participants present several practical advantages. Only one 3D
model needs to be developed and rigged, and greater bodily consistency might afford more uni-
form experimental practices—for instance, connected with stroking the virtual and physical body
simultaneously. Furthermore, some studies suggest that there are gender differences in somatosen-
sory perception [33, 90], with the potential to confound embodiment scores. Also, some research
questions or settings have an inherently gender-bound component, as in conditions of maternity
[56] or being Sigmund Freud [130]. In addition, there may be a gendered confound to research
questions on factors such as sexual harassment [125] or anorexia nervosa [74]. These grounds
have together been used to argue for recruiting people of only one gender for a BOI study.
  Consequently, 26 of the articles we reviewed used a single-gender sample (10 recruited only
males; 16 used only females). Of these, 14 included both an embodiment and a disembodiment
condition (seven of the male-only studies and seven of the female-only ones), allowing comparison
of effect sizes between genders.
  We did not find conclusive evidence for a gender effect on body ownership (see Figure 6). The
BOI studies with female-only participants present a mean effect size ofд = 1.08, 95% CI [0.53; 1.63];
the corresponding figure for male-only studies is д = 1.29, 95% CI [0.53; 2.05]. Neither did we
identify a gender effect for agency—female-only: д = 1.45; male-only: д = 1.79. Furthermore, the
ratio of female/male participants across all studies did not correlate with body ownership effect
size: Pearson’s r (69) = 0.10, p = 0.40; the effect of gender ratio on agency effect size was, however,
more pronounced: r (39) = 0.28, p = 0.08.

5.11  Participants and Designs

The 111 articles report on a total of 142 empirical studies (the median number of studies is 1, with
SD = 0.65), involving 4,925 participants. The studies employed between 10 and 282 participants,
with a median participant count of 30 (SD = 31.3). A similar number of male and females partici-
pated, with an average of 17.5 males and 17.2 females per study. Twenty-six studies recruited only
one gender (10 enrolling only males and 16 only females). Across all 142 empirical BOI studies,
eight participants were reported as non-binary (across two studies [11, 122]).
  The experiment design cannot be readily characterized: BOI studies employ various designs.
There are commonly both within-subjects factors (e.g., synchronicity of stimulation) and between-
subjects ones (e.g., avatar manipulation), though many studies feature either exclusively within-
or between-subjects factors.
  Summarizing only the research with experimental manipulations of embodiment (presented in
71 studies), we found a mean power for body ownership of 0.53, which is relatively modest in that
it implies an approximately 50% chance of null findings even when an effect exists (note that this
figure pertains only to the fundamental differences in body ownership, not the behavioral effects
that followed). We computed the power using the R-function stats::power.t.test [150], which
takes the mean difference, pooled standard deviation, and the number of participants as inputs.
Accordingly, research into embodiment could benefit from, among other improvements, larger
sample sizes and greater precision of the measurements.

5.12  Apparatus and Environments

Most often, studies employ the HMD Oculus Rift (42 articles), HTC Vive units (33 articles), and
the NVIS nVisor (25 articles), with various versions of the devices being employed (Rift CV1/DK2,
Vive / Vive Pro, nVisor SX111/SX60, etc.).
  Most articles presented the BOI from first-person perspective, while considerably fewer adopted
a third-person one (1PP: 74 articles; 3PP: 8 articles). Thirteen utilized both perspectives.

ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 23 / 42 -->

```text
Body Ownership Illusions in VR                                                           76:23





Fig. 6. Body ownership effect sizes found in studies with participants of only one gender, grouped by gen-
der (error bars denote 95% CIs, and red diamonds show the weighted means of means with a 95% CI of
means), with the disembodiment manipulation highlighted for each study: Appearance, Visio-motor syn-
chrony, Perspective, and Invisible.

  Most articles (76 of them) describe a full-body ownership illusion; i.e., the participant is repre-
sented by a complete humanoid avatar. Seventeen articles used only the hand(s), 17 used only the
arm(s), and the rest involved some combination of virtual limbs.

5.13  Induction Procedures
About half of the articles reviewed (N = 58) present details of the induction of virtual embodiment,
collectively referred to as the embodiment phase. A mean duration of induction of slightly more
than three minutes (M = 190 s, SD = 146) was found. The procedures and their length vary
between studies, oftentimes as a function of the manipulation employed (e.g., synchronicity of
tactile feedback has a more immediate impact on induction procedures).
  For this phase, it is common practice to ask participants to look down at their body or tilt their
head downward [140]. This is a powerful induction, as emphasized by Slater et al. [164].

     The very act of looking down, changing head orientation in order to gaze in a certain
       direction, with the visual images changing as they would in reality is already a powerful
      clue that you are located in the virtual place that you perceive.
      Slater et al. [164, p. 219]

This induction is most effectively conducted using visuo-motor synchrony (i.e., physical body
movements are virtually reflected in real time), since participant movements would otherwise
break the illusion. The induction can also be further underpinned, using visuo-tactile synchrony:
Here, tactile cues on the participant’s body (e.g., vibration, poking, or stroking) are performed in
synchrony with visual stimuli (e.g., a virtual ball, stick, or brush).
  The practice of directing participants to look down at their body is linked to the two-construct
operationalization of body ownership (oftentimes abbreviated DownBody and MyBody) wherein a

     ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 24 / 42 -->

```text
76:24                                                                       A. Mottelson et al.


distinction is proposed between, on one hand, subjective body ownership as experienced during
looking down (“I had the sensation that the virtual body I saw when I looked down at myself
was mine”) and, on the other, a more generic sense (“I had the sensation that the virtual body I
saw was my body”). Querying ownership from the perspective of looking down (7 articles) shows
35% reduction in ownership (M = 0.52, SD = 2.00) compared to the generic operationalization
(M = 0.81, SD = 1.73). No significant correlation emerged between induction duration and body
ownership scores (Pearson’s r (55) = 0.02, p = 0.86); similarly, we did not find induction duration
to be strongly correlated to the size of the embodiment manipulation’s effect on body ownership:
r (37) = 0.19, p = 0.25. Agency displays a slightly stronger correlation to the duration of induction:
r (32) = 0.31, p = 0.07.

5.14 How Embodiment is Treated Statistically

Subjective embodiment measurement shows heterogeneity across BOI studies; the statistical anal-
yses conducted show comparable variation. The introduction of a measurement instrument or
scale is often accompanied by directions for the statistical handling of the outcome variables. Ta-
ble 2 presents the scale-linked differences in proposed statistical procedures. The range includes
Student’s t-test for single items, ANOVA for means of constructs, non-parametric testing, logistic
regression, and Bayesian analysis, with each practice having specific implications for statistical
validity and power, in addition to particular purposes in the explanation of results.
   Generally, statistical analyses should follow the protocols prescribed by the original source of
the instrument. This is especially true of validated scales and pressing for small samples. Many
analyses in the BOI domain could benefit from more conservative statistical analyses, such as
non-parametric tests, since embodiment scores seldom consist of ratio data and certain assump-
tions of general linear models are typically violated (e.g., those of normality and homogeneity of
variance). We provide example pseudo-R code in Table 2 for an overview of statistical procedures
corresponding to the various subjective metrics and their scales.
  There are, however, valid reasons for deviating from such analysis practices. Hence, we consider
it most important to characterize the intended methods explicitly at the outset (i.e., through pre-
registration, per Nosek et al. [127]).
  In some cases, specific statistical tests are preceded by various pre-processing of the embodiment
variables. Among these steps are binning [165] and PCA decomposition [48]. Perhaps even more
importantly from a data-processing standpoint, some researchers also remove outliers. Because
ownership over the virtual avatar is a fundamental requirement for subsequent scientific inquiry
in BOI studies, it may be reasonable to formulate standard quantitative embodiment-score criteria
for respondents’ inclusion in the analyses. Several methods have been proposed to detect outlying
embodiment scores, among them a cutoffvalue for residual error [8, 79], visual identification [5],
use of box plots for outliers [114, 168], and definition in terms of standard deviations—such as
2SD + M [159] or 3SD [128]. While simpler manipulation checks such as a mean embodiment
score (e.g., across ownership and agency) of ≥0 might suffice, these have not achieved widespread
adoption in BOI studies.

6  DISCUSSION
The findings of this review and meta-analysis serve two purposes: They aid in the important task of
distinguishing sensory prominence—the relative importance of each embodiment-related factor—
to advance multi-sensory integration theory. Furthermore, the outputs and critical assessments
can contribute to guiding future BOI research and, thereby, serve as a resource for conducting
good science that addresses BOIs in VR. We can thus enrich our understanding of how the body
shapes the mind.


ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 25 / 42 -->

```text
Body Ownership Illusions in VR                                                           76:25


6.1  Implications

Investigating which factors are associated with embodiment of virtual bodies has both theoretical,
practical, and empirical implications.
  Our meta-analysis identified the most effective experimental manipulations for BOIs. Visuo-
motor synchrony emerged as the most important means to this end, for the outcomes of body
ownership and agency (see Figure 2). The results shed light on the sensory prominence for in-
ducing ownership illusions, and our findings suggest that visuo-motor synchrony is of greater
importance than congruence of other visual congruence (e.g., realism, tactile stimuli, or perspec-
tive). This finding supports that avatar realism is not a critical top-down factor, as previously
suggested [64, 77, 105]. In comparing realistic and personalized hand models, Heinrich et al. [60]
found mostly differences related to subjective realism, and not embodiment. Some evidence, how-
ever, suggests that avatar realism positively influences acceptance of the virtual body [92]. About
half of the studies in this meta-review found the appearance of the avatar to affect body owner-
ship; the other half did not (see Figure 2). It should be noted that appearance covers a wide array
of avatar changes (e.g., facial features, skin color, and age), hence a future categorical investigation
of avatar appearance is needed. For agency, however, the appearance of the avatar seems to have
little importance (see Figure 3). For agency, visuo-motor synchrony showed to be the only reliable
manipulation for induction of illusions of body ownership (see Figure 3).
  When calculating the means of the embodiment scores across the four key constructs, agency,
body ownership, mirror body, and two bodies, we identified body ownership and the mirror-body
construct to be nearly identical statistically (i.e., querying ownership from looking down or in the
mirror yields identical responses). We, therefore, suggest omitting the latter, or only include it for
sanity testing rather than formulating specific hypotheses in relation to it.
  Studies with the presence of mirrors generally report smaller effects on body ownership, com-
pared to studies without mirrors. This observation is purely correlational, and the causal mech-
anism for this effect could be unrelated to the presence of the mirror itself. Speculatively, mir-
rors might reduce the sense of body ownership by making the facial region clearly appear non-
interactive and that misalignment of visual features between the participant and the avatar is
especially pronounced in the face area. Future support for continuous eye and mouth tracking
in HMDs could mitigate these concerns. Furthermore, there are design opportunities to design
illusions of body ownership in VR. In such environments, participants could observe their virtual
bodies without the direct presence of mirrors, such as through reflective surfaces, through virtual
video recording, or from tasks that systematically guide the participant’s gaze across body parts.
  For agency, in contrast, the presence of a mirror does not seem to demonstrate a negative effect.
While any conclusions must remain speculative due to the variety of agency measurements across
mirror-using studies and the modest number of these studies (N = 25), the mean size of the effect
on agency is higher in these studies (д = 1.07, 95% CI [0.35; 1.78]) than in those without mirrors
(д = 0.80, 95% CI [0.12; 1.47]).
  Recent evidence suggests that virtual embodiment of different-gendered avatars can have spe-
cific behavioral effects, but that the effects are not consistently aligned stereotypically with the
gender of the avatar (e.g., the authors observed an increase in selfishness for both male and fe-
male gender swaps [19]; however, with an increased effect for women embodying a male avatar).
Peck et al. [134] successfully demonstrated induction of a stereotype threat, wherein female partic-
ipants were embodying male avatars, hence demonstrating a stereotype lift considering working
memory. Schwind et al. [158] reported subjective differences attributable to gender, from embody-
ing an avatar with gender-swapped hands. In this study, females reported less acceptance of male
hands, compared to males who accepted and experienced presence with avatar hands of both gen-
ders [158]. Our data suggest that gender likely does not affect the likelihood that participants will


     ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 26 / 42 -->

```text
76:26                                                                       A. Mottelson et al.


accept a virtual body as their own. There is, therefore, little validity gain from restricting recruit-
ment to one gender only if it is not strictly imperative given the domain of study, such as through
mismatch between the participant’s and an avatar’s gender. There might still be practical benefits
from recruitment of one gender related to avatar creation, rigging, and for adjusting body-worn
equipment. We further encourage researchers to consider the underrepresented in empirical VR
research, which, however, appears to have a more fair representation for embodiment VR research
compared to other areas of VR research [138]. To this end, Peck et al. [138] report 39% female par-
ticipants in the IEEE VR conference proceedings, while our data show 49.7% female participants.
  In characterizing the commonly used embodiment questionnaires, their origins, and related sta-
tistical treatment, we found that the practices of measuring subjective embodiment are hetero-
geneous and rarely follow validated procedures. Furthermore, the analysis showed that the em-
ployed questionnaires in most cases refer to questions developed for the RHI. On these bases, we
see great scientific potential in validating these processes and in requiring scientists to adhere to
stricter protocols when working with subjective embodiment. Some recent work has tackled this
issue (e.g., [135, 154]), but for practical reasons, we too see great potential in developing cross-
laboratory validated scales with few items.
  We found that participants tended to report higher levels of agency than body ownership for
virtual bodies; that is, participants generally feel in control of virtual avatars, but less so experience
the avatars’ bodies as theirs. While this potentially could be an artifact of the employed psychome-
tric tool—this could also point to various areas of profitable improvements in tracking equipment
and kinematics algorithms to foster body ownership on par with agency scores in BOI studies.

6.2  Issues Facing Embodiment VR Research
A critical assessment of the embodiment VR research shows multiple areas where there are oppor-
tunities to improve empirical practices related to study design, recruitment of participants, and
dissemination of data. We have documented a variety of empirical issues within the literature.
These relate to subjective instruments and their analysis, small sample sizes, and terminological
confusion. Below, we point towards opportunities for further advancing the scientific quality of
BOI research.

   6.2.1  Replication and Open Science. We examined correlations of subjective embodiment scores
to other dependent measurements, grouped into subjective, cognitive, motor, and physiological
ones. Some of these links have been thoroughly investigated and replicated; however, many such
connections to embodiment still hold potential for scientific confirmation.
  Experimental virtual body manipulations (e.g., changes to visuo-motor synchrony, avatar per-
spective, or the limbs) influence subjective embodiment scores, and the literature offers abundant
documentation of this. Likewise, such manipulations’ effects on subsequent behavior and social
attitudes are frequently referred to. Yet, these effects are rarely replicated. In most cases, any given
specific finding is reported once in the entire literature. Hence, while there is solid empirical sup-
port for the methodology behind BOIs, the specific behavioral and cognitive effects identified lack
definitive verification (most findings are one-of, see Table 4). This is especially troublesome in light
of the relatively low power that tends to characterize studies in this field. To this end, the long list
of variables empirically found to connect to embodiment shown in Table 4 could serve as a starting
point for initiating replication attempts to verify embodiment correlates.
   Pre-registration is considered methodologically necessary in many disciplines, most notably psy-
chology, but is currently rarely used in BOI research (we found 26 pre-registrations on Open Sci-
ence Framework by querying (“embodiment” OR “body ownership”) AND (“virtual reality”
OR “VR”); 18 of these were from 2021 and 2022). To this end, even as pre-registration counts are still


ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 27 / 42 -->

```text
Body Ownership Illusions in VR                                                           76:27


modest, the recent increase provides aspirations for adoption of open science practices within BOI
research. Increasing use of preregistration in BOI research would not only alleviate concerns about
statistical practices, but could also serve as a repository for description and reason for procedures
and tasks that could aid standardization.
  The BOI field as a whole could benefit from stricter scientific rigor, for mitigating problematic
publication practices. For instance, adopting standards from open science will yield benefits. These
standards prescribe pre-registering hypotheses, specifying the analysis plans, and conducting a
priori power analysis for estimation of the required participant numbers.
  Any part of empirical science can gain from adopting open science principles. VR studies and
BOI in particular, are well suited for conducting replication studies, as study procedures, group
assignment, data collection, and so on. can be encoded into the application. This way, researchers
across labs can share materials, and expect to collect consistent data. We, therefore, foresee that VR
technology, and BOIs in particular can be a driver for replication attempts in behavioral science.

   6.2.2  Measures. Our review has documented the disparate use of subjective measures in embod-
iment research to quantify (sub-dimensions) of embodiment. While standardized questionnaires
are emerging (e.g., Peck and Gonzalez-Franco [135], Roth and Latoschik [154]) the prevalence of
ad-hoc measures, or adaptations that do not follow original sources is high. Picking suitable subjec-
tive measures for quantifying embodiment is non-trivial, taking, among other things, procedures,
time, language, and experimental design into consideration. To this end Table 2 can serve as inspi-
ration, showing the complexity, standardization, and suggested statistical treatment for a number
of commonly used scales.
   6.2.3  Power. For the weighted mean effect size of д = 0.50 for subjective body ownership that
we estimated in our meta-analysis across embodiment/disembodiment studies and a power of 0.95,
there must be 25 participants per group (or more, depending on the specifics of the power analysis).
Such estimations contrast the documented median employed participant count of 30 (per study, per
group the median is 20). Note that while this participant count would normally be considered a
precondition for declaring significant effects on body ownership, it is not necessarily enough to
uncover subsequent behavioral or cognitive effects produced by changes to the virtual body. Recent
studies have successfully recruited large samples by conducting remote VR studies [121, 122, 151].

7  LIMITATIONS

In most respects, the data obtained from the 111 articles demonstrate heterogeneity; procedures,
methods, measurements, scales, and statistical analyses vary greatly between studies. Therefore,
even providing descriptive statistics that encompass this corpus has required a fair amount of
sophistication in computational techniques (e.g., for estimating means and rendering the scales
compatible). Conclusions drawn from this material should take into account that the source data
represent diverse scientific practices and have been post-processed for visualization purposes.
  Most commonly, subjective embodiment scores are collected as ordinal data. Describing said
data with means and standard deviations or conducting parametric statistical tests is not recom-
mended, since the assumptions behind such analyses (e.g., as to normality) are violated. For our
meta-analysis, we nonetheless estimated means of embodiment scores from the available statis-
tics and conducted some parametric tests, when deemed necessary. We chose this method because
estimating medians from a mean score provides less precision than doing the reverse.





     ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 28 / 42 -->

```text
76:28                                                                       A. Mottelson et al.


APPENDICES

A  STATISTICAL PRACTICE
A.1  Estimation of Means and Standard Deviations

For comparison across studies and for computing effect sizes, we normalized the descriptive sta-
tistics. Where means (M) and standard deviations (SD values) were reported, we used them in the
meta-analysis directly; otherwise, we converted the standard-error (SE) values reported into SDs:       √
SD = SE ×  N. As the availability of descriptive statistics allows, we provide per-study estimates
of means and SDs for each common variable here, using the methods formulated by Wan et al.
[183]. For instance, if the first and third interquartile range, Q1 and Q3, are known, M and SD are
obtained via the following estimations (note that the source scale’s min. and max. values are used
for this operation):
                         + max + 2Med + 2Q1 + 2Q3               M ≈min                                              ,                               (1)
                                            8
                         max −min       Q3 −Q1                   SD ≈          +                              .                             (2)
                             4Φ−1  n−0.375n+0.25    4Φ−1  0.75n−0.125n+0.25

A.2  Mean-of-means Estimates

To provide a field-wide overview of the response ranges for the most commonly employed embod-
iment variables, we plot estimated means across all studies for the four most typical constructs
(see Figure 5). For compatibility, measurements have been scaled to the [−3; 3] range as necessary:
x = (b −a) maxx−min(x)(x)−min(x) + a, where min(x) and max(x) are the limits of the source scale and
where a and b are −3 and 3, respectively. This scale was chosen as its commonplace throughout
BOI research (hence not requiring any scaling), and as it offers a compelling direct explanation as
0 represents neither embodied or disembodied.

A.3  Outliers
Examining the magnitude of the embodiment manipulations’ effects on the central dimension of
interest, body ownership, yields a weighted mean Hedges’ д of 0.50. Most studies (94%) fall within
the range of −0.25 > д < 2.0 (see Figure 7). Since only five articles present effect sizes outside
this range, we introduced a simple outlier criterion of д > 2.0 to reduce the distorting influence of
individual studies’ extreme values on the results. For the sake of completeness, outliers are retained
in the plots, but they are filtered out for reporting of descriptive statistics. To limit the influence
of individual findings further, we report weighted means whenever possible, with each study’s
statistical power determining the weight (computed by the R function stats::power.t.test).





ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 29 / 42 -->

```text
Body Ownership Illusions in VR                                                           76:29





    Fig. 7. A histogram of the effect sizes of the embodiment manipulations’ effect on body ownership.

B  RISK OF PUBLICATION BIAS
   Publication bias. To assess the possibility of publication bias, we looked at funnel plots, con-
structed for each of four key embodiment constructs using the R package metafor [180] (see Fig-
ure 8). Asymmetry in funnel plots that compare effect size and study precision can suggest publi-
cation bias. Consistently, we found no evidence of systematic publication bias for any of the four
funnel plots; some few studies showing large effect sizes are most prominent towards the lower
end of standard errors; we deal with such extreme effect sizes as outliers, as described above.
  For further assessing the risk of publication bias, we employed weight-function modeling [179]
using the R package weightr [29]. Here, the fit of a publication-bias-adjusted model is compared
to that of an unadjusted model. An increase in fit may be indicative of publication bias. The weight-
function modeling did not uncover an increase in fit; hence, do not find evidence for publication
bias; χ2(1, N = 77) = 0.36, p = 0.55.
  We inspected the heterogeneity for study effects for body ownership and agency, respectively.
The data showed Higgin’s and Thompson’s I 2 = 17% for body ownership and I 2 = 79% for agency;
for body ownership this is considered low heterogeneity and, conversely, for agency it is considered
substantial heterogeneity. Interestingly, body ownership scores showed a substantial reduction in
variation compared to agency, while it should also be noted that agency scores in general are higher
compared to body ownership (i.e., it appears easier to induce participant control over virtual limbs,
than creating the illusion that the virtual body is theirs).

   Publication year. Our results show no significant correlation between publication year and effect
size; Pearson’s r (75) = 0.03, p = 0.81.

  Between- versus within-subjects design. Our results indicate that BOIs emerge both in within-
subjects experiment designs (д = 0.97, 95% CI [0.64; 1.31]) and in between-subjects designs (д =
0.45, 95% CI [0.21; 0.69]).
  We did find a significantly larger effect of embodiment scores for within-subjects designs, of
about twice the size; t(43.5) = 2.6, p = 0.01. This likely stems from the fact that visuo-motor asyn-
chrony (i.e., incongruence between the participant’s and the avatar’s movements), which is the
most effective manipulation for body ownership, is frequently a within-subjects condition. When
comparing only manipulations of visuo-motor synchrony, we did not find a significant difference
in body ownership effect sizes across experimental designs; t(16.1) = −0.6, p = 0.53.


     ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 30 / 42 -->

```text
76:30                                                                       A. Mottelson et al.





Fig. 8. Funnel plots for VR BOI studies, comparing the effect size (Hedges’ д) and precision (standard error),
for the four main subjective aspects of embodiment measured: agency, body ownership, mirror body, and
two bodies.


C COMMON SUBJECTIVE MEASUREMENTS OF EMBODIMENT IN VR
Here, we summarize the six most commonly used questionnaires for measuring embodiment (see
Table 2, that also summarizes three additional, less commonly employed, questionnaires).

   C.0.1  Botvinick and Cohen (1998). In a seminal article, Botvinick and Cohen [21] presented the
RHI. In the RHI, tactile stimuli are introduced synchronously to an artificial rubber hand and (hid-
den behind a screen) the subject’s real hand. The participants (N = 10) anchored the touches at
the location of the rubber hand. This indicates interactions between vision, touch, and proprio-
ception. The authors investigated the phenomenon by using a questionnaire with nine items, of
which three were considered likely to evoke affirmative responses (e.g., “I felt as if the rubber hand
were my hand”). The questions were administered in random order, on a seven-step [−3; 3] visual-
analogue scale from “agree strongly” to “disagree strongly.” Although the article does not present
any specific guidance on statistical analysis, single-item means and p-values are reported.

   C.0.2  Lenggenhager et al. (2007). In their article “Video Ergo Sum”, Lenggenhager et al. [95]
described two experiments (N = 14, 14) wherein participants experienced themselves through an


ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 31 / 42 -->

```text
Body Ownership Illusions in VR                                                           76:31


HMD from a distance, in a so-called out-of-body experience. Using synchronous and asynchronous
visual and tactile stimulation to the subject’s own, foreign, and fake bodies, the authors showed a
disruption of spatial unity between the self and the body. In addition to objective measurements
of drift, the authors collected responses to a subjective questionnaire on “self-attribution of the
virtual character” adapted from the work of Botvinick and Cohen [21]. The scores reported were
analyzed for each of the seven items (which employ a seven-step scale from −3 to 3) by means of
parametric repeated-measures ANOVA and subsequent t-tests. The first three questions, related
to touch and “my body,” show significant differences for the synchrony of stroking.

   C.0.3  Longo et al. (2008). Taking a psychometric approach, Longo et al. [102] investigated the
experience of having a body during the RHI. Working with transcripts of qualitative reports from
five participants, they developed an initial set of 27 items. Participants in this between-subjects
study (N = 131) were exposed to two conditions—synchronous and asynchronous tactile stimuli—
and then rated their agreement with the 27 randomly ordered items on a 7-point scale from −3 (for
strong disagreement) to +3 (for strong agreement). Principal-component analysis (PCA) revealed
four major components of having a body, with embodiment being the primary one. Subsequent
analysis identified 10 embodiment-related items (e.g., “It seemed like the rubber hand was part of
my body”) as representing three subcomponents: ownership, location, and agency. Results from
ANOVA testing showed a significant effect connected with the condition (synchrony) and for the
components, along with an interaction of the two.

   C.0.4  Banakou et al. (2013) and Banakou and Slater (2014). Two influential BOI studies by
Banakou and colleagues [5, 8] showed that the illusion of ownership over a virtual body yields con-
sequences for subsequent behavior—specifically, expression of child-like attitudes and a changed
manner of speech. Alongside objective measurements of these behavior changes, the authors col-
lected subjective embodiment data. Both studies applied four single-item embodiment variables:
VRBody/MyBody, Mirror, Features, and TwoBodies), with the latter two affording consistency checks.
The 2014 article cites the questionnaire used in the aforementioned RHI study as inspiration, and
an item addressing agency was included. Beyond these four or five constructs, the researchers
utilized a range of study-specific questions related to age perception and room size. While these
studies were not intended to recommend a standardized way of measuring embodiment, they have
inspired many scholars, who, accordingly, often refer to them in relation to their own embodiment
questionnaires; 15 embodiment articles in our review feature such references. The items from both
studies use a range of −3 (“strongly disagree”) to +3 (“strongly agree”). The results in the 2013 study
were obtained with a non-parametric Friedman test, while the second study employed ordinal lo-
gistic regression.

   C.0.5  Gonzalez-Franco and Peck (2018). More recently, Gonzalez-Franco and Peck [48] pre-
sented a questionnaire on VR avatar embodiment, informed by a review of previous experiments’
embodiment questionnaires that reference the work of Botvinick and Cohen [21]. The authors
found six types of questions to be frequently used in BOI research: items on (1) ownership,
(2) agency, (3) tactile sensations, (4) location, (5) appearance, and (6) response, with classes 1, 2,
and 4 being the most important. The resulting questionnaire consists of 25 items, with random ad-
ministration order, divided among the six constructs. The common practice of applying a 7-point
scale from “strongly disagree” (−3) to “strongly agree” (3) was followed. The authors recommended
analyzing responses using non-parametric tests for either sum-of-scores or principal-component
scores. A recently published validation of the scale [135] further improves this instrument.

   C.0.6  Other Practices Related to BOIs. Several articles about embodiment in VR by Martini and
colleagues [23, 111, 112] have used a one-question operationalization of virtual arm ownership:


     ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 32 / 42 -->

```text
76:32                                                                       A. Mottelson et al.


“Did you feel as if the virtual right arm was your own right arm?” (the most recent study used a
similar question about agency as well). In this setting, participants answer the question verbally,
using a 7-point (1–7) Likert scale (“not at all” to “yes, completely/totally”), in a repeated-measures
design with several within-subjects conditions. The data analysis uses a non-parametric Friedman
test after which single comparisons are computed by means of Wilcoxon tests.
   Recently, Roth and Latoschik [154] presented a three-dimensional 12-item questionnaire on em-
bodiment, specifically targeted at VR. Through three studies and a validation study, the authors
derived their final set of questions and constructs for measuring embodiment in VR. Items are an-
swered on a 7-point scale, and the recommended analysis approach involves means of items and
subsequent parametric testing with ANOVA. On account of its recency, the questionnaire was not
employed in any studies in our survey.
   In a full-body VR illusion incorporating three binary between-subjects manipulations—of per-
spective, movement, and touch—Slater et al. [165] collected subjective measurements of embodi-
ment (in addition to heart-rate deceleration) from 24 male participants. After the procedure, the
experimenters posed eight questions about body ownership, on various aspects of body perspec-
tive, touch, and response to a virtual threat. The responses, on an 11-point scale of 0–10 (“not at
all” to “very much”), were then mapped to five bins: Very Low (0), Low (1–3), Medium (4–6), High
(7–9), and Very High (10). The mapping afforded applying a proportional-odds cumulative logit
model (used in addition to parametric ANOVA).

ACKNOWLEDGMENTS

We would like to thank Sandra Lihn Nielsen, Valdemar Aksel Stenberdt, and Sara Klingenberg
for their efforts in sourcing data for the article. We also thank Anna Shefl for proofreading the
manuscript.

REFERENCES

    [1] Sil Aarts, Marjan Van Den Akker, and Bjorn Winkens. 2014. The importance of effect sizes. The European Journal
        of General Practice 20, 1 (2014), 61–64. DOI:https://doi.org/10.3109/13814788.2013.818655
    [2] Parastoo Abtahi, Mar Gonzalez-Franco, Eyal Ofek, and Anthony Steed. 2019. I’m a giant: Walking in large virtual
       environments at high speed gains. In Proceedings of the 2019 CHI Conference on Human Factors in Computing Systems
        (CHI’19). Association for Computing Machinery. DOI:https://doi.org/10.1145/3290605.3300752
    [3] Maryam Alimardani, Shuichi Nishio, and Hiroshi Ishiguro. 2016. The importance of visual feedback design in BCIs;
       from embodiment to motor imagery learning. PLOS ONE 11, 9 (2016), e0161945. DOI:https://doi.org/10.1371/journal.
       pone.0161945
    [4] Laura Aymerich-Franch, René F. Kizilcec, and Jeremy N. Bailenson. 2014. The relationship between virtual self
        similarity and social anxiety. Frontiers in Human Neuroscience 8 (2014), 944. DOI:https://doi.org/10.3389/fnhum.
       2014.00944
    [5] Domna Banakou, Raphaela Groten, and Mel Slater. 2013. Illusory ownership of a virtual child body causes overesti-
       mation of object sizes and implicit attitude changes. Proceedings of the National Academy of Sciences 110, 31 (2013),
       12846–12851. DOI:https://doi.org/10.1073/pnas.1306779110
    [6] Domna Banakou, Parasuram D. Hanumanthu, and Mel Slater. 2016. Virtual embodiment of white people in a black
        virtual body leads to a sustained reduction in their implicit racial bias. Frontiers in Human Neuroscience 10 (2016),
        601. DOI:https://doi.org/10.3389/fnhum.2016.00601
    [7] Domna Banakou, Sameer Kishore, and Mel Slater. 2018. Virtually being einstein results in an improvement in cogni-
        tive task performance and a decrease in age bias. Frontiers in Psychology 9 (2018), 917. DOI:https://doi.org/10.3389/
       fpsyg.2018.00917
    [8] Domna Banakou and Mel Slater. 2014. Body ownership causes illusory self-attribution of speaking and influences
       subsequent real speaking. Proceedings of the National Academy of Sciences 111, 49 (2014), 17678–17683. DOI:https:
        //doi.org/10.1073/pnas.1414936111
    [9] Domna Banakou and Mel Slater. 2017. Embodiment in a virtual body that speaks produces agency over the speaking
       but does not necessarily influence subsequent real speaking. Scientific Reports 7, 1 (2017), 14227. DOI:https://doi.org/
       10.1038/s41598-017-14620-5


ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 33 / 42 -->

```text
Body Ownership Illusions in VR                                                           76:33


  [10] Itxaso Barberia, Ramon Oliva, Pierre Bourdin, and Mel Slater. 2018. Virtual mortality and near-death experience
        after a prolonged exposure in a shared virtual reality may lead to positive life-attitude changes. PLOS ONE 13,
       11 (2018), 1–31. DOI:https://doi.org/10.1371/journal.pone.0203358
  [11] Baptiste Barbot and James C. Kaufman. 2020. What makes immersive virtual reality the ultimate empathy machine?
       Discerning the underlying mechanisms of change. Computers in Human Behavior 111 (2020), 106431. DOI:https:
       //doi.org/10.1016/j.chb.2020.106431
  [12] Joseph Bates. 1992. Virtual reality, art, and entertainment. Presence: Teleoperators and Virtual Environments 1,
       1 (1992), 133–138. DOI:https://doi.org/10.1162/pres.1992.1.1.133
  [13] Antoine Bechara, Hanna Damasio, and Antonio R. Damasio. 2000. Emotion, decision making and the orbitofrontal
        cortex. Cerebral Cortex 10, 3 (03 2000), 295–307. DOI:https://doi.org/10.1093/cercor/10.3.295
  [14] Robin Bekrater-Bodmann, Jens Foell, Martin Diers, Sandra Kamping, Mariela Rance, Pinar Kirsch, Jørg Trojan, Xaver
       Fuchs, Felix Bach, Hüseyin Kemal Çakmak, Heiko Maaß, and Herta Flor. 2014. The importance of synchrony and
       temporal order of visual and tactile input for illusory limb ownership experiences—an fMRI study applying virtual
         reality. PLOS ONE 9, 1 (2014), e87013. DOI:https://doi.org/10.1371/journal.pone.0087013
  [15] Joanna Bergström, Aske Mottelson, Andreea Muresan, and Kasper Hornbæk. 2019. Tool extension in human-
      computer interaction. In Proceedings of the 2019 CHI Conference on Human Factors in Computing Systems (CHI’19).
       Association for Computing Machinery, 1–11. DOI:https://doi.org/10.1145/3290605.3300798
  [16] Ilias Bergstrøm, Konstantina Kilteni, and Mel Slater. 2016. First-person perspective virtual body posture influences
        stress: A virtual reality body ownership study. PLOS ONE 11, 2 (2016), e0148060. DOI:https://doi.org/10.1371/journal.
       pone.0148060
  [17] Olaf Blanke, Theodor Landis, Laurent Spinelli, and Margitta Seeck. 2004. Out-of-body experience and autoscopy of
       neurological origin. Brain 127, 2 (2004), 243–258. DOI:https://doi.org/10.1093/brain/awh040
  [18] Corey J. Bohil, Bradly Alicea, and Frank A. Biocca. 2011. Virtual reality in neuroscience research and therapy. Nature
       Reviews Neuroscience 12, 12 (2011), 752–762. DOI:https://doi.org/10.1038/nrn3122
  [19] Elena Bolt, Jasmine T. Ho, Marte Roel Lesur, Alexander Soutschek, Philippe N. Tobler, and Bigna Lenggenhager.
       2021. Effects of a virtual gender swap on social and temporal decision-making. Scientific Reports 11, 1 (2021), 1–15.
       DOI:https://doi.org/10.1038/s41598-021-94869-z
  [20] D. Borland, T. Peck, and M. Slater. 2013. An evaluation of self-avatar eye movement for virtual embodiment. IEEE
       Transactions on Visualization and Computer Graphics 19, 4 (2013), 591–596. DOI:https://doi.org/10.1109/TVCG.2013.
       24
  [21] Matthew Botvinick and Jonathan Cohen. 1998. Rubber hands “feel” touch that eyes see. Nature 391, 6669 (1998),
       756–756. DOI:https://doi.org/10.1038/35784
  [22] Pierre Bourdin, Itxaso Barberia, Ramon Oliva, and Mel Slater. 2017. A virtual out-of-body experience reduces fear
        of death. PLOS ONE 12, 1 (01 2017), e0169343. DOI:https://doi.org/10.1371/journal.pone.0169343
  [23] Pierre Bourdin, Matteo Martini, and Maria V. Sanchez-Vives. 2019. Altered visual feedback from an embodied avatar
       unconsciously influences movement amplitude and muscle activity. Scientific Reports 9, 1 (2019), 1–9. DOI:https:
       //doi.org/10.1038/s41598-019-56034-5
  [24] S. Bovet, H. G. Debarba, B. Herbelin, E. Molla, and R. Boulic. 2018. The critical role of self-contact for embodiment
        in virtual reality. IEEE Transactions on Visualization and Computer Graphics 24, 4 (2018), 1428–1436. DOI:https:
       //doi.org/10.1109/TVCG.2018.2794658
  [25] Bill Brewer. 1995. Bodily awareness and the self. In Proceedings of the Body and the Self. Jose Luis Bermudez, An-
      thony J. Marcel, and Naomi M. Eilan (Eds.), MIT, Cambridge, MA, 291–303.
  [26] Victòria Brugada-Ramentol, Ivar Clemens, and Gonzalo G. de Polavieja. 2019. Active control as evidence in favor of
       sense of ownership in the moving virtual hand illusion. Consciousness and Cognition 71 (2019), 123–135. DOI:https:
       //doi.org/10.1016/j.concog.2019.04.003
  [27] Dalila Burin, Konstantina Kilteni, Marco Rabuffetti, Mel Slater, and Lorenzo Pia. 2019. Body ownership increases
       the interference between observed and executed movements. PLOS ONE 14, 1 (2019), e0209899. DOI:https://doi.org/
       10.1371/journal.pone.0209899
  [28] Maria Christofi, Despina Michael-Grigoriou, and Christos Kyrlitsias. 2020. A virtual reality simulation of drug users’
       everyday life: The effect of supported sensorimotor contingencies on empathy. Frontiers in Psychology 11 (2020),
       1242. DOI:https://doi.org/10.3389/fpsyg.2020.01242
  [29] Kathleen M. Coburn and Jack L. Vevea. 2019. weightr: Estimating Weight-Function Models for Publication Bias. Re-
        trieved from https://CRAN.R-project.org/package=weightr. Accessed 1 June 2020.
  [30] Frederique de Vignemont. 2017. Agency and Bodily Ownership: The Bodyguard Hypothesis. MIT, Cambridge, MA,
       217–238.
  [31] Martin Dobricki and Stephan de la Rosa. 2013. The structure of conscious bodily self-perception during full-body
        illusions. PLOS ONE 8, 12 (2013), e83840. DOI:https://doi.org/10.1371/journal.pone.0083840



     ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 34 / 42 -->

```text
76:34                                                                       A. Mottelson et al.


  [32] Gerald M. Edelman. 2006. Second Nature: Brain Science and Human Knowledge. Yale University Press.
  [33] Line Lindhardt Egsgaard, Laura Petrini, Giselle Christoffersen, and Lars Arendt-Nielsen. 2011. Cortical responses
        to the mirror box illusion: A high-resolution EEG study. Experimental Brain Research 215, 3–4 (2011), 345–357.
       DOI:https://doi.org/10.1007/s00221-011-2902-x
  [34] H. Henrik Ehrsson. 2012. The Concept of Body Ownership and Its Relation to Multisensory Integration. MIT Press.
  [35] H. Henrik Ehrsson, Charles Spence, and Richard E. Passingham. 2004. That’s my hand! Activity in [the] premotor
       cortex reflects feeling of ownership of a limb. Science 305, 5685 (2004), 875–877. DOI:https://doi.org/10.1126/science.
       1097011
  [36] Panteleimon Ekkekakis and James A. Russell. 2013. Untangling the Terminological Gordian Knot. Cambridge Univer-
        sity Press. DOI:https://doi.org/10.1017/CBO9780511820724.004
  [37] Caroline J. Falconer, Mel Slater, Aitor Rovira, John A. King, Paul Gilbert, Angus Antley, and Chris R. Brewin. 2014.
      Embodying compassion: A virtual reality paradigm for overcoming excessive self-criticism. PLOS ONE 9, 11 (2014),
       e111933. DOI:https://doi.org/10.1371/journal.pone.0111933
  [38] Tiare Feuchtner and Jörg Müller. 2017. Extending the body for interaction with reality. In Proceedings of the 2017
      CHI Conference on Human Factors in Computing Systems (CHI’17). Association for Computing Machinery, 5145–5157.
       DOI:https://doi.org/10.1145/3025453.3025689
  [39] Tiare Feuchtner and Jörg Müller. 2018. Ownershift: Facilitating Overhead Interaction in Virtual Reality with an
       Ownership-Preserving Hand Space Shift. Association for Computing Machinery, 31–43. DOI:https://doi.org/10.1145/
       3242587.3242594
  [40] Daniel Freeman, Polly Haselton, Jason Freeman, Bernhard Spanlang, Sameer Kishore, Emily Albery, Megan Denne,
      Poppy Brown, Mel Slater, and Alecia Nickless. 2018. Automated psychological therapy using immersive virtual real-
        ity for treatment of fear of heights: A single-blind, parallel-group, randomised controlled trial. The Lancet Psychiatry
         5, 8 (2018), 625–632. DOI:https://doi.org/10.1016/S2215-0366(18)30226-8
  [41] Doron Friedman, Rodrigo Pizarro, Keren Or-Berkers, Solène Neyret, Xueni Pan, and Mel Slater. 2014. A method for
       generating an illusion of backwards time travel using immersive virtual reality-an exploratory study. Frontiers in
       Psychology 5 (2014), 943. DOI:https://doi.org/10.3389/fpsyg.2014.00943
  [42] M. Fusaro, G. Tieri, and S. M. Aglioti. 2019. Influence of cognitive stance and physical perspective on subjective and
      autonomic reactivity to observed pain and pleasure: An immersive virtual reality study. Consciousness and Cognition
       67 (2019), 86–97. DOI:https://doi.org/10.1016/j.concog.2018.11.010
  [43] Shaun Gallagher. 2000. Philosophical conceptions of the self: Implications for cognitive science. Trends in Cognitive
        Sciences 4, 1 (2000), 14–21. DOI:https://doi.org/10.1016/S1364-6613(99)01417-5
  [44] Shaun Gallagher. 2006. How the Body Shapes the Mind. Oxford University Press.
  [45] Shaun Gallagher and Anthony J. Marcel. 1999. The self in contextualized action. Journal of Consciousness Studies 6,
       4 (1999), 4–30.
  [46] Henrique Galvan Debarba, Sidney Bovet, Roy Salomon, Olaf Blanke, Bruno Herbelin, and Ronan Boulic. 2017. Char-
        acterizing first and third person viewpoints and their alternation for embodied interaction in virtual reality. PLOS
     ONE 12, 12 (2017), e0190109. DOI:https://doi.org/10.1371/journal.pone.0190109
  [47] Mar Gonzalez-Franco and Jaron Lanier. 2017. Model of illusions and virtual reality. Frontiers in Psychology 8 (2017).
       DOI:https://doi.org/10.3389/fpsyg.2017.01125
  [48] Mar Gonzalez-Franco and Tabitha C. Peck. 2018. Avatar embodiment: Towards a standardized questionnaire. Fron-
         tiers in Robotics and AI 5 (2018), 74. DOI:https://doi.org/10.3389/frobt.2018.00074
  [49] Cristina Gonzalez-Liencres, Luis E. Zapata, Guillermo Iruretagoyena, Sofia Seinfeld, Lorena Perez-Mendez, Jorge
       Arroyo-Palacios, David Borland, Mel Slater, and Maria V. Sanchez-Vives. 2020. Being the victim of intimate partner
       violence in virtual reality: First- versus third-person perspective. Frontiers in Psychology 11 (2020), 820. DOI:https:
       //doi.org/10.3389/fpsyg.2020.00820
  [50] Mar González-Franco, Daniel Pérez-Marcos, Bernhard Spanlang, and Mel Slater. 2010. The contribution of real-time
       mirror reflections of motor actions on virtual body ownership in an immersive virtual environment. In Proceedings
        of the 2010 IEEE Virtual Reality Conference (VR). IEEE, 111–114. DOI:https://doi.org/10.1109/VR.2010.5444805
  [51] Klaudia Grechuta, Jelena Guga, Giovanni Maffei, Belen Rubio Ballester, and Paul F. M. J. Verschure. 2017. Visuotactile
        integration modulates motor performance in a perceptual decision-making task. Scientific Reports 7, 1 (2017), 3333.
       DOI:https://doi.org/10.1038/s41598-017-03488-0
  [52] Klaudia Grechuta, Laura Ulysse, Belén Rubio Ballester, and Paul F. M. J. Verschure. 2019. Self beyond the body:
       Action-driven and task-relevant purely distal cues modulate performance and body ownership. Frontiers in Human
       Neuroscience 13 (2019), 91. DOI:https://doi.org/10.3389/fnhum.2019.00091
  [53] Michael Gusenbauer and Neal R. Haddaway. 2020. Which academic search systems are suitable for systematic re-
       views or meta-analyses? Evaluating retrieval qualities of Google scholar, PubMed, and 26 other resources. Research
        Synthesis Methods 11, 2 (2020), 181–217. DOI:https://doi.org/10.1002/jrsm.1378



ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 35 / 42 -->

```text
Body Ownership Illusions in VR                                                           76:35


  [54] Shlomi Haar, Guhan Sundar, and A. Aldo Faisal. 2021. Embodied virtual reality for the study of real-world motor
        learning. PLOS ONE 16, 1 (2021), 1–17. DOI:https://doi.org/10.1371/journal.pone.0245717
  [55] Patrick Haggard and Manos Tsakiris. 2009. The experience of agency: Feelings, judgments, and responsibility. Cur-
        rent Directions in Psychological Science 18, 4 (2009), 242–246. DOI:https://doi.org/10.1111/j.1467-8721.2009.01644.x
  [56] Catherine Hamilton-Giachritsis, Domna Banakou, Manuela Garcia Quiroga, Christos Giachritsis, and Mel Slater.
       2018. Reducing risk and improving maternal perspective-taking and empathy using virtual embodiment. Scientific
       Reports 8, 1 (2018), 1–10. DOI:https://doi.org/10.1038/s41598-018-21036-2
  [57] Masayuki Hara, Polona Pozeg, Giulio Rognini, Takahiro Higuchi, Kazunobu Fukuhara, Akio Yamamoto, Toshiro
       Higuchi, Olaf Blanke, and Roy Salomon. 2015. Voluntary self-touch increases body ownership. Frontiers in Psychol-
      ogy 6 (2015), 1509. DOI:https://doi.org/10.3389/fpsyg.2015.01509
  [58] Béatrice S. Hasler, Bernhard Spanlang, and Mel Slater. 2017. Virtual race transformation reverses racial in-group
        bias. PLOS ONE 12, 4 (2017), e0174965. DOI:https://doi.org/10.1371/journal.pone.0174965
  [59] Larry V. Hedges. 1981. Distribution theory for Glass’s estimator of effect size and related estimators. Journal of
       Educational Statistics 6, 2 (1981), 107–128. DOI:https://doi.org/10.3102/10769986006002107
  [60] Chris Heinrich, Matthew Cook, Tobias Langlotz, and Holger Regenbrecht. 2020. My hands? Importance of person-
        alised virtual hands in a neurorehabilitation scenario. Virtual Reality 25, 2 (2020), 1–18. DOI:https://doi.org/10.1007/
       s10055-020-00456-4
  [61] Lukas Heydrich, Trevor Dodds, Jane Aspell, Bruno Herbelin, Heinrich Buelthoff, Betty Mohler, and Olaf Blanke.
       2013. Visual capture and the experience of having two bodies—evidence from two different virtual reality techniques.
        Frontiers in Psychology 4 (2013), 946. DOI:https://doi.org/10.3389/fpsyg.2013.00946
  [62] Matt C. Howard. 2017. A meta-analysis and systematic literature review of virtual reality rehabilitation programs.
      Computers in Human Behavior 70 (2017), 317–327. DOI:https://doi.org/10.1016/j.chb.2017.01.013
  [63] Robert J. K. Jacob, Audrey Girouard, Leanne M. Hirshfield, Michael S. Horn, Orit Shaer, Erin Treacy Solovey, and
       Jamie Zigelbaum. 2008. Reality-based interaction: A framework for post-WIMP interfaces. In Proceedings of the
      SIGCHI Conference on Human Factors in Computing Systems (CHI’08). Association for Computing Machinery, 201–
        210. DOI:https://doi.org/10.1145/1357054.1357089
  [64] Dongsik Jo, Kangsoo Kim, Gregory F. Welch, Woojin Jeon, Yongwan Kim, Ki-Hong Kim, and Gerard Jounghyun
      Kim. 2017. The impact of avatar-owner visual similarity on body ownership in immersive virtual reality. In Proceed-
        ings of the 23rd ACM Symposium on Virtual Reality Software and Technology (VRST’17). Association for Computing
       Machinery, 2 pages. DOI:https://doi.org/10.1145/3139131.3141214
  [65] Joohee Jun, Myeongul Jung, So-Yeon Kim, and Kwanguk (Kenny) Kim. 2018. Full-body ownership illusion can
      change our emotion. In Proceedings of the 2018 CHI Conference on Human Factors in Computing Systems (CHI’18).
       Association for Computing Machinery, Paper 601. DOI:https://doi.org/10.1145/3173574.3174175
  [66] Myeongul Jung, Jejoong Kim, and Kwanguk Kim. 2020. Measuring recognition of body changes over time: A human–
      computer interaction tool using dynamic morphing and body ownership illusion. PLOS ONE 15, 9 (2020), e0239322.
       DOI:https://doi.org/10.1371/journal.pone.0239322
  [67] Sungchul Jung, Gerd Bruder, Pamela J. Wisniewski, Christian Sandor, and Charles E. Hughes. 2018. Over my hand:
      Using a personalized hand in VR to improve object size estimation, body ownership, and presence. In Proceedings
        of the 2018 ACM Symposium on Spatial User Interaction (SUI’18). Association for Computing Machinery, 60–68.
       DOI:https://doi.org/10.1145/3267782.3267920
  [68] Sungchul Jung, Christian Sandor, Pamela J. Wisniewski, and Charles E. Hughes. 2017. RealME: The influence of
      body and hand representations on body ownership and presence. In Proceedings of the 5th Symposium on Spatial
       User Interaction (SUI’17). Association for Computing Machinery, 3–11. DOI:https://doi.org/10.1145/3131277.3132186
  [69] S. Jung, P. J. Wisniewski, and C. E. Hughes. 2018. In limbo: The effect of gradual visual transition between real
      and virtual on virtual body ownership illusion and presence. In Proceedings of the 2018 IEEE Conference on Virtual
        Reality and 3D User Interfaces (VR). IEEE, 267–272. DOI:https://doi.org/10.1109/VR.2018.8447562
  [70] Andreas Kalckert and H. Ehrsson. 2012. Moving a rubber hand that feels like your own: A dissociation of ownership
      and agency. Frontiers in Human Neuroscience 6 (2012), 40. DOI:https://doi.org/10.3389/fnhum.2012.00040
  [71] Marjolein P. M. Kammers, Katy Rose, and Patrick Haggard. 2011. Feeling numb: Temperature, but not thermal
        pain, modulates feeling of body ownership. Neuropsychologia 49, 5 (2011), 1316–1321. DOI:https://doi.org/10.1016/
       j.neuropsychologia.2011.02.039
  [72] Hans-Otto Karnath, Simone Claire Mølbert, Anna Katharina Klaner, Joachim Tesch, Katrin Elisabeth Giel, Hong Yu
      Wong, and Betty J. Mohler. 2019. Visual perception of one’s own body under vestibular stimulation using biometric
        self-avatars in virtual reality. PLOS ONE 14, 3 (2019), e0213944. DOI:https://doi.org/10.1371/journal.pone.0213944
  [73] Samantha Keenaghan, Lucy Bowles, Georgina Crawfurd, Simon Thurlbeck, Robert W. Kentridge, and Dorothy
       Cowie. 2020. My body until proven otherwise: Exploring the time course of the full body illusion. Consciousness
      and Cognition 78 (2020), 102882. DOI:https://doi.org/10.1016/j.concog.2020.102882



     ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 36 / 42 -->

```text
76:36                                                                       A. Mottelson et al.


  [74] Anouk Keizer, Annemarie van Elburg, Rossa Helms, and H. Chris Dijkerman. 2016. A virtual reality full body illusion
       improves body image disturbance in anorexia nervosa. PLOS ONE 11, 10 (2016), 1–21. DOI:https://doi.org/10.1371/
       journal.pone.0163921
  [75] K. Kilteni, I. Bergstrom, and M. Slater. 2013. Drumming in immersive virtual reality: The body shapes the way we
        play. IEEE Transactions on Visualization and Computer Graphics 19, 4 (2013), 597–605. DOI:https://doi.org/10.1109/
      TVCG.2013.29
  [76] Konstantina Kilteni, Jennifer Grau-Sánchez, Misericordia Veciana De Las Heras, Antoni Rodríguez-Fornells, and
      Mel Slater. 2016. Decreased corticospinal excitability after the illusion of missing part of the arm. Frontiers in Human
       Neuroscience 10 (2016), 145. DOI:https://doi.org/10.3389/fnhum.2016.00145
  [77] Konstantina Kilteni, Antonella Maselli, Konrad P. Kording, and Mel Slater. 2015. Over my fake body: Body owner-
       ship illusions for studying the multisensory basis of own-body perception. Frontiers in Human Neuroscience 9 (2015),
        141. DOI:https://doi.org/10.3389/fnhum.2015.00141
  [78] Konstantina Kilteni, Jean-Marie Normand, Maria V. Sanchez-Vives, and Mel Slater. 2012. Extending body space in
       immersive virtual reality: A very long arm illusion. PLOS ONE 7, 7 (2012), 1–15. DOI:https://doi.org/10.1371/journal.
       pone.0040867
  [79] Konstantina Kilteni, Jean-Marie Normand, Maria V. Sanchez-Vives, and Mel Slater. 2012. Extending body space
        in immersive virtual reality: A very long arm illusion. PLOS ONE 7, 7 (2012), e40867. DOI:https://doi.org/10.1371/
       journal.pone.0040867
  [80] So-Yeon Kim, Hyojin Park, Myeongul Jung, and Kwanguk Kim. 2020. Impact of body size match to an avatar on
       the body ownership illusion and user’s subjective experience. Cyberpsychology, Behavior, and Social Networking 23,
       4 (2020), 234–241. DOI:https://doi.org/10.1089/cyber.2019.0136
  [81] Martin Kocur, Sarah Graf, and Valentin Schwind. 2020. The impact of missing fingers in virtual reality. In Proceed-
        ings of the 26th ACM Symposium on Virtual Reality Software and Technology (VRST’20). Association for Computing
       Machinery, 5 pages. DOI:https://doi.org/10.1145/3385956.3418973
  [82] Martin Kocur, Florian Habler, Valentin Schwind, Paweł W. Woźniak, Christian Wolff, and Niels Henze. 2021. Phys-
        iological and perceptual responses to athletic avatars while cycling in virtual reality. In Proceedings of the 2021
      CHI Conference on Human Factors in Computing Systems (CHI’21). Association for Computing Machinery, 18 pages.
       DOI:https://doi.org/10.1145/3411764.3445160
  [83] Martin Kocur, Melanie Kloss, Valentin Schwind, Christian Wolff, and Niels Henze. 2020. Flexing muscles in virtual
         reality: Effects of avatars’ muscular appearance on physical performance. In Proceedings of the Annual Symposium
      on Computer-Human Interaction in Play (CHI PLAY’20). Association for Computing Machinery, 193–205. DOI:https:
       //doi.org/10.1145/3410404.3414261
  [84] Martin Kocur, Philipp Schauhuber, Valentin Schwind, Christian Wolff, and Niels Henze. 2020. The effects of self-
      and external perception of avatars on cognitive task performance in virtual reality. In Proceedings of the 26th ACM
      Symposium on Virtual Reality Software and Technology (VRST’20). Association for Computing Machinery. DOI:https:
       //doi.org/10.1145/3385956.3418969
  [85] Elena Kokkinara, Konstantina Kilteni, Kristopher J. Blom, and Mel Slater. 2016. First person perspective of seated
        participants over a walking virtual body leads to illusory agency over the walking. Scientific Reports 6, 1 (2016),
       28879. DOI:https://doi.org/10.1038/srep28879
  [86] Elena Kokkinara, Mel Slater, and Joan López-Moliner. 2015. The effects of visuomotor calibration to the perceived
       space and body, through embodiment in immersive virtual reality. ACM Transactions on Applied Perception 13,
       1 (2015), 22 pages. DOI:https://doi.org/10.1145/2818998
  [87] Ryota Kondo, Maki Sugimoto, Kouta Minamizawa, Takayuki Hoshi, Masahiko Inami, and Michiteru Kitazaki. 2018.
        Illusory body ownership of an invisible body interpolated between virtual hands and feet via visual-motor syn-
        chronicity. Scientific Reports 8, 1 (2018), 7541. DOI:https://doi.org/10.1038/s41598-018-25951-2
  [88] Ryota Kondo, Yamato Tani, Maki Sugimoto, Masahiko Inami, and Michiteru Kitazaki. 2020. Scrambled body differ-
        entiates body part ownership from the full body illusion. Scientific Reports 10, 1 (2020), 5274. DOI:https://doi.org/
       10.1038/s41598-020-62121-9
  [89] Gaiqing Kong, Kang He, and Kunlin Wei. 2017. Sensorimotor experience in virtual reality enhances sense of agency
       associated with an avatar. Consciousness and Cognition 52 (2017), 115–124. DOI:https://doi.org/10.1016/j.concog.
       2017.04.018
  [90] Michael Landgrebe, Kewir Nyuyki, Elmar Frank, Thomas Steffens, Simone Hauser, Peter Eichhammer, Goeran
       Hajak, and Berthold Langguth. 2008. Effects of colour exposure on auditory and somatosensory perception–Hints
        for cross-modal plasticity. Neuroendocrinology Letters 29, 4 (2008), 518–521.
  [91] Marc Erich Latoschik, Daniel Roth, Dominik Gall, Jascha Achenbach, Thomas Waltemate, and Mario Botsch. 2017.
      The effect of avatar realism in immersive social virtual realities. In Proceedings of the 23rd ACM Symposium on
        Virtual Reality Software and Technology (VRST’17). Association for Computing Machinery, 10 pages. DOI:https:
       //doi.org/10.1145/3139131.3139156

ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 37 / 42 -->

```text
Body Ownership Illusions in VR                                                           76:37


  [92] Marc Erich Latoschik, Daniel Roth, Dominik Gall, Jascha Achenbach, Thomas Waltemate, and Mario Botsch. 2017.
      The effect of avatar realism in immersive social virtual realities. In Proceedings of the 23rd ACM Symposium on
        Virtual Reality Software and Technology (VRST’17). Association for Computing Machinery, 10 pages. DOI:https:
       //doi.org/10.1145/3139131.3139156
  [93] Juyoung Lee, Myungho Lee, Gerard Jounghyun Kim, and Jae-In Hwang. 2020. Effects of synchronized leg motion in
       walk-in-place utilizing deep neural networks for enhanced body ownership and sense of presence in VR. In Proceed-
        ings of the 26th ACM Symposium on Virtual Reality Software and Technology (VRST’20). Association for Computing
       Machinery. DOI:https://doi.org/10.1145/3385956.3418959
  [94] Bigna Lenggenhager, Michael Mouthon, and Olaf Blanke. 2009. Spatial aspects of bodily self-consciousness. Con-
        sciousness and Cognition 18, 1 (2009), 110–117. DOI:https://doi.org/10.1016/j.concog.2008.11.003
  [95] Bigna Lenggenhager, Tej Tadi, Thomas Metzinger, and Olaf Blanke. 2007. Video ergo sum: Manipulating bodily
        self-consciousness. Science 317, 5841 (2007), 1096–1099. DOI:https://doi.org/10.1126/science.1143439
  [96] Markus Leyrer, Sally A. Linkenauger, Heinrich H. Bülthoff, Uwe Kloos, and Betty Mohler. 2011. The influence of eye
       height and avatars on egocentric distance estimates in immersive virtual environments. In Proceedings of the ACM
      SIGGRAPH Symposium on Applied Perception in Graphics and Visualization (APGV’11). Association for Computing
       Machinery, 67–74. DOI:https://doi.org/10.1145/2077451.2077464
  [97] Lan Li, Fei Yu, Dongquan Shi, Jianping Shi, Zongjun Tian, Jiquan Yang, Xingsong Wang, and Qing Jiang. 2017.
       Application of virtual reality technology in clinical medicine. American Journal of Translational Research 9, 9 (2017),
       3867.
  [98] Alvin M. Liberman, Franklin S. Cooper, Donald P. Shankweiler, and Michael Studdert-Kennedy. 1967. Perception of
       the speech code. Psychological Review 74, 6 (1967), 431. DOI:https://doi.org/10.1037/h0020279
  [99] Benjamin Libet. 1985. Unconscious cerebral initiative and the role of conscious will in voluntary action. Behavioral
      and Brain Sciences 8, 4 (1985), 529–539. DOI:https://doi.org/10.1017/S0140525X00044903
 [100] Lorraine Lin and Sophie Jörg. 2016. Need a hand? How appearance affects the virtual hand illusion. In Proceedings
        of the ACM Symposium on Applied Perception (SAP’16). Association for Computing Machinery, 69–76. DOI:https:
       //doi.org/10.1145/2931002.2931006
 [101] L. Lin, A. Normoyle, A. Adkins, Y. Sun, A. Robb, Y. Ye, M. Di Luca, and S. Jørg. 2019. The effect of hand size and
        interaction modality on the virtual hand illusion. In Proceedings of the 2019 IEEE Conference on Virtual Reality and
      3D User Interfaces (VR). IEEE, 510–518. DOI:https://doi.org/10.1109/VR.2019.8797787
 [102] Matthew R. Longo, Friederike Schüür, Marjolein P. M. Kammers, Manos Tsakiris, and Patrick Haggard. 2008. What
         is embodiment? A psychometric approach. Cognition 107, 3 (2008), 978–998.
 [103] Sarah Lopez, Yi Yang, Kevin Beltran, Soo Jung Kim, Jennifer Cruz Hernandez, Chelsy Simran, Bingkun Yang, and
       Beste F. Yuksel. 2019. Investigating implicit gender bias and embodiment of white males in virtual reality with full
      body visuomotor synchrony. In Proceedings of the 2019 CHI Conference on Human Factors in Computing Systems
        (CHI’19). Association for Computing Machinery. DOI:https://doi.org/10.1145/3290605.3300787
 [104]  J. Lugrin, M. Ertl, P. Krop, R. Klüpfel, S. Stierstorfer, B. Weisz, M. Rück, J. Schmitt, N. Schmidt, and M. E. Latoschik.
       2018. Any “body” there? Avatar visibility effects in a virtual reality game. In Proceedings of the 2018 IEEE Conference
      on Virtual Reality and 3D User Interfaces (VR). IEEE, 17–24. DOI:https://doi.org/10.1109/VR.2018.8446229
 [105] Jean-Luc Lugrin, Johanna Latt, and Marc Erich Latoschik. 2015. Avatar anthropomorphism and illusion of body
      ownership in VR. In Proceedings of the 2015 IEEE Virtual Reality (VR). IEEE, 229–230. DOI:https://doi.org/10.1109/
       VR.2015.7223379
 [106] Peter Lush, Simine Vazire, and Alex Holcombe. 2020. Demand characteristics confound the rubber hand illusion.
        Collabra: Psychology 6, 1 (2020), 22. DOI:https://doi.org/10.1525/collabra.325
 [107] Daniel Lüdecke. 2019. esc: Effect Size Computation for Meta Analysis (Version 0.5.1). DOI:https://doi.org/10.5281/
       zenodo.1249218
 [108] Lara Maister, Mel Slater, Maria V. Sanchez-Vives, and Manos Tsakiris. 2015. Changing bodies changes minds: Own-
       ing another body affects social cognition. Trends in Cognitive Sciences 19, 1 (2015), 6–12. DOI:https://doi.org/10.
        1016/j.tics.2014.11.001
 [109] Guido Makransky, Thomas S. Terkildsen, and Richard E. Mayer. 2019. Adding immersive virtual reality to a science
        lab simulation causes more presence but less learning. Learning and Instruction 60 (2019), 225–236. DOI:https://doi.
        org/10.1016/j.learninstruc.2017.12.007
 [110] Michael G. F. Martin. 1995. Bodily awareness: A sense of ownership. In Proceedings of the Body and the Self. Jose Luis
      Bermudez, Anthony J. Marcel, and Naomi M. Eilan (Eds.), MIT, 267–289.
 [111] Matteo Martini, Konstantina Kilteni, Antonella Maselli, and Maria V. Sanchez-Vives. 2015. The body fades away: In-
       vestigating the effects of transparency of an embodied virtual body on pain threshold and body ownership. Scientific
       Reports 5, 1 (2015), 1–8. DOI:https://doi.org/10.1038/srep13948




     ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 38 / 42 -->

```text
76:38                                                                       A. Mottelson et al.


 [112] Matteo Martini, Daniel Pérez Marcos, and Maria Sanchez-Vives. 2013. What color is my arm? Changes in skin color
        of an embodied virtual arm modulates pain threshold. Frontiers in Human Neuroscience 7 (2013), 438. DOI:https:
       //doi.org/10.3389/fnhum.2013.00438
 [113] Antonella Maselli and Mel Slater. 2013. The building blocks of the full body ownership illusion. Frontiers in Human
       Neuroscience 7 (2013), 83. DOI:https://doi.org/10.3389/fnhum.2013.00083
 [114] Antonella Maselli and Mel Slater. 2014. Sliding perspectives: Dissociating ownership from self-location during full
      body illusions in virtual reality. Frontiers in Human Neuroscience 8 (2014), 693. DOI:https://doi.org/10.3389/fnhum.
       2014.00693
 [115] Marta Matamala-Gomez, Antonella Maselli, Clelia Malighetti, Olivia Realdon, Fabrizia Mantovani, and Giuseppe
        Riva. 2021. Virtual body ownership illusions for mental health: A narrative review. Journal of Clinical Medicine 10,
       1 (2021), 139. DOI:https://doi.org/10.3390/jcm10010139
 [116] Daniel Medeiros, Rafael K. dos Anjos, Daniel Mendes, João Madeiras Pereira, Alberto Raposo, and Joaquim Jorge.
       2018. Keep my head on my shoulders! Why third-person is bad for navigation in VR. In Proceedings of the 24th ACM
      Symposium on Virtual Reality Software and Technology (VRST’18). Association for Computing Machinery. DOI:https:
       //doi.org/10.1145/3281505.3281511
 [117] Maurice Merleau-Ponty. 2014. Phenomenology of Perception. Routledge.
 [118] Daisuke Mine, Nami Ogawa, Takuji Narumi, and Kazuhiko Yokosawa. 2020. The relationship between the body and
       the environment in the virtual world: The interpupillary distance affects the body size perception. PLOS ONE 15,
       4 (2020), e0232290. DOI:https://doi.org/10.1371/journal.pone.0232290
 [119] David Moher, Alessandro Liberati, Jennifer Tetzlaff, Douglas G. Altman, and The PRISMA Group. 2009. Preferred
       reporting items for systematic reviews and meta-analyses: The PRISMA statement. PLOS Medicine 6, 7 (2009),
       e1000097. DOI:https://doi.org/10.1371/journal.pmed.1000097
 [120] Aske Mottelson and Kasper Hornbæk. 2017. Virtual reality studies outside the laboratory. In Proceedings of the
       23rd ACM Symposium on Virtual Reality Software and Technology (VRST’17). Association for Computing Machinery,
       10 pages. DOI:https://doi.org/10.1145/3139131.3139141
 [121] Aske Mottelson, Gustav Bøg Petersen, Klemen Lilija, and Guido Makransky. 2021. Conducting unsupervised virtual
        reality user studies online. Frontiers in Virtual Reality 2 (2021), 66. DOI:https://doi.org/10.3389/frvir.2021.681482
 [122] Aske Mottelson, Clara Vandeweerdt, Michael Atchapero, Tiffany Luong, Christian Holz, Robert Bøhm, and Guido
       Makransky. 2021. A self-administered virtual reality intervention increases COVID-19 vaccination intention. Vac-
        cine 39, 46 (2021), 6746–6753. DOI:https://doi.org/10.1016/j.vaccine.2021.10.004
 [123] Raviraj Nataraj, Sean Sanford, Aniket Shah, and Mingxiao Liu. 2020. Agency and performance of reach-to-grasp
       with modified control of a virtual hand: Implications for rehabilitation. Frontiers in Human Neuroscience 14 (2020),
        126. DOI:https://doi.org/10.3389/fnhum.2020.00126
 [124] Alessandro Nesti, Giulio Rognini, Bruno Herbelin, Heinrich H. Bülthoff, Lewis Chuang, and Olaf Blanke. 2018.
       Modulation of vection latencies in the full-body illusion. PLOS ONE 13, 12 (2018), e0209189. DOI:https://doi.org/10.
       1371/journal.pone.0209189
 [125] Solène Neyret, Xavi Navarro, Alejandro Beacco, Ramon Oliva, Pierre Bourdin, Jose Valenzuela, Itxaso Barberia,
      and Mel Slater. 2020. An embodied perspective as a victim of sexual harassment in virtual reality reduces action
       conformity in a later milgram obedience scenario. Scientific Reports 10, 1 (2020), 1–18. DOI:https://doi.org/10.1038/
       s41598-020-62932-w
 [126] Jean-Marie Normand, Elias Giannopoulos, Bernhard Spanlang, and Mel Slater. 2011. Multisensory stimulation can
       induce an illusion of larger belly size in immersive virtual reality. PLOS ONE 6, 1 (2011), e16128. DOI:https://doi.
       org/10.1371/journal.pone.0016128
 [127] Brian A. Nosek, Charles R. Ebersole, Alexander C. DeHaven, and David T. Mellor. 2018. The preregistration revo-
        lution. Proceedings of the National Academy of Sciences 115, 11 (2018), 2600–2606. DOI:https://doi.org/10.1073/pnas.
       1708274114
 [128] N. Ogawa, T. Narumi, and M. Hirose. 2019. Virtual hand realism affects object size perception in body-based scaling.
       In Proceedings of the 2019 IEEE Conference on Virtual Reality and 3D User Interfaces (VR). IEEE, 519–528. DOI:https:
       //doi.org/10.1109/VR.2019.8798040
 [129] Nami Ogawa, Takuji Narumi, Hideaki Kuzuoka, and Michitaka Hirose. 2020. Do you feel like passing through
        walls?: Effect of self-avatar appearance on facilitating realistic behavior in virtual environments. In Proceedings of
        the 2020 CHI Conference on Human Factors in Computing Systems (CHI’20). Association for Computing Machinery,
       1–14. DOI:https://doi.org/10.1145/3313831.3376562
 [130] Sofia Adelaide Osimo, Rodrigo Pizarro, Bernhard Spanlang, and Mel Slater. 2015. Conversations between self and
         self as sigmund freud-a virtual body ownership paradigm for self counselling. Scientific Reports 5, 1 (2015), 1–14.
       DOI:https://doi.org/10.1038/srep13899




ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 39 / 42 -->

```text
Body Ownership Illusions in VR                                                           76:39


 [131] Matthew J. Page, Joanne E. McKenzie, Patrick M. Bossuyt, Isabelle Boutron, Tammy C. Hoffmann, Cynthia D.
      Mulrow, Larissa Shamseer, Jennifer M. Tetzlaff, Elie A. Akl, Sue E. Brennan, et al. 2021. The PRISMA 2020 state-
       ment: An updated guideline for reporting systematic reviews. Systematic Reviews 10, 1 (2021), 1–11. DOI:https:
       //doi.org/10.1136/bmj.n71
 [132] Ivan Patané, Anne Lelgouarch, Domna Banakou, Gregoire Verdelet, Clement Desoche, Eric Koun, Romeo Salemme,
      Mel Slater, and Alessandro Farnè. 2020. Exploring the effect of cooperation in reducing implicit racial bias and its
        relationship with dispositional empathy and political attitudes. Frontiers in Psychology 11 (2020), 2281. DOI:https:
       //doi.org/10.3389/fpsyg.2020.510787
 [133] Ivan Patané, Anne Lelgouarch, Domna Banakou, Gregoire Verdelet, Clement Desoche, Eric Koun, Romeo Salemme,
      Mel Slater, and Alessandro Farnè. 2020. Exploring the effect of cooperation in reducing implicit racial bias and its
        relationship with dispositional empathy and political attitudes. Frontiers in Psychology 11 (2020), 2281. DOI:https:
       //doi.org/10.3389/fpsyg.2020.510787
 [134] Tabitha C. Peck, My Doan, Kimberly A. Bourne, and Jessica J. Good. 2018. The effect of gender body-swap illusions
      on working memory and stereotype threat. IEEE Transactions on Visualization and Computer Graphics 24, 4 (2018),
       1604–1612. DOI:https://doi.org/10.1109/TVCG.2018.2793598
 [135] Tabitha C. Peck and Mar Gonzalez-Franco. 2021. Avatar embodiment: A standardized questionnaire. Frontiers in
        Virtual Reality 1 (2021), 44. DOI:https://doi.org/10.3389/frvir.2020.575943
 [136] Tabitha C. Peck, Jessica J. Good, and Kimberly A. Bourne. 2020. Inducing and mitigating stereotype threat through
       gendered virtual body-swap illusions. In Proceedings of the 2020 CHI Conference on Human Factors in Computing
       Systems (CHI’20). Association for Computing Machinery, 1–13. DOI:https://doi.org/10.1145/3313831.3376419
 [137] Tabitha C. Peck, Sofia Seinfeld, Salvatore M. Aglioti, and Mel Slater. 2013. Putting yourself in the skin of a black
       avatar reduces implicit racial bias. Consciousness and Cognition 22, 3 (2013), 779–787. DOI:https://doi.org/10.1016/j.
       concog.2013.04.016
 [138] Tabitha C. Peck, Laura E. Sockol, and Sarah M. Hancock. 2020. Mind the gap: The underrepresentation of female
        participants and authors in virtual reality research. IEEE Transactions on Visualization and Computer Graphics 26,
       5 (2020), 1945–1954. DOI:https://doi.org/10.1109/TVCG.2020.2973498
 [139] Olga Perepelkina, Viktoriia Vorobeva, Olga Melnikova, Galina Arina, and Valentina Nikolaeva. 2018. Artificial hand
        illusions dynamics: Onset and fading of static rubber and virtual moving hand illusions. Consciousness and Cognition
       65 (2018), 216–227. DOI:https://doi.org/10.1016/j.concog.2018.09.005
 [140] Valeria I. Petkova and H. Henrik Ehrsson. 2008. If I were you: Perceptual illusion of body swapping. PLOS ONE 3,
       12 (2008), e3832. DOI:https://doi.org/10.1371/journal.pone.0003832
 [141] Christian Pfeiffer, Christophe Lopez, Valentin Schmutz, Julio Angel Duenas, Roberto Martuzzi, and Olaf Blanke.
       2013. Multisensory origin of the subjective first-person perspective: Visual, tactile, and vestibular mechanisms.
      PLOS ONE 8, 4 (2013), e61751. DOI:https://doi.org/10.1371/journal.pone.0061751
 [142] Ivelina V. Piryankova, Hong Yu Wong, Sally A. Linkenauger, Catherine Stinson, Matthew R. Longo, Heinrich H.
        Bülthoff, and Betty J. Mohler. 2014. Owning an overweight or underweight body: Distinguishing the physical, expe-
       rienced and virtual body. PLOS ONE 9, 8 (2014), Article e103428. DOI:https://doi.org/10.1371/journal.pone.0103428
 [143] Dario Pittera, Elia Gatti, and Marianna Obrist. 2019. I’m Sensing in the Rain: Spatial Incongruity in Visual-tactile Mid-
        air Stimulation Can Elicit Ownership in VR Users. In Proceedings of the 2019 CHI Conference on Human Factors in
      Computing Systems (CHI’19). Association for Computing Machinery. DOI:https://doi.org/10.1145/3290605.3300362
 [144] Iana Podkosova and Hannes Kaufmann. 2018. Co-presence and proxemics in shared walkable virtual environments
      with mixed colocation. In Proceedings of the 24th ACM Symposium on Virtual Reality Software and Technology
       (VRST’18). Association for Computing Machinery, 11 pages. DOI:https://doi.org/10.1145/3281505.3281523
 [145] Ausias Pomes and Mel Slater. 2013. Drift and ownership toward a distant virtual body. Frontiers in Human Neuro-
        science 7 (2013), 908. DOI:https://doi.org/10.3389/fnhum.2013.00908
 [146] T. Porssut, B. Herbelin, and R. Boulic. 2019. Reconciling being in-control vs. being helped for the execution of
      complex movements in VR. In Proceedings of the 2019 IEEE Conference on Virtual Reality and 3D User Interfaces (VR).
       IEEE, 529–537. DOI:https://doi.org/10.1109/VR.2019.8797716
 [147] Stephen C. Pritchard, Regine Zopf, Vince Polito, David M. Kaplan, and Mark A. Williams. 2016. Non-hierarchical
       influence of visual form, touch, and position cues on embodiment, agency, and presence in virtual reality. Frontiers
        in Psychology 7 (2016), 1649. DOI:https://doi.org/10.3389/fpsyg.2016.01649
 [148] Maria Pyasik and Lorenzo Pia. 2021. Owning a virtual body entails owning the value of its actions in a detection-
       of-deception procedure. Cognition 212 (2021), 104693. DOI:https://doi.org/10.1016/j.cognition.2021.104693
 [149] Maria Pyasik, Gaetano Tieri, and Lorenzo Pia. 2020. Visual appearance of the virtual hand affects embodiment in
       the virtual hand illusion. Scientific Reports 10, 1 (2020), 5412. DOI:https://doi.org/10.1038/s41598-020-62394-0
 [150] R Core Team. 2021. R: A Language and Environment for Statistical Computing. R Foundation for Statistical Comput-
        ing, Vienna, Austria. Retrieved from https://www.R-project.org/. Accessed 1 June 2020.



     ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 40 / 42 -->

```text
76:40                                                                       A. Mottelson et al.


 [151] Jack Ratcliffe, Francesco Soave, Nick Bryan-Kinns, Laurissa Tokarchuk, and Ildar Farkhatdinov. 2021. Extended
        reality (XR) remote research: A survey of drawbacks and opportunities. In Proceedings of the 2021 CHI Conference
      on Human Factors in Computing Systems. Association for Computing Machinery, 13 pages. DOI:https://doi.org/10.
       1145/3411764.3445170
 [152] Martin Riemer, Jørg Trojan, Marta Beauchamp, and Xaver Fuchs. 2019. The rubber hand universe: On the impact of
       methodological differences in the rubber hand illusion. Neuroscience and Biobehavioral Reviews 104 (2019), 268–280.
        DOI:https://doi.org/10.1016/j.neubiorev.2019.07.008
 [153] Daniel Roth, Gary Bente, Peter Kullmann, David Mal, Chris Felix Purps, Kai Vogeley, and Marc Erich Latoschik. 2019.
       Technologies for social augmentations in user-embodied virtual reality. In Proceedings of the 25th ACM Symposium
      on Virtual Reality Software and Technology (VRST’19). Association for Computing Machinery, 12 pages. DOI:https:
       //doi.org/10.1145/3359996.3364269
 [154] Daniel Roth and Marc Latoschik. 2020. Construction of the virtual embodiment questionnaire (VEQ). IEEE Transac-
        tions on Visualization and Computer Graphics 26 (2020), 3546–3556. DOI:https://doi.org/10.1109/TVCG.2020.3023603
 [155] Marius Rubo and Matthias Gamer. 2019. Visuo-tactile congruency influences the body schema during full body
      ownership illusion. Consciousness and Cognition 73 (2019), 102758. DOI:https://doi.org/10.1016/j.concog.2019.05.006
 [156] Roy Salomon, Melanie Lim, Christian Pfeiffer, Roger Gassert, and Olaf Blanke. 2013. Full body illusion is associated
       with widespread skin temperature reduction. Frontiers in Behavioral Neuroscience 7 (2013), 65. DOI:https://doi.org/
       10.3389/fnbeh.2013.00065
 [157] Valentin Schwind, David Halbhuber, Jakob Fehle, Jonathan Sasse, Andreas Pfaffelhuber, Christoph Tögel, Julian
        Dietz, and Niels Henze. 2020. The effects of full-body avatar movement predictions in virtual reality using neural
       networks. In Proceedings of the 26th ACM Symposium on Virtual Reality Software and Technology (VRST’20). Associ-
       ation for Computing Machinery. DOI:https://doi.org/10.1145/3385956.3418941
 [158] Valentin Schwind, Pascal Knierim, Cagri Tasci, Patrick Franczak, Nico Haas, and Niels Henze. 2017. "These are not
     my hands!": Effect of gender on the perception of avatar hands in virtual reality. In Proceedings of the 2017 CHI
       Conference on Human Factors in Computing Systems (CHI’17). Association for Computing Machinery, 1577–1582.
       DOI:https://doi.org/10.1145/3025453.3025602
 [159] Sofia Seinfeld, Jorge Arroyo-Palacios, Guillermo Iruretagoyena, Ruud Hortensius, Luis E. Zapata, David Borland,
       Beatrice de Gelder, Mel Slater, and Maria V. Sanchez-Vives. 2018. Offenders become the victim in virtual reality:
       impact of changing perspective in domestic violence. Scientific Reports 8, 1 (2018), 2692. DOI:https://doi.org/10.
       1038/s41598-018-19987-7
 [160] Sofia Seinfeld and Jörg Müller. 2020. Impact of visuomotor feedback on the embodiment of virtual hands detached
      from the body. Scientific Reports 10, 1 (2020), 22427. DOI:https://doi.org/10.1038/s41598-020-79255-5
 [161] Mincheol Shin, Sanguk Lee, Stephen W. Song, and Donghun Chung. 2021. Enhancement of perceived body owner-
       ship in virtual reality-based teleoperation may backfire in the execution of high-risk tasks. Computers in Human
       Behavior 115 (2021), 106605. DOI:https://doi.org/10.1016/j.chb.2020.106605
 [162] Mel Slater, Solène Neyret, Tania Johnston, Guillermo Iruretagoyena, Mercè Álvarez de la Campa Crespo, Miquel
       Alabèrnia-Segura, Bernhard Spanlang, and Guillem Feixas. 2019. An experimental study of a virtual reality coun-
        selling paradigm using embodied self-dialogue. Scientific Reports 9, 1 (2019), 10903. DOI:https://doi.org/10.1038/
       s41598-019-46877-3
 [163] Mel Slater, Daniel Pérez Marcos, Henrik Ehrsson, and Maria Sanchez-Vives. 2008. Towards a digital body: The
        virtual arm illusion. Frontiers in Human Neuroscience 2 (2008), 6. DOI:https://doi.org/10.3389/neuro.09.006.2008
 [164] Mel Slater, Daniel Pérez Marcos, Hans Henrik Ehrsson, and Maria Sanchez-Vives. 2009. Inducing illusory ownership
        of a virtual body. Frontiers in Neuroscience 3, 2 (2009), 29. DOI:https://doi.org/10.3389/neuro.01.029.2009
 [165] Mel Slater, Bernhard Spanlang, Maria V. Sanchez-Vives, and Olaf Blanke. 2010. First person experience of body
        transfer in virtual reality. PLOS ONE 5, 5 (2010), 1–9. DOI:https://doi.org/10.1371/journal.pone.0010564
 [166] Bernhard Spanlang, Birgit Nierula, Maud Haffar, and J. Bruno Debruille. 2019. Mimicking schizophrenia: Reducing
      p300b by minimally fragmenting healthy participants’ selves using immersive virtual reality embodiment. Frontiers
        in Human Neuroscience 12 (2019), 504. DOI:https://doi.org/10.3389/fnhum.2018.00504
 [167] Bernhard Spanlang, Jean-Marie Normand, David Borland, Konstantina Kilteni, Elias Giannopoulos, Ausiàs Pomés,
      Mar González-Franco, Daniel Perez-Marcos, Jorge Arroyo-Palacios, Xavi Navarro Muncunill, and Mel Slater. 2014.
     How to build an embodiment lab: Achieving body representation illusions in virtual reality. Frontiers in Robotics
      and AI 1 (2014), 9. DOI:https://doi.org/10.3389/frobt.2014.00009/full
 [168] W. Steptoe, A. Steed, and M. Slater. 2013. Human tails: Ownership and control of extended humanoid avatars. IEEE
       Transactions on Visualization and Computer Graphics 19, 4 (2013), 583–590. DOI:https://doi.org/10.1109/TVCG.2013.
       32
 [169] Paul Strohmeier, Aske Mottelson, Henning Pohl, Jess McIntosh, Jarrod Knibbe, Joanna Bergström, Yvonne Jansen,
      and Kasper Hornbæk. 2022. Body-based User Interfaces. Routledge.



ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 41 / 42 -->

```text
Body Ownership Illusions in VR                                                           76:41


 [170] Ana Tajadura-Jiménez, Domna Banakou, Nadia Bianchi-Berthouze, and Mel Slater. 2017. Embodiment in a child-like
        talking virtual body influences object size perception, self-identification, and subsequent real speaking. Scientific
       Reports 7, 1 (2017),9637. DOI:https://doi.org/10.1038/s41598-017-09497-3
 [171] Riccardo Tambone, Giulia Poggio, Maria Pyasik, Dalila Burin, Olga Dal Monte, Selene Schintu, Tommaso Ciorli,
       Laura Luca, Maria Vittoria Semino, Fabrizio Doricchi, et al. 2021. Changing your body changes your eating attitudes:
      Embodiment of a slim virtual avatar induces avoidance of high-calorie food. Heliyon 7, 7 (2021), e07515. DOI:https:
       //doi.org/10.1016/j.heliyon.2021.e07515
 [172] N. Toothman and M. Neff. 2019. The impact of avatar tracking errors on user experience in VR. In Proceedings of
        the 2019 IEEE Conference on Virtual Reality and 3D User Interfaces (VR). IEEE, 756–766. DOI:https://doi.org/10.1109/
       VR.2019.8798108
 [173] Tanh Quang Tran, HyunJu Shin, Wolfgang Stuerzlinger, and Jung Hyun Han. 2017. Effects of virtual arm repre-
       sentations on interaction in virtual environments. In Proceedings of the 23rd ACM Symposium on Virtual Reality
       Software and Technology (VRST’17). Association for Computing Machinery, 9 pages. DOI:https://doi.org/10.1145/
       3139131.3139149
 [174] Manos Tsakiris. 2010. My body in the brain: A neurocognitive model of body-ownership. Neuropsychologia 48,
       3 (2010), 703–712. DOI:https://doi.org/10.1016/j.neuropsychologia.2009.09.034
 [175] Manos Tsakiris, Gita Prabhu, and Patrick Haggard. 2006. Having a body versus moving your body: How agency
        structures body-ownership. Consciousness and Cognition 15, 2 (2006), 423–432. DOI:https://doi.org/10.1016/j.concog.
       2005.09.004
 [176] Collin Turbyne, Abe Goedhart, Pelle de Koning, Frederike Schirmbeck, and Damiaan Denys. 2021. Systematic review
      and meta-analysis of virtual reality in mental healthcare: Effects of full body illusions on body image disturbance.
        Frontiers in Virtual Reality 2 (2021). DOI:https://doi.org/10.3389/frvir.2021.657638
 [177] Albert van der Veer, Adrian Alsmith, Matthew Longo, Hong Yu Wong, Daniel Diers, Matthias Bues, Anna P. Giron,
      and Betty J. Mohler. 2019. The influence of the viewpoint in a self-avatar on body part and self-localization. In
       Proceedings of the ACM Symposium on Applied Perception 2019 (SAP’19). Association for Computing Machinery,
       11 pages. DOI:https://doi.org/10.1145/3343036.3343124
 [178] Clara Vandeweerdt, Tiffany Luong, Michael Atchapero, Aske Mottelson, Christian Holz, Guido Makransky, and
       Robert Böhm. 2022. Virtual reality reduces COVID-19 vaccine hesitancy in the wild: A randomized trial. Scientific
       Reports 12, 1 (2022), 1–7. DOI:https://doi.org/10.1038/s41598-022-08120-4
 [179] Jack L. Vevea and Larry V. Hedges. 1995. A general linear model for estimating effect size in the presence of publi-
       cation bias. Psychometrika 60, 3 (1995), 419–435. DOI:https://doi.org/10.1007/BF02294384
 [180] Wolfgang Viechtbauer. 2010. Conducting meta-analyses in R with the metafor package. Journal of Statistical Soft-
      ware 36, 3 (2010), 1–48. DOI:https://doi.org/10.18637/jss.v036.i03
 [181] Filip Škola and Fotis Liarokapis. 2019. Examining and enhancing the illusory touch perception in virtual reality
       using non-invasive brain stimulation. In Proceedings of the 2019 CHI Conference on Human Factors in Computing
       Systems (CHI’19). Association for Computing Machinery. DOI:https://doi.org/10.1145/3290605.3300477
 [182] T. Waltemate, D. Gall, D. Roth, M. Botsch, and M. E. Latoschik. 2018. The impact of avatar personalization and
      immersion on virtual body ownership, presence, and emotional response. IEEE Transactions on Visualization and
      Computer Graphics 24, 4 (2018), 1643–1652. DOI:https://doi.org/10.1109/TVCG.2018.2794629
 [183] Xiang Wan, Wenqian Wang, Jiming Liu, and Tiejun Tong. 2014. Estimating the sample mean and standard deviation
      from the sample size, median, range and/or interquartile range. BMC Medical Research Methodology 14, 12 (2014),
        135. DOI:https://doi.org/10.1186/1471-2288-14-135
 [184] A. Weeth, A. Mühlberger, and Y. Shiban. 2017. Was it less painful for knights? Influence of appearance on pain
       perception. European Journal of Pain 21, 10 (2017), 1756–1762. DOI:https://doi.org/10.1002/ejp.1087
 [185] Marieke L. Weijs, Elle Macartney, Moritz M. Daum, and Bigna Lenggenhager. 2021. Development of the bodily self:
        Effects of visuomotor synchrony and visual appearance on virtual embodiment in children and adults. Journal of
       Experimental Child Psychology 210 (2021), 105200. DOI:https://doi.org/10.1016/j.jecp.2021.105200
 [186] Erik Wolf, Nathalie Merdan, Nina Dølinger, David Mal, Carolin Wienrich, Mario Botsch, and Marc Erich Latoschik.
       2021. The embodiment of photorealistic avatars influences female body weight perception in virtual reality. In
       Proceedings of the 2021 IEEE Virtual Reality and 3D User Interfaces (VR). IEEE, 65–74. DOI:https://doi.org/10.1109/
       VR50410.2021.00027
 [187] Andrea Stevenson Won, Jeremy Bailenson, Jimmy Lee, and Jaron Lanier. 2015. Homuncular flexibility in virtual
         reality. Journal of Computer-Mediated Communication 20, 3 (2015), 241–259. DOI:https://doi.org/10.1111/jcc4.12107
 [188] Yuanjie Wu, Yu Wang, Sungchul Jung, Simon Hoermann, and Robert W. Lindeman. 2019. Exploring the use of a
       robust depth-sensor-based avatar control system and its effects on communication behaviors. In Proceedings of the
       25th ACM Symposium on Virtual Reality Software and Technology (VRST’19). Association for Computing Machinery.
       DOI:https://doi.org/10.1145/3359996.3364267



     ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```


<!-- page: 42 / 42 -->

```text
76:42                                                                       A. Mottelson et al.


 [189] Jingjing Zhang, Mengjie Huang, Lixiang Zhao, Rui Yang, Hai-Ning Liang, Ji Han, Liu Wang, and Wenxin Sun. 2020.
       Influence of hand representation design on presence and embodiment in virtual environment. In Proceedings of
        the 2020 13th International Symposium on Computational Intelligence and Design (ISCID). IEEE, 364–367. DOI:https:
       //doi.org/10.1109/ISCID51228.2020.00088
 [190] Filip Škola, Simona Tinková, and Fotis Liarokapis. 2019. Progressive training for [a] motor imagery brain–computer
        interfaces using gamification and virtual reality embodiment. Frontiers in Human Neuroscience 13 (2019), 329.
       DOI:https://doi.org/10.3389/fnhum.2019.00329

Received 26 August 2021; revised 6 January 2023; accepted 16 March 2023





ACM Transactions on Computer-Human Interaction, Vol. 30, No. 5, Article 76. Publication date: September 2023.
```
