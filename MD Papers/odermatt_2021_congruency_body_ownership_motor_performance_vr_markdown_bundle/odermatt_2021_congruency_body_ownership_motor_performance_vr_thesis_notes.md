# Thesis notes — Odermatt et al. 2021, “Congruency of Information Rather Than Body Ownership Enhances Motor Performance in Highly Embodied Virtual Reality”

## Citation identity

Odermatt, I. A., Buetler, K. A., Wenk, N., Özen, Ö., Penalver-Andres, J., Nef, T., Mast, F. W., & Marchal-Crespo, L. (2021). *Congruency of Information Rather Than Body Ownership Enhances Motor Performance in Highly Embodied Virtual Reality*. Frontiers in Neuroscience, 15, Article 678909. https://doi.org/10.3389/fnins.2021.678909

## What this paper is

This is an original experimental VR study on body ownership, multisensory congruency, and motor performance. It is not about rowing, cycling, sports VR, or avatar rowing specifically. Its value for the XR rowing thesis is methodological and conceptual: it shows that in immersive embodied VR, improved motor performance may be driven more by congruent task-relevant information than by body ownership alone.

For the thesis, this is a high-priority source for the distinction between:

- body ownership,
- agency,
- self-location/location,
- congruent versus incongruent information,
- motor performance.

It is especially useful for avoiding the overclaim that “higher body ownership automatically improves performance.” The paper’s title is almost the thesis warning: congruency of information may matter more than body ownership for performance.

## Content summary

Odermatt et al. investigate whether body ownership over a virtual hand improves motor performance in immersive VR, and whether previous findings may have been confounded by congruent versus incongruent multisensory information.

The authors start from the idea that HMD-based VR can replace symbolic limb representations, such as cursors, with realistic first-person avatars. Such avatars may create embodiment, including body ownership, agency, and self-location. Body ownership and motor control share neural correlates, especially in frontal and premotor areas, but it is unclear whether body ownership itself functionally improves motor performance.

The key methodological problem is that many studies induce body ownership by giving congruent multisensory stimulation, and reduce ownership by giving incongruent stimulation. That means “high body ownership” is often confounded with “congruent information,” and “low body ownership” with “incongruent/competing information.” Odermatt et al. therefore add unimodal conditions to separate congruency effects from ownership effects.

The study tested 50 healthy right-handed participants in immersive VR. Participants saw a gender-matched avatar from first-person perspective. The right virtual hand was visible. Participants received visuo-tactile stimulation: a real brush stroked their real fingers while a virtual brush appeared to stroke the virtual fingers.

The five experimental conditions were:

1. Congruent:
   - real and virtual brush stroked the same finger.

2. Incongruent visual:
   - real and virtual brush stroked different fingers; participant responded to visual information.

3. Incongruent haptic:
   - real and virtual brush stroked different fingers; participant responded to haptic information.

4. Only visual:
   - participant saw the virtual brush but did not feel real stroking.

5. Only haptic:
   - participant felt real stroking but did not see the virtual brush.

Participants completed two tasks:

1. Sensorimotor decision-making task:
   - press a button as fast as possible when the target finger was stroked.

2. Motor task:
   - follow predefined 3D paths with the virtual hand/controller as accurately and quickly as possible.

The study measured:

- subjective body ownership,
- location,
- agency,
- disownership / loss of own hand,
- control items,
- GSR response to a virtual knife threat,
- reaction times,
- trajectory accuracy,
- completion time.

A useful practical detail: the paper includes embodiment questionnaire items in Table 2. These include body ownership items such as “It seemed like the virtual hand was my hand,” location items such as “It seemed like my hand was in the location where the virtual hand was,” and agency items such as “It seemed like I was in control of the virtual hand” and “It seemed like I was causing the movements I saw.”

The main result is that congruency of information affected speed/performance. Incongruent information slowed participants down. In the decision-making task, reaction times were slower in incongruent conditions than in the corresponding unimodal conditions. In the motor task, participants in the incongruent haptic condition needed more time to complete the task than participants in congruent or unimodal conditions.

