# Skarbez, Brooks & Whitton (2017) — A Survey of Presence and Related Concepts

## Extraction notes

- Source PDF: Skarbez-et-al.-2017-A-Survey-of-Presence-and-Related-Concepts-2.pdf

- Clean reading copy with page markers preserved.

- Light cleanup only; no interpretive notes mixed into source text.

- Verify exact quotations and numerical/table claims against the original PDF before thesis use.


---



<!-- page: 1 -->

96
A Survey of Presence and Related Concepts
RICHARD SKARBEZ, FREDERICK P. BROOKS, Jr., and MARY C. WHITTON,
University of North Carolina at Chapel Hill, USA
The presence construct, most commonly defined as the sense of “being there,” has driven research and development of virtual environments (VEs) for decades. Despite that, there is not widespread agreement on how
to define or operationalize this construct. The literature contains many different definitions of presence and
many proposed measures for it. This article reviews many of the definitions, measures, and models of presence
from the literature. We also review several related constructs, including social presence, copresence, immersion, agency, transportation, reality judgment, and embodiment. In addition, we present a meta-analysis of
existing presence models and propose a model of presence informed by Slater’s Place Illusion and Plausibility
Illusion constructs.
CCS Concepts: • Human-centered computing →Virtual reality;
Additional Key Words and Phrases: Presence, place illusion, plausibility illusion, social presence, copresence,
immersion, coherence, virtual reality, virtual environments
ACM Reference format:
Richard Skarbez, Frederick P. Brooks, Jr., and Mary C. Whitton. 2017. A Survey of Presence and Related
Concepts. ACM Comput. Surv. 50, 6, Article 96 (November 2017), 39 pages.
https://doi.org/10.1145/3134301
1
INTRODUCTION
Since the early days of virtual environments (VE) research, presence has been a very important
concept for VE creators, representing both the desired outcome of exposure to virtual experiences
and a way to measure the quality of a given VE. Despite—or perhaps because of—its central importance, presence has been defined and measured in many different ways. This has also led to
many related terms, such as social presence, being introduced to the VE literature. Our goals in this
survey are to introduce the important terms used in the study of virtual experiences, to explore
different definitions and models of presence and identify important commonalities and differences
among them, to provide a single point of reference for the many methods that have been proposed
for the measurement of presence, and to define or coin (where necessary) terms in such a way as
to enable more effective—and less confusing—communication about virtual experiences.
This survey begins with an introduction to presence and related concepts to present the concepts
and definitions that inform the analysis of the presence concept itself that makes up the bulk of
this article. We then review many of the definitions of presence that appear in the literature. We
Authors’ addresses: R. Skarbez, Grado Department of Industrial and Systems Engineering, Virginia Polytechnic Institute
and State University, Blacksburg, VA, 24061; email: rskarbez@vt.edu; F. P. Brooks, Jr. and M. C. Whitton, Department
of Computer Science, University of North Carolina at Chapel Hill, Chapel Hill, NC, 27599-3175; emails: {brooks, whitton}@cs.unc.edu.
Permission to make digital or hard copies of all or part of this work for personal or classroom use is granted without fee
provided that copies are not made or distributed for profit or commercial advantage and that copies bear this notice and
the full citation on the first page. Copyrights for components of this work owned by others than ACM must be honored.
Abstracting with credit is permitted. To copy otherwise, or republish, to post on servers or to redistribute to lists, requires
prior specific permission and/or a fee. Request permissions from Permissions@acm.org.
© 2017 ACM 0360-0300/2017/11-ART96 $15.00
https://doi.org/10.1145/3134301
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 2 -->

96:2
R. Skarbez et al.
group these definitions into categories and argue for a definition of presence that more closely
matches how it is commonly used. We then review many of the models of the presence construct
that have been proposed. We also present a meta-analysis of these presence models, identifying
commonalities between them and presenting a new model informed by Slater’s Place Illusion and
Plausibility Illusion. We conclude with a review of existing presence measures, presenting and
commenting on many of the self-report, behavioral, physiological, and psychophysical measures
that have appeared in the VE literature.
2
EVALUATING THE EFFECTIVENESS OF VIRTUAL ENVIRONMENTS
Virtual environments (VEs) are tremendously sophisticated human-computer interfaces that are
used for a wide variety of applications. Examples include psychological treatment, psychological
research, military and medical training, entertainment, and sociological research. Each of these
applications has different task requirements and objectives and those suggest different hardware
and/or software implementations. Additionally, there is no consistent definition for what constitutes an effective VE, even within application domains. For these reasons, the identification of one
or more generalizable constructs that can be used to determine the effectiveness of VEs has driven
and continues to drive research in this area.
It is possible to identify specific measures that determine the effectiveness of a particular VE.
For example, if a VE is developed to train participants to complete an assembly task, one could create tests of that training, for example, number of units assembled per unit time, number of errors
per unit time, or percentage of units correctly assembled. One could then develop a controlled experiment where some participants are trained using the VE and some are trained using whatever
the traditional technique is. Then, when both sets of users are tested post-training, these measures
would give some concrete evidence for whether the VE was effective at training. Such formal training transfer studies are rarely conducted, due to the time, effort, and cost required. That said, they
are sometimes done, especially for training of mission critical personnel such as astronauts [79],
shipboard firefighters [143], and surgeons [72, 74]. Even when such studies are performed, though,
they do not enable the comparison of results among different VEs designed for different purposes.
The development of generalizable measures of VE effectiveness, then, remains an open research
problem. The identification of potential constructs, such as presence, and the development of appropriate measures for said constructs have been driving VE research for decades, and continue
to do so today.
2.1
Presence: What and Why
The presence concept was introduced to the computing literature by Akin and colleagues, who
defined telepresence as the condition that occurs when, “At the worksite, the manipulators have
the dexterity to allow the operator to perform normal human functions. At the control station,
the operator receives sufficient quantity and quality of sensory feedback to provide a feeling of
actual presence at the worksite” [2]. Presence has since been defined and operationalized in many
ways by different researchers, but it is most commonly defined as something akin to the feeling of
“being there” in a virtual place. One example comes from Witmer and Singer, who defined presence
as “the subjective experience of being in one place or environment, even when one is physically
situated in another” [157].
Presence has the distinct advantage of being a metric applicable to any VE. One can reasonably
ask how present a user was in any given VE A, and then ask how present the user was in some
VE B, and if the user reports more presence in VE A, then that is some evidence that enables the
comparison of VEsA and B, though they may represent entirely different scenarios and be designed
for entirely different purposes.
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 3 -->

A Survey of Presence and Related Concepts
96:3
While conceptually appealing, the evaluation procedure described in the previous paragraph
has several important flaws. First is that determining “how present” a user is is in itself a very
difficult problem. Presence is what the philosophy literature calls a quale (plural qualia), which is
defined as a subjective and internal feeling elicited by sense perceptions. This subjective and internal nature makes measurement of presence (or any quale) extremely difficult. The predominant
method has been to use one or more post-experiment questionnaires to measure presence, but this
is itself problematic. There have been efforts to develop objective correlates of presence, including
physiological [87] and behavioral [47] measures, but these are also flawed, requiring addition to
or modification of elements of the VE to enable measurement of presence.
For example, the most common physiological surrogate for presence is arousal, which can be detected using measures such as heart rate or skin conductance. The change in heart rate associated
with the onset of a stressful stimulus was shown by Meehan to correlate with presence [87]. However, adding a stressful stimulus to a non-stressful training task may violate the ecological validity
of the training. Or, if a task also involves physical exertion, it may not be possible to distinguish the
effect of the stressful stimulus from the heart rate changes associated with the exertion. Therefore,
while physiological and behavioral measures are promising, they are not universal solutions.
Hendrix and Barfield proposed that a subjective measure of presence should be relevant, sensitive, convenient, nonintrusive, and reliable [63]. In Meehan’s dissertation he posited that an ideal
measurement of presence would be reliable, that is, producing repeatable results, both within and
between subjects; valid, that is, demonstrated to correlate with the subjective feeling of presence;
multi-level-sensitive; and objective [88]. These are standard principles of sound testing practices
[1]. We would go further and suggest that such an ideal metric should also be measurable contemporaneously, continually, and without modification to the scenario, and should be generalizable
across VEs. No measure of presence yet exists that meets all of these criteria.
A second important flaw regarding the use of presence as a universal VE effectiveness measure,
beyond the difficulty inherent in measuring presence, is that it has not been conclusively demonstrated that more presence is necessarily a good thing. Welch argues powerfully that there is no
inherent reason to think that more presence leads to improved task performance in a VE [151].
Experimental results linking presence and task performance are mixed [90, 124, 135, 157], and
even so, it is difficult to distinguish whether any benefits would be due to increased presence or
increased immersion.
2.2
Immersion
The concept of immersion is the source of some confusion in its own right. Slater has consistently regarded immersion as an objective characteristic of a VE system [118]. This is in contrast
to Witmer and Singer, who define immersion as, “a psychological state characterized by perceiving
oneself to be enveloped by, included in, and interacting with an environment that provides a continuous stream of stimuli and experiences” [157]. Lombard and colleagues refer to these different
conceptions of immersion as perceptual immersion [16] and psychological immersion, respectively
[81]. These are clearly related concepts—Slater’s immersion is what makes it possible to experience Witmer and Singer’s immersion—but using them interchangeably has led to a lack of clarity
in the VE literature. In addition, immersion is often used as a term synonymous with presence.
(For some examples of such, see References [97, 153].) In this document, we follow Slater in using
immersion to mean an objective characteristic of a VE system. Specifically, we define immersion
as the set of valid actions supported by a VE system [121].
We believe, again following Slater, that, “Immersion provides the boundaries within which [presence] can occur” [121]. However, studying the immersion of VE systems has significant utility beyond the fact that it enables presence. For example, Bowman and McMahan argue that, “Presence
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 4 -->

96:4
R. Skarbez et al.
might not be immersion’s only benefit: Applications can take advantage of other side effects of
high levels of immersion,” such as spatial understanding or increased peripheral awareness [27].
2.3
Social Presence, Copresence, and Related Terms
One shortcoming in the common understanding of presence is that it does not include any notion
of social interaction: The prevalent interpretations and uses of the term presence focus on a single
user’s interaction with an environment. In practice, a VE may contain other characters, controlled
by computers or humans, with whom the user may (or may not) interact. To overcome this deficiency, researchers have adopted the terms copresence and social presence to discuss and reason
about users’ interactions with characters in virtual environments.
The term copresence was first coined by Goffman in the course of his describing human behavior
in public places as, “exist[ing] when people sensed that they were able to perceive others and that
others were able to actively perceive them...render[ing] persons uniquely accessible, available, and
subject to one another” [56]. It has also been defined as, “a condition in which instant two-way
human interactions can take place” [159], and even more succinctly as, “being there together” [107,
108]. Note that although these concepts are clearly related, there are important differences: The copresence definitions from Goffman and Zhao refer to properties of a communication medium, and
so are objective, immersive characteristics of a system; on the other hand, Schroeder’s definition
implies that copresence is a quale, the feeling of being together in a place.
The term social presence was first defined by Short et al. in their investigation of the social
psychology of telecommunications as, “the degree of salience of the other person in the interaction
and the consequent salience of the interpersonal relationships” [114]. It has also been defined as
“when one person feels another person is ‘there”’ [31], “the perception of a medium’s ability to
connect people” [94], and “the awareness of being present with others in a mediated environment
combined with a certain degree of attention to the other’s intentional, cognitive, or affective states”
[148]. Here, while all of these authors define social presence as a quale, the definitions again differ
in important ways: The feeling described by Nowak and Biocca does not involve another being,
but all the others do; the definition of van der Land and colleagues requires attention on the part
of the user, while Bull’s definition does not.
Note also that the terms copresence and social presence can have significant overlap, and in fact,
are often used interchangeably [6, 19]. Additionally, the term social presence is used with multiple
meanings, both as a system characteristic that is a prerequisite for copresence (Social presence
is “[H]ow well a communications medium transmits verbal and nonverbal cues as well as the
apparent distance or ‘realness’ of the communicators” [91].), and as a quale that is contingent upon
copresence (“Mediated social presence is the moment-by-moment awareness of the co-presence of
another sentient being accompanied by a sense of engagement with the other (i.e., human, animate,
or artificial being)” [17].)
In this review, we follow Biocca et al. and define copresence as a quale that is required for a
user to experience social presence [17]. Specifically, we define copresence as the sense of being
together with another or others, and social presence as the moment-by-moment awareness of the
copresence of another sentient being accompanied by a sense of engagement with them. Following
Biocca et al., the difference between the two is the extent to which one’s experience depends on
the other or others. All that is required for copresence is the awareness that another being exists in
the space; social presence, on the other hand, does not develop without some degree of interaction,
wherein one’s behavior and/or psychological state is affected by the other or vice versa.
At this point, we would like to coin and argue for the use of the term Social Presence Illusion, rather than the term social presence, to refer to the feeling of social presence engendered
by characters in virtual or mediated environments. We have shown in this section that the terms
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 5 -->

A Survey of Presence and Related Concepts
96:5
copresence and social presence have confusing and occasionally contradictory definitions. The use
of the term Social Presence Illusion makes explicit that we are referring to the illusory (false) feeling of being together with and engaging with a real sentient being. To refer to the feeling of being
together and interacting with a real person in the real world, we continue to endorse the term social presence. Similarly for the terms Copresence Illusion and copresence, which refer to the feeling
of “being together” in a virtual or mediated space and the feeling of “being together” in a real space,
respectively.
Note, however, that so defining copresence and social presence means that we no longer have a
term to refer to the feeling that a medium provides the necessary affordances for social interaction.
In the words of Sivunen and Nordbäck, “some researchers have separated copresence from social
presence on the basis that the latter relates to the quality of the medium and users’ perceptions
of it, whereas copresence...addresses the psychological interaction of the individuals” [115]. For
example, Lombard et al. used social presence to refer to “the extent to which a medium is perceived
as sociable, warm, sensitive, personal or intimate when it is used to interact with other people”
[80]. To address this shortcoming, we propose the term communicative salience to refer to this
feeling, as well as the term communicative immersion to refer to the objective characteristics of the
underlying medium that contribute to communicative salience.
As presence depends on immersion, and Plausibility Illusion on coherence (these are discussed
in Sections 2.5 and 2.6), so Social Presence Illusion must be constrained by some characteristics
of the underlying system. We argue that Social Presence Illusion depends on three things: (1) The
company of another “sentient” being or beings in the virtual or mediated environment, (2) The
ability of the medium to transmit communicative signals (voice, eye contact, posture, etc.), and (3)
“Appropriate” behavior of the other sentient being or beings. (1) is the Copresence Illusion, (2) is
what we previously defined as communicative immersion, and is a subset of the overall immersion
of the VE, and (3) is a subset of coherence. (Communicative coherence, perhaps.)
Note that a medium can support Copresence Illusion and Social Presence Illusion without giving
rise to the feeling of being in another place. Consider the case of speaking with someone on the
telephone: “[F]or example, talking on a telephone with someone might give a strong sense of
‘being with them’ but not of being in the same place as them” [125]. Here, you are certainly aware
of the person on the other end of the line (Copresence Illusion), and you can interact with that
other person (Social Presence Illusion). However, you do not get the impression that you have
been transported to another place.
2.4
Realism and Fidelity
Another potential shortcoming of presence as a generalizable measure is that it does not account
for the realism of the scenario being presented. However, for some scenarios, such as military or
surgical training, it may be important that the scenario correspond to reality to the maximum
extent possible. Alexander et al. describe fidelity as “the extent to which the virtual environment
emulates the real world,” and identify several relevant subcategories of fidelity, including physical (“the physical simulation looks, sounds, and feels like the operational environment”), functional (“the simulation acts like the operational equipment in reacting to the tasks executed by the
trainee”), and psychological (“the simulation replicates the psychological factors...experienced in
the real-world environment”) [3].
Stoffregen et al. describe stimulus fidelity as the extent to which sensory stimuli produced by
a simulator are identical to those produced by the system being simulated. Stimulus fidelity is
therefore an objective characteristic of a simulation, as it depends only on sensory stimuli, rather
than perceptions of those stimuli. The authors also cite work by Riccio, who described experiential
fidelity as “fidelity of subjective experience” and action fidelity as “fidelity of performance” [99].
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 6 -->

