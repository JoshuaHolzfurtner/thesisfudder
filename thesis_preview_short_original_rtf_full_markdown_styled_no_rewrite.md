# Summary Topic:

This thesis investigates how XR rowing can support sense of embodiment through the subcomponents of self-location, agency, and body ownership. Its core comparison is between an erg-centered, high-congruence mode, in which the user’s real handle and seat motion are mapped as precisely as possible to the avatar, and a boat-centered, sport-depiction mode, in which the user still rows on an erg but sees a more realistic on-water rowing action with virtual oars. The first mode prioritizes visuomotor congruence and close bodily alignment, while the second prioritizes rowing-specific realism and athletic depiction, even though the virtual motion no longer matches the real handle trajectory exactly. The central question is therefore whether embodiment in XR rowing is better supported by precise movement correspondence or by a more realistic rowing representation. In this context, engineering variables such as spatial alignment, temporal congruence, morphology, and motion mapping are treated not merely as technical details, but as factors that may directly shape immersion, perceived realism, and the feeling that the virtual rowing body and stroke are one’s own.

A bottom-of-outline version of core question:
How do spatial alignment, temporal congruence, and avatar realism influence embodiment in XR rowing, particularly when comparing a precisely mapped erg-centered avatar with a more sport-realistic but less movement-congruent boat-centered representation?

---

# First thesis outline

## 1. Introduction

- Introduce VR indoor rowing as a case where realistic sport depiction and visuomotor congruence can conflict.
- Present the core problem: should a VR rowing system prioritize
- precise alignment with the real erg and body,
- or realistic boat/oar depiction?
- State research questions around Sense of Ownership (SoO) and Sense of Agency (SoA), Sense of Embodiment/ Body Ownership (SoBo):

## 2. Theoretical Background / Related Work

- SoO and SoA in embodiment research.
- Rubber Hand Illusion (RHI) and related VR embodiment paradigms.
- Visuomotor congruence and avatar embodiment in VR.
- Brief background on VR sports / rowing applications.
- Optional section on physiological threat measures as implicit embodiment indicators.

## 3. System / Prototype

- Describe the VR rowing setup and hardware/software stack.
- Give short Introduction and Summary of rowing and the movement of a rowing stroke
- Explain the two embodiment modes:
- Ergometer-based embodiment: high visuomotor congruence (see glossary).
- Boat-based embodiment: higher rowing realism, possible mismatch.
- Describe avatar mapping / IK / hand tracking setup.
- If used: describe optional threat scene and HR integration.

## 4. Study Design / Method

- Experimental design and conditions.
- Participants and procedure.
- Measures:
- SoO / SoA questionnaires,
- optional preference / presence / realism ratings,
- optional heart-rate response to virtual threat.
- Analysis plan.

## 5. Results

- Compare conditions on:
- ownership,
- agency,
- optional physiological threat response,
- optional realism/presence ratings.
- Report main statistical outcomes and notable participant patterns.

## 6. Discussion

- Interpret whether congruence or realistic sport depiction mattered more.
- Relate findings back to embodiment theory and RHI-style work.
- Discuss what this means for designing VR sport/training systems.
- Cover limitations and possible explanations for weak/null effects.

## 7. Conclusion

- Summarize the main contribution:
- VR rowing as a testbed for embodiment,
- comparison of erg-based vs boat-based embodiment,
- implications for SoO/SoA and VR sports design.
- Brief future work outlook.


---


# Quick glossary for handoff

## Embodiment / Bodily self-consciousness
The basic experience of being a self that is located in, and tied to, a body. In the literature, this is treated as something built from multisensory and sensorimotor signals rather than only from abstract thought.

## Visuomotor / Multisensory congruence
The degree to which what I see matches what I feel and do. Embodiment gets stronger when visual, tactile, proprioceptive, vestibular (balance, spatial orientation, and eye movement), and motor signals line up in space and time; conflicts can shift self-identification and even self-location.
Visuomotor being the combination of visual and motoric congruence, so how well the movements we see match the actual ones (a ‘fake’ for example virtual movement, experienced through an illusory XR Avatar can at times appear ‘real’ to the perception of the user while being starkly incongruent).

## Sense of Self-Location (SoL)
Self-location is a determinate volume in space where one feels to be located. Normally self-location and body-space coincide in the sense that one feels self-located inside a physical body. Within the sense of embodiment framework, SoL is one of the three core subcomponents alongside sense of agency and body ownership.

## Sense of Ownership (SoO)
The feeling that a body part, or an entire body, is one’s own (experienced to the full degree to one’s own biological body). A classic example is the rubber hand illusion, in which temporally congruent seen and felt touch can induce the feeling that an artificial hand belongs to oneself. The same logic extends beyond hands to broader body illusions, and similar effects have also been reported for virtual hands and virtual bodies.

## Sense of Agency (SoA)
The feeling that one is the initiator or controller of an action or movement. In the context of this thesis, SoA concerns whether the user experiences the stroke, handle motion, or avatar movement as being caused by their own action. Agency is commonly discussed as distinct from, though related to, body ownership.

## Sense of Embodiment (SoE)
Sense of embodiment refers to the extent to which a body, especially a virtual body, is experienced as one’s own embodied self. A commonly used framework treats SoE as comprising three subcomponents: self-location, agency, and body ownership. One experiences SoE toward a body B if at least one of these components is present to some minimal degree; full SoE would correspond to all three being present strongly at once (this is always present for your biological body as the ‘gold standard’).

