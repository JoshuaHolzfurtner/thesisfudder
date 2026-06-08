# First pitch — Thesis literature map and source coverage

## Working thesis topic

This thesis investigates how XR rowing can support sense of embodiment through the subcomponents of self-location, agency, and body ownership. The core comparison is between two virtual rowing representation modes:

1. **Erg-centered / high-congruence mode**
   - The user rows on a real ergometer.
   - Real handle, seat, and body motion are mapped as closely as possible to the avatar.
   - This mode prioritizes visuomotor congruence, spatial alignment, temporal congruence, haptic/proprioceptive consistency, and agency.

2. **Boat-centered / sport-depiction mode**
   - The user still rows on a real ergometer.
   - The virtual avatar appears to row in a boat with oars, oarlocks, blades, and on-water rowing movement.
   - This mode prioritizes sport-action realism and rowing-specific depiction.
   - It introduces mismatch because the virtual oar/hand path cannot perfectly match the real ergometer handle trajectory.

The central question is whether embodiment in XR rowing is better supported by precise movement correspondence or by a more realistic rowing representation.

Working core question:

> How do spatial alignment, temporal congruence, and avatar realism influence embodiment in XR rowing, particularly when comparing a precisely mapped erg-centered avatar with a more sport-realistic but less movement-congruent boat-centered representation?

---

## Main source-health verdict

The current source base is strong enough to write from. The main risk is not lack of sources, but scope creep.

### Strongly covered

- Sense of embodiment / body ownership / agency / self-location.
- Rubber Hand Illusion and moving rubber-hand style paradigms.
- VR embodiment and virtual body ownership.
- Temporal congruence / latency.
- Threat or impact probes as auxiliary embodiment indicators.
- Presence, place illusion, plausibility illusion, and response-as-if-real.
- Rowing stroke vocabulary and ergometer vs on-water rowing caveats.
- Prior VR rowing / rowing simulator projects.

### Slightly light / should be tightened

- Exact questionnaire choice and operational definitions.
- Spatial alignment as an embodiment-relevant variable, not only as a technical alignment problem.
- Statistical and methodological justification for a small within-subject study.
- One clean XR/VR definitions source.
- One clean authoritative rowing-basics source for catch, drive, finish, recovery, feathering/squaring, and erg/on-water wording.

### Not a real priority

- Avatar morphology / realism as a direct independent variable, because the planned comparison does not evaluate cartoon vs realistic avatar appearance.
- Motor-learning feedback papers, unless training feedback becomes part of the evaluated system.
- More VR rowing performance/fitness papers, unless they are used only in an appendix or related-work table.

### Overloaded

- VR rowing project examples.
- Rowing feedback / form-analysis / rowing simulator papers.
- General exergame / VR sport performance literature.

---

# Chapter-by-chapter literature map

## 1. Introduction

### Purpose of this chapter

Introduce VR indoor rowing as a case where realistic sport depiction and visuomotor congruence can conflict.

The opening problem:

- Indoor rowing is physically ergometer-based.
- Rowing as a sport is visually and culturally boat/oar-based.
- XR embodiment depends on coherent body/action feedback.
- Therefore, XR rowing creates a meaningful design conflict:
  - Should the system prioritize the real ergometer and body?
  - Or should it prioritize the visual logic of on-water rowing?

### Source coverage

This chapter is well covered. Use only a few load-bearing citations.

Recommended citation roles:

- **Kilteni et al. 2012**: sense of embodiment framing.
- **Slater 2009**: place illusion / plausibility illusion distinction.
- **Waltemate et al. 2016**: temporal congruence / latency / agency / ownership relevance.
- **Lamb 1989 or another rowing biomechanics source**: ergometer vs on-water movement is not identical.
- **Murray 2016 or Arndt 2018**: prior VR rowing systems exist, but mostly targeted motivation/performance/feedback rather than embodiment tradeoffs.
- **Witte et al. 2025**: modern VR sport review and visual-perception/transfer caution.

### Caution

Do not overload the introduction with every VR rowing paper. One or two examples are enough.

Possible thesis positioning sentence:

> Prior virtual rowing systems have explored motivation, performance, pacing, feedback, and social rowing, but the specific embodiment tradeoff between physically congruent ergometer mapping and sport-faithful oar/boat depiction remains underexplored.

---

## 2. Theoretical Background / Related Work

## 2.1 Sense of embodiment

### Strongly covered

Core sources:

- **Kilteni, Groten & Slater 2012** — core sense of embodiment structure.
- **Mottelson et al. 2023** — systematic review / meta-analysis of VR body-ownership studies.
- **Girondini et al. 2025** — systematic review of body ownership and agency in VR.
- **Ionta et al. 2011** — multisensory and sensorimotor foundations of self-location and bodily self-consciousness.

Use these to define:

- body ownership,
- agency,
- self-location,
- sense of embodiment,
- multisensory integration,
- bodily self-consciousness.

### Thesis role

This is the theoretical core. It should remain cleaner and less polluted by rowing-project papers.

---

## 2.2 Rubber Hand Illusion and moving rubber-hand paradigms

### Strongly covered

Core sources:

- **Botvinick & Cohen 1998** — classic Rubber Hand Illusion.
- **Kalckert & Ehrsson 2012** — moving rubber hand; dissociation of ownership and agency.
- **Kalckert & Ehrsson 2017** — onset time / timing of ownership emergence.

### Thesis role

Use this section to explain why embodiment can be experimentally manipulated by synchrony, movement, and multisensory congruence.

For the thesis:

- Erg-centered mode resembles a high-congruence visuomotor mapping.
- Boat-centered mode may preserve sport-action plausibility but introduces mapping mismatch.
- Ownership and agency should not be assumed to move together.

---

## 2.3 Visuomotor and temporal congruence

### Strongly covered

Core source:

- **Waltemate et al. 2016** — latency in full-body VR affects motor performance, simultaneity perception, agency, and body ownership.

Supporting sources:

- **Kalckert & Ehrsson 2012 / 2017**.
- **Brugada-Ramentol et al. 2019** if active control / virtual hand ownership is needed.
- **Seinfeld & Müller 2020** for detached virtual hands and visuomotor feedback.

### Thesis role

This section supports the engineering argument that latency and movement mapping are not only technical issues. They may directly affect embodiment.

Important thesis logic:

> The boat-centered mode may have low technical latency, but still feel less temporally or actionally coherent if the user’s motor intention does not match the visible avatar/oar movement.

This is not the same as system latency, but it may be experienced similarly as reduced action-response coherence.

---

## 2.4 Spatial alignment and visuoproprioceptive congruence

### Current coverage

Slightly light.

Relevant existing sources:

- **Ionta et al. 2011** — self-location / multisensory bodily self-consciousness.
- **RHI / moving RHI sources** — likely useful for spatial congruence and real/virtual body-location mismatch.
- **Mottelson / Girondini reviews** — likely contain spatial congruence and visuoproprioceptive congruence material.
- **Martin-Gomez et al. 2020** — MR alignment difficulty and egocentric depth ambiguity.
- **Martin-Gomez et al. 2019** — alignment visualization techniques for precise object alignment.

### Thesis-specific alignment context

The project has a custom alignment method:

- hand-tracking based,
- approximately 3-second setup,
- intended to reach image-marker-like accuracy for ergometer/world alignment,
- used to align the real ergometer, virtual ergometer/boat scene, avatar, handle, and interaction space.

This is a system USP, but probably not the theoretical heart of the thesis.

### Suggested treatment

Use alignment in two layers:

1. **Technical system layer**
   - Describe the custom method.
   - Explain why fast and accurate erg/world alignment is needed.
   - Mention only briefly that MR/XR alignment is a known challenge.

2. **Embodiment layer**
   - Explain that poor spatial alignment could weaken visuoproprioceptive congruence, because the seen body/handle/erg would no longer match the felt body/handle/erg.
   - Do not overclaim that the alignment method itself proves stronger embodiment unless directly measured.

### Gap status

Light but manageable. Probably no major new paper needed unless the alignment method becomes a central evaluation variable.

Possible source need:

- One direct body-illusion / spatial discrepancy source, if existing core reviews do not provide a clean quote.
- Otherwise keep it concise.

---

## 2.5 Avatar morphology / realism

### Current coverage

Moderate, but not urgent.

Relevant sources:

- **Kocur et al. 2025** — customized avatars / Proteus effect in VR exercise.
- **Lok et al. 2002** — real objects / self-avatar fidelity in virtual environments.
- **Mottelson / Girondini** — broad avatar embodiment factors.
- **Slater 2009** — plausibility and virtual body.

### Thesis decision

This is not a main comparison if avatar appearance is held constant between conditions.