96:6
R. Skarbez et al.
Stimulus fidelity as so defined is akin to our definition of immersion; it is an objective characteristic
of the simulator/VE. Experiential fidelity is similar to presence, in that it is a user’s subjective
experience of the reality of the scenario. (In fact, it is even more similar to Plausibility Illusion,
defined in Section 2.5). Action fidelity is akin to, or perhaps a component of, training transfer: Do
the actions a user takes in the simulator/VE match the actions that he or she would take in the real
world?
In this document, we accept Alexander’s definition of fidelity as “the extent to which the virtual environment emulates the real world” [3]. Fidelity as a construct is logically orthogonal to
immersion. On the one hand, it is possible to create a high level of immersion in an unrealistic
or fantastical scenario, and on the other, it is possible to have a high degree of fidelity in lowimmersion media.
2.5
Place Illusion and Plausibility Illusion
To address some of the confusion relating to the presence construct (as explicated in Section 3),
Slater proposed a theory that presence is composed of two logically orthogonal components, Place
Illusion (PI) and Plausibility Illusion (Psi). He defined PI as, “the...illusion of being in a place in spite
of the sure knowledge that you are not there,” and Psi as, “the illusion that what is apparently
happening is really happening (even though you know for sure that it is not)” [121]. PI, then,
corresponds to the traditional conception of (spatial or place) presence as “being there,” while Psi
represents an entirely different conception of presence, that of believing what you are seeing. For
example, assume you are in a VE intended to represent a library. Here, presence would be your
feeling of, “I am in a real library.” If you turned your head and saw more bookshelves, then that
would reinforce your feeling of PI. If all the library patrons were being quiet, then that would
reinforce your feeling of Psi. Contrarily, if you turned your head and the imagery didn’t change,
then that would break PI, and if patrons were yelling loudly in the library, then that would break
Psi.
We believe that that there are several benefits to this theoretical framework. First, by introducing
the terminology Place Illusion to replace spatial/place/tele/presence, Slater “make[s] it clear that
we refer specifically and only to the strong illusion of being in a place and not to other multiple
meanings that have since been attributed to the word ‘presence”’ [121]. Second, by introducing the
concept of Plausibility Illusion and making it comparable in importance to Place Illusion, Slater
reifies fidelity and correct behavior as important components of virtual experience.
2.6
Coherence
In the article that introduced Place Illusion and Plausibility Illusion, Slater stated that “Immersion
provides the boundaries within which [Place Illusion] can occur” [121]. That is, the immersion of
a system enables the feeling of Place Illusion. In his dissertation, Skarbez argues that there must be
a construct parallel to immersion that is an objective characteristic of a virtual scenario that gives
rise to Plausibility Illusion. To that end, he defines coherence as the set of reasonable circumstances
that can be demonstrated by the scenario without introducing unreasonable circumstances, where
a reasonable circumstance is a state of affairs in a virtual scenario that is self-evident given prior
knowledge [116].
Coherence can be thought of as a superset of realism or fidelity. Specifically, coherence makes no
assumptions about a VE having to faithfully represent the real world. Rather, coherence depends
on the internal logical and behavioral consistency of the virtual experience. If one has been led
to believe that he or she is going to experience a virtual fantasy world, then the appearance of
a character flying hundreds of feet in the air would be coherent behavior. On the other hand, if
one has been led to believe that he or she is going to experience a realistic training scenario, the
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 7 -->

A Survey of Presence and Related Concepts
96:7
very same behavior would be incoherent, and would likely decrease a user’s feeling of Plausibility
Illusion.
Gilbert independently proposed a very similar construct, that of authenticity [55]. He defines
the authenticity of a VE as the degree to which it supports “(1) users’ expectations based on their
Bayesian priors for regularities in the real world and (2) the users’ intentions in the VE.” It “refers to
whether the virtual environment provides the experience expected by the user, both consciously
and unconsciously.” As written, authenticity applies only to VEs that attempt to replicate some
aspect of the real world, while coherence makes no such requirement. Gilbert’s definition, however,
does enable an alternative definition of reasonable circumstances, which can now be considered
as those circumstances that align with users’ Bayesian priors. We believe that authenticity and
coherence are in fact different terms for the same construct; throughout this review, we will use
the term coherence to refer to this construct.
An open question regarding coherence is whether it is truly an objective construct. Skarbez’s
original definition of a reasonable circumstance given previously raises the question, “Whose prior
knowledge?” The redefinition prompted by Gilbert raises the question, “Whose Bayesian priors?”
As a thought experiment, one can imagine a VE in which every depicted action (or inaction) can
be explained by information previously presented in the VE; that is, it requires no prior knowledge
whatsoever. It seems to us, however, that the existence of such a VE would imply the existence
of a perfect simulation of the history of the universe. Practically, every VE assumes some prior
knowledge and set of experiences on the part of its users. If this is the case, then coherence cannot
be purely objective.
That said, we believe that it is useful to treat coherence as if it were objective. A VE developer
may not be able to control users’ prior knowledge; however, he or she is able to control whether
the events depicted in the VE are internally consistent, and he or she is able to minimize the extent
to which the “reasonableness” of events depends on assumptions made by the user by explicitly
priming the user to expect certain types of behavior—thereby altering the user’s Bayesian priors (consider the flying example presented earlier). By doing so, the set of objectively reasonable
circumstances—that is, states of affairs that are self-evident given prior knowledge provided in the
context of the virtual experience—can be maximized. We therefore propose to redefine coherence as
the set of objectively reasonable circumstances that can be demonstrated by the scenario without
introducing objectively unreasonable circumstances.
2.7
Embodiment, Body Ownership, and Self-Presence
Within the computing literature, embodiment generally refers to the representation of a user (also
known as an avatar) within a mediated or virtual environment. As examples, Gabbard states that,
“Representing the user within a VE is known as user embodiment” [50], and Benford et al. state
that, “User embodiment concerns the provision of users with appropriate body images to represent
them to others (and also to themselves) in collaborative situations” [11].
In the psychology and philosophy fields, though, embodiment has a different meaning, that is,
“The psychology of presence is related to the body and to the embodiment process” [102]. Blanke
and Metzinger state that embodiment includes, “the subjective experience of using and ‘having’
a body” [18]. De Vignemont defines embodiment as follows: “E is embodied if and only if some
properties of E are processed in the same way as the properties of one’s body” [41]. Inspired by de
Vignemont’s definition of embodiment, Kilteni, Groten, and Slater define Sense of Embodiment as
follows: “[Sense of Embodiment] toward a body B is the sense that emerges when B’s properties
are processed as if they were the properties of one’s own biological body” [70]. De Vignemont’s
embodiment refers to a properties of a single body part or object being processed as if it were part
of one’s own body, while Kilteni et al.’s Sense of Embodiment refers to properties of a whole body
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 8 -->

96:8
R. Skarbez et al.
being processed in the same way. Kilteni et al. also provide a “working definition” for Sense of
Embodiment, defining it as a combination of three subcomponents, “the sense of self-location, the
sense of agency, and the sense of body ownership” [70].
Embodiment so defined can be measured by questionnaires and behavioral measures; for an
example of such, see Botvinick and Cohen’s presentation of the Rubber Hand Illusion [22].
Ownership is the sense that a body (or body part) is one’s own. De Vignemont states that, “Embodiment is a necessary condition for the feeling of ownership” [41]. But the two are distinct.
Embodiment can be felt with tools, for example, but that does not lead to a sense of ownership.
Slater et al. have explored the illusion of body ownership with regard to a purely virtual body
[127].
Related to embodiment and ownership is the feeling of self-presence.
“Self-presence is defined as users’ mental model of themselves inside the virtual
world, but especially differences in self-presence due to the short term or long
term effect of virtual environment on the perception of one’s body (i.e., body
schema or body image), physiological states, emotional states, perceived traits, and
identity...Self-presence refers to the effect of embodiment in [a] virtual environment
on mental models of the self” [13].
Alternatively, Lee defines self-presence as, “a psychological state in which virtual (para-authentic
or artificial) self/selves are experienced in the actual self in either sensory or nonsensory ways”
[77].
2.8
Other Concepts Related to Presence
The preceding sections address constructs frequently and specifically explored using or regarding virtual environments. There are other constructs from outside the VE literature that are related to presence, however. The following paragraphs provide an introduction to several of these
constructs.
Involvement and Engagement. We group involvement and engagement under one heading as
the terms are generally used interchangeably (as in, “the term ‘engagement’ [is] used as a generic
indicator of game involvement” [28]), to mean something like a state of focused attention or interest. For example, Witmer and Singer define involvement as, “a psychological state experienced
as a consequence of focusing one’s energy and attention on a coherent set of stimuli or meaningfully related activities and events. Involvement depends on the degree of significance or meaning
that the individual attaches to the stimuli, activities, or events” [157]. Böcking et al. define involvement as, “the intense cognitive engagement with a media environment that can be observed via
processes of appraisal, elaboration, evaluations, and mental explorations...the active and intense
processing of the world presented by the media” [20]. McQuarrie and Munson’s Revised Product Involvement Inventory (RPII) identifies two facets of involvement: perceived importance and
interest [86].
The Witmer-Singer Presence Questionnaire [157], the ITC-Sense of Presence Inventory (ITCSOPI) [78], and the Igroup Presence Questionnaire (IPQ) [109] all contain subscales regarding involvement or engagement. In addition, the Game Engagement Questionnaire (GEQ) of Brockmyer
et al. is an instrument specifically designed to measure the level of involvement/engagement in
video games [28], although it has been adapted and used in the study of virtual environments as
well [85].
We note that while some presence questionnaires, including those listed previously, explicitly
consider involvement to be a component of the presence construct, we do not. As with some
of the other constructs discussed previously, presence is logically orthogonal to involvement, as
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 9 -->

A Survey of Presence and Related Concepts
96:9
illustrated by the following examples: “One can be present but not involved (as in many situations
in everyday life). One can be involved but not present (e.g., watching a soap opera, reading a book)”
[120], or “[A] user can feel spatially present in a VE designed to be boring without feeling engaged
in it or cognitively involved” [39].
Flow. Flow is described as an optimal state of concentration, “the state in which individuals are
so involved in an activity that nothing else seems to matter” [37]. Novak et al. describe Csikszentmihalyi’s model of flow as follows:
A good starting point is the comprehensive listing of eight components of flow
provided by [38]: (1) a clear goal, (2) feedback, (3) challenges match skills, (4) concentration and focus, (5) control, (6) loss of self consciousness, (7) transformation
of time, and (8) the activity becomes autotelic (that is, perceived as worth doing for
its own sake). While structural relations among the constructs are not specified,
the constructs are grouped according to whether they specify antecedent conditions of flow (1, 2, and 3), its characteristics (4 and 5), or the consequences of the
experience (6, 7, and 8) [93].
In Novak et al.’s model of flow, telepresence appears as a contributing factor to flow [93]. This
finding is supported by a study by Takatalo, who found a similar connection between presence
and flow in a virtual environment [141]. (Novak et al.’s study regarded use of the World Wide
Web.) Brockmyer et al. argue that flow, since it involves experiencing an altered state, may be a
deeper state of engagement with media than presence [28]. Hoffman and Novak present a survey
of existing literature on flow on the Web, as well as a discussion regarding flow and virtual worlds,
in Reference [66].
Absorption. Absorption is described as, “the ability to get lost in the task at hand whether it is
watching a movie, reading a book, or experiencing VR” [9], or as “the tendency to become fully
involved in a perceptual, imaginative, or ideational experience” [144]. Brockmyer et al. argue that
absorption is an even a deeper state of engagement with media than flow or presence [28].
The Tellegen-Atkinson Absorption Scale is an instrument consisting of six Likert-scale questions
that measures openness to absorption [144]. Note that this is a measure of trait (a consistent and
long-lasting tendency), not state (a temporary feeling based on one’s situation); as such, it is a
measure of individual differences, which will be discussed further elsewhere in this article.
Transportation. Broadly speaking, the concept of transportation is to narrative worlds as the
concept of presence is to technology-mediated worlds [53]. In a state of transportation, “[T]he
reader loses access to some real-world facts in favor of accepting the narrative world that the
author has created...transported readers may experience strong emotions and motivations, even
when they know the events in the story are not real” [58].
Transportability refers to a person’s inherent ability to be transported by a narrative. There is
not an equivalent term in the field of presence research, although this idea was explored in the
form of Witmer and Singer’s Immersive Tendencies Questionnaire [157]. There are transportation
and transportability questionnaires that are analogous to the PQ and ITQ, respectively [57, 58].
Agency. Agency [104] is, “the sense that I am the one who is causing or generating an action”
[51], or “the satisfying power to take meaningful action and see the results of our decisions and
choices” [92]. Agency has been identified as a concept that may share some features and factors
with presence [65]. There is some speculation that the brain mechanisms that give rise to the sense
of agency may be related to those that give rise to presence [40, 112].
Reality Judgment. Baños and colleagues argue for the existence of reality judgment as a construct
separate from presence. They point out that one can attribute reality to something without feeling
a sense of presence, for example, when watching a news broadcast; or vice versa, as when playing a
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 10 -->