One experiences SoE toward a body B,
- if one feels self-located inside B (SoL) at least in a minimal intensity (P1)
- if one feels to be an agent of B (SoA) at least in a minimal intensity (P2)
- if one feels B as one’s own body (SoO) at least in a minimal intensity (P3)
if and only if one experiences at least one of the three senses at least in a minimal intensity (P4)

One experiences full SoE toward a body B,
if one experiences all of the three senses at the maximum intensity (P5)

## Bottom-up influences
Bottom-up influences are sensory-driven processes that arise from incoming signals from the body and environment. In embodiment research, these include correlations between what one feels and what one sees, such as synchronized visuotactile or visuoproprioceptive stimulation. In this thesis, examples include the user’s real handle motion, seat motion, proprioception, muscle effort, and the temporal alignment between these physical cues and the seen movement of the avatar.  The literature suggests that the strongest though would be the simultaneous real haptic grip of the rowing handle simultaneously to the virtual avatar.

## Top-down influences
Top-down influences are cognitive and perceptual expectations that shape how sensory information is interpreted. In embodiment research, these include whether the virtual body appears human-like, anatomically plausible, self-similar, or recognizable as a body that could be one’s own. In this thesis, examples include the realism of the avatar’s hands (experienced through a headset fully immersed), similarity to the participant’s body, and whether the displayed rowing body looks plausible as the participant’s own body in action

## Rubber Hand Illusion (RHI)
A classic experimental paradigm used to study body ownership. In the RHI, a participant’s real hand is hidden from view while a visible rubber hand is stroked in synchrony with the participant’s real hand. Under synchronous stimulation, participants may begin to experience the rubber hand as if it were their own, often accompanied by subjective ownership reports and shifts in perceived hand location. The RHI is widely used to investigate how visual, tactile, and proprioceptive information contribute to body representation and ownership.  It often ends with a physiological threat measure of hitting the fake hand and seeing the participant shriek back at that sight. The Top-down Influence here would be the masked real arm with the rubber hand, while Bottom-up Influence would be the synchronous simulation of real and rubber hand for example by feather.

## Cyborg’s Dilemma
The paradox that interfaces become more powerful and natural-feeling as they are incorporated into the user’s body schema, but that this incorporation also requires the user to adapt to the logic of the machine.
In the present work, the cyborg’s dilemma helps frame the tradeoff between two rowing representations. The erg-centered mode maximizes tight coupling and visuomotor congruence, potentially strengthening embodiment by making the virtual body behave as a close extension of the user’s real action. The boat-centered mode preserves a more sport-faithful visual depiction of rowing, but does so at the cost of looser correspondence between real handle motion and displayed oar motion. The dilemma, in this context, is whether embodiment is better supported by direct and full bodily incorporation (more natural but less close to rowing boat experience) or by a representation that is more faithful to the sport itself (gets the experience the user might want to have, but under the constraint that he has to accept his hands are offset from their real position, very much adapting to machine limitations).

Interestingly rowing machines already themselves might be THE perfect example of the cyborg dilemma: Accessibility to on-water training for rowers has always been an issue and while early rowing machines did have oars bolted to the gym floor since these contraptions were A too expensive and B took up too much room, rowers started to opt for much cheaper machines, with a singular handle attached to a strap you pulled in a straight line instead of an arc, that very much took away the so-called feathering and squaring so the rotation of the wrist during the rowing stroke. To this day still for that price reason (modern oar based rowing machines are higher 4 digit figures) they accept the tradeoff to still train the muscle groups and (similar) movements they need.
In my XR setup, the same dilemma reappears in an almost inverted form. The physically most congruent solution is now the erg-centered representation, because the virtual handle and seat can closely follow the real machine. However, the sport-realistic solution is the boat-centered representation, because it restores the visual experience of sitting in a racing shell and moving oars on water. The question is therefore not simply whether VR should be more or less realistic, but which kind of realism matters more for embodiment and preferences: the bodily realism of matching the user's actual erg movement, or the sport-specific realism of visually returning the user to the on-water rowing action that the erg originally abstracted away.

## Proteus effect
The Proteus effect refers to changes in a user’s behavior, attitudes, or self-perception caused by the visual appearance of the avatar they embody or control in a virtual environment. The term was introduced by Yee and Bailenson (2007) and is named after Proteus, the shape-shifting figure from Greek mythology. The basic idea is that users may partly adapt to the traits implied by their virtual body: for example, an athletic avatar may influence perceived exertion, self-perceived fitness, or physical performance during VR exercise. In the context of this thesis, the Proteus effect is relevant because a realistic, athletic, or customized rowing avatar may not only represent the user visually, but may also influence how the user experiences effort, agency, and identification during XR rowing.

## Optic flow
Optic flow is the visual evidence that movement through a world is happening. In real outdoor sport, it occurs automatically: when a cyclist, runner, skier, or rower moves forward, the road, water, shoreline, trees, buoys, and other objects appear to move past them. Virtual sport systems such as Zwift, Holofit, or XR rowing recreate this visual pattern while the user remains physically stationary. The user’s effort moves an avatar, bike, boat, or camera through a virtual route, and the changing scenery provides the visual impression of travel. In this thesis, optic flow is important because it helps stationary ergometer exercise feel like locomotion through an Virtual Reality environment experienced inside a headset rather than a stationary effort stuck in place.