Do not create a large morphology section unless the thesis actually manipulates avatar appearance.

Suggested treatment:

- Mention avatar realism/morphology as a design factor and limitation.
- Keep the evaluation focus on mapping/congruence, not avatar aesthetics.
- If body proportions are matched, describe this as a control/quality measure.

### Gap status

Not urgent.

---

## 2.6 Presence, place illusion, plausibility illusion

### Strongly covered

Core sources:

- **Slater 2009** — place illusion, plausibility illusion, response-as-if-real.
- **Skarbez et al. 2017** — survey of presence and related concepts.

### Thesis role

This section is useful because the thesis must not collapse all experience terms into one fuzzy “immersion” concept.

Important distinction:

- **Place illusion**: feeling located in the virtual rowing environment.
- **Plausibility illusion**: feeling that the events are actually happening in relation to the user.
- **Embodiment**: feeling that the virtual body/action is self-related.
- **Sport-action plausibility**: rowing looks like rowing.
- **Device congruence**: virtual motion matches the real ergometer.

Use Slater to explain why boat-centered mode may support rowing-scene plausibility even if it weakens device/body congruence.

---

## 2.7 Vection / optic flow

### Current status

Covered enough for optional explainer / future work.

Use only briefly unless the thesis measures vection.

Potential role:

- Explain that moving river/shore/boat visuals can contribute to subjective self-motion.
- Do not make vection a core dependent variable unless measured.

### Gap status

No urgent source work needed.

---

## 2.8 Threat / impact response

### Covered

Core source:

- **Ma & Hommel 2013** — virtual hand impact/threat, affective resonance, ownership caution.

Optional backup:

- **Zhang & Hommel 2016** — threat/anxiety/morphology, but not necessary.

### Thesis role

Use only if the study includes an optional mild threat/impact probe.

Main caution:

- A mild impact may be more ownership-sensitive.
- A severe/gory threat may trigger generic defensive response and be less diagnostic.
- Threat response should be auxiliary, not the main ownership measure.

---

## 2.9 VR sports and rowing applications

### Strongly covered / overloaded

Core related-work examples:

- **Murray et al. 2016** — projected VR rowing, companion avatar, distance/power/enjoyment.
- **Arndt et al. 2018** — HMD rowing prototype, modest performance/experience metrics.
- **Hoffmann et al. 2013** — screen-based virtual rowing pacing / Zwift-like.
- **Parton & Neumann** — challenge level / virtual competitor in VR rowing.
- **Voskeuil et al. 2025** — embodied coxswain and social presence in VR rowing.
- **Vogel / Westra / Twente works** — VR rowing technique/feedback lineage.
- **SPRINT / Ruffaldi / Filippeschi / Rauter / Basalp / Sigrist** — high-end rowing simulators, CAVE/robotic oar/haptic/feedback lineage.

### Suggested format

Do not write a long narrative for every system. Use a table.

Suggested columns:

| Work | Setup | Input/device | Focus | Relation to this thesis |
|---|---|---|---|---|
| Murray et al. | Projected VR | Concept2 | companion/performance | prior VR rowing, not embodiment |
| Arndt et al. | HMD | Augletics | experience/performance | HMD rowing prototype |
| Hoffmann et al. | Screen-based virtual rowing | Concept2 | pacing | Zwift-like energy-management feedback |
| Voskeuil et al. | HMD / two RP3s | co-located or networked rowers | embodied coxswain/social presence | social rowing future work |
| SPRINT/Rauter/Sigrist | CAVE/robotic oar | boat/oar simulator | technique/feedback | full rowing simulator contrast |
| This thesis | XR/HMD | erg + avatar mapping | embodiment/congruence | core contribution |

### Main message

Prior systems mostly target:

- motivation,
- pacing,
- technique feedback,
- social rowing,
- motor learning,
- simulator fidelity.

This thesis instead targets:

- embodiment,
- agency,
- ownership,
- self-location,
- mapping tradeoff between erg congruence and boat/oar depiction.

---

# 3. System / Prototype

## 3.1 Hardware/software stack

### Source needs

Mostly implementation documentation, not theory papers.

Useful source types:

- Unity XR / OpenXR docs.
- Unity XR Hands docs.
- OpenXR specification or Khronos landing page.
- Platform docs if needed.
- Internal prototype description.

### Gap status

Fine. Use technical docs in appendix/system section, not as theory.

---

## 3.2 Rowing stroke basics

### Current status