96:10
R. Skarbez et al.
fantasy video game. So reality judgment (the belief that our experiences are real) should be treated
as related to, but distinct from, presence [7, 8]. Thus, reality judgment is roughly synonymous with
Plausibility Illusion.
2.9
Analysis
As we’ve seen in this section, presence is not the only relevant construct in the evaluation of virtual environments, nor is it truly a universal measure of VE effectiveness. In particular, virtual
environments that do not represent a particular place, such as visualization applications, are unlikely to benefit from a sense of “being there.” They may, however, benefit from other side effects
of increased immersion [27].
Even in the many VE applications for which presence is likely to be an effective measure, one
or more of the other constructs discussed in this section may be equally or more relevant. For
example, in applications that have the goal of predicting real world behavior, such as ergonomic
evaluations, immersion and fidelity are likely most important [67, 96]. In telepresence or group
training applications, Social Presence Illusion is likely at least as important as (spatial) presence.
In applications where users are doing real work inside a VE, the ability to induce a state of involvement or flow might be more important. For applications whose goal is transfer of training to the
real world, fidelity is likely to be important. For entertainment applications, or other applications
that seek to elicit a feeling of absorption, coherence might be more important than immersion. (Or
in terms of desired outcomes, Plausibility Illusion might be more important than Place Illusion.)
Even taking all of this into account, presence remains a centrally important idea in the development and evaluation of virtual environments. In this section, we introduced the presence
construct, as well as several related constructs including immersion, social presence, copresence,
fidelity, coherence, Place Illusion, and Plausibility Illusion. The remainder of this article focuses
on the explication of presence, commenting on the many ways it is defined, its proposed models,
and the methods that have been employed for its measurement.
3
DEFINING PRESENCE
Many definitions of presence have been proposed in the literature. We propose that these can be
grouped into three categories: being there, non-mediation, and other. Those definitions we classify
as being there consider presence to be the feeling of being in an environment, while those we
classify as non-mediation consider presence to be a lack of attention to the mediating technology.
Those definitions grouped under other define presence as the experience of virtual objects as a
focus on direct perceptual processing [150], presence as the perception of objects as real [77],
presence as the feeling that the simulator is actually the simulated [140], or presence as the sense
of feeling real [95].
We further propose that the being there definitions can be subdivided into two subcategories:
active (in which the ability to act is specifically considered as part of the definition) and passive (in
which user actions are not specifically addressed). We also propose that non-mediation definitions
consist of two subcategories: internal (in which the focus is on one’s thoughts, as in “suspension
of disbelief” and external (in which the focus is on the technology, as in the “illusion of nonmediation”). The publications in which the definitions appear are, in Table 1, sorted into these
categories and subcategories.
In the remainder of this section, we present these definitions grouped by category and arranged
in chronological order within each category, to better highlight the evolution of the concept over
time. The definitions are listed so the reader can better appreciate the important differences between the various definitions and to provide context for the analysis presented in Section 3.2.
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 11 -->

A Survey of Presence and Related Concepts
96:11
Table 1. Sources of Definitions of Presence Sorted by Category
Being there
Non-mediation
Other
Active
Passive
External
Internal
Perceptual processing
Steuer, 1992 [139]
Witmer and Singer,
1998 [157]
Lombard and Ditton,
1997 [80]
Slater and Usoh, 1993
[131]
Waterworth and
Waterworth, 2001 [150]
Schloerb, 1995 [106]
Sas and O’Hare, 2003
[105]
ISPR, 2000 [69]
Flach and Holden, 1998
[46]
Spagnolli and
Gamberini, 2004 [138]
Simulator is simulated
Zahorik and Jenison, 1998
[158]
Wirth et al., 2004 [155]
Stoffregen et al., 2003
[140]
Mantovani and Riva, 2001
[84]
Biocca, 2001 [14]
Real objects
Slater, 2004 [120]
Lee, 2004 [77]
Carassa et al., 2005 [34]
Witmer et al., 2005 [156]
Feeling real
Riva et al., 2006 [101]
Parola et al., 2016 [95]
Herrera et al., 2006 [65]
Wirth et al., 2007 [154]
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 12 -->

96:12
R. Skarbez et al.
3.1
Definitions
The notion of presence as it is used in the context of virtual reality can be traced to psychologist
James Gibson, via Jonathan Steuer [139].
Presence can be thought of as the experience of one’s physical environment; it
refers not to one’s surroundings as they exist in the physical world, but to the
perception of those surroundings as mediated by both automatic and controlled
mental processes [54]: Presence is defined as the sense of being in an environment.
From Gibson comes the notion that, “The environment of animals and men is what they perceive.
The environment is not the same as the physical world, if one means by that the world described
by physics” [54]. In this Gibsonian context presence is explicitly in the context of the real world,
but already the idea is in place that presence can’t be determined simply by considering the ground
truth of the real environment: Presence is a subjective feeling generated by our perception of the
real world as mediated by our sense organs and the mental processes governing and integrating
them.
The term telepresence can be traced back to Marvin Minsky’s 1980 essay of the same name.
Minsky does not explicitly provide a definition for the term, but does state that, “The biggest
challenge to developing telepresence is achieving that sense of ‘being there’ [89].
3.1.1
Being There. Steuer introduced Gibson’s notion of presence to the field of computermediated environments, defining the term telepresence as “the experience of presence (in the
sense of Gibson) in an environment by means of a communication medium” [139]. Steuer’s definition marks the start of some significant confusion, as many researchers have been concerned
primarily—or only—with the sense of presence in computer-mediated or virtual environments, but
common practice has been to refer to the sensation simply as presence, rather than “telepresence,”
“mediated presence,” or “virtual presence.”
Schloerb introduced an “objective” definition of presence in Reference [106]. Subjective presence
occurs when one perceives oneself as physically present in an environment. However, one is only
objectively present if one can successfully complete a specified task in the environment. Here, then,
we have an explicit, and in fact definitional, link between presence and task performance: If one
can successfully complete more tasks more often, then one is more present. This suggests a very
natural method for measuring presence, however, we disagree with this conception of presence.
For example, a professional baseball player would likely perform much better than an average
person in a virtual baseball-hitting scenario, but to suggest that this means that the professional is
more present seems inappropriate, especially if this difference in performance also applies in the
real world.
Flach and Holden returned to Gibson’s research as the basis of presence [46]. To Gibson, “the
reality of experience is grounded in action”—humans see the world in terms of affordances, that is,
in how can they interact with the world around them. The important characteristics of the world
(in particular, the characteristics of the world that are important for experiencing presence), then,
are behavioral, rather than aesthetic.
Continuing that line of thinking, Zahorik and Jenison described presence as “tantamount to successfully supported action in the environment” [158]. To them, presence is determined by the extent that the perception/action coupling in the virtual world matches our learned perception/action
coupling in the real world.
Mantovani and Riva presented a view of the Gibsonian actor in [84]. For such an ecologically
situated actor there is not a clear separation of the subjective internal model of the world and the
objective ground truth of the outer world. Rather, the actor is constantly in a process of adaptation
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 13 -->

A Survey of Presence and Related Concepts
96:13
to the estimated (that is, mediated) world in which it exists. In this picture, one’s willingness
to “react as if real” to the observed stimuli and the world’s ability to “react as if real” to their
sensorimotor actions are in fact inseparable.
These Gibsonian arguments (of Flach and Holden, Zahorik and Jenison, and Mantovani and
Riva) are echoed in later conceptions of presence, such as Slater’s Place Illusion, in which the
illusion derives from the valid actions that are supported by the experience [121].
In the article that presented their landmark Presence Questionnaire, Witmer and Singer defined
presence as, “the subjective experience of being in one place or environment, even when one is
physically situated in another” [157].
In 2001, Biocca defined presence as “the phenomenal state by which an individual feels located
and active in an environment, and, especially in the case of telepresence, the class of experience
where the environment is mediated by a technology” [14]. So here, the user must not only be
“located” (the traditional sense of “being there”), but must also be “active.” This is in keeping with
the Gibsonian tradition, as in Zahorik and Jenison [158] and Flach and Holden [46]. Note also that
all these authors treat telepresence as a special case of presence, and that presence can be (and
normally is) felt in the real world.
In 2003, Slater revisited presence terminology, describing presence as a “response” to “an appropriate conjunction of the human perceptual and motor system and immersion” [120]. This is quite
similar (albeit using very different terminology) to Zahorik and Jenison’s conception of presence as
being-in-the-world [158]. To Slater, if we assume there is an actor (with a functioning perceptuomotor system) ecologically situated in the world (the precise nature of the world and this situation
being defined as immersion), then presence arises to the extent that a valid perception/action coupling is supported by the virtual environment system. Also, note the novel conception of presence
as a “response.” Presence, in this conception, can occur involuntarily: if the correct set of stimuli
are provided (in terms of the immersion of the system and the perceptuomotor characteristics of
the individual user), then presence will result. This seems to represent an evolution in thinking
from Slater’s earlier definition of presence involving suspension of disbelief.
Sas and O’Hare offered a slightly different conception of presence: one is present in another
world (mediated or imaginary) if (1) one’s cognitive processes are oriented toward that world
to the extent that one experiences “being there,” and (2) one’s focus of consciousness is on the
proximal (body-oriented, perhaps) stimuli in the mediated or imaginary world [105]. Here, as in
Biocca [14], we see a definition of presence as “being there plus,” in this case, the “plus” being the
fact that one is responding to stimuli from the virtual world, rather than the real one. It appears
that this definition assumes that one can, at any given moment, be present in one or the other
environment; that is, that presence is binary. That consciousness can simultaneously have two
foci seems unlikely.
Spagnolli and Gamberini, on the other hand, maintained the focus of presence on location [138]:
“Whenever a person is qualified as ‘present’...her location is the salient, characterizing feature.” If
one follows this line of thinking, then an interaction with a virtual human in the real world might
elicit a whole host of feelings, but it would not elicit a sense of presence in a mediated environment.
Wirth and colleagues defined spatial presence as “the subjective experience of being in the mediated environment” [155]. Here, again, we have presence limited to mediated environments. For
the authors it has two components: the sensation of being physically situated in the environment
(self-location) and the perception of possibilities to act in that environment (possible actions). This
is another example of “being there plus,” as well as another definition of presence that is largely
in keeping with the traditional Gibsonian definition.
Carassa and her colleagues proposed a definition of presence inspired by situated cognition
theory, in which “presence depends on the proper integration of aspects relevant to an agent’s
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 14 -->

96:14
R. Skarbez et al.
movement and perception, to her actions, and to her conception of the overall situation in which
she finds herself, as well as on how these aspects mesh with the possibilities for action afforded in
the interaction with the virtual environment” [34]. In our interpretation, this correctly integrates
a user’s learned expectations for correct behavior into the Gibsonian model of presence in virtual
environments.
Witmer and Singer clarified their definition of presence in Reference [156]. Here, presence is defined as a psychological state of “being there mediated by an environment that engages our senses,
captures our attention, and fosters our active involvement.” Witmer and Singer also define involvement as “a psychological state experienced as a consequence of focusing one’s mental energy and
attention on a coherent set of stimuli or meaningfully related activities or events.”
Riva and colleagues defined presence as “the non-mediated (prereflexive) perception of successfully transforming intentions in action (enaction) within an external world” [101]. This builds on
Zahorik and Jenison’s conception of presence as successfully supported action in the environment
[158]. Here, we have no distinction between real, virtual, or imaginary worlds: you can feel present
in any or all of them if you are able to transform your intentions into action. Also, it is a prereflexive, or intuitive, perception: it is again something that “just happens” if the system is sufficiently
in tune with your needs (or vice versa), similar to Slater’s conception of presence as a response
[120].
Herrera et al. defined presence as the “conscious awareness of self, as both agent and experiencer, which characterizes the experiencing self of natural environments” [65]. Here again, this
could apply to real, virtual, and mediated environments (although, the authors state, not imaginary ones—the environments they refer to are “experienc[ed],” not imagined). This conception of
self as both “agent and experiencer” again echoes Gibson, in whose view one is always both acting
on and being acted upon by the environment.
Wirth and colleagues refined their definition of spatial presence as, “a binary experience, during
which perceived self-location and, in most cases, perceived action possibilities are connected to
a mediated spatial environment, and mental capacities are bound by the mediated environment
instead of reality” [154].
3.1.2
Non-mediation. Slater and Usoh introduced the notion that presence in a mediated environment is “(suspension of dis-)belief that [one] is in a world other than where [one’s] body is
located” [131]. Slater and Usoh’s definition introduced several new ideas: one, that we first believe
that we are not in the mediated environment, and two, that by some process, we can overcome
that belief. This idea of presence involving “suspension of disbelief” is a recurring concept in the
presence literature.
Lombard and Ditton proposed that presence is “the perceptual illusion of nonmediation” [80].
Note that this definition is explicitly for tele- or virtual presence, not presence in a real environment; it assumes the existence of a communication medium that can seem to disappear. One could
make the argument, as in Gibson, that our experience of the world is always mediated—that our
perception of the world is not the same as the world itself—and so presence in the real world is
only a special case of such mediated presence experiences. Lombard and Ditton did not make this
argument.
Lombard and Ditton also explicitly defined presence as binary: “It does not occur in degrees
but either does or does not occur at any instance during media use.” This is associated with the
conceptualization of presence as an illusion: either the illusion is in place, or it is broken. Slater’s
later conceptions of Place Illusion and Plausibility Illusion are very much in keeping with this
school of thought [121].
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 15 -->

A Survey of Presence and Related Concepts
96:15
Presence was officially defined by the International Society for Presence Research as follows:
Presence (a shortened version of the term “telepresence”) is a psychological state
or subjective perception in which even though part or all of an individual’s current experience is generated by and/or filtered through human-made technology,
part or all of the individual’s perception fails to accurately acknowledge the role of
the technology in the experience. Except in the most extreme cases, the individual
can indicate correctly that s/he is using the technology, but at *some level* and to
*some degree*, her/his perceptions overlook that knowledge and objects, events,
entities, and environments are perceived as if the technology was not involved in
the experience. Experience is defined as a person’s observation of and/or interaction with objects, entities, and/or events in her/his environment; perception, the
result of perceiving, is defined as a meaningful interpretation of experience [69].
This definition is clearly indebted to Lombard and Ditton, as the focus is on the illusion of
nonmediation rather than the experience of a place. However, it would seem that the ISPR authors
reject Lombard and Ditton’s belief that presence is binary, with the language of “part or all” of
an individual overlooking the mediating technology to “some level and to some degree.” Note
also that the authors are explicit about the fact that they are using presence to mean telepresence,
indicating clearly that this definition is only applicable to technology-mediated interactions.
3.1.3
Other. Waterworth and Waterworth defined presence as “psychological focus on direct
perceptual processing,” and absence as “...conceptual processing,” such as reflection or hypothesis
testing. They specifically stated that presence as so defined can be felt in the real world, as the
perceptual processing is “of things that are present in the current environment, whether real or
virtual” [150]. In this article the authors also proposed that there are three dimensions of experience: focus (whether one is processing information perceptually or conceptually), locus (whether
attention is devoted to the real or the virtual world), and sensus (whether one is conscious or
unconscious). All of these indicate an attentional component of presence in their conception of it.
Stoffregen et al. defined presence as, “[A]n illusory (false) perception that the simulator is the
simulated” [140]. This echoes Schloerb’s test for subjective presence, in which a person is asked
to choose whether he or she is physically present in an environment, or interacting with the environment remotely, and their degree of subjective presence is equal to the probability that the
person says that he or she is physically present when he or she is actually interacting remotely
[106]. Also, note that Stoffregen et al. make it part of the definition that this is a false impression,
following Lombard and Ditton [80] and foreshadowing Slater [121].
Kwan Min Lee defined presence as “a psychological state in which virtual (para-authentic or artificial) objects are experienced as actual objects in either sensory or nonsensory ways” [77]. This is
a new definition, that clearly puts the focus on things in the virtual world. If one experiences these
things as actual objects, then he or she is present; if one doesn’t, he or she isn’t. The “sensory or
nonsensory” language is included specifically to account for situations where feelings of presence
are elicited by non-immersive media such as text (known as the “book problem”). So “being there”
is no longer the primary quality of the experience, making this definition more amenable to usages
in applications where one, for example, interacts with a virtual human rather than experiencing a
new place.
Parola et al. defined presence as “the sense of feeling real.” They refer to the presence formation
process as an “alignment of external stimuli with an internal set of schemata,” which highlights
the importance of user expectations and prior experiences in that process [95]. This definition has
more in common with Slater’s Psi [121] or Baños’s reality judgment [8] than it does with any
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 16 -->

96:16
R. Skarbez et al.
other definitions of presence. Notably, it conflicts with definitions that place a central focus on the
feeling of being in a place, including, but not limited to, Spagnolli and Gamberini’s [138].
3.2
Analysis
So what, in the end, do we mean when we say presence? It seems to us that the shortest and most
commonly used definition, “the feeling of ‘being there’” actually comes quite close to the heart
of the matter. Defining presence as a feeling has some theoretical grounding, as well; Schubert
conceptualizes presence as a “cognitive feeling,” with all that entails. (It is caused by unconscious
processes, it is immediate, it can vary in intensity, etc.) [111].
We do not agree with some aspects of presence that appear in the definitions in the previous
section. First, we disagree with definitions that require the illusion of nonmediation. Spagnolli
and Gamberini showed that users were capable of acting simultaneously in the virtual/mediated
environment and the real environment [137]. It seems clear in this case that the user is aware, at
least on some level, that it is a mediated experience, since he or she is able to speak and act in
ways that demonstrate their awareness of the mediation. Similarly, we feel that the very existence
of the book problem [15] is reason to doubt this conception of presence. We are not aware of any
study that attempted to demonstrate that readers are present only in the environment presented
in the book, but we suspect, on face, that while a user reading a book may report feeling presence,
he or she is always aware of the fact that he or she is reading a book.
We also feel that the conception of presence as a binary (on/off) construct is not necessarily
true. The Spagnolli and Gamberini study cited previously provides some evidence to the contrary,
and Schubert also argues against this requirement. It may be true that users will report feeling
present primarily in one space at any given time, but even so, there is no reason to believe that the
strength of this feeling must be constant. It may be that “feeling of presence” can be conceived of
as a continuous function that, as it rises and falls, may rise above or fall below a binary threshold.
In addition, the definitions of Schloerb and Stoffregen et al., while conceptually clear, are of limited practical utility. In no known VE system would a user actually believe themselves to be “really
in” the virtual environment, and it would be nearly impossible to conduct a study investigating
presence as so defined, as it would have to be carried out in the absence, “not just of informed
consent but of any consent at all” [140].
Definition of presence in this article. In this article, we follow Schubert in defining (spatial) presence as the cognitive feeling of being in a place. This feeling can change based on the sensory
representation of the place (particularly in the case of a mediated environment, where this is dictated by the immersion of the mediating technology), the affordances available to the user, the
scenario in which the user finds himself, and the user’s personal history, state, and traits. Or, in
short, the user who is present is located and active in the space.
We, however, would also argue for the use of the term Place Illusion, rather than the term presence, to refer to this sensation in virtual or mediated environments. As this section has shown,
the term presence has many definitions in the literature, and these describe a range of different
constructs. The use of the term Place Illusion would make explicit that it is referring to the illusory
(false) feeling of being in a remote or virtual place. To refer to the feeling of being in a real place,
we recommend the term placeness.
Adopting the term Place Illusion for this construct also frees up the general term presence for
other usage. It is already commonly in use to mean the overall “goodness” of a virtual experience.
(For one example, see Reference [21], which describes presence as “a buzzword for what virtual
reality can offer.”) To that end, we propose a new definition of presence as, “The perceived realness
of a mediated or virtual experience.” Note that presence as so defined is a quale, with the focus on
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 17 -->

A Survey of Presence and Related Concepts
96:17
perceived realness. Actual realness, on the other hand, would be a function of a system’s ability to
provide stimuli that match reality—that is, a function of immersion and coherence.
This section has focused on theoretical definitions of presence. In the following section, we focus
on structural definitions of presence, as we present and analyze models that propose components
that contribute to or compose the presence construct.
4
MODELS OF PRESENCE
In this section, we have grouped together those articles that posit a list of components asserted
to contribute to presence. Some of these groupings are purely theoretical, and some are either the
basis for questionnaires or factors derived from questionnaires in use. Therefore, some articles
mentioned in this section will also appear in Section 6.1.1 where presence questionnaires are discussed. As well as presenting these theorized components of the presence construct here together,
we also demonstrate how these components can be usefully grouped. The models are presented
in chronological order, as in Table 2. There is no implied relationship among the data columns in
Table 2: The components for each publication are listed across each row in the order they appear
in the source publication. Figure 1 contains an illustration of these same components, grouped by
higher-order concept. Note also that Slater’s Place Illusion and Plausibility Illusion are not included
in Table 2, but they do appear as higher-order concepts in Figure 1.
4.1
Models
Akin and colleagues defined telepresence as the condition that occurs when, “At the worksite, the
manipulators have the dexterity to allow the operator to perform normal human functions. At
the control station, the operator receives sufficient quantity and quality of sensory feedback to
provide a feeling of actual presence at the worksite” [2]. In other words, we would argue that the
authors identified two factors of telepresence: ability to act in the remote environment and sensory
fidelity delivered to the user. Note that this definition is specifically referring to telepresence and
not presence or virtual presence, hence the references to worksite and control station.
Heeter proposed three dimensions of presence: subjective personal presence (feeling that you
are in the virtual environment), social presence (feeling that other beings exist in the world and
react to you), and environmental presence (feeling that the environment acknowledges and reacts
to you) [60]. Note that here Heeter is using presence as a general term to refer essentially to the
goodness or realness of a virtual experience, as we proposed in 3.2. Subjective personal presence
is most like the traditional definition of presence as “being there,” while social presence is akin
to Biocca’s definition of social presence (what we call Social Presence Illusion) and we consider
environmental presence to be a component of Plausibility Illusion.
Sheridan proposed three factors of presence: extent of sensory information, control of the relation of sensors to the environment, and ability to modify the physical environment [113]. He also
argues that presence is likely task-dependent, and that “fixed” characteristics of the experience (immersion factors and task properties) should affect dependent measures of user experience, such
as presence, training efficiency, task performance, and so on. This supports the idea that different
applications might require different aspects of user response, as discussed in 2.9.
Held and Durlach speculated on the value of telepresence, as well as its potential causal factors in [61]. They argued that telepresence is most desirable in applications where the tasks are
wide-ranging, complex, and uncertain, “because the best general purpose system known to us...is
us.” The authors go on to speculate on the factors that contribute to telepresence, identifying sensory factors—resolution, field of view, consistency of information across modalities, and displays
that are “free from production of artificial stimuli that signal the existence of the display,” motor factors—support for movements of sensory organs and of viewed effectors, high correlation
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 18 -->

96:18
R. Skarbez et al.
Table 2. List of Presence/Telepresence Models and Their Components
Source
Model components (order as listed in source)
Akin et al., 1983 [2]
Ability to act in remote
environment
Ability to sense in local
environment
Heeter, 1992 [60]
Subjective personal
presence
Social presence
Environmental presence
Sheridan, 1992 [113]
Extent of sensory
information
Control of sensors
Ability to modify physical
environment
Task dependent
characteristics
Held and Durlach,
1992 [61]
Sensory factors
Motor factors
Correlation between feedback
and actions
Identification with the
robot
Familiarity with
the system
Kim and Biocca, 1997
[71]
Arrival
Departure
Draper et al., 1998
[44]
Attention to mediated
environment
Attention to ignoring
distractors
Witmer and Singer,
1998 [157]
Control
Sensory
Distraction
Realism
Baños et al., 2000 [8]
Reality judgment
Presence
Emotional involvement
Interaction
Control
Attention/Flow
Realism
Congruence/Continuity
Expectations
IJsselsteijn et al.,
2000 [68]
Extent and fidelity of
sensory information
Match between sensors
and display
Content factors
User characteristics
Lombard et al., 2000
[81]
Social Richness
Realism (Social)
Realism (Perceptual)
Transportation
Immersion
Social Actor in a Medium
Medium as Social Actor
Sas and O’Hare, 2003
[105]
General cognitive factors
Task-specific cognitive
factors
Technological factors
Media content
Takatalo et al. 2008
[142]
Spatial
Action
Attention
Real[ness]
Arousal
Vorderer et al., 2004
[149]
Attention allocation
Spatial situation model
Spatial presence: self-location
Spatial presence: possible
actions
Higher cognitive
involvement
Suspension of disbelief
Domain-specific interest
Visual/Spatial imagery
Absorption
Chertoff et al., 2010
[36]
Affective
Cognitive
Sensory
Active
Relational
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 19 -->

A Survey of Presence and Related Concepts
96:19
Fig. 1. Groupings of presence model components.
between kinesthetic feedback and sensed actions from the remote environment, identification
with the robot (visual similarity), familiarity with the system, and “the cognitive representation
of the operator’s interaction with the world” as factors that are likely to contribute to greater
telepresence.
Arrival and departure were identified as the two factors in the presence questionnaire created
by Kim and Biocca [71]. Arrival is the feeling of being there in a mediated environment, departure
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 20 -->

96:20
R. Skarbez et al.
is the feeling of not being in the real environment, and presence arises from the combination of
the two.
Draper and his colleagues reviewed existing conceptions of telepresence, and put forward an
attentional resource model for telepresence in Reference [44]. This model argues that telepresence increases as a function of the sum of attentional resources devoted to processing task-related
stimuli from the mediated environment and the attentional resources devoted to overcoming
distractors.
In the development of their presence questionnaire, Witmer and Singer proposed four major
categories of factors that affect presence: Control, Sensory, Distraction, and Realism [157]. They
also claimed that factors may influence presence by acting on psychological immersion, involvement, or both. For example, Witmer and Singer theorize that control factors impact psychological
immersion but not involvement, while realism factors impact involvement but not psychological
immersion. Distraction and sensory factors are theorized to affect both. Control factors include
predictability, interactivity of the environment, and input controls; sensory factors include richness of the environment, number and fidelity of sensory modalities, and consistency of multimodal
stimuli; distraction factors include isolation from the physical environment and interface awareness; and realism factors concern the degree to which the experience is meaningful and coherent
with expectations from the real world. Each question on the PQ is intended to address some aspect of one of these factors. The results of a cluster analysis of four studies using the Witmer
and Singer PQ identified three subscales in the PQ data—Involvement/Control, Naturalness, and
Interface Quality.
Bystrom et al. proposed the immersion, presence, performance (IPP) model for interaction in
virtual environments. The authors adopt Slater’s definition of immersion, and presence is used in
the common sense of “being there.” The IPP model, in brief, claims that sensory fidelity (resulting
from a sufficiently immersive system) causes a user to allocate attentional resources to the VE,
and that this allocation of attentional resources enables the user to experience presence in the VE
and perform the given task. Furthermore, it claims that there is a feedback loop: more attention
causes more presence and more task engagement, and increased task engagement causes the user
to allocate more attentional resources [33]. This is supported by a recent study from Skarbez et al.
[117].
Bystrom et al. state that this model is based on the two models of presence proposed by Slater
and colleagues [124, 134] and by Barfield and colleagues [63, 64]. The Slater model as outlined
here described presence as, “determined not only by...aspects of displays...but also mediated by the
sorts of sensory information required to perform the task at hand...and individual differences in
preferences for information.” The Barfield model described presence as “dependent on the degree
to which...transformations of objects in a virtual environment are similar to...transformations of
objects in the real world.”
Schubert et al. presented the results of a factor analysis on an experiment in which 246 participants answered a 75-item survey of new questions and questions taken from Carlin et al. [35], Ellis
et al. [45], Slater et al., [133], Towell and Towell [146], Witmer and Singer [157], and Regenbrecht
et al. [98]. The authors extracted eight factors that combined express 50.27% of the total variance.
These factors, in decreasing order of importance, were spatial presence, quality of immersion, involvement, drama, interface awareness, exploration of the VE, predictability and interaction, and
realness. The authors then performed a second order factor analysis to see how the factors grouped
together. In a two-factor solution, the first factor grouped spatial presence, quality of immersion,
involvement, drama, and realness, and the second factor grouped interface awareness, exploration,
and predictability and interaction. In a three-factor solution, the first factor grouped spatial presence, involvement, and realness, the second factor grouped interface awareness, predictability and
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 21 -->

A Survey of Presence and Related Concepts
96:21
interaction, and exploration, and the third factor grouped drama and quality of immersion [109,
110].
IJsselsteijn et al. reviewed the existing presence literature to summarize research into the factors
contributing to presence and the methods for measuring it. The authors identified four determinants of presence: (1) the extent and fidelity of sensory information, (2) the match between sensors
and display, (3) content factors (a broad category covering most anything else that is part of the
virtual scenario), and (4) user characteristics [68].
Lombard et al. discussed their efforts to develop an instrument for presence based on their theoretical model of its components. In the literature, they identified six “dimensions” of presence:
presence as social richness, presence as realism (both social and perceptual), presence as transportation, presence as immersion, presence as a social actor within a medium, and presence where
the medium is a social actor. The authors claim that the common element among these types of
presence is a perceptual illusion of nonmediation [81].
Sas and O’Hare presented a “presence equation,” where 45% of presence variation can be predicted as
0.37 ×Willinдness to Suspend Disbelie f + 0.29 × Creative Imaдination/Absorption.
(1)
They later presented a more general form of the presence equation,
Presence = a × (General coдnitive f actors) + b × (Task −specif ic coдnitive f actors)
+ c × (Technoloдical f actors) + d × (Media content).
(2)
Note that general cognitive factors is the only term that is entirely dependent on the participant,
whereas technological factors and media content are entirely dependent on the specific VE, and
Task-specific cognitive factors is at least partially dependent on the specific VE. Furthermore, Sas
and O’Hare’s own discussion regarding immersive vs. non-immersive VEs seems to indicate that
they believe c > a,b. They argued for the use of a non-immersive VE for this experiment, because
then any presence differences would be due to human factors rather than immersion [105].
Witmer and colleagues revisited their presence questionnaire with a factor analysis. They identified four factors of their presence questionnaire, which combined account for 52.2% of the variance.
These factors are Involvement (accounting for 31.9% of variance), Sensory Fidelity, Adaptation/
Immersion, and Interface Quality [156].
Wirth and colleagues presented a theoretical model of how spatial presence might be generated
in a participant. They proposed a two-stage model. In the first stage, one constructs a spatial situation model (SSM), that is, a mental model of the spatial environment that one constructs based
on (1) spatial cues that one processes and (2) relevant personal spatial memories and cognitions.
In the second stage, one defines his or her primary egocentric reference frame (PERF), which is
either the SSM representing the mediated environment, in which case one is present in the virtual
environment, or the SSM representing the real world, in which case one is not present in the VE.
Specifically, the authors claim that “spatial presence occurs when the medium-as-PERF hypothesis
is confirmed repeatedly through processed information and is thus stabilized over time” [154]. It
seems to us that the SSM formalizes Held and Durlach’s “cognitive representation of the operator’s
interaction with the world” [61].
For Wirth et al., then, an individual’s sense of presence in any mediated environment is dependent on both characteristics of the environment—for example, richness, salience, consistency—and
of the individual user—for example, attention, involvement, suspension of disbelief.
Chertoff and colleagues presented a questionnaire developed to measure “holistic virtual environment experiences.” The development of this questionnaire was guided by the five dimensions
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 22 -->

96:22
R. Skarbez et al.
of experiential design: affective (emotion), cognitive (engagement), sensory (immersion), active
(“personal connection...to an experience”), and relational (social) [36].
Kent Bye proposed a theory of presence with a metaphor inspired by the four elements of natural philosophy: earth (embodied presence), fire (active presence), air (social and mental presence),
and water (emotional presence) [32]. The similarity of these elements to the dimensions of experiential design used by Chertoff et al. is notable, as the two models were developed independently
[36].
4.2
Analysis
Unlike the definitions of presence in Section 3.1, the models of presence are strikingly similar.
Almost all can be transformed into one another, or into, for example, the PI/Psi/Social Presence
Illusion/immersion/coherence framework endorsed in this review. Akin et al.’s conception of telepresence being composed of the ability to act in the remote environment plus the ability to display
sense data in the local environment is very similar to Slater’s conception of immersion being composed of effective and sensorimotor valid actions [2, 121]. (A sensorimotor valid action is any action
a user can take that changes his or her perception of the virtual environment; an effective valid
action is an action a user can take that changes the state of the VE itself.) Those authors do not
consider coherence, but they have no need to, since they are explicitly talking about remote real
environments as opposed to virtual ones. Heeter’s subjective personal presence is precisely Place
Illusion, while social presence is Social Presence Illusion and environmental presence is similar to
Plausibility Illusion [60]. Sheridan’s factors contributing to telepresence are, again, sensorimotor
and effective valid actions, plus the extent of sensor information, which is also an aspect of immersion [113]. Witmer and Singer’s conception of presence as arising from control factors, sensory
factors, distraction factors, and realism factors can be restated as immersion (control and sensory)
plus coherence (distraction and realism) [157].
IJsselsteijn et al., Sas and O’Hare, and Wirth et al. introduce individual differences to the discussion [68, 105, 154]. Specifically, Sas and O’Hare’s presence equation (Equation (2)), consists of
individual differences of both state and trait (general cognitive factors and task-specific cognitive
factors both comprise both states and traits), immersion (technological factors), and coherence (media content). It also consists of the respective coefficients on each of these terms, which might be
better restated as
Presence = A[Vector of coдnitive f actors] + B[Vector of task −specif ic coдnitive f actors]
+ C[Vector of technoloдical f actors] + D[Vector of media content f actors],
(3)
to more accurately represent the difficulty involved in computing a “presence equation.”
Grouping presence components. In Figure 1, we have grouped the presence components discussed
in this section (and presented in Table 2). This grouping demonstrates that most of the components
that have previously been proposed as making up the presence construct can in fact be grouped
as components of PI, Psi, Social Presence Illusion, immersion, or coherence. Several others can
be grouped under the heading of attention or distraction, and another subset can be grouped under individual differences. Taken together, these categories account for the overwhelming majority of components that have been proposed as part of the presence construct. (Note that while
we include Attention/Distraction as a heading in this diagram, since it appears in many of the
models of presence discussed in this section, we do not believe that this is properly a component of the sense of presence. For our reasoning, refer to Section 2.8, under “Involvement and
Engagement.”)
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 23 -->

A Survey of Presence and Related Concepts
96:23
Fig. 2. Proposed relationships between presence concepts.
While immersion and coherence (and therefore PI and Psi) are largely under the control of the
VE developer, attention and individual differences are generally not. Many of these models of
presence, then, take into consideration the impact of individual differences on presence (at least
implicitly).
Our model of presence. In Section 3.2, we proposed a new definition of presence, inspired by
its common usage, as “The perceived realness of a mediated or virtual experience.” In Sections
2.3 and 2.5, we discussed three illusions that are commonly experienced in virtual environments,
those being Place Illusion, Plausibility Illusion, and Social Presence Illusion. In Figure 2, we present
a conceptual model of presence based on these illusions and the environmental characteristics
that give rise to them. Of note is the similarity of our model to that proposed by Heeter [60],
with presence being a function of Place Illusion, Plausibility Illusion, and Social Presence Illusion.
Specifically, we claim that presence arises from the immersion of the system (the sensorimotor and
effective valid actions it supports), the coherence of the scenario, whether the virtual experience
offers company to the user, and the individual characteristics of the user. That is, it arises naturally
in a user who experiences Place Illusion, Plausibility Illusion, or Social Presence Illusion.
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 24 -->

96:24
R. Skarbez et al.
In this section, we have presented many proposed models of presence from the literature and
have argued for these models being reconsidered in the light of the Place Illusion/Plausibility
Illusion/Social Presence Illusion framework. The following section focuses on a special subset of
models of presence, those that have been derived empirically via factor analysis.
5
FACTOR ANALYSES
There have been three significant factor analyses of presence and presence questionnaires in the
literature: Schubert et al., Lessiter et al., and Witmer et al. [78, 109, 110, 156]. Schubert et al. identified eight factors—spatial presence, quality of immersion, involvement, drama, interface awareness, exploration of the VE, predictability and interaction, and realness—that then grouped into
three second-order factors—spatial presence, involvement, and realness. Lessiter et al. identified
four factors—sense of physical space, engagement, naturalness, and negative effects. Witmer et al.
identified four factors as well, which were involvement, sensory fidelity, adaptation/immersion,
and interface quality.
An inherent limitation of factor analyses is that they can only group based on the items
that were actually used in the measure. So if a questionnaire does not include questions about
the coherence of social interactions, for example, there cannot be a factor that addresses that
construct. On the other hand, if a questionnaire does ask questions about a construct that others
do not—as with the ITC-SOPI and negative effects—that construct is likely to be represented by
a factor. The initial selection of items, then, inherently biases the factor analysis that follows.
That said, it is enlightening to look at the similarities and differences among these factor lists.
All three include a factor they call involvement or engagement. (We will use involvement going
forward.) However, a look at the questions that make up these factors reveals that they may actually represent different constructs. For Lessiter et al., this factor is represented by items such as, “I
enjoyed myself,” and “My experience was intense.” Responses to these items seem to measure a
user’s overall affinity for the experience, rather than specifically relating to their feeling of presence. For Witmer et al., the involvement factor contains items including “How much were you
able to control events?”, “How much did the visual aspects of the environment involve you?”, and
“How much did your experiences in the virtual environment seem consistent with your real world
experiences?”, which don’t on face seem to represent any one construct. On the other hand, for
Schubert et al., involvement is represented by items including “I concentrated only on the virtual
space,” and “I was completely captivated by the virtual world,” which seems clearly to represent
an attentional component. This discussion demonstrates that these factors are not as similar as
one would assume from the names.
From Schubert et al., we classify the Spatial Presence factor as a sub-questionnaire asking directly about the feeling of spatial presence (as the Slater-Usoh-Steed questionnaire does [147]),
Involvement as an attentional component, Predictability and Interaction, Realness, and Drama as
coherence factors, and Quality of Immersion, Interface Awareness, and Exploration as immersion
factors.
From Lessiter et al., we classify the Sense of Physical Space factor as a sub-questionnaire asking
directly about the feeling of spatial presence, Engagement as an affinity component, Naturalness
as a coherence factor, and Negative Effects as a (reverse-coded) immersion factor.
From Witmer et al., we classify their Interface Quality and Sensory Fidelity factors as immersion
factors, and Involvement and Adaptation/Immersion as primarily coherence factors.
This concludes our discussion of definitions and models of presence. The following section focuses on operationalizing the sense of presence, and discusses the many questionnaires and other
techniques that have been used to measure the sense of presence in virtual environments.
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 25 -->

A Survey of Presence and Related Concepts
96:25
6
MEASURING PRESENCE
Welch and colleagues identified self-report, behavioral, and physiological measures as potential
means of measuring presence [152]. We employ that categorization here in discussing the variety of presence measures that appear in the literature and add one more category of measure,
psychophysical. The following sections list the various measures that have appeared in the literature; the purposes of providing this list are twofold. First, we seek to provide useful context for
the analysis that appears in Section 6.5. Second, we hope to provide the reader with a toolbox
of presence-measuring techniques. No single measure is perfect, and perhaps one or more of the
measures referenced here may prove useful or inspirational to the reader.
In Section 2.1, we listed several desirable characteristics of presence measures. These include
sensitivity, convenience, nonintrusiveness, reliability, validity, objectivity, contemporaneousness,
continuousness, and generalizability. We will refer to these characteristics as we discuss and evaluate the measures that appear in the following sections.
6.1
Self-report
Self-report refers to all techniques in which users actively report some information about their
experience to the experimenter. An important subset of self-report measures are post-experience
questionnaires, which are discussed separately in the following.
6.1.1
Questionnaires. This section briefly describes several existing questionnaires designed to
measure presence (typically referred to as presence questionnaires), discusses the history of use of
the most popular questionnaires, and concludes with an analysis of questionnaire measures in light
of the desired measure characteristics presented previously. These questionnaires are summarized
in Table 3. (This table inspired by similar ones appearing in References [82] and [83].)
The first commonly used presence questionnaire to appear in the literature was the Slater-UsohSteed (SUS) questionnaire, which first appeared in some form in Reference [129] (later republished
as Reference [130]). In the 1993 version of the SUS questionnaire there were only three questions.
The more common form of the questionnaire has six questions, and can be seen in, for example,
Reference [147].
(Note that the SUS presence questionnaire discussed here and elsewhere in this review is not
related to the System Usability Scale (also SUS) [30]. The usability SUS is a ten-item Likert-scaled
questionnaire used to evaluate the usability of a system, and as such also appears in the VR literature on occasion.)
Kim and Biocca introduced a questionnaire based around the constructs of arrival and departure
[71]. Arrival is the feeling of being there in a mediated environment; departure is the feeling of not
being in the real environment.
Witmer and Singer introduced their Presence Questionnaire (PQ) in Reference [157]. The PQ is
based on the authors’ conception of presence as having four major categories of factors: control,
sensory, distraction, and realism. Each of the 19 questions (reduced from 32) is designed to address
some aspect of one of these four factors.
In the same article, Witmer and Singer introduced their Immersive Tendencies Questionnaire
(ITQ). This questionnaire is intended to measure an individual’s tendency to become involved in
everyday activities, as a proxy for their likelihood to experience presence in a VE. The ITQ contains
18 questions, reduced from 29.
Lombard et al. discussed their efforts to develop an instrument for presence based on their theoretical model of its components in Reference [81]. In the article, they identify six “dimensions”
of presence they found in the literature: presence as social richness, presence as realism (both
social and perceptual), presence as transportation, presence as immersion, presence as a social
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 26 -->

96:26
R. Skarbez et al.
Table 3. List of Presence/Telepresence Questionnaires
Questionnaire
# Items
Subscales
Intended use
Slater-Usoh-Steed (SUS)
questionnaire [147]
6
No separate subscales
Virtual
environments
Arrival/Departure [71]
8
Arrival; Departure
Cross-media
Witmer-Singer Presence
Questionnaire (PQ) [157]
19
Involved/Control; Natural; Interface
Quality
Virtual
environments
Lombard et al.
questionnaire [81]
103
Social richness; Realism;
Transportation; Immersion; Social
actor within a medium; Medium is a
social actor
Cross-media
Reality Judgment and
Presence Questionnaire
(RJPQ) [8]
77
Reality judgment; Presence; Emotional
involvement; Interaction; control;
Attention/Flow; Realism,
Congruence/Continuity; Expectations
Virtual
environments
Swedish Viewer-User
Presence (SVUP)
questionnaire [75]
150
“quality evaluations, attitudes,
presence, and realism, and information
from different modalities as well as
simulation sickness items”
Virtual
environments
ITC-Sense of Presence
Inventory (ITC-SOPI) [78]
44
Sense of physical space; Engagement;
Naturalness; Negative effects
Cross-media
Igroup Presence
Questionnaire (IPQ) [109]
14
Presence; Spatial presence;
Involvement; Realness
Virtual
environments
Sas and O’Hare
questionnaire [105]
34
Being there; Not being here; Reflective
consciousness
Virtual
environments
MEC-Spatial Presence
Questionnaire
(MEC-SPQ) [149]
L: 72; M:
54; S: 36
Attention allocation; Spatial situation
model; Self-location; Possible actions;
Cognitive involvement; Suspension of
disbelief; Domain-specific interest;
Visual/spatial imagery; absorption
Cross-media
Bouchard et al.
questionnaire [24]
1
No separate subscales
Virtual
environments
Experimental Virtual
Environment-Experience
Questionnaire (EVEQ)
[141]
124
Physical presence; Situational
involvement; Competence
Virtual
environments
Temple Presence
Inventory (TPI) [82]
42
Transportation; Immersion; Realism;
Social actor within a medium; Social
richness
Cross-media
Virtual Experience Test
(VET) [36]
17
Affective; Cognitive; Sensory; Active;
Relational
Cross-media
actor within a medium, and presence where the medium is a social actor. The authors claim that
the common element among these types of presence is a perceptual illusion of nonmediation. To
measure these different conceptions of presence, the authors present a 103-item questionnaire.
Baños and her colleagues argued that presence and reality judgment (the belief that our experiences are real, or, the authors say, willing suspension of disbelief) are separate constructs and
should be treated as such [8]. They presented an initial 77-item questionnaire, the Reality Judgment
and Presence Questionnaire (RJPQ), intended to measure both constructs. Baños et al. chose questions to address nine factors of experience: reality judgment, presence, emotional involvement,
interaction, control, attention/flow, realism, congruence/continuity, and expectations.
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 27 -->

A Survey of Presence and Related Concepts
96:27
Larsson, Västfjäll, and Kleiner used a subset of the Swedish Viewer-User Presence Questionnaire
(SVUP) to measure presence in [75]. In this experiment, they used 18 items covering interaction,
presence, awareness of external factors, sound quality, enjoyment, and simulation sickness. The
full questionnaire is unpublished, but is said to comprise, “150 items covering quality evaluations,
attitudes, presence, and realism, and information from different modalities as well as simulation
sickness items.”
Lessiter and colleagues introduced the ITC Sense of Presence Inventory (ITC-SOPI) in [78]. The
intent of this 44-item questionnaire is to focus entirely on the user’s experience with the media, and
so there are no questions that address specific properties of either the system (e.g., input devices),
or the content (e.g., story elements). It is intended to be usable with a variety of media types,
including non-immersive and non-interactive media, such as television programs or movies.
Schubert, Friedmann, and Regenbrecht introduced the igroup Presence Questionnaire (IPQ) in
Reference [109]. The authors follow Zahorik and Jenison in connecting presence to supported
action in the VE [158]. This 14-item questionnaire is intended for use in all forms of virtual environments, including immersive VR systems, desktop VR, 3D games, and text-based VEs such as
MUDs (multi-user dungeons).
Sas and O’Hare developed a novel 34-item questionnaire for their experiment in Reference [105].
They validated this questionnaire by demonstrating that it was highly significantly correlated with
the SUS questionnaire.
Vorderer et al. presented the MEC Spatial Presence Questionnaire (MEC-SPQ) in Reference
[149]. This questionnaire assumes that spatial presence is built of nine constructs: four process factors (attention allocation, spatial situation model, spatial presence—self location, spatial presence—
possible actions), two psychological state factors (higher cognitive involvement, suspension of disbelief), and three psychological trait factors (domain-specific interest, visual/spatial imagery, and
absorption). The authors offer short, medium, and long versions of the MEC-SPQ, comprised of
four, six, or eight questions, respectively, for each construct (36, 54, or 72 questions in total).
Bouchard et al. argued for the reliability and validity of a single item measure for presence in
Reference [24]. The authors used the single question “To [what] [extent] do you feel present in
the virtual environment, as if you were really there?” as a measure of presence, and subjected it
to a content and face validity study, two test-retest reliability studies, a convergent and divergent
validity study, and two sensitivity studies. Results show that the question is well-understood, reliable between tests for the same users, correlates better with the Witmer-Singer PQ than either the
Perceived Realism Scale or the Witmer-Singer ITQ, and is sensitive between high and low levels
of presence.
Takatalo and colleagues developed the Experimental Virtual Environment-Experience Questionnaire (EVEQ) [141]. The EVEQ consists of 124 questions drawn from other questionnaires and
translated into Finnish. These were reduced into 19 subscales, five of which comprised the physical
presence scale. These subscores were spatial, action, attention, real[ness], and arousal [142].
Lombard, Ditton, and Weinstein continued their efforts to develop a “conceptually comprehensive” (based on their literature-based model of presence put forward in Reference [81]) measure of
presence with the Temple Presence Inventory (TPI) [82]. The TPI consists of 42 questions (reduced
from 137) relating to five of their six dimensions of presence (excluding medium as social actor).
Chertoff and colleagues presented a survey developed to measure “holistic virtual environment
experiences” in Reference [36]. By holistic, the authors seem to mean that the environment incorporates aspects of experiential design; specifically that it includes affective (emotion) and cognitive
(engagement) aspects. The survey includes 17 questions addressing five dimensions of experiential
design: affective, cognitive, sensory (immersion), active (“personal connection...to an experience”),
and relational (social).
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 28 -->

96:28
R. Skarbez et al.
Published use of questionnaires Rosakranse and Oh identified five canonical presence
questionnaires—the Slater-Usoh-Steed (SUS) questionnaire, the Witmer-Singer Presence Questionnaire (PQ), the igroup Presence Questionnaire (IPQ), the ITC-Sense of Presence Inventory (ITCSOPI), and the Lombard and Ditton questionnaire—and tracked their histories of use in three academic publishing outlets—Presence: Teleoperators and Virtual Environments, the ISPR conference
proceedings, and Cyberpsychology, Behavior, and Social Networking [103]. It is notable that these
three outlets represent different research communities. Presence tends to focus on research in immersive virtual environments, while the ISPR conference primarily focuses on media scholarship,
and Cyberpsychology is an outlet primarily for psychology researchers.
Rosakranse and Oh found that in Presence, the PQ and SUS questionnaires have remained dominant, while in ISPR, the ITC-SOPI questionnaire is now most commonly used, and in Cyberpsychology, SUS, PQ, IPQ and ITC-SOPI are all used approximately equally often. Note that all of
these questionnaires came into use before 2002 and are still in use in 2014 (when the article was
published). Of particular note, the authors do not consider the usage of the TPI or the MEC-SPQ.
Cummings and Bailenson performed a meta-analysis of published studies that explored the effect of different levels of immersion on presence as measured by questionnaires [39]. Eighty-three
studies were included in this meta-analysis, using many of the questionnaires discussed in this
section. The purpose of the study was to examine the correlation between immersion and presence; the authors found a medium-sized effect of immersion on presence overall, with components
of immersion varying in their effect sizes.
Analysis of questionnaires. Questionnaires are the most widely used means of measuring presence by a considerable margin. This is primarily due to their convenience and generalizability; it
is very easy to ask users to complete a questionnaire (or many questionnaires) after an experience,
and the questionnaires generally do not require substantial (or any) modification to be used with
any type of experience. In addition, many questionnaires have been demonstrated to be valid, sensitive, and reliable. That said, questionnaires are intrusive, are not continuous, are generally not
contemporaneous (questionnaires are most commonly conducted post-experience, but Bouchard’s
single-item measure is intended to be administered during an experience as well), are subjective,
and rely on users’ interpretations of potentially difficult concepts to generate meaningful results.
(For a discussion regarding this last point, consult [119].)
6.1.2
Other Self-report Measures. Welch et al. reported the results of two studies where participants experienced a simulated driving scene [152]. In these studies, presence was measured by
means of paired comparisons—after every pair of exposures, the participant marked on a scale of
1 to 100 how different their senses of presence were between the most recent exposure and the
previous one.
Snow and Williges used the technique of free-modulus magnitude estimation to measure presence in VEs [136]. In free-modulus magnitude estimation, a participant is presented with a series of
stimuli and asked to assign a numeric value representing their level of the desired quantity—in this
case, presence—to each stimulus. There is no predetermined scale. The participant is instructed to
assign any positive number to the first stimulus, and then score all successive stimuli relative to
that first number.
Freeman et al. presented a novel form of direct subjective presence evaluation and the results of
three experimental studies using it [48]. They gave users a handheld slider that was continuously
sampled during each trial. The experimenters instructed users to move the slider depending on
how present they felt. However, rather than analyze these slider values as a continuous measure
of presence, the mean of the slider value was computed for each trial for each participant, and
these means were the values used in their analyses.
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 29 -->

A Survey of Presence and Related Concepts
96:29
Techniques based on measuring breaks in presence, as introduced by Slater and Steed, are important variations on the self-report theme. In these methods, rather than reporting their level of
felt presence, users report the moments when they do not feel present, and this series of events can
be analyzed to generate a measure of presence. In the original article [128], the breaks in presence
were used to generate a Markov chain that continuously modeled the probability that a user felt
present at any given time. Subsequent research evaluated raw counts of breaks in presence, rather
than the more complex Markov chain analysis, and demonstrated that the overall count of breaks
in presence is significantly negatively correlated with presence as measured by questionnaire [29].
Breaks in presence have also been investigated in combination with physiological measures
[122, 123], as well as with other types of self-report measures. Garau et al. induced breaks in presence in a virtual environment, then followed up with semi-structured interviews, the transcripts
of which were subjected to content analysis (in which researchers define categories of interest
before the experiment and then measure them quantitatively by looking for key words or phrases
in the transcript) and thematic analysis (which looks for ideas that are not connected to the initial
research questions). Participants also were asked to draw graphs corresponding to their sense of
“being there,” with time on the X-axis and the environment (lab or bar) on the Y-axis [52].
Kuschel and colleagues proposed a new measure of presence based on perception of conflicting
information across multiple sensory modalities (in their specific case, visual and haptic). In this
measure, the user is presented with two or more streams of conflicting sensory data in different
modalities, and is considered present in whichever one he or she reports as dominant [73].
Riener and Proffitt proposed a means of quantifying spatial presence by comparing the results of
visual illusions (specifically the vertical-horizontal illusion and the Ponzo illusion) in photographs,
the real world, and in virtual environments. Here the measure is the users’ estimated lengths of the
lines in each illusion. They found that the size misestimations in virtual environments were closer
to those in the real world for the vertical-horizontal illusion, while they were closer to photographs
with strong perspective cues for the Ponzo illusion [100].
Analysis of other self-report measures. These other self-report measures generally share both their
strengths and weaknesses with questionnaire measures, discussed in the previous section. Notable
exceptions are measures based on breaks in presence; these are contemporaneous measures, and
it can be argued that they are minimally intrusive; since users are only asked to report when their
presence breaks, the reporting does not cause additional breaks in presence. Sensory-conflict-based
measures (such as proposed in Reference [73]) also have the benefit of being contemporaneous.
The presence slider used in Reference [48] is potentially both continuous and contemporaneous
but was not analyzed in that way by the authors.
6.2
Behavioral Measures
Sheridan proposed that in addition to self-report methods, presence could be measured by behavioral methods such as response to threatening stimuli (for example, flinching out of the way of a
virtual ball) or to socially conditioned behaviors (for example, saying, “Gesundheit,” in response
to a sneeze in the VE) [113].
Slater, Usoh, and Chrysanthou used pointing to an ambiguous object as a measure of presence.
Participants saw a radio in one location in the real world, and in a different location in the virtual
world, and were told at various times during the experiment to point to “the radio.” It was assumed that participants who pointed to the virtual radio were experiencing greater presence than
participants who pointed to the location of the real radio. This was operationalized as a ratio of
the differences between the actual pointing angle and the directions to the real and virtual angles.
The authors observed a positive correlation between the number of shadows and this ratio [132].
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 30 -->

96:30
R. Skarbez et al.
Thie and van Wijk used “comeback rate” as a means to behaviorally evaluate presence. Participants were told before the experiment to bring something to read, then after the experiment
were given the option of reading or re-entering the virtual environment after the experiment had
“officially” ended. They found that users “came back” more often when the experience contained
more social presence cues [145].
Regenbrecht, Schubert, and Friedmann demonstrated that fear increased with higher presence in
a virtual environment designed to elicit fear of heights [98]. Presence was measured using Likertstyle responses to 14 questions that included questions from References [62, 133]; anxiety was
measured using the State-Trait Anxiety Index, a 20-item questionnaire [76]. We classify this with
the behavioral measures rather than the self-report measures, because the self-reported quantity
is not presence, as it is in all the other measures classified as self-report.
Freeman et al. proposed the use of a behavioral measure for presence; specifically the magnitude of postural response for seated participants viewing a video [47]. The authors conducted
a 24-participant study to evaluate this metric. Participants viewed two video clips: one was excerpted from a video recorded from the hood of a rally car, and the other was a still frame from a
video taken at the side of the rally track. The soundtrack was the same in both videos, giving the
impression of a car off in the distance in the still video case. All participants saw both stimuli in
both monoscopic and stereoscopic presentations. Participants rated their presence (as well as involvement, self-motion, and sickness) on a scale from 0 to 100 on a visual analogue scale after each
trial, and their postural responses were tracked. Participants’ self-rated presence scores showed
significantly higher presence for stereoscopic presentation and for the moving video stimulus,
with no interaction between the factors. There was no significant relationship between presence
and postural response, however.
Analysis of behavioral measures. Behavioral measures address one of the major shortcomings of
the self-report measures in that they are objective measures (at least on the part of the user; they
may require humans to score the behavior). They are generally contemporaneous, although not
continuous. They are also nonintrusive, in that they attempt to capture users’ “natural” behaviors. (They may require elements to be added to the virtual experience to trigger those behaviors,
though; the examples from [113] previously would only apply in VEs where balls are thrown at
users or other characters sneeze, respectively.)
6.3
Physiological Measures
Dillon et al. put forward a plan to compare skin conductance response (SCR) (also referred to
as galvanic skin response, GSR, or electrodermal activity, EDA) and electrocardiogram (EKG) data
with presence as measured by the ITC-SOPI [78] in a study where participants view a video stream
presented either stereoscopically or monoscopically [43]. The results of that study are summarized
in Reference [42], and the results of another study investigating the effects of emotional media
content and display size on presence and arousal are also presented there. The authors did not find
a correlation between physiological metrics and presence. Note that the stimuli in these studies
were neither immersive nor inherently arousing.
Meehan explored the same measures as well as skin temperature in an immersive virtual environment that did contain an inherently stressful stimulus, a visual cliff scenario [87]. There,
Meehan and colleagues did find that a larger increase in heart rate when exposed to the visual
cliff significantly correlated with an increase in presence as measured by the SUS questionnaire,
indicating that physiological measures such as change in heart rate may be able to serve as an objective proxy measure for presence in such scenarios (that is, in virtual environments that contain
a known arousal-inducing stimulus, such as the visual cliff).
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 31 -->

A Survey of Presence and Related Concepts
96:31
As mentioned in the previous section, when talking about breaks in presence, Slater and colleagues have used physiological metrics (heart rate, heart rate variability, and EEG) to measure
users’ responses to breaks in presence in virtual environments, both experimenter-caused [59,
123] and incidental [122].
More recently, Baumgartner et al. [10] and Bouchard et al. [23, 25, 26] have used fMRI technology to investigate the neural correlates of presence. Both authors have identified regions of the
brain that seem to correlate with the feeling of presence in participants; Baumgartner et al. point
to the dorsolateral prefrontal cortex, while Bouchard et al. identify the parahippocampus as the
brain region most associated with the feeling of presence. Baumgartner et al. speculate that this
difference may be due to the different study methodologies (Baumgartner et al. presented two different VEs for the two groups in their study, while Bouchard et al. presented the same VE to both
groups, but it was explained differently.)
Analysis of physiological measures. Physiological measures address one of the major shortcomings of the self-report measures in that they are truly objective measures. Also, they are both
contemporaneous and continuous. However, they are inconvenient and intrusive, and they are
not generalizable. Rather, they can be collected in a very general way, but are only meaningful
when collected during experiences that are known to affect physiological signals in certain ways.
In addition, the collection of such measures requires the use of additional specialized equipment,
which can encumber the user (and thereby reduce presence).
6.4
Psychophysical Methods
Slater, Spanlang, and Corominas demonstrated a method for evaluating the relative importance of
different aspects of a virtual environment on participants’ feelings of Place Illusion and Plausibility
Illusion [126]. This method involved exposing each participant to a VE that was configured with
the “highest levels” of various immersion and coherence factors, instructing the participant to
remember how much PI or Psi he or she felt in that environment, then exposing the participant to
various diminished versions of the virtual environment, and enabling the participant to improve
the immersion or coherence factors in whatever order he or she saw fit. By so doing, the authors
were able to generate an ordering of the experimental factors ranked by how important each factor
was for generating a sense of PI or Psi in users. Similar methods were employed by Azevedo, Jorge,
and Campos [4, 5], by Bergström et al. [12], and by Skarbez et al. [117].
Analysis of psychophysical methods. The psychophysical methods discussed here are notably unlike all the other measures discussed in this section in that they have not actually been used to
measure presence. As such, the measure properties discussed elsewhere don’t really apply here.
Rather, what these psychophysical methods offer is a new way to measure how presence is impacted by changes to the immersion or coherence of a virtual experience.
6.5
Analysis
The proliferation of questionnaires adds complexity to presence research. Our experience with
using multiple presence questionnaires following a single virtual experience suggests that the
questionnaire scores are very highly correlated. Based on these observations, we believe that it
is only necessary to use one questionnaire, although which to use may change based on the specific circumstances. For example, if one is particularly interested in reality judgment, or one or
more of the subscores of the MEC questionnaire, one should consider using the RJPQ or MECSPQ, respectively. For a direct presence measure, we recommend either the SUS questionnaire or
the Bouchard et al. single-item measure, as these are the shortest questionnaires in use (saving
both experimenter and participant time) and they both directly measure the feeling of presence. In
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 32 -->

96:32
R. Skarbez et al.
particular, Bouchard et al.’s single-item measure is especially useful if a contemporaneous subjective measure of presence is desired.
We believe that behavioral measures represent a promising area of study that has so far been
understudied. Physiological measures may ultimately be limited in their utility as they have been
shown to be useful only in experiments that are known to affect physiological signals in particular
ways (e.g., increasing arousal in a stressful environment), or place severe restrictions on the design
of the VE (as in fMRI studies), but it is likely that appropriate behavioral signals could be found in
nearly any virtual scenario. However, these are not likely to be generalizable across scenarios. Per
Reference [49]: “[C]ontent-dependency makes the development of a general behavioural metric
unlikely.” Thus, the identification of a universal measure of the quality of a virtual environment
remains an open problem.
The psychophysical methods described previously are new and promising techniques for measuring presence or other qualia relating to the experience of virtual environments. If one’s objective
is the study of different factors of virtual experience and their effects on presence or other qualia,
then we believe that one should absolutely consider using such psychophysical methods. However,
the nature of these methods is such that they cannot be used to generate a single value corresponding to a level of presence in the way that self-report, physiological, and behavioral methods do.
Furthermore, since such psychophysical methods require the ability to dynamically reconfigure
the VE, they are ill-suited to the evaluation of production VEs.
All of the measures and methods discussed in this section have their applications, and none of
them possess all the desirable characteristics that have been discussed. Because there is no “silver
bullet,” we recommend instead the use multiple measures of different types whenever feasible. If all
the measures suggest the same interpretation, then the results can be used with greater confidence.
This multiple measure technique, which is common in other fields of qualitative research, is called
triangulation.
7
CONCLUSION
This article has reviewed the existing literature regarding presence and other concepts important
in the study of virtual experiences. We first reviewed several of these other concepts, including social presence, copresence, immersion, agency, transportation, reality judgment, and embodiment.
We also coined the term Social Presence Illusion to mean Biocca et al.’s definition of social presence, as well as several related terms, in an attempt to reduce the confusion in the literature regarding the terms social presence and co-presence. We then discussed many of the definitions for presence that have been proposed, grouped them into categories based on common factors (Table 1),
and ultimately argued for the use of the term Place Illusion rather than the term (spatial) presence,
and the re-definition of the word presence to match its common usage as “the perceived realness of a
mediated or virtual experience.” We presented many of the proposed models of presence (Table 2),
grouped the factors of these models into categories informed by the Place Illusion/Plausibility
Illusion/immersion/coherence framework (Figure 1), and presented a model of presence based on
the feelings of Place Illusion, Plausibility Illusion, and Social Presence Illusion (Figure 2). Finally,
we discussed a variety of measures of presence from the literature, categorized them as self-report,
behavioral, physiological, or psychophysical, and argued for the use of short, direct instruments
(such as the Slater-Usoh-Steed presence questionnaire or Bouchard et al.’s single-item measure)
for measuring presence, the use of other questionnaires if their constructs or subscores are relevant to the research, the use of psychophysical methods to evaluate the importance of immersion
and coherence factors on presence or related qualia, the development and use of appropriate behavioral measures, and the use of multiple measures of different types when feasible. We hope
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 33 -->

A Survey of Presence and Related Concepts
96:33
that the results of the survey and analyses presented here have laid the groundwork for a more
inclusive and less confusing literature regarding the study of virtual experiences.
ACKNOWLEDGMENTS
The authors thank Dr. Benjamin Lok, Dr. Abigail Panter, Dr. Mel Slater, and Dr. Gregory Welch for
their guidance and helpful feedback during the writing of the dissertation from which this work
is derived. We also thank the anonymous reviewers of this article, who provided extensive and
productive feedback. The final article was significantly improved by their contributions.
REFERENCES
[1] AERA/APA/NCME. 2014. Standards for Educational and Psychological Testing. AERA, Washington, DC.
[2] David L. Akin, Marvin L. Minsky, Eric D. Thiel, and Clifford R. Kurtzman. 1983. Space Applications of Automation,
Robotics, and Machine Intelligence Systems (ARAMIS), Phase II, Vol. 3: Executive Summary. Technical Report. Massachusetts Institute of Technology, Cambridge, MA.
[3] Amy L. Alexander, Tad Brunyé, Jason Sidman, and Shawn A. Weil. 2005. From gaming to training: A review of
studies on fidelity, immersion, presence, and buy-in and their effects on transfer in PC-based simulations and games.
In Proceedings of the Interservice/Industry Training, Simulation, and Education Conference (I/ITSEC’05). NTSA.
[4] António Sérgio Azevedo. 2013. 3D Sound Enhanced Presence in Virtual Environments. Master’s thesis. University of
Lisbon.
[5] António Sérgio Azevedo, Joaquim Jorge, and Pedro Campos. 2014. Combining EEG data with place and plausibility
responses as an approach to measuring presence in outdoor virtual environments. Presence: Teleoper. Virtual Environ.
23, 4 (September 2014), 354–368.
[6] Jeremy N. Bailenson, Kim Swinth, Crystal Hoyt, Susan Persky, Alex Dimov, and Jim Blascovich. 2005. The independent and interactive effects of embodied-agent appearance and behavior on self-report, cognitive, and behavioral
markers of copresence in immersive virtual environments. Presence: Teleoper. Virtual Environ. 14, 4 (August 2005),
379–393.
[7] Rosa M. Baños, Cristina Botella, Mariano Alcañiz, Víctor Liaño, Belén Guerrero, and Beatriz Rey. 2004. Immersion
and emotion: Their impact on the sense of presence. CyberPsychol. Behav. 7, 6 (February 2004), 734–741.
[8] Rosa M. Baños, Cristina Botella, A. García-Palacios, H. Villa, C. Perpiña, and Mariano Alcañiz. 2000. Presence and
reality judgment in virtual environments: A unitary construct. CyberPsychol. Behav. 3, 3 (July 2000), 327–335.
[9] Rosa M. Baños, Cristina Botella, A. García-Palacios, H. Villa, C. Perpiña, and M. Gallardo. 1999. Psychological variables and reality judgment in virtual environments: The roles of absorption and dissociation. CyberPsychol. Behav.
2, 2 (April 1999), 143–148.
[10] Thomas Baumgartner, Dominique Speck, Denise Wettstein, Ornella Masnari, Gian Beeli, and Lutz Jäncke. 2008. Feeling present in arousing virtual reality worlds: Prefrontal brain regions differentially orchestrate presence experience
in adults and children. Front. Hum. Neurosci. 2 (2008), 8.
[11] Steve Benford, John Bowers, Lennart E. Fahlén, Chris Greenhalgh, and Dave Snowdon. 1995. User embodiment in
collaborative virtual environments. In Proceedings of the SIGCHI conference on Human Factors in Computing Systems.
ACM Press/Addison-Wesley Publishing Co. 242–249.
[12] Ilias Bergström, Sérgio Azevedo, Panos Papiotis, Nuno Saldanha, and Mel Slater. 2017. The plausibility of a string
quartet performance in virtual reality. IEEE Trans. Visual. Comput. Graph. 23, 4 (April 2017), 1352–1359.
[13] Frank Biocca. 1997. The Cyborg’s dilemma: Progressive embodiment in virtual environments. J. Comput.-Med. Commun. 3, 2 (1997).
[14] Frank Biocca. 2001. Inserting the presence of mind into a philosophy of presence: A response to Sheridan and
Mantovani and Riva. Presence: Teleoper. Virtual Environ. 10, 5 (October 2001), 554–556.
[15] Frank Biocca. 2002. Presence working group research targets. Proceedings ofthe “Presence Info Day” of the European
Commission (January 2002).
[16] Frank Biocca and Ben Delaney. 1995. Immersive virtual reality technology. In Communication in the Age of Virtual
Reality, Frank Biocca and Mark R. Levy (Eds.). Lawrence Erlbaum Associates Inc., Hillsdale, NJ, 57–124.
[17] Frank Biocca, Chad Harms, and Jenn Gregg. 2001. The networked minds measure of social presence: Pilot test of
the factor structure and concurrent validity. In Proceedings of the 4th Annual International Workshop on Presence
(PRESENCE’01). 1–9.
[18] Olaf Blanke and Thomas Metzinger. 2009. Full-body illusions and minimal phenomenal selfhood. Trends Cogn. Sci.
13, 1 (2009), 7–13.
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 34 -->

96:34
R. Skarbez et al.
[19] Jim Blascovich. 2002. A theoretical model of social influence for increasing the utility of collaborative virtual environments. In Proceedings of the 4th International Conference on Collaborative Virtual Environments. ACM, 25–30.
[20] Saskia Böcking, Andre Gysbers, Werner Wirth, Christoph Klimmt, Tilo Hartmann, Holger Schramm, Jari Laarni,
Ana Sacau, and Peter Vorderer. 2004. Theoretical and empirical support for distinctions between components and
conditions of spatial presence. In Proceedings of the 7th Annual International Workshop on Presence (PRESENCE’04).
224–231.
[21] David Bolton. 2016. The presence: Virtual reality is the last true medium (March 2016). Retrieved from https://arc.
applause.com/2016/03/23/presence-virtual-reality/.
[22] M. Botvinick and J. Cohen. 1998. Rubber hands “feel” touch that eyes see. Nature 391, 6669 (1998), 756.
[23] Stéphane Bouchard, Stéphanie Dumoulin, Jeanne Talbot, André-Anne Ledoux, Jennifer Phillips, Johana MonthuyBlanc, Geneviève Labonté-Chartrand, Geneviéve Robillard, Matteo Cantamesse, and Patrice Renaud. 2012. Manipulating subjective realism and its impact on presence: Preliminary results on feasibility and neuroanatomical correlates. Interact. Comput. 24, 4 (2012), 227–236. Special Issue on Presence and Interaction.
[24] Stéphane Bouchard, Geneviéve Robillard, Julie St-Jacques, Stéphanie Dumoulin, M. J. Patry, and Patrice Renaud.
2004. Reliability and validity of a single-item measure of presence in VR. In Proceedings of the 2nd International
Conference on Creating, Connecting and Collaborating through Computing. 59–61.
[25] Stéphane Bouchard, Jeanne Talbot, André-Anne Ledoux, Jennifer Phillips, Matteo Cantamasse, and Geneviève
Robillard. 2009. The meaning of being there is related to a specific activation in the brain located in the parahypocampus. In Proceedings of the 12th Annual International Workshop on Presence (PRESENCE’09).
[26] Stéphane Bouchard, Jeanne Talbot, André-Anne Ledoux, Jennifer Phillips, Matteo Cantamesse, and Geneviéve
Robillard. 2010. Presence is just an illusion: Using fMRI to locate the brain area responsible to the meaning given to
places. Annu. Rev. Cyberther. Telemed.: Adv. Technol. Behav. Soc. Neurosci. 154 (2010), 193–196.
[27] Doug A. Bowman and Ryan P. McMahan. 2007. Virtual reality: How much immersion is enough? Computer 40, 7
(July 2007), 36–43.
[28] Jeanne H. Brockmyer, Christine M. Fox, Kathleen A. Curtiss, Evan McBroom, Kimberly M. Burkhart, and Jacquelyn
N. Pidruzny. 2009. The development of the game engagement questionnaire: A measure of engagement in video
game-playing. J. Exper. Soc. Psychol. 45, 4 (2009), 624–634.
[29] Andrea Brogni, Mel Slater, and Anthony Steed. 2003. More breaks less presence. In Proceedings of the 6th Annual
International Workshop on Presence (PRESENCE’03).
[30] John Brooke. 1996. SUS—A quick and dirty usability scale. Usabil. Eval. Ind. 189, 194 (1996), 4–7.
[31] Peter Bull. 1983. Body Movement and Interpersonal Communication. John Wiley & Sons.
[32] Kent Bye. 2017. #502: An Elemental Theory of Presence + Future of AI & Interactive Storytelling. (February 2017).
Retrieved from http://voicesofvr.com/502-an-elemental-theory-of-presence-future-of-ai-interactive-storytelling/.
[33] Karl-Erik Bystrom, Woodrow Barfield, and Claudia Hendrix. 1999. A conceptual model of the sense of presence in
virtual environments. Presence: Teleoper. Virtual Environ. 8, 2 (April 1999), 241–244.
[34] Antonella Carassa, Francesca Morganti, and Maurizio Tirassa. 2005. A situated cognition perspective on presence.
In Proceedings of the 27th Annual Conference of the Cognitive Science Society. Sheridan Printing, Stresa, Italy, 384–389.
[35] Albert S. Carlin, Hunter G. Hoffman, and Suzanne Weghorst. 1997. Virtual reality and tactile augmentation in the
treatment of spider phobia: A case report. Behav. Res. Ther. 35, 2 (February 1997), 153–158.
[36] Dustin B. Chertoff, Brian Goldiez, and Joseph J. LaViola Jr. 2010. Virtual experience test: A virtual environment
evaluation questionnaire. In IEEE Virt. Real. (VR). 103–110.
[37] Mihaly Csikszentmihalyi. 1990. Flow: The Psychology of Optimal Experience. Harper and Row, New York.
[38] Mihaly Csikszentmihalyi. 1997. Finding Flow: The Psychology of Engagement with Everyday Life. Basic Books, New
York.
[39] James J. Cummings and Jeremy N. Bailenson. 2016. How immersive is enough? A meta-analysis of the effect of
immersive technology on user presence. Media Psychol. 19, 2 (2016), 272–309.
[40] Nicole David, Albert Newen, and Kai Vogeley. 2008. The “sense of agency” and its underlying cognitive and neural
mechanisms. Conscious. Cogn. 17, 2 (2008), 523–534.
[41] Frédérique de Vignemont. 2011. Embodiment, ownership and disownership. Conscious. Cogn. 20, 1 (2011), 82–93.
[42] Cath Dillon, Edmund Keogh, and Jonathan Freeman. 2002. “It’s been emotional”: Affect, physiology, and presence.
In Proceedings of the 5th Annual International Workshop on Presence (PRESENCE’02).
[43] Cath Dillon, Edmund Keogh, Jonathan Freeman, and Jules Davidoff. 2000. Aroused and immersed: The psychophysiology of presence. In Proceedings of the 3rd International Workshop on Presence (PRESENCE’00).
[44] John V. Draper, David B. Kaber, and John M. Usher. 1998. Telepresence. Hum. Fact.: J. Hum. Fact. Ergonom. Soc. 40,
3 (1998), 354–375.
[45] Stephen R. Ellis, Nancy S. Dorighi, Brian M. Menges, Bernard D. Adelstein, and Richard H. Jacoby. 1997. In search
of equivalence classes in subjective scales of reality. In Human-Computer Interaction, Vol. 2. 873–876.
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 35 -->

A Survey of Presence and Related Concepts
96:35
[46] John M. Flach and John G. Holden. 1998. The reality of experience: Gibson’s way. Presence: Teleoper. Virtual Environ.
7, 1 (February 1998), 90–95.
[47] Jonathan Freeman, Steve E. Avons, Ray Meddis, Don E. Pearson, and Wijnand IJsselsteijn. 2000. Using behavioral
realism to estimate presence: A study of the utility of postural responses. Presence: Teleoper. Virtual Environ. 9, 2
(April 2000), 149–164.
[48] Jonathan Freeman, Steve E. Avons, Don E. Pearson, and Wijnand A. IJsselsteijn. 1999. Effects of sensory information
and prior experience on direct subjective ratings of presence. Presence: Teleoper. Virtual Environ. 8, 1 (February 1999),
1–13.
[49] Jonathan Freeman, Jane Lessiter, and Wijnand IJsselsteijn. 2001. An introduction to presence: A sense of being there
in a mediated environment. Psychologist 14 (2001), 190–194.
[50] Joseph L. Gabbard. 1997. A Taxonomy of Usability Characteristics in Virtual Environments. Ph.D. Dissertation. Virginia
Polytechnic Institute and State University.
[51] Shaun Gallagher. 2000. Philosophical conceptions of the self: Implications for cognitive science. Trends Cogn. Sci. 4,
1 (2000), 14–21.
[52] Maia Garau, Doron Friedman, Hila Ritter Widenfeld, Angus Antley, Andrea Brogni, and Mel Slater. 2008. Temporal
and spatial variations in presence: Qualitative analysis of interviews from an experiment on breaks in presence.
Presence: Teleoper. Virtual Environ. 17, 3 (June 2008), 293–309.
[53] Richard J. Gerrig. 1993. Experiencing Narrative Worlds. Yale University Press, New Haven, CT.
[54] James J. Gibson. 1979. The Ecological Approach to Visual Perception. Houghton-Mifflin, Boston, MA.
[55] Stephen B. Gilbert. 2017. Perceived realism of virtual environments depends on authenticity. Presence: Teleoper.
Virtual Environ. 25, 4 (Fall 2017), 322–324.
[56] Erving Goffman. 1963. Behavior in Public Places: Notes on the Social Organization of Gatherings. The Free Press, New
York.
[57] Melanie Colette Green. 1996. Mechanisms of Narrative-based Belief Change. Master’s thesis. The Ohio State University.
[58] Melanie C. Green and Timothy C. Brock. 2000. The role of transportation in the persuasiveness of public narratives.
J. Personal. Soc. Psychol. 79, 5 (November 2000), 701–721.
[59] Cristoph Guger, Guenter Edlinger, Robert Leeb, and Gert Pfurtscheller. 2004. Heart-rate variability and event-related
ECG in virtual environments. In Proceedings of the 7th International Conference on Presence (PRESENCE’04). 240–245.
[60] Carrie Heeter. 1992. Being there: The subjective experience of presence. Presence: Teleoper. Virtual Environ. 1, 2 (May
1992), 262–271.
[61] Richard M. Held and Nathaniel I. Durlach. 1992. Telepresence. Presence: Teleoper. Virtual Environ. 1, 1 (January 1992),
109–112.
[62] Claudia Hendrix and Woodrow Barfield. 1995. Presence in virtual environments as a function of visual and auditory cues. In Proceedings of the Virtual Reality Annual International Symposium (VRAIS’95). IEEE Computer Society,
Washington, DC, 74–82.
[63] Claudia Hendrix and Woodrow Barfield. 1996. Presence within virtual environments as a function of visual display
parameters. Presence: Teleoper. Virtual Environ. 5, 3 (Summer 1996), 274–289.
[64] Claudia Hendrix and Woodrow Barfield. 1996. The sense of presence within auditory virtual environments. Presence:
Teleoper. Virtual Environ. 5, 3 (Summer 1996), 290–301.
[65] Gerardo Herrera, Rita Jordan, and Lucí Vera. 2006. Agency and presence: A common dependence on subjectivity?
Presence: Teleoper. Virtual Environ. 15, 5 (October 2006), 539–552.
[66] Donna L. Hoffman and Thomas P. Novak. 2009. Flow online: Lessons learned and future prospects. J. Interact. Market.
23, 1 (2009), 23–34.
[67] Bo Hu, Liang Ma, Wei Zhang, Gavriel Salvendy, Damien Chablat, and Fouad Bennis. 2011. Predicting real-world
ergonomic measurements by simulation in a virtual environment. Int. J. Industr. Ergon. 41, 1 (January 2011), 64–71.
[68] Wijnand A. IJsselsteijn, Huib de Ridder, Jonathan Freeman, and Steve E. Avons. 2000. Presence: Concept, determinants and measurement. In Proceedings of the Society for Optics and Photonics (SPIE’00), Vol. 3959.
[69] International Society for Presence Research. 2000. The concept of presence: Explication statement. Retrieved from
https://ispr.info/about-presence-2/about-presence/.
[70] Konstantina Kilteni, Raphaela Groten, and Mel Slater. 2012. The sense of embodiment in virtual reality. Presence:
Teleoper. Virtual Environ. 21, 4 (September 2012), 373–387.
[71] Taeyong Kim and Frank Biocca. 1997. Telepresence via television: Two dimensions of telepresence may have different connections to memory and persuasion. J. Comput.-Med. Commun. 3, 2 (1997).
[72] Irina Kruglikova, Teodor P. Grantcharov, Asbjorn M. Drewes, and Peter Funch-Jensen. 2010. The impact of constructive feedback on training in gastrointestinal endoscopy using high-fidelity virtual-reality simulation: A randomised
controlled trial. Gut 59, 2 (2010), 181–185.
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 36 -->

96:36
R. Skarbez et al.
[73] Martin Kuschel, Franziska Freyberger, Martin Buss, and Berthold Färber. 2007. A presence measure for virtual reality and telepresence based on multimodal conflicts. In Proceedings of the 10th International Workshop on Presence
(PRESENCE’07).
[74] Christian R. Larsen, Jette L. Soerensen, Teodor P. Grantcharov, Torur Dalsgaard, Lars Schouenborg, Christian
Ottosen, Torben V. Schroeder, and Bent S. Ottesen. 2009. Effect of virtual reality training on laparoscopic surgery:
Randomised controlled trial. BMJ 338 (2009).
[75] Pontus Larsson, Daniel Västfjäll, and Mendel Kleiner. 2001. The actor-observer effect in virtual reality presentations.
CyberPsychol. Behav. 4, 2 (April 2001), 239–246.
[76] Lothar Laux, Peter Glanzmann, Paul Schaffner, and Charles D. Spielberger. 1981. State-Trait-Angstinventar [StateTrait Anxiety Inventory]. Beltz, Weinheim, Germany.
[77] Kwan Min Lee. 2004. Presence, explicated. Commun. Theory 14, 1 (2004), 27–50.
[78] Jane Lessiter, Jonathan Freeman, Edmund Keogh, and Jules Davidoff. 2001. A cross-media presence questionnaire:
The ITC-sense of presence inventory. Presence: Teleoper. Virtual Environ. 10, 3 (June 2001), 282–297.
[79] R. Bowen Loftin and P. Kenney. 1995. Training the hubble space telescope flight team. IEEE Comput. Graph. Appl.
15, 5 (September 1995), 31–37.
[80] Matthew Lombard and Theresa Ditton. 1997. At the heart of it all: The concept of presence. J. Comput.-Med. Commun.
3, 2 (1997).
[81] Matthew Lombard, Theresa B. Ditton, Daliza Crane, Bill Davis, Gisela Gil-Egui, Karl Korvath, and Jessica Rossman.
2000. Measuring presence: A literature-based approach to the development of a standardized paper-and-pencil instrument. In Proceedings of the 3rd International Workshop on Presence (PRESENCE’00).
[82] Matthew Lombard, Theresa B. Ditton, and Lisa Weinstein. 2009. Measuring presence: The temple presence inventory.
In Proceedings of the 12th International Workshop on Presence (PRESENCE’09).
[83] Matthew Lombard, Lisa Weinstein, and Theresa B. Ditton. 2011. Measuring telepresence: The validity of the temple
presence inventory (TPI) in a gaming context. In Proceedings of the 13th International Workshop on Presence (ISPR’11).
[84] Giuseppe Mantovani and Giuseppe Riva. 2001. Building a bridge between different scientific communities: On Sheridan’s eclectic ontology of presence. Presence: Teleoper. Virtual Environ. 10, 5 (October 2001), 537–543.
[85] Ryan P. McMahan, Doug A. Bowman, David J. Zielinski, and Rachael B. Brady. 2012. Evaluating display fidelity and
interaction fidelity in a virtual reality game. IEEE Trans. Visual. Comput. Graph. 18, 4 (2012), 626–633.
[86] Edward F. McQuarrie and J. Michael Munson. 1992. A revised product involvement inventory: Improved usability
and validity. NA—Adv. Consum. Res. 19 (1992), 108–115.
[87] Michael Meehan, Brent Insko, Mary Whitton, and Frederick P. Brooks, Jr. 2002. Physiological measures of presence
in stressful virtual environments. In Proceedings of the 29th Annual Conference on Computer Graphics and Interactive
Techniques (SIGGRAPH’02). ACM, New York, NY, 645–652.
[88] Michael John Meehan. 2001. Physiological Reaction as an Objective Measure of Presence in Virtual Environments. Ph.D.
Dissertation. The University of North Carolina at Chapel Hill.
[89] Marvin Minsky. 1980. Telepresence. Omni (1980), 45–51.
[90] David Modjeska and John A. Waterworth. 2000. Effects of desktop 3D world design on user navigation and search
performance. In Proceedings of the IEEE International Conference on Information Visualization (IV’00). 215–220.
[91] Lothar Muhlbach, Martin Bocker, and Angela Prussog. 1995. Telepresence in videocommunications: A study on
stereoscopy and individual eye contact. Hum. Fact.: J. Hum. Fact. Ergonom. Soc. 37, 2 (1995), 290–305.
[92] Dinah K. C. Murray. 1997. Autism and information technology: Therapy with computers. In Autism and Learning:
A Guide to Good Practice, S. Powelland R. Jordan (Eds.). David Fulton, London, UK.
[93] Thomas P. Novak, Donna L. Hoffman, and Yiu-Fai Yung. 2000. Measuring the customer experience in online environments: A structural modeling approach. Market. Sc. 19, 1 (2000), 22–42.
[94] Kristine L. Nowak and Frank Biocca. 2003. The effect of the agency and anthropomorphism on users’ sense of telepresence, copresence, and social presence in virtual environments. Presence: Teleoper. Virtual Environ. 12, 5 (October
2003), 481–494.
[95] Max Parola, Samuel Johnson, and Ruth West. 2016. Turning presence inside-out: MetaNarratives. Electron. Imag.
2016, 4 (February 2016), 1–9.
[96] Charles Pontonnier, Afshin Samani, Marwan Badawi, Pascal Madeleine, and Georges Dumont. 2014. Assessing the
ability of a VR-based assembly task simulation to evaluate physical risk factors. IEEE Trans. Visual. Comput. Graph.
20, 5 (May 2014), 664–674.
[97] Joseph Psotka, Sharon Davison, and Sonya A. Lewis. 1993. Exploring immersion in virtual space. VR Syst. 1, 2 (Fall
1993), 70–82.
[98] Holger T. Regenbrecht, Thomas W. Schubert, and Frank Friedmann. 1998. Measuring the sense of presence and its
relations to fear of heights in virtual environments. Int. J. Hum.-Comput. Interact. 10, 3 (1998), 233–249.
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 37 -->

A Survey of Presence and Related Concepts
96:37
[99] Gary E. Riccio. 1995. Coordination of postural control and vehicular control: Implications for multimodal perception
and simulation of self-motion. Local Appl. Ecol. Approach Hum. Mach. Syst. 2 (1995), 122–181.
[100] Cedar Riener and Dennis Proffitt. 2002. Quantifying spatial presence. In Proceedings of the 5th Annual International
Conference on Presence (PRESENCE’02).
[101] Giuseppe Riva, M. Teresa Anguera, Brenda K. Wiederhold, and Fabrizia Mantovani (Eds.). 2006. From Communication to Presence. In Emerging Communication: Studies in New Technologies and Practices in Communication, Vol. 9.
IOS Press, Amsterdam.
[102] Giuseppe Riva, John A. Waterworth, Eva L. Waterworth, and Fabrizia Mantovani. 2011. From intention to action: The
role of presence. New Ideas Psychol. 29, 1 (2011), 24–37. Retrieved from DOI:https://doi.org/10.1016/j.newideapsych.
2009.11.002.
[103] Christine Rosakranse and Soo Youn Oh. 2014. Measuring presence: The use trends of five canonical presence quesionnaires from 1998-2012. In Proceedings of the 15th International Workshop on Presence (ISPR’14).
[104] James Russell. 1996. Agency: Its Role in Mental Development. Psychology Press, East Sussex, UK.
[105] Corina Sas and Gregory M. P. O’Hare. 2003. Presence equation: An investigation into cognitive factors underlying
presence. Presence: Teleoper. Virtual Environ. 12, 5 (October 2003), 523–537.
[106] David W. Schloerb. 1995. A quantitative measure of telepresence. Presence: Teleoper. Virtual Environ. 4, 1 (Winter
1995), 64–80.
[107] Ralph Schroeder. 2002. Copresence and interaction in virtual environments: An overview of the range of issues. In
Proceedings of the 5th Annual International Workshop on Presence (PRESENCE’02). 274–295.
[108] Ralph Schroeder. 2002. Social interaction in virtual environments: Key issues, common themes, and a framework
for research. In The Social Life of Avatars. Springer, 1–18.
[109] Thomas Schubert, Frank Friedmann, and Holger Regenbrecht. 2001. The experience of presence: Factor analytic
insights. Presence: Teleoper. Virtual Environ. 10, 3 (June 2001), 266–281.
[110] Thomas Schubert and Holger Regenbrecht. 1999. Decomposing the sense of presence: Factor analytic insights. In
Proceedings of the 2nd Annual International Workshop on Presence (PRESENCE’99).
[111] Thomas W. Schubert. 2009. A new conception of spatial presence: Once again, with feeling. Commun. Theory 19, 2
(2009), 161–187.
[112] Anil K. Seth, Keisuke Suzuki, and Hugo D. Critchley. 2012. An interoceptive predictive coding model of conscious
presence. Front. Psychol. 2, 395 (2012).
[113] Thomas B. Sheridan. 1992. Musings on telepresence and virtual presence. Presence: Teleoper. Virtual Environ. 1, 1
(Winter 1992), 120–126.
[114] John Short, Ederyn Williams, and Bruce Christie. 1976. The Social Psychology of Telecommunications. John Wiley &
Sons, Ltd., Hoboken, NJ.
[115] Anu Sivunen and Emma Nordbäck. 2015. Social presence as a multi-dimensional group construct in 3D virtual
environments. J. Comput.-Med. Commun. 20, 1 (2015), 19–36.
[116] Richard Skarbez. 2016. Plausibility Illusion in Virtual Environments. Ph.D. Dissertation. The University of North
Carolina at Chapel Hill.
[117] Richard Skarbez, Solène Neyret, Frederick P. Brooks Jr., Mel Slater, and Mary C. Whitton. 2017. A psychophysical
experiment regarding components of the plausibility illusion. IEEE Trans. Visual. Comput. Graph. 23, 4 (April 2017),
1369–1378.
[118] Mel Slater. 1999. Measuring presence: A response to the Witmer and singer presence questionnaire. Presence:
Teleoper. Virtual Environ. 8, 5 (October 1999), 560–565.
[119] Mel Slater. 2004. How colorful was your day? Why questionnaires cannot assess presence in virtual environments.
Presence: Teleoper. Virtual Environ. 13, 4 (August 2004), 484–493.
[120] Mel Slater. 2004. A note on presence terminology. In Presence Connect, Vol. 3. 1–5.
[121] Mel Slater. 2009. Place illusion and plausibility can lead to realistic behavior in immersive virtual environments.
Philosoph. Trans. Roy. Soc. London. Ser. B, Biol. Sci. 364 (2009), 3549–3557.
[122] Mel Slater, Andrea Brogni, and Anthony Steed. 2003. Physiological responses to breaks in presence: A pilot study.
In Proceedings of the 6th Annual International Workshop on Presence (PRESENCE’03).
[123] Mel Slater, Christoph Guger, Guenter Edlinger, Robert Leeb, Gert Pfurtscheller, Angus Antley, Maia Garau, Andrea
Brogni, and Doron Friedman. 2006. Analysis of physiological responses to a social situation in an immersive virtual
environment. Presence: Teleoper. Virtual Environ. 15, 5 (October 2006), 553–569.
[124] Mel Slater, Vasilis Linakis, Martin Usoh, Rob Kooper, and G. Street. 1996. Immersion, presence, and performance
in virtual environments: An experiment with tri-dimensional chess. In Proceedings of ACM Virtual Reality Software
and Technology (VRST’96). 163–172.
[125] Mel Slater, Amela Sadagic, Martin Usoh, and Ralph Schroeder. 2000. Small group behavior in a virtual and real
environment: A comparative study. Presence: Teleoper. Virtual Environ. 9, 1 (February 2000), 37–51.
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 38 -->

96:38
R. Skarbez et al.
[126] Mel Slater, Bernhard Spanlang, and David Corominas. 2010. Simulating virtual environments within virtual environments as the basis for a psychophysics of presence. ACM Trans. Graph. 29, 4 (July 2010), 92:1–92:9.
[127] Mel Slater, Bernhard Spanlang, Maria V. Sanchez-Vives, and Olaf Blanke. 2010. First person experience of body
transfer in virtual reality. PLOS ONE 5, 5 (May 2010), 1–9.
[128] Mel Slater and Anthony Steed. 2000. A virtual presence counter. Presence: Teleoper. Virtual Environ. 9, 5 (October
2000), 413–434.
[129] Mel Slater, Anthony Steed, and Martin Usoh. 1993. The virtual treadmill: A naturalistic metaphor for navigation in
immersive virtual environments. In Proceedings of the 1st Eurographics Workshop on Virtual Environments, Martin
Goebel (Ed.). 71–83.
[130] Mel Slater, Anthony Steed, and Martin Usoh. 1995. The virtual treadmill: A naturalistic metaphor for navigation
in immersive virtual environments. In Proceedings of the Eurographics Workshops on Virtual Environments (VE’95).
Springer-Verlag, London, UK, 135–148.
[131] Mel Slater and Martin Usoh. 1993. Representations systems, perceptual position, and presence in virtual environments. Presence: Teleoper. Virtual Environ. 2, 3 (Summer 1993), 221–233.
[132] Mel Slater, Martin Usoh, and Yiorgos Chrysanthou. 1995. The influence of dynamic shadows on presence in immersive virtual environments. In Proceedings of the Workshops on Virtual Environments (VE’95). Springer, 8–21.
[133] Mel Slater, Martin Usoh, and Anthony Steed. 1994. Depth of presence in virtual environments. Presence: Teleoper.
Virtual Environ. 3, 2 (Spring 1994), 130–144.
[134] Mel Slater and Sylvia Wilbur. 1997. A framework for immersive virtual environments (FIVE): Speculations on the
role of presence in virtual environments. Presence: Teleoper. Virtual Environ. 6, 6 (December 1997), 603–616.
[135] Michael Potter Snow. 1998. Charting Presence in Virtual Environments and Its Effects on Performance. Ph.D. Dissertation. Virginia Polytechnic Institute and State University, Blacksburg, VA.
[136] Michael P. Snow and Robert C. Williges. 1998. Empirical models based on free-modulus magnitude estimation of
perceived presence in virtual environments. Hum. Fact. 40, 3 (September 1998), 386–402.
[137] Anna Spagnolli and Luciano Gamberini. 2002. Immersion/emersion: Presence in hybrid environments. In Proceedings
of the 5th Annual International Workshop on Presence (PRESENCE’02). 421–434.
[138] Anna Spagnolli and Luciano Gamberini. 2004. The sense of being “there”: A model for the space of presence. In
Proceedings of the 7th Annual International Workshop on Presence (PRESENCE’04). 48–53.
[139] Jonathan Steuer. 1992. Defining virtual reality: Dimensions determining telepresence. J. Commun. 42, 4 (1992), 73–
93.
[140] Thomas A. Stoffregen, Benoit G. Bardy, L. J. Smart, and R. J. Pagulayan. 2003. On the nature and evaluation of fidelity
in virtual environments. In Virtual and Adaptive Environments: Applications, Implications, and Human Performance
Issues, Lawrence J. Hettingerand Michael W. Haas (Eds.). Lawrence Erlbaum Associates, Inc., Mahwah, NJ, 111–128.
[141] Jari Takatalo. 2002. Presence and Flow in Virtual Environments: An Explorative Study. Master’s thesis. University of
Helsinki.
[142] Jari Takatalo, Göte Nyman, and Leif Laaksonen. 2008. Components of human experience in virtual environments.
Comput. Hum. Behav. 24, 1 (2008), 1–15.
[143] David L. Tate, Linda Sibert, and Tony King. 1997. Virtual environments for shipboard firefighting training. In Proceedings of IEEE 1997 Annual International Symposium on Virtual Reality. 61–68, 215.
[144] Auke Tellegen and Gilbert Atkinson. 1974. Openness to absorbing and self-altering experiences (‘absorption’), a trait
related to hypnotic susceptibility. J. Abnorm. Psychol. 83, 3 (1974), 268–277.
[145] Stefan Thie and Jacoliene van Wijk. 1998. A general theory on presence. In Proceedings of the 1st Annual International
Workshop on Presence (PRESENCE’98).
[146] John Towell and Elizabeth Towell. 1997. Presence in text-based networked virtual environments or “MUDS”. Presence: Teleoper. Virtual Environ. 6, 5 (October 1997), 590–595.
[147] Martin Usoh, Ernest Catena, Sima Arman, and Mel Slater. 2000. Using presence questionnaires in reality. Presence:
Teleoper. Virtual Environ. 9, 5 (October 2000), 497–503.
[148] Sarah van der Land, Alexander Schouten, Bart van den Hooff, and Frans Feldberg. 2011. Modeling the metaverse: A
theoretical model of effective team collaboration in 3D virtual environments. J. Virtual Worlds Res. 4, 3 (2011).
[149] Peter Vorderer, Werner Wirth, Feliz Ribiero Gouveia, Frank Biocca, Timo Saari, Lutz Jäncke, Saskia Böcking, Holger
Schramm, Andre Gysbers, Tilo Hartmann, Cristoph Klimmt, Jari Laarni, Niklas Ravaja, Ana Sacau, Thomas Baumgartner, and Petra Jäncke. 2004. MEC Spatial Presence Questionnaire (MEC-SPQ): Short Documentation and Instructions
for Application. Technical Report. Report to the European Community, Project Presence: MEC (IST-2001-37661).
[150] Eva L. Waterworth and John A. Waterworth. 2001. Focus, locus, and sensus: The three dimensions of virtual experience. CyberPsychol. Behav. 4, 2 (July 2001), 203–213.
[151] Robert B. Welch. 1999. How can we determine if the sense of presence affects task performance? Presence: Teleoper.
Virtual Environ. 8, 5 (October 1999), 574–577.
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.



<!-- page: 39 -->

A Survey of Presence and Related Concepts
96:39
[152] Robert B. Welch, Theodore T. Blackmon, Andrew Liu, Barbara A. Mellers, and Lawrence W. Stark. 1996. The effects
of pictorial realism, delay of visual feedback, and observer interactivity on the subjective sense of presence. Presence:
Teleoper. Virtual Environ. 5, 3 (Summer 1996), 263–273.
[153] Wikipedia. 2017. Immersion (virtual reality)—Wikipedia, The Free Encyclopedia.Retrieved from https://en.
wikipedia.org/w/index.php?title=Immersion_(virtual_reality)&oldid=769910362.
[154] Werner Wirth, Tilo Hartmann, Saskia Böcking, Peter Vorderer, Christoph Klimmt, Holger Schramm, Timo Saari,
Jari Laarni, Niklas Ravaja, Feliz Ribeiro Gouveia, Frank Biocca, Ana Sacau, Lutz Jäncke, Thomas Baumgartner, and
Petra Jäncke. 2007. A process model of the formation of spatial presence experiences. Media Psychol. 9, 3 (2007),
493–525.
[155] Werner Wirth, Susanne Wolf, Ursina Mögerle, and Saskia Böcking. 2004. Measuring the subjective experience of
presence with think-aloud method: Theory, instruments, implications. In Proceedings of the 7th Annual International
Workshop on Presence (PRESENCE’04). 351–358.
[156] Bob G. Witmer, Christian J. Jerome, and Michael J. Singer. 2005. The factor structure of the presence questionnaire.
Presence: Teleoper. Virtual Environ. 14, 3 (June 2005), 298–312.
[157] Bob G. Witmer and Michael J. Singer. 1998. Measuring presence in virtual environments: A presence questionnaire.
Presence: Teleoper. Virtual Environ. 7, 3 (June 1998), 225–240.
[158] Pavel Zahorik and Rick L. Jenison. 1998. Presence as being-in-the-world. Presence: Teleoper. Virtual Environ. 7, 1
(February 1998), 78–89.
[159] Shanyang Zhao. 2003. Toward a taxonomy of copresence. Presence: Teleoperat. Virtual Environ. 12, 5 (October 2003),
445–455.
Received November 2016; revised May 2017; accepted August 2017
ACM Computing Surveys, Vol. 50, No. 6, Article 96. Publication date: November 2017.