## Vection
Vection is the visually induced sensation of self-motion, where a person feels as if they are moving despite being physically stationary. In stationary virtual-sport systems such as indoor cycling or rowing applications, continuous optic flow and sensorimotor coupling between user effort and virtual movement may create vection-like self-motion cues. This can help the user experience indoor exercise less as stationary repetition and more as locomotion through a virtual environment.
For us that can be an embodied exergame / virtual sport system that transforms repetitive indoor exercise into meaningful, visible, and socially situated progress. Kopelasia can be framed as an embodied virtual-sport system that counters the “Sisyphus” character of indoor exercise by turning repetitive exertion into sensorimotor progress, avatar-mediated self-representation, and virtual locomotion through a sport-specific environment, be that on desktop or inside the headset.
Formula: stationary exercise → optic flow → vection/spatial presence → reduced awareness of being stationary
Vection is the sensation of self-motion that can arise from optic flow. In other words, optic flow is the visual motion pattern, while vection is the felt impression that “I am moving.” In virtual sport systems, the user may know they are physically stationary, but effort-coupled optic flow can still make the workout feel like moving through a world.

- Presence (often “spatial presence” / “being there”)
Presence is the subjective feeling of being located in a mediated or virtual environment rather than merely observing it from outside. In XR rowing, spatial presence concerns whether the user feels situated on the river, in the boat, or in the virtual training environment, rather than only sitting on a stationary erg in a room.

## Place Illusion
a more specific framing of feeling of “being in a place” that’s often used in VR research. Place Illusion is Slater’s term for the illusion of “being there” in a virtual place and is related to presence, but more specifically emphasizes the perceptual illusion that one is located inside the virtual environment. In XR rowing, Place Illusion concerns whether the user feels present in the virtual rowing scene, independently of whether the virtual rowing body feels like their own (so it parts out the virtual avatar and is only location focussed).

## Plausibility Illusion
Plausibility Illusion is Slater’s term for the illusion that events in a virtual environment are really happening. In XR rowing, this concerns whether the avatar, oars, boat, water, opponents, and feedback behave coherently enough that the rowing scenario feels believable. This is distinct from Place Illusion: a user may feel located in the virtual environment but still find the rowing action implausible, or vice versa.

- Flow / absorption: the attentional state where you’re so engaged that you lose awareness of time and the outside world. Flow is a state of deep task engagement in which attention is focused, action feels smooth, feedback is immediate, and the activity becomes intrinsically rewarding. In virtual sport systems, flow may help explain why stationary exercise can become engaging and time-distorting when effort, feedback, challenge, and progress are well matched. In this thesis, flow is relevant as a design goal, but it should not be treated as a measured outcome unless explicitly assessed.

## Anti-Sisyphus effect
Working term for the design effect where stationary exercise stops feeling like repetitive effort in place and begins to feel like meaningful locomotion through a world. In virtual sport systems such as Zwift-style cycling or XR rowing, this effect can be understood through established constructs such as optic flow, vection, spatial presence, flow, and sensorimotor coupling between user effort and virtual displacement. The user remains physically stationary, but the system gives the exertion spatial consequence: power, cadence, or stroke output becomes visible forward motion.

## ‘Zwift formula’ built on the concept of Vection
A design pattern in virtual sport systems where stationary physical effort is mapped to continuous virtual locomotion. The formula combines real exertion, live performance metrics, optic flow, spatial presence, route progression, goals, and social comparison so that indoor training feels less like static repetition and more like movement through a meaningful environment.

stationary effort on erg (be that bike, ski, treadmill or rowing)
+ continuous optic flow
+ power/pace-to-world-speed mapping
+ spatial presence in the virtual world
+ goals/social comparison
+ presence of other users
= perceived fun and purposeful exertion instead of static will breaking repetition

# Motion Sickness & stationary Cardio will breaking

## Stationary-exercise frustration & VR Motion sickness
Stationary ergometers create a peculiar sensorimotor and motivational mismatch: the user produces rhythmic locomotor effort, but the physical environment provides no corresponding displacement through space - leading to a frustration of the user many digital apps try to resolve. On the complete other end is the motion sickness many experience inside a VR Headset, which is caused by conflicts between visual motion artificially being triggered decoupled from the real movement of the user and vestibular/proprioceptive signals of his body, resulting in nausea and discomfort .
Interestingly, both cases involve a mismatch between bodily signals and perceived motion consequences. Virtual sport systems can reduce this mismatch by mapping effort to visible locomotion, route progression, optic flow, and spatial presence. In this sense, the virtual environment gives stationary exertion an action consequence: the user’s work moves a body, boat, or avatar through a world. Interestingly this mechanism also resolves motion sickness by tapping into the same reason we dont have car sickness on rowing boats (while this has not been documented in scientific studies tests inside this thesis have not led to single case of motion sickness yet, even in users highly susceptible to it, see questionnaire). The brain builds a bridge between the exertion you perform and you being moved in accordance to that exertion.
In other words the layer of abstraction to reality can be so thin, that regular motivational and perceptive mechanism of the real sport kick back in fully.
This effect isn’t speed related as tests even at very high speed still lead to that effect, yet when we decouple and artificially move the user it set back in.