Need one clean authoritative rowing-basics source.

Existing sources help, but they are either:

- too sports-science,
- too preview-like,
- too historical,
- too simulator-specific.

Useful target:

- World Rowing / FISA coaching handbook,
- Rowing Australia / British Rowing / USRowing coaching manual,
- a clean rowing textbook chapter,
- Nolte / Rowing Faster if accessible,
- Complete Guide to Indoor Rowing if you want erg-specific wording.

Need definitions for:

- catch,
- drive,
- finish,
- recovery,
- feathering,
- squaring,
- oarlock/blade basics,
- ergometer vs boat caveat.

### Suggested treatment

Keep rowing basics concise. The thesis is XR/embodiment, not rowing biomechanics.

---

## 3.3 Erg-centered mode

### Supported by

- embodiment/congruence papers,
- latency papers,
- rowing stroke basics,
- your implementation.

### Key wording

This mode prioritizes:

- visuomotor congruence,
- temporal congruence,
- haptic/proprioceptive consistency,
- real/virtual handle alignment,
- agency over the avatar movement.

---

## 3.4 Boat-centered mode

### Supported by

- rowing basics,
- erg vs on-water distinction,
- rowing simulator papers as contrast.

### Key wording

This mode prioritizes:

- sport-action congruence,
- rowing-specific depiction,
- oars/oarlocks/blades/boat movement,
- plausibility as “rowing.”

It sacrifices:

- exact real handle trajectory matching,
- potentially some visuoproprioceptive congruence,
- potentially some agency if mapping feels indirect.

---

## 3.5 Alignment method

### Current special note

This is a custom USP.

Describe it clearly:

- What is aligned?
- What does the user do?
- How long does it take?
- What sensors are used?
- How accuracy is estimated or qualitatively validated?
- What happens if alignment is wrong?
- How it differs from marker/image-target based alignment?

### Source need

Only light citation needed.

Possible citation roles:

- MR/XR alignment is difficult due to egocentric depth ambiguity.
- Alignment aids and multi-view helpers exist.
- Your method solves a practical version for ergometer alignment.

Do not overdo it.

---

# 4. Study Design / Method

## 4.1 Questionnaire choice

### Current status

This is now much better because of the VEQ.

Core questionnaire source:

- **Roth & Latoschik 2020 — Virtual Embodiment Questionnaire (VEQ).**

The VEQ measures:

- **Acceptance / Body Ownership**
- **Control / Agency**
- **Change / perceived body schema change**

This maps well to the thesis because ownership and agency are central constructs.

### Suggested use

Primary questionnaire:

- VEQ Acceptance = body ownership.
- VEQ Control = agency.
- VEQ Change = optional; maybe not core unless avatar body-change feeling matters.

Add custom/exploratory items for:

- sport-action realism,
- rowing realism,
- perceived handle/avatar alignment,
- preference,
- discomfort/cybersickness if needed,
- presence/place/plausibility if not using a separate presence scale.

### Important caveat

VEQ does not directly solve self-location unless the scale or source includes relevant items elsewhere. If self-location is a major subcomponent, either:

- add a small self-location item set from embodiment literature, or
- state that this thesis primarily operationalizes ownership and agency, while self-location is discussed theoretically or measured with a simple exploratory item.

### Candidate construct table

| Construct | Primary measure | Status |
|---|---|---|
| Body ownership | VEQ Acceptance | Strong |
| Agency | VEQ Control | Strong |
| Body schema change | VEQ Change | Optional |
| Self-location | needs item/source or exploratory item | Slightly light |
| Presence/place | optional presence/plausibility items | Optional |
| Sport realism | custom Likert items | Exploratory |
| Mapping realism/congruence | custom Likert items | Exploratory |
| Preference | forced choice + comment | Exploratory |
| Threat response | mild impact reaction/HR if used | Auxiliary only |

---

## 4.2 Experimental design

### Likely design

Within-subjects / repeated-measures design:

- Each participant tries both modes.
- Order is counterbalanced/randomized.
- The main comparison is within participant.

This is a good design because embodiment ratings are subjective and likely vary strongly between users.

### Need to tighten

- exact order counterbalancing,
- familiarization time,
- rest time,
- whether threat probe appears after both conditions,
- whether the boat-centered condition always comes with the same scenery and avatar as the erg-centered mode,
- what is held constant between conditions.

### Source support

Use:

- VEQ source for measurement.
- Kalckert & Ehrsson 2017 for exposure/familiarization logic.
- Waltemate 2016 for latency/temporal congruence concerns.
- Stats source for repeated-measures / within-subject analysis.

---

## 4.3 Small-N / statistics

### Current status

Not fully solved by literature stack.

You may have a repeated-measures ANOVA tutorial/source, but the actual plan should be methodologically conservative.

Possible analysis plan:

- If two conditions only:
  - paired t-test if assumptions acceptable,
  - Wilcoxon signed-rank if non-normal / small N,
  - report effect sizes and confidence intervals.
- If multiple dependent variables:
  - repeated-measures ANOVA or nonparametric alternatives,
  - avoid overclaiming if underpowered.
- Treat qualitative comments and preference ratings as exploratory.

### Important thesis honesty

For a student thesis prototype, small N is not fatal if you do not overclaim.

Use wording like:

> The study is exploratory and prototype-oriented. The analysis focuses on within-subject differences, effect directions, and construct-specific patterns rather than broad population claims.

---

# 5. Results

No source gap. This chapter depends on collected data.

Pre-plan interpretation categories:

1. Erg-centered higher ownership/agency:
   - supports precise visuomotor/device congruence.

2. Boat-centered higher realism/preference but lower ownership/agency:
   - supports distinction between sport realism and embodiment.

3. Boat-centered equal or higher embodiment:
   - sport-action plausibility may compensate for mapping mismatch.

4. Null effects:
   - possible insufficient sensitivity, strong baseline embodiment in both modes, prototype limitations, small sample, short exposure, or users prioritizing different cues.

---

# 6. Discussion

## Main discussion structure

1. What did the study show about the core tradeoff?
2. Did ownership and agency move together or diverge?
3. Did sport realism differ from embodiment?
4. Did alignment and latency seem adequate?
5. What does this mean for XR rowing design?
6. What are limitations?
7. What should future systems evaluate?

### Source support

- **Kilteni / RHI / Kalckert** for embodiment interpretation.
- **Waltemate** for temporal congruence and motor performance / agency / ownership.
- **Slater** for plausibility vs place vs embodiment.
- **Witte** for VR sport transfer/visual perception caution.
- **Rowing sources** for erg/on-water mismatch.
- **Ma & Hommel** only if threat probe is used.

---

# 7. Conclusion

No source gap.

Main contribution:

- XR rowing as a testbed for embodiment.
- Comparison between physically congruent erg-centered representation and sport-faithful boat-centered representation.
- Practical implications for XR sport systems: “realism” is not one thing.

---

# Current missing / next-source priorities

## Priority A — operationalization

Most important next work:

- finalize VEQ usage,
- decide self-location measurement,
- decide presence/plausibility/realism items,
- decide statistical plan.

## Priority B — rowing basics

Find or choose one clean rowing basics source.

Goal:

- not deep sports science,
- just authoritative terminology and stroke phases.

## Priority C — XR glossary

One clean XR/VR definitions source.

Possible use:

- XR,
- VR,
- MR,
- HMD,
- tracking,
- avatar,
- IK,
- hand tracking.

## Priority D — spatial alignment

Only add one more paper if existing core embodiment papers do not provide a clean spatial congruence / visuoproprioceptive congruence sentence.

Otherwise, keep it mostly as system description.

---

# What to avoid

- Do not make the thesis about rowing technique training.
- Do not make it about feedback design.
- Do not make it about exergame performance improvement.
- Do not make it about social rowing unless only future work.
- Do not make it about avatar customization unless not evaluated.
- Do not claim the boat-centered mode is “more realistic” without specifying **sport-action realism** versus **bodily/device congruence**.

---

# Short Codex / agent note

This thesis source base is already sufficient for a strong embodiment-focused thesis. The core theory should be built from Kilteni, RHI/moving-RHI sources, Mottelson/Girondini, Waltemate, Slater, and Skarbez. Rowing and VR-rowing sources should mostly be used to define the application domain and related work, not to drive the argument. The main thesis contribution is not “VR rowing improves performance,” but “XR rowing exposes a design tradeoff between physically congruent ergometer embodiment and sport-faithful boat/oar depiction.”

The highest-priority remaining work is operational: define exact questionnaire items, self-location measurement, order counterbalancing, familiarization duration, and analysis plan. The alignment method is a system USP and should be described clearly, but it should not become a separate alignment thesis unless evaluated as an independent variable.