The authors did not find strong differences in body ownership between conditions after the tasks. Body ownership was high across conditions, likely because first-person immersive VR, realistic virtual limb appearance/posture, and a virtual limb connected to the body already induced body ownership strongly. Body ownership was also higher after the motor task than after the decision-making task, likely because visuomotor synchrony reinforced ownership.

The authors conclude that congruent multisensory/task-relevant information may improve reaction and completion times in immersive VR motor tasks, while the independent role of body ownership remains harder to isolate. They warn that previous studies linking body ownership and motor performance may have been confounded by congruency effects.

## Why it matters for the XR rowing thesis

This paper is highly relevant because the XR rowing thesis compares two avatar/action mappings:

1. Erg-centered / high-congruence mode:
   - real erg handle, seat, and user motion are mapped closely to the virtual body and handle.

2. Boat-centered / sport-depiction mode:
   - the user still rows on an erg, but sees a rower in a boat with oars, oarlocks, blades, and on-water rowing logic.

The central issue is that the boat-centered mode may be more sport-realistic but less directly congruent with the real physical action. The real hand/handle path says one thing, while the virtual oar/hand path may say another. Odermatt et al. provide strong support for taking this mismatch seriously.

The paper helps phrase the thesis question more carefully:

- If the erg-centered mode performs better, it may not simply be because it creates more body ownership.
- It may be because the visual, haptic, proprioceptive, and task-relevant information is more congruent and less confusing.
- If users go faster or hesitate less in the erg-centered mode, this could be because they have to question the mapping less.
- If the boat-centered mode feels less direct, the problem may be competing information, not merely “less realism.”

This is especially relevant to your offset oar-arm IK system. The issue is not just whether the virtual arms look plausible. The issue is whether the mapping remains coherent enough that the user does not experience conflicting task information.

## Core findings / cheat sheet

- Body ownership and motor control share neural correlates, but the functional benefit of body ownership for motor performance remains unclear.
- Many studies confound body ownership with congruent multisensory stimulation.
- Odermatt et al. controlled for this by adding unimodal visual-only and haptic-only conditions.
- Fifty healthy participants performed a decision-making task and a motor task in immersive VR.
- Participants saw a first-person virtual hand and received congruent, incongruent, visual-only, or haptic-only information.
- Congruent/unimodal conditions led to faster reaction times and completion times than incongruent conditions, especially compared with incongruent haptic information.
- Incongruent information slowed participants down.
- Improved speed did not come at the cost of reduced accuracy.
- Body ownership was high across conditions, likely due to first-person immersive VR, realistic limb appearance/posture, and connected virtual limb.
- Body ownership was higher after the motor task than after the decision task, likely due to visuomotor synchrony.
- Subjective body ownership was weakly associated with faster reaction times.
- Body ownership/agency correlations with motor performance were fragile and partly influenced by an outlier.
- GSR threat response did not significantly differ between conditions and did not correlate with subjective body ownership.
- The authors caution that body ownership questionnaires must be selected carefully because some items may actually reflect location or congruency effects.
- The main conclusion is that congruency of information may enhance motor performance more clearly than body ownership alone.

## Relation to thesis concepts

### Congruency

Very high relevance. This paper is one of the cleanest sources for saying that congruent information in immersive VR motor tasks can improve reaction/completion times, and that incongruence can slow users down.

For the thesis, it supports separating:
- spatial congruence,
- temporal congruence,
- visuomotor congruence,
- haptic/proprioceptive congruence,
- action-outcome congruence,
- sport-action congruence.

### Body ownership

High relevance, but as a caution. The paper shows that body ownership may be associated with faster reaction times, but its independent effect on motor performance is not straightforward. Body ownership can be high in first-person VR even when visuo-tactile congruency is not manipulated strongly.

### Agency

High relevance. Agency items were included, and agency was associated with performance in congruent/unimodal conditions in some analyses. For XR rowing, agency is likely the most important embodiment component because the user continuously causes avatar/boat movement through rowing.

### Self-location / location

High relevance. The questionnaire separates body ownership and location. This is useful for your evaluation because an erg-centered mode may support hand/body location more strongly than a boat-centered offset mapping.

### Visuomotor congruence

Very high relevance. The paper supports the idea that synchrony and congruent movement feedback matter for embodied VR motor tasks. In XR rowing, visuomotor congruence is central to the erg-centered mode.