Stationary ergometers create a peculiar sensorimotor and motivational mismatch: the user produces rhythmic locomotor effort, but the physical environment provides no corresponding displacement through space, leading to a frustration that many digital fitness apps try to resolve. On the other end is the motion sickness many users experience inside a VR headset, which is caused by conflicts between artificially triggered visual motion, decoupled from the user’s real movement, and the vestibular/proprioceptive signals of the body, resulting in nausea and discomfort.
Interestingly, both cases involve a mismatch between bodily signals and perceived motion consequences. Virtual sport systems can reduce this mismatch by mapping effort to visible locomotion, route progression, optic flow, and spatial presence. In this sense, the virtual environment gives stationary exertion an action consequence: the user’s work moves a body, boat, or avatar through a world.
Interestingly, this mechanism may also reduce motion sickness by tapping into the same reason we do not normally experience car-sickness-like discomfort on rowing boats: the brain can build a bridge between the exertion being performed and the movement that follows from that exertion. While this has not yet been documented as a general scientific claim, tests within this thesis have not led to a single case of motion sickness so far, even among users highly susceptible to it (see questionnaire).
In other words, the layer of abstraction to reality can become so thin that regular motivational and perceptual mechanisms of the real sport begin to reappear.
This effect does not appear to be simply speed-related: in prototype tests, even very high virtual speeds did not trigger discomfort when coupled to rowing effort. However, when the user was moved artificially and the motion was decoupled from rowing action, discomfort reappeared.


## Motion sickness, simulator sickness, and cybersickness

Motion sickness is the broad term for nausea and discomfort related to motion, including car sickness and seasickness. Simulator sickness refers to motion-sickness-like symptoms caused by simulator systems (e.g., flight or driving simulators), typically when visual motion cues do not match vestibular and proprioceptive signals. Cybersickness (or VR sickness) is the closely related term used in VR/XR research for the same symptom family occurring in virtual environments. In this thesis, “VR motion sickness” is used as the readable umbrella, with simulator sickness and cybersickness treated as related research terms.

## VR Motion Sickness / Cybersickness

VR motion sickness, often called cybersickness in XR research, refers to motion-sickness-like discomfort caused by exposure to virtual environments. Common symptoms include nausea, dizziness, disorientation, eye strain, headache, sweating, stomach awareness, and general discomfort. It is often explained through conflicts between visually presented motion and bodily motion cues from the vestibular and proprioceptive systems. In this thesis, “VR motion sickness” is used for readability, while “cybersickness” is treated as the corresponding research term.

## Simulator sickness
Simulator sickness is the older simulator-research term for motion-sickness-like symptoms caused by non-XR or pre-consumer-VR simulator systems, especially flight and driving simulators (often displays around the user see ‘rowing cave’ setups Thesis). It overlaps with VR motion sickness and cybersickness, but historically refers to simulator setups such as cockpit, vehicle, projection, or training simulators rather than modern headset-based XR. In this thesis, the more readable term “VR motion sickness” is used for the headset rowing case, while simulator sickness is only mentioned as part of the broader research history.

## Cybersickness / Discomfort Rating Users
Please rate how strongly you experienced the following during or after the XR rowing condition.

0 = not at all
1 = slight
2 = moderate
3 = severe

- nausea
- dizziness
- eye strain
- headache
- disorientation
- stomach awareness
- sweating / warmth
- general discomfort

Optional open question:
Did the virtual boat/world movement feel connected to your own rowing effort?
- not at all
- slightly
- moderately
- strongly
- very strongly

Optional open text:
Did anything about the motion feel uncomfortable, artificial, or disconnected?


## Sea Sickness Rowing
### 1. Sea sickness Flat-water rowing:
There is little evidence that seasickness is a common or central issue in ordinary flat-water rowing. This is plausible because the athlete is outdoors, visually oriented, actively self-propelling, and usually moving over comparatively smooth water. The boat may bob slightly, but the wave-induced motion is normally minimal compared with rough-water or ocean conditions.

### 2. Sea Sickness Ocean rowing / rough-water boats:
Seasickness is clearly possible in ocean rowing or rough-water boating. In these cases, the boat and rower are continuously moved by waves, producing stronger pitch, roll, and heave. The user is no longer only moving through self-generated rowing action, but is also being passively moved by the water. This can create stronger sensory conflict and discomfort.This reminds us a lot to motion sickness a form of cyber Seasickness, in which artificial movement is triggering nausea.

### 3. Sea Sickness VR Rowing:
In the XR rowing prototype, simulated wave motion was uncomfortable when it visually moved or rocked the user/boat in a way that was not caused by the user’s own rowing action. A practical solution was to keep the user’s viewpoint and embodied position in stable equilibrium, while letting the world, water, and boat bob in accordance to a water simulation. In other words, the system can show rowing on water without forcing the user’s virtual body or camera to bob with every simulated wave.
This suggests a useful design rule: rowing effort should produce forward motion, but wave motion should be treated carefully. Stroke-coupled locomotion can support vection and spatial progress, while passive camera/boat rocking may reintroduce the sensory conflict associated with seasickness or motion sickness.

## Multisensory / sensorimotor congruence

Multisensory and sensorimotor congruence describe how well the user’s sensory and motor signals fit together. In embodiment research, virtual bodies are more likely to feel believable or self-related when what the user sees matches what they feel, do, and expect. In XR rowing, congruence is not one single property, but a combination of spatial, temporal, visuomotor, visuoproprioceptive, haptic, and morphological relationships between the real rower, the ergometer, and the virtual avatar.

### Visuomotor congruence

Visuomotor congruence describes how well seen movement matches the user’s own real movement. In XR rowing, this concerns whether the avatar’s hands, arms, torso, handle, seat, and stroke timing appear to move in accordance with the user’s actual rowing action. The erg-centered mode prioritizes visuomotor congruence by mapping the real handle and seat movement as directly as possible to the virtual body.

### Visuotactile congruence

Visuotactile congruence describes how well seen touch matches felt touch. The classic example is the rubber hand illusion, where seeing a rubber hand touched at the same time as one’s hidden real hand can produce ownership over the rubber hand. In XR rowing, the strongest visuotactile cue is the simultaneous real grip of the rowing handle and the seen virtual hand/handle contact. The user feels the handle while seeing the avatar hold the corresponding virtual handle or oar.

### Visuoproprioceptive congruence

Visuoproprioceptive congruence describes how well the seen body position matches the felt position of the real body. Proprioception tells the user where their limbs, torso, and body are. In XR rowing, this concerns whether the avatar’s arms, hands, torso, and seat position appear where the user’s body feels them to be. Poor visuoproprioceptive congruence can occur if the virtual hands, oars, or body are visibly offset from the user’s felt posture.

### Spatial congruence

Spatial congruence describes how well real and virtual elements line up in physical space. In XR rowing, this includes alignment between the real ergometer and the virtual erg/boat, the real handle and virtual handle or oar, the user’s head and virtual camera, and the real seat motion and virtual body position. Spatial congruence is especially important because the user is physically sitting on and interacting with a real machine.

### Temporal congruence

Temporal congruence describes how well the timing of virtual feedback matches the timing of real movement. In XR rowing, the avatar, handle, seat, oars, boat speed, and visual feedback should respond at the right moment. Even small delays can weaken agency, make the avatar feel less self-controlled, or make the rowing motion feel artificial.

### Haptic / force congruence

Haptic or force congruence describes how well physical forces match the visual action. In XR rowing, the real ergometer provides handle resistance, grip pressure, seat motion, and muscular effort. The erg-centered mode benefits from these real physical cues. The boat-centered mode may look more like on-water rowing, but it cannot fully reproduce oar-water forces unless additional haptics are added.

### Morphological congruence / similarity

Morphological congruence describes how well the virtual body matches the user’s real or expected body shape. This includes body proportions, arm length, hand size, posture, and possibly face or clothing similarity. In XR rowing, morphological congruence matters because an avatar with mismatched limb lengths or hand positions may weaken body ownership or make the rowing motion feel less plausible.

### Action-outcome congruence

Action-outcome congruence describes whether the system response makes sense as a consequence of the user’s action. In XR rowing, each stroke should produce believable avatar motion, boat movement, optic flow, and progress through the environment. This is central to the “Zwift formula”: stationary effort becomes meaningful when it produces visible locomotion and progress.

### Sport-action congruence

Sport-action congruence describes how well the virtual action matches the expected movement logic of the sport. In rowing, this includes catch, drive, finish, recovery, oarlock behavior, blade movement, feathering, squaring, and boat response. The boat-centered mode prioritizes sport-action congruence, even if it sacrifices some direct congruence with the real erg handle trajectory.


## Core congruence tradeoff in this thesis

The erg-centered mode prioritizes bodily and device congruence: the virtual avatar follows the user’s real handle, seat, and body motion as closely as possible.

The boat-centered mode prioritizes sport-action congruence: the user still rows on an ergometer, but the virtual scene restores the visual logic of on-water rowing with oars, oarlocks, blades, and boat movement with the hands being repositioned to oar handles moving about in a car in accordance to boat not erg rowing.

The central research question is therefore not whether one mode is simply more realistic, but which kind of congruence better supports embodiment: direct congruence with the user’s physical erg action, or congruence with the expected visual and athletic logic of rowing.

---
# Rowing Terms

## Rowing stroke phases Catch, Drive, Finish & Release (ergometer and boat)
A rowing stroke starts at the catch: the rower sits forward on the sliding seat, knees bent, arms extended, upper body leaning slightly forward, and the handle is farthest away from the body.
The drive begins with the legs. The rower pushes the seat backwards by extending the legs, while the arms stay long and the upper body initially remains stable. Once the legs are mostly extended, the upper body swings back from the forward lean into a slightly backward position, roughly around the “eleven o’clock” position. Only after this body swing do the arms pull the handle in toward the lower ribs or upper stomach.
At the finish, the legs are extended, the upper body is slightly leaned back, and the handle is close to the body. The recovery then reverses the sequence: first the arms move away again, then the upper body swings forward, and only after the hands and body have moved forward does the seat slide toward the next catch as the knees bend again.
The drive begins with the legs. The rower pushes the seat backwards by extending the legs, while the arms stay long and the upper body initially remains stable. Once the legs are mostly extended, the upper body swings back from the forward lean into a slightly backward position, roughly around the “eleven o’clock” position. Only after this body swing do the arms pull the handle in toward the lower ribs or upper stomach.
On an ergometer, this movement is simplified into a straight-line handle pull. In a rowing boat, the same body sequence drives oars that move through an arc around the oarlocks. This adds boat-specific elements such as blade placement, extraction, feathering, and squaring, which are not present on most common ergs.