### Visuotactile congruence

High relevance. The study manipulates visuo-tactile congruency directly. In rowing, the real handle/touch and visible virtual handle/hand contact may create a visuotactile congruence problem if the virtual hands or oars visually diverge from the felt handle.

### Haptic / proprioceptive congruence

High relevance. The incongruent haptic condition was especially slow. This is useful for rowing because the felt physical action on the erg is a strong cue. If virtual oar motion competes with felt handle motion, users may hesitate or move less efficiently.

### Motor performance

High relevance. The paper directly links congruent information to reaction and completion time. It does not prove rowing performance effects, but it supports a careful interpretation if one rowing condition produces faster pace/strokes or lower hesitation.

### Offset oar-arm IK

Very relevant. The paper helps warn that offset virtual oar arms are not just a visual design choice. If the offset creates competing information, it may slow performance or reduce clarity. If the offset is temporally coherent and sport-legible, it may be acceptable, but this must be evaluated.

### Tool-mediated action

Relevant when paired with Di Pino et al. Di Pino suggests humans can adapt to tool-mediated mappings. Odermatt warns that congruency still matters and competing sensory information can impair performance. Together they are a very good pair:
- Di Pino = plasticity/adaptation plausibility.
- Odermatt = congruency/mismatch caution.

### Presence / cybersickness / latency

Relevant as background. The paper notes that HMD display lag and multisensory conflicts can affect cybersickness and presence. Use Waltemate for latency more directly, but this paper reinforces the broader idea that multisensory mismatch matters.

### Questionnaire design

High relevance. The paper’s questionnaire tables are useful because they separate body ownership, location, agency, disownership, and control items. They also caution that some questionnaire items used as body ownership items may actually reflect location or visuotactile congruency.

## How it maps to my thesis modes

### Erg-centered mode

This paper strongly supports the erg-centered mode’s rationale.

The erg-centered mode is designed to reduce competing information:
- real handle and virtual handle match,
- real hand trajectory and virtual hand trajectory match,
- real seat motion and virtual body motion match,
- felt grip/force and seen hand/handle contact match,
- the user does not need to mentally reinterpret what their hands are doing.

Odermatt et al. support the idea that this kind of congruent information may improve motor-task speed and reduce hesitation. In thesis language, this mode may produce stronger action clarity and agency because the user has to question the mapping less.

### Boat-centered mode

This paper also helps analyze the boat-centered mode, but mostly as a caution.

The boat-centered mode may increase sport-action realism by showing on-water rowing with oars, oarlocks, blades, feathering/squaring, and boat movement. However, if the real erg handle and virtual oar/hand motion diverge too much, the user may receive competing information:
- felt handle path vs visible oar path,
- real finish/release timing vs animated oar release,
- real resistance vs visible blade/water force,
- real central handle vs visually separate oars.

This does not mean the boat-centered mode is bad. It means the design must make the mismatch coherent as tool-mediated rowing action rather than confusing as body-motion error.

### Core tradeoff

Odermatt et al. are central for the core tradeoff because they show that congruency of information can affect motor performance independently of body ownership.

The thesis should therefore avoid framing the comparison as:
- more embodiment vs less embodiment,
- more realism vs less realism.

Better framing:
- Which representation provides the more coherent sensorimotor/action information?
- Does precise erg congruence improve agency and task clarity?
- Does boat-centered sport realism compensate for reduced direct hand/handle congruence?
- Are users slowed down by competing information in the boat-centered condition?
- Are performance or questionnaire differences better explained by congruency, agency, ownership, or sport-action plausibility?

## What not to overclaim

- Do not claim this paper proves body ownership improves motor performance.
- Do not claim this paper proves body ownership is irrelevant.
- Do not claim this paper proves erg-centered rowing will perform better.
- Do not claim this paper proves boat-centered rowing will perform worse.
- Do not claim all incongruence is harmful; the study is specific to virtual hand/finger tasks.
- Do not generalize directly from hand/finger brushing tasks to rowing without caution.
- Do not claim GSR is a reliable objective body ownership measure in every context; this study did not find GSR differences or correlations.
- Do not collapse ownership, agency, self-location, and congruency.
- Do not treat questionnaire items as interchangeable; some “ownership” items may actually reflect location or congruency.
- Do not ignore skill level: the paper suggests embodiment-performance effects may depend on task difficulty or participant skill.