## Feathering and squaring (boat)
Feathering and squaring describe the rotation of the oar blade during the rowing stroke. Before the drive, the blade is squared, meaning it is turned vertically so it can enter the water and apply force. During the recovery, the blade is feathered, meaning it is turned flatter so it moves through the air with less resistance. Most common ergometers remove this blade-rotation component because the user pulls a single handle in a straight line instead of controlling two oars through an arc.

## Ergometer / erg / ergo
An ergometer is a stationary rowing machine used for indoor rowing training. Rowers often shorten the term to “erg”; in Europe, “ergo” is also common. In this thesis, the user physically rows on an ergometer while seeing either an erg-centered or boat-centered virtual representation.

## Handle
The handle is the part of the rowing machine that the user pulls during the stroke. On most common ergometers, the handle is attached to a chain, strap, or cord and moves mostly in a straight line toward and away from the body.

## Sliding seat
The sliding seat is the seat on which the rower moves forward and backward during the stroke. It allows the legs to contribute strongly to the rowing movement. In this thesis, the seat position is important because it helps infer the avatar’s body pose.In both versions the position of it is approximatively simulated on the virtual 3d Model of boat/erg .

## Racing shell / rowing shell
A racing shell is the narrow boat used in rowing. In the boat-centered VR condition, the user visually sits in such a shell, even though they are physically still rowing on an ergometer.

## Oar
An oar is the long lever used to move a rowing boat through the water. In real boat rowing, the rower does not pull a central handle in a straight line, but moves one or two oars through an arc around the oarlocks.
The oar handle is the part of the oar held by the rower. In the boat-centered condition, the avatar’s hands are visually attached to virtual oar handles rather than to the real ergometer handle.
The oarlock is the pivot point that holds the oar on the boat. Because the oar rotates around this point, the oar handle follows an arc rather than a straight line. This is one reason why real boat rowing and ergometer rowing differ mechanically.
The blade is the flat end of the oar that enters the water and applies force during the drive phase. Blade movement is visually important in boat rowing but is absent from most common ergometers.

## Stroke rate
Stroke rate describes how many strokes are rowed per minute. It is often shown as “spm” or “strokes per minute” and is one of the main rhythm metrics in rowing.

## Split
Split usually refers to the time needed to row 500 meters, for example 2:00/500m. It is the standard performance metric for speed in rowing.

## Stroke length
Stroke length describes how long the rowing movement is, for example how far the handle travels or how much of the slide is used. In this thesis, stroke length can be relevant as an objective movement metric and is used inside a mini game.

## Erg-centered representation
An erg-centered representation is a virtual rowing mode where the virtual handle and seat closely match the user’s real ergometer handle and seat. This prioritizes visuomotor congruence.

## Boat-centered representation
A boat-centered representation is a virtual rowing mode where the user still rows on an ergometer, but the avatar appears to row in a boat with oars. This prioritizes sport-specific rowing realism, but introduces a mismatch between the real handle path and the virtual oar-handle path.

## Boat classes
Rowing boats are usually named by crew size and oar type. “x” means sculling, where each rower uses two oars, for example 1x, 2x, or 4x. “+” means the boat has a coxswain, while “-” means it does not. Common examples are the single scull (1x), double scull (2x), quadruple scull (4x), four (4-/4+), and eight (8+). For this thesis, the exact class is less important than the distinction between solo rowing and crew rowing.

## Sculling and sweep rowing
In sculling, each rower uses two oars, one in each hand. In sweep rowing, each rower uses one oar with both hands. This matters because common ergometers do not reproduce either setup exactly: the erg handle is a simplified training interface, while the boat-centered VR condition visually restores an oar-based rowing action.

## Crew rowing / synchronisation
In crew rowing, several rowers must match timing, rhythm, and pressure so the boat moves efficiently.

## Stroke seat
The rower who sets the rhythm for the crew.

## Coxswain / cox
The person who steers some crew boats and gives rhythm, strategy, and motivation cues.

---
# XR Terms

## VR motion sickness / cybersickness

VR motion sickness, often called cybersickness in XR research, refers to motion-sickness-like discomfort caused by exposure to virtual environments. Common symptoms include nausea, dizziness, disorientation, eye strain, headache, sweating, stomach awareness, and general discomfort. It is usually discussed as a conflict or mismatch between visually presented motion and bodily motion cues from the vestibular and proprioceptive systems.

Related terms include simulator sickness, visually induced motion sickness (VIMS), and VR sickness. Simulator sickness is the older term from simulator research, especially flight and driving simulation. Cybersickness is the common XR/HCI term for sickness caused by virtual or extended-reality environments. Visually induced motion sickness emphasizes the role of visual motion and optic flow in triggering symptoms. In this thesis, the term VR motion sickness is used for readability, while cybersickness is treated as the corresponding research term.