## Thesis-use priority

High priority for:
- congruency vs body ownership,
- evaluation interpretation,
- motor performance in immersive VR,
- offset oar IK caution,
- erg-centered vs boat-centered comparison,
- questionnaire design and subscales,
- avoiding overclaiming embodiment as a magic performance variable.

Medium priority for:
- VR rehabilitation/training,
- body ownership measurement,
- GSR/threat-response limitations,
- agency-performance relationship,
- latency/multisensory conflict background.

Low priority for:
- rowing biomechanics,
- vection,
- sport-specific related work,
- tool plasticity alone.

Suggested placement:
- Theoretical background: congruence and embodiment.
- Evaluation methods: questionnaire/item selection.
- Discussion: interpreting performance/agency differences.
- System/design rationale: why erg-centered direct mapping may reduce cognitive hesitation.
- Boat-centered limitations: offset oar-arm IK may introduce competing information.

## Candidate thesis paragraph

Odermatt et al. show why embodiment effects in VR motor tasks should be interpreted carefully. Their study separated body ownership from the congruency of task-relevant information by comparing congruent, incongruent, and unimodal sensory conditions during immersive VR hand tasks. They found that incongruent information slowed reaction and completion times, while body ownership was high across conditions and its independent benefit for motor performance remained less clear. For the present XR rowing thesis, this distinction is important because the erg-centered mode and boat-centered mode differ not only in visual realism, but also in how congruent the real and virtual action information is. If users move faster or feel more in control in the erg-centered condition, this may reflect reduced competition between felt handle motion and seen avatar motion rather than body ownership alone.

## Candidate short thesis sentence

Odermatt et al. suggest that congruent multisensory information, rather than body ownership alone, can improve reaction and completion times in immersive VR motor tasks.

## Candidate footnote

A useful caution comes from Odermatt et al., who found that incongruent visual-haptic information slowed VR motor-task performance, while body ownership remained high across conditions. This suggests that performance differences in embodied VR may reflect congruency of task-relevant information rather than body ownership alone.

## Candidate glossary wording

### Congruency of information

Congruency of information means that the sensory and task-relevant cues available to the user do not compete with one another. In VR motor tasks, this can include alignment between what the user sees, feels, and does. Odermatt et al. show that incongruent information can slow reaction and completion times even when body ownership over the virtual limb is high.

### Competing information

Competing information occurs when different cues suggest different actions or body states. In XR rowing, this could happen if the user feels a central erg handle moving along one path while seeing virtual oar handles or arms moving along another. The user may still understand the sport depiction, but the mismatch can reduce action clarity or slow motor response if it is not made coherent.

### Ownership versus congruency

Body ownership is the feeling that a virtual body or body part is mine. Congruency is the match between visual, tactile, proprioceptive, and task-relevant information. These should be separated because a virtual body can feel owned while still presenting incongruent information that affects task performance.

## Codex / agent note

Use this paper as a high-priority source for the thesis’s congruency argument. It is especially important for interpreting performance or agency differences between erg-centered and boat-centered modes.

Core agent memory:
- Odermatt et al. distinguish body ownership from congruency of information.
- Incongruent information slowed reaction and completion times in immersive VR tasks.
- Body ownership was high across conditions, likely due to first-person immersive avatar presentation and visuomotor synchrony.
- Therefore, do not interpret performance differences as “body ownership effects” without considering congruency.
- For XR rowing, the erg-centered mode may work better because it reduces competing information, not simply because it is more embodied.
- The boat-centered mode may still work if the virtual oar mapping is coherent as tool-mediated action, but offset IK is a risk point.

Suggested use:
- theory section on congruence,
- evaluation interpretation,
- discussion of offset oar-arm IK,
- questionnaire/methods caution.

Do not use this paper:
- as rowing evidence,
- as proof that body ownership does not matter,
- as proof that erg-centered mode is superior,
- as proof that virtual oars are invalid.