For XR rowing, this is relevant because virtual locomotion is central to the experience: the user remains physically seated on an ergometer, while the visual scene suggests forward motion through water. If this motion is artificially imposed or decoupled from the user’s stroke, it may create sensory conflict. If forward motion is tightly coupled to rowing effort, the visual displacement may feel more self-generated and therefore more coherent with the user’s action.


## Extended Reality (XR)

Extended Reality (XR) is an umbrella term for technologies that blend or mediate the user’s perception of the physical and digital world. It commonly includes Virtual Reality (VR), Augmented Reality (AR), and Mixed Reality (MR). In this thesis, XR is used as the broader term because the rowing system concerns both immersive headset-based rowing and possible future extensions in which virtual rowing elements are combined with the physical rowing machine and surrounding room.

## Virtual Reality (VR)

Virtual Reality (VR) refers to a computer-generated environment that surrounds or replaces the user’s view of the physical world, usually through a head-mounted display. In this thesis, VR describes the headset-based rowing experience in which the user rows on a physical ergometer while seeing a virtual rowing environment, avatar body, boat, oars, and water.

## Augmented Reality (AR)

Augmented Reality (AR) refers to systems that overlay digital information or objects onto the user’s view of the physical world. AR does not necessarily replace the real environment, but adds virtual elements to it. In the context of this thesis, AR is not the main target, but it is relevant as a possible future direction for showing rowing feedback, avatar overlays, or technique guidance around the real ergometer.

## Mixed Reality (MR)

Mixed Reality (MR) refers to systems in which physical and virtual elements are spatially registered and can appear to coexist or interact. Compared with simple AR overlays, MR usually implies a stronger relationship between digital objects and the physical environment. In XR rowing, an MR version could align virtual oars, avatars, UI, or coaching feedback with the real ergometer and room.

## Head-Mounted Display (HMD)

A head-mounted display (HMD) is a display device worn on the head that presents visual content directly in front of the user’s eyes. VR HMDs usually replace the user’s view of the real world with a virtual environment, while AR/MR HMDs may combine digital content with the real world. In this thesis, the HMD is important because it determines the user’s field of view, head-tracked perspective, immersion, and possible experience of self-location inside the virtual rowing scene.

## Six Degrees of Freedom (6DoF)

Six degrees of freedom (6DoF) tracking measures both position and rotation in three-dimensional space. The six components are translation along the X, Y, and Z axes, plus rotation around those axes. In XR rowing, 6DoF tracking is relevant for the headset, hands, controllers, and potentially tracked objects such as the handle or seat.

## Three Degrees of Freedom (3DoF)

Three degrees of freedom (3DoF) tracking measures rotation but not positional movement. A 3DoF device can detect where the user is looking, but not where the device has moved in space. For embodied rowing, 3DoF is usually insufficient for precise avatar alignment because rowing depends on spatial relationships between the head, hands, handle, seat, and ergometer.

## Tracking

Tracking refers to the system’s ability to estimate the position, rotation, or movement of the user, device, or physical objects. In this thesis, tracking includes headset tracking, hand/controller tracking, and possibly handle or seat tracking. Tracking quality directly affects spatial alignment, temporal congruence, agency, and embodiment.

## Hand Tracking

Hand tracking refers to detecting the pose and movement of the user’s hands without necessarily using physical controllers. In XR rowing, hand tracking is relevant because the user’s hands are central to the rowing stroke and because virtual hands may strongly influence agency and body ownership. However, hand tracking alone may not capture the physical constraints of the erg handle unless it is combined with handle tracking or a model of the rowing machine.

## Controller Tracking

Controller tracking refers to measuring the position and orientation of handheld input devices. Controllers can provide reliable tracked points and button input, but they may not match the physical rowing handle unless mounted, aligned, or modeled carefully. In XR rowing, controller tracking can be useful for prototyping but may introduce a mismatch if the controller does not correspond to the real handle interaction.

## Inside-Out Tracking

Inside-out tracking uses sensors on the headset or device to estimate movement relative to the environment. Most modern standalone VR headsets use inside-out tracking. In XR rowing, inside-out tracking is useful because it avoids external tracking hardware, but it can be challenged by occlusion, limited camera views, low texture environments, or unusual hand/handle positions.

## Outside-In Tracking

Outside-in tracking uses external cameras, base stations, or sensors to track the headset, controllers, or markers. It can be highly accurate but requires additional setup. For XR rowing, outside-in tracking could improve handle/seat/body tracking precision, but it may reduce accessibility compared with a standalone or consumer-friendly system.

## Spatial Alignment

Spatial alignment refers to matching the virtual scene, avatar, or interaction objects to the real physical setup. In XR rowing, spatial alignment means that the virtual erg, handle, seat, body, and viewpoint should correspond closely to the user’s real rowing machine and body position. Poor spatial alignment can reduce agency, ownership, and realism.

## Calibration

Calibration is the process of measuring or adjusting the system so that the virtual setup matches the real user and physical environment. In this thesis, calibration may include aligning the virtual erg to the real erg, matching avatar proportions, setting handle and seat positions, and ensuring that the virtual rowing body appears in the correct location relative to the user.

## Latency

Latency is the delay between a user’s real movement or input and the corresponding response in the virtual system. In XR rowing, latency can affect agency, timing, motor performance, comfort, and embodiment. Low latency is especially important when the virtual avatar, hands, handle, or oars are expected to feel tightly coupled to the user’s real motion.

## Temporal Congruence

Temporal congruence describes how well the timing of virtual feedback matches the timing of the user’s real action. In XR rowing, temporal congruence means that the avatar, handle, seat, oars, boat motion, and feedback should respond at the right moment. Even if spatial mapping is imperfect, good timing may support agency and plausibility.

## Field of View (FOV)

Field of view (FOV) describes how much of the visual environment is visible at once. In HMDs, FOV affects immersion, spatial presence, optic flow, and the feeling of being inside the virtual scene. In XR rowing, a wider FOV can strengthen the feeling of being on the water, but strong peripheral optic flow may also influence comfort and VR motion sickness.

## Frame Rate

Frame rate is the number of rendered images displayed per second. High and stable frame rates are important in VR because low or unstable frame rates can reduce comfort, increase latency, and contribute to motion sickness. In XR rowing, stable performance matters because the user is physically exerting themselves while relying on continuous visual feedback.

## Refresh Rate

Refresh rate is the frequency at which the display updates, usually measured in hertz. Common VR refresh rates include 72 Hz, 80 Hz, 90 Hz, or higher depending on the headset. Higher refresh rates can improve smoothness and comfort, but also increase rendering performance requirements.

## Locomotion

Locomotion refers to movement through an environment. In many VR applications, locomotion is triggered through joystick input, teleportation, walking-in-place, or artificial camera movement. In XR rowing, locomotion is stroke-coupled: the user’s rowing effort moves the virtual boat or avatar through the environment.

## Stroke-Coupled Locomotion

Stroke-coupled locomotion is a design pattern in which the virtual movement through the world is driven by the user’s rowing stroke. Instead of moving the user passively through the environment, the system maps rowing effort, stroke timing, or pace to visible forward motion. This is central to the “Zwift formula” for rowing because it gives stationary exertion spatial consequence.

## Artificial Locomotion

Artificial locomotion refers to virtual movement that is not produced by equivalent real-world body movement. Examples include joystick movement, automatic camera motion, or scripted movement through a scene. Artificial locomotion can be useful, but it may increase VR motion sickness if visual motion is decoupled from the user’s bodily signals.

## Embodied Interaction

Embodied interaction refers to interaction in which the user’s body, movement, posture, and physical environment are central to how the system is used. XR rowing is an embodied interaction problem because the user’s real rowing movement, effort, handle grip, seat motion, and avatar feedback are all part of the interaction loop.

## Inverse Kinematics (IK)

Inverse kinematics is a method for calculating joint rotations so that a character’s body parts reach desired target positions. In XR rowing, IK can be used to make the avatar’s hands, arms, torso, and body align with tracked targets such as the handle, head, or seat. IK is important because the avatar must appear plausible while also responding to the user’s real movement.

## Avatar

An avatar is the user’s represented body or character in a virtual environment. In this thesis, the avatar is not merely decorative: its body, hands, posture, and rowing movement are central to agency, body ownership, self-location, and perceived realism.

## Self-Avatar

A self-avatar is an avatar experienced or intended as representing the user’s own body. In XR rowing, a self-avatar may support embodiment if it appears spatially aligned, temporally responsive, anatomically plausible, and sufficiently similar to the user’s body or expected rowing body.

## Morphological Similarity

Morphological similarity describes how closely the virtual body resembles the user’s real body in shape, proportions, size, posture, and appearance. In XR rowing, matching arm length, hand size, body proportions, or face appearance may support body ownership and plausibility, but it should be distinguished from the Proteus effect unless avatar appearance is tested as an independent manipulation.

## World-Space UI

World-space UI is user-interface content placed inside the 3D virtual environment rather than attached flatly to the screen. In XR rowing, examples could include a boat-mounted display, floating pace indicators, or diegetic rowing instruments. World-space UI can support immersion if it appears as part of the rowing environment.

## Diegetic UI

Diegetic UI refers to interface elements that exist inside the fictional or virtual world itself. For example, a rowing monitor mounted on the virtual boat or erg would be diegetic, while a floating abstract HUD may be non-diegetic. In XR rowing, diegetic UI can help maintain the illusion of being inside a rowing scenario.

## Non-Diegetic UI

Non-diegetic UI refers to interface elements that are visible to the user but do not belong to the virtual world itself. Examples include floating menus, overlays, or debugging-style metrics. Non-diegetic UI can be efficient but may reduce sport realism or spatial plausibility if overused.

## Haptics

Haptics refers to tactile or force feedback provided through physical interaction. In XR rowing, haptics include the real grip of the handle, seat motion, resistance from the ergometer, vibration, and any additional feedback that helps the user feel the rowing action. The real erg already provides strong haptic grounding, which is one reason it matters for embodiment.

## Proprioception

Proprioception is the sense of the position and movement of one’s own body. In XR rowing, proprioception comes from the user’s real arms, legs, torso, hands, handle grip, and seat motion. The relationship between proprioception and visual avatar feedback is central to visuomotor congruence.

## Vestibular System

The vestibular system contributes to balance, orientation, and the perception of head motion and acceleration. In VR, conflicts between visual motion and vestibular signals are a major factor in motion sickness. In XR rowing, the user is visually moving through water while physically remaining mostly stationary, so vestibular conflict must be handled carefully.
