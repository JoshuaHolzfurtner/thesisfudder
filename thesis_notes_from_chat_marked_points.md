# Thesis notes from chat — marked points / reminders to check later

This file collects the main “note to self”, optional/future-work, and thesis-checklist points that came up in this chat. It is not final thesis prose. Use it as a checklist when drafting, trimming, and reviewing.

---

# 1. Core thesis logic to preserve

## Main comparison

The thesis should stay centered on the comparison between:

- **Erg-centered / high-congruence mode**
  - Real ergometer handle, seat, and body motion are mapped as closely as possible to the avatar.
  - Prioritizes visuomotor congruence, haptic/proprioceptive consistency, temporal congruence, spatial alignment, and agency.

- **Boat-centered / sport-depiction mode**
  - User still rows on the ergometer.
  - Avatar appears to row in a boat with virtual oars, oarlocks, blades, and on-water rowing depiction.
  - Prioritizes sport-action realism and rowing-specific visual depiction, but introduces mismatch with the real ergometer handle path.

Core framing:

> XR rowing exposes a conflict between two forms of realism: embodied action congruence and sport-depiction realism.

Do not let the thesis become generic “VR rowing is immersive.” The sharp thesis distinction is:

> Is embodiment in XR rowing better supported by precise movement correspondence with the real ergometer, or by a more realistic visual/sport depiction of rowing on water?

## Key claim shape

Use the literature to sharpen the comparison, not to expand the thesis.

Everything should answer:

> Does this source, section, or system detail clarify the tradeoff between embodied action congruence and sport-depiction realism?

If yes: keep/compress.  
If no: footnote, appendix, or cut.

---

# 2. Things not to overclaim

Avoid these claims unless directly measured:

- Do not claim the prototype teaches rowing technique.
- Do not claim boat-centered mode simulates real rowing physics.
- Do not claim full on-water transfer.
- Do not claim virtual oars become body parts.
- Do not claim presence equals embodiment.
- Do not claim “more realism” without specifying which realism.
- Do not claim alignment accuracy as scientific evidence unless measured.
- Do not claim physiological threat response proves ownership by itself.
- Do not claim a small-N thesis study establishes general user preference.
- Do not claim physical exertion changes embodiment susceptibility as established fact unless sourced/measured.
- Do not claim Change/body-schema transformation is central unless measured and theoretically framed.

Safe limitation phrasing:

- “may support”
- “may influence”
- “can be interpreted as”
- “exploratory”
- “suggests”
- “in this setup”
- “participants reported”
- “this does not establish transfer/training effects”

---

# 3. System contribution notes

## What the thesis brings to the table

The main contribution is not a new theory of embodiment. The contribution is:

- a custom XR rowing prototype,
- a fast real–virtual erg/world alignment method,
- two full-body IK/action mappings,
- a physically grounded haptic/action anchor through the real ergometer,
- and an evaluation comparing two competing embodiment strategies.

## Alignment note

The alignment method is a USP internally, but the thesis is not mainly about alignment.

Use alignment as enabling infrastructure:

> Accurate and fast alignment is required to make the embodiment comparison meaningful.

Safe argument:

> Without real–virtual alignment, mismatches between the real handle/seat/body and the virtual avatar/environment would contaminate the comparison by undermining visuoproprioceptive and visuotactile congruence.

Do not over-expand alignment into a separate thesis unless measured.

## Constant identical physical simulation

Important methods point:

Both conditions share:

- same real rower,
- same real ergometer,
- same real handle and seat,
- same real physical effort,
- same basic exercise task.

This is scientifically useful because differences between conditions can be interpreted primarily as effects of the virtual body/action representation layer rather than changes in the physical exercise task.

Possible thesis wording:

> Because both conditions are grounded in the same physical ergometer interaction, differences between conditions can be interpreted primarily as effects of virtual body/action representation rather than differences in physical exercise task.

---

# 4. Haptic anchor / RHI bridge

## Handle as haptic anchor

The real ergometer handle is not just an input device. It is a persistent tactile/proprioceptive anchor.

In the erg-centered mode, the user:

- feels the real handle,
- sees the virtual hands/handle contact,
- moves the real handle,
- sees avatar movement coupled to it,
- feels real muscular effort and seat motion.

This creates a bridge to RHI-style multisensory binding, but through active movement and real sport interaction rather than passive brush stroking.

Safe phrasing:

> Like RHI-style paradigms, the system attempts to bind seen virtual body/action with felt physical input. In XR rowing, the handle becomes a persistent haptic anchor linking real and virtual action.

Do not say:

> “This is the Rubber Hand Illusion.”

Better:

> “This follows a related multisensory/visuomotor embodiment logic.”

## Boat mode haptic ambiguity

In boat-centered mode, the same real handle becomes more ambiguous:

- user feels a central erg handle,
- but sees virtual oar handles and boat action,
- sport depiction increases,
- device congruence decreases.

This is part of the core tradeoff.

---

# 5. Realism vocabulary to keep precise

## Realism is plural

Use the thesis to distinguish:

- visual realism,
- sport-action realism,
- biomechanical fidelity,
- haptic/force congruence,
- proprioceptive congruence,
- temporal congruence,
- visuomotor congruence,
- plausibility,
- presence,
- embodiment.

Key framing:

> The boat-centered mode may score higher on sport-action realism, while the erg-centered mode may score higher on embodied action congruence.

Avoid generic “more realistic” claims without specifying realism type.

## Harris / VR sport caution

Use the Harris-style caution:

> Visual realism does not automatically equal action realism.

This is important for your exact thesis: a visually realistic rowing boat can still be less congruent with the user’s real physical action than a visually less boat-like erg-centered setup.

---

# 6. Embodiment components and expected patterns

## Keep SoO and SoA separate

Do not collapse everything into one total embodiment score unless necessary. Your thesis is interesting exactly because subcomponents may diverge.

Possible outcomes:

- Erg mode higher agency but not ownership.
- Boat mode higher sport realism/preference but lower agency.
- Boat mode higher plausibility but not ownership.
- Both modes similar because shared physical exertion/handle/seat loop dominates.
- Participants prefer boat mode even if erg mode scores higher on agency.

## Strong possible results

Beautiful result:

> Participants rated the boat-centered mode as more rowing-realistic and visually plausible, but rated the erg-centered mode higher in agency and movement ownership.

Also strong:

> Participants preferred the boat-centered mode despite stronger agency in the erg-centered mode.

Even null result can be useful:

> Both representations produced comparable embodiment, suggesting that sport-action plausibility may compensate for some sensorimotor mismatch, or that the shared real haptic/erg anchor dominated both conditions.

---

# 7. Questionnaire / evaluation notes

## Main questionnaire plan

Primary:

- VEQ Ownership
- VEQ Agency

Possible secondary/exploratory:

- VEQ Change
- custom movement-match questions
- custom rowing realism questions
- preference
- presence/plausibility
- cybersickness/discomfort
- optional threat or offset probe

## VEQ notes

VEQ is useful because it is data-driven and validated around three factors:

- Ownership
- Agency
- Change

Use VEQ to avoid inventing a fully ad-hoc scale. It gives comparable, recognized measurement vocabulary.

Change is real in VEQ, but for this thesis likely secondary/exploratory unless avatar body transformation/body-schema change becomes central.

## Gonzalez-Franco & Peck questionnaire notes

Useful as a standardized/avatar embodiment questionnaire proposal and as source for situation-specific items.

It is not fully validated per se; it is based on items that were prevalent and significant in prior studies. Frame it as backwards-compatible and useful for comparability, not as a fully psychometrically validated gold standard.

Important categories:

- Body ownership
- Agency and motor control
- Tactile sensations
- Location of the body
- External appearance
- Response to external stimuli

Use/adapt selected items, not necessarily all 25.

## Candidate custom rowing-specific items

Potential extra items:

- “The virtual rowing movement felt like my own movement.”
- “The virtual handle/oars felt connected to my real action.”
- “The rowing representation felt realistic as rowing.”
- “The virtual movement matched what I physically felt.”
- “I preferred this rowing representation.”
- “The virtual boat/world movement felt connected to my own rowing effort.”
- “Did anything about the motion feel uncomfortable, artificial, or disconnected?”

## Direct quote candidate

From Gonzalez-Franco & Peck:

> “However, despite the growing usage of self-avatar embodiment among the VR community, and the prevalence of questionnaires to measure perceived embodiment, there is not yet a standardized embodiment questionnaire.”

Use only if motivating questionnaire standardization.

## Measurement logic

Reason for using established questionnaires:

> They make results more comparable to prior VR embodiment studies and avoid building an ad-hoc scale without psychometric grounding.

## Order of measures

Recommended order after each condition:

1. VEQ / main embodiment questions
2. realism / plausibility / preference-related items
3. cybersickness/discomfort if relevant
4. optional exploratory probe after main measures only

Do not place offset/threat before VEQ because it can contaminate the embodiment ratings.

---

# 8. Within-subjects / between-subjects note

Likely design:

> Within-subjects / repeated-measures: every participant tests both the erg-centered and boat-centered condition.

Why:

- fewer participants needed,
- each participant acts as their own control,
- controls for individual VR susceptibility,
- controls for rowing familiarity differences,
- controls for general embodiment tendency.

Need to handle:

- order effects,
- learning effects,
- fatigue effects,
- carryover effects,
- questionnaire awareness after first condition.

Design safeguards:

- counterbalance condition order,
- same duration per condition,
- rest between conditions,
- same questionnaire after each condition,
- preference comparison at the end.

Possible thesis wording:

> A within-subjects design was chosen because the study compares two alternative representations of the same physical rowing action. This allows each participant to serve as their own control, reducing variability caused by individual differences in VR experience, rowing familiarity, and general susceptibility to embodiment illusions. To reduce order and carryover effects, condition order was counterbalanced and participants received a short rest between conditions.

Mottelson can support that within-participant designs are common in BOI research, but no big source hunt needed.

---

# 9. Ethics / consent notes

## Minimum ethics handling

Use a proper participation-information + consent setup, not just informal “AGB.”

Include:

- what participants will do,
- VR headset use,
- rowing on ergometer,
- two virtual variants,
- questionnaire,
- approximate duration,
- possible physical exertion,
- possible VR sickness/dizziness,
- voluntary participation,
- right to stop at any time without reason,
- anonymized/pseudonymized data use,
- data storage/access,
- photo/video consent only if recorded.

## Health/safety check

Ask/warn about:

- acute injuries,
- cardiovascular concerns if exertion is non-trivial,
- strong VR/motion sickness susceptibility,
- epilepsy/seizure warning,
- dizziness/balance issues,
- pain/discomfort during rowing.

Stop criteria:

- dizziness,
- nausea,
- pain,
- distress,
- unsafe movement,
- participant request.

## When ethics gets more serious

Ask supervisor/department if formal approval is needed if using:

- heart-rate data,
- physiological measures,
- threat/hammer scene,
- hidden hand-offset manipulation,
- deception/detection task,
- meaningful physical exertion.

Main study should be boring-safe if possible:

- consent,
- health check,
- VEQ/questionnaire,
- anonymized data,
- rest/stop criteria.

---

# 10. Threat / hammer / physiological probe notes

## Threat response

Threat or impact can be an auxiliary embodiment indicator, but it is not proof of ownership by itself.

If used:

- keep it mild,
- do it after main questionnaires,
- debrief,
- avoid harsh threats.

Potential issue:

A very harsh threat like chopping/cutting a virtual body part may cause a general defensive reaction even without strong ownership. A rubber hammer/ball/mild impact is cleaner.

## Physiological measures

Common measures in embodiment literature include:

- heart rate,
- skin conductance,
- EEG.

For this thesis:

- heart rate can be exploratory,
- do not overinterpret,
- physical exercise confounds HR strongly.

Potential use:

- document that objective/physiological measures exist in the field,
- explain why questionnaire remains main measure,
- present HR only as exploratory if collected.

---

# 11. Offset / drift / hand-location probe ideas

## Post-condition hand-location probe

Idea:

After condition, briefly offset or reveal real/virtual hand positions and ask where the participant felt their hand was located.

Possible scale:

```text
1 = clearly at my real physical hand position
3 = somewhere between real and virtual hand
5 = clearly at the virtual/avatar hand position
```

Thesis-safe name:

- Exploratory proprioceptive-drift-style probe
- Hand-offset detection task
- Visuoproprioceptive offset tolerance probe

Use after VEQ, not before.

## Gradual unnoticed offset challenge

Idea:

Gradually increase spatial offset between physical hand/handle position and virtual hand position, and measure when the participant notices mismatch.

Academic framing:

> Gradually increase the spatial offset between the user’s physical hand/handle position and the virtual hand position, and measure the point at which the user notices the mismatch.

Possible dependent variable:

> Visuoproprioceptive mismatch tolerance threshold.

Why useful:

- directly tests how far virtual body mapping can drift before agency/ownership breaks,
- compares tolerance in erg vs boat mode,
- boat mode may tolerate more offset because users interpret virtual oars as tools,
- erg mode may require stricter 1:1 congruence.

Important:

- this is mild deception if not announced,
- needs debrief,
- should not contaminate main VEQ,
- likely future work / exploratory add-on unless very clean.

Possible in-app gamified version:

- “Virtual hand alignment challenge”
- reward coins,
- help research,
- but formal study still needs consent/debrief.

---

# 12. Physical exertion / embodiment novelty notes

## Exertive embodiment angle

Interesting field value:

> XR rowing combines self-avatar embodiment, sustained physical exertion, real haptic resistance, sport-specific action, full-body IK, and continuous locomotion consequence.

Most RHI/moving-RHI/virtual body setups are relatively passive or low-effort.

Your setup may be a rare case where embodiment is studied under:

- full-body rhythmic exertion,
- real resistance,
- persistent haptic grip,
- sliding seat motion,
- first-person avatar embodiment,
- repeated sport action,
- continuous action outcome.

Safe framing:

> While virtual embodiment has often been studied with relatively constrained or low-effort movements, XR rowing offers a physically demanding case in which embodiment cues are coupled to sustained rhythmic exertion, real haptic resistance, and continuous action outcomes.

Do not claim exertion increases suggestibility unless measured.

## Possible mechanisms to mention cautiously

Physical exertion may modulate embodiment by changing:

- bodily attention,
- interoceptive state,
- effort perception,
- physiological arousal,
- action-outcome salience,
- analytic checking of small mismatches,
- agency reinforcement.

Safe discussion wording:

> Physical exertion may have influenced how participants attended to congruence/mismatch, especially because the rowing action continuously couples effort, haptic feedback, avatar motion, and locomotion.

Future work:

> Future studies could explicitly manipulate exertion level to test whether physical effort modulates ownership, agency, and tolerance of visuomotor mismatch.

---

# 13. Cyborg / cybernetics notes

## Cybernetics explanation

Cybernetics studies control, feedback, communication, and regulation in systems across organisms, machines, and social systems.

Relevant loop for XR rowing:

```text
real rowing action
→ tracking / sensing
→ virtual avatar + boat response
→ visual / haptic / proprioceptive feedback
→ next rowing action
```

## Cyborg’s Dilemma

Use cautiously as conceptual side note:

- interfaces become more powerful/natural as they are incorporated into body/action schema,
- but incorporation also requires adapting to the machine’s logic.

Rowing machines themselves are already a tradeoff:

- on-water oar arcs and blade work are abstracted into a straight-line handle pull,
- rowers accept this because ergs are accessible and train important movement/fitness patterns.

XR re-inverts the dilemma:

- erg-centered representation is physically congruent with the real machine,
- boat-centered representation restores sport depiction but requires accepting offset/mapping constraints.

Possible brand note:

- “Cyboats” fictional manufacturer is thematically funny because of cybernetics/cyborg/feedback-loop boat.

---

# 14. Tool-mediated action / virtual oars

## Oars as tools, not body parts

Do not claim virtual oars are embodied as body parts unless measured.

Better:

> Virtual oars can be described as tool-mediated action representations: the user acts through a rowing tool that visually extends the real handle action into the virtual boat and water.

This is safer and fits tool-use/body-schema literature.

Potential phrasing:

> In rowing, the oar extends the rower’s action beyond the hands to the blade and water. In XR rowing, virtual oars may therefore be interpreted as tools that extend action into the virtual environment, even if the real user holds a central ergometer handle.

---

# 15. Brain plasticity / body schema notes

## Brain plasticity

Treat as background plausibility, not proof.

Useful thesis definition:

> Brain plasticity is the nervous system’s capacity to reorganize its sensory, motor, and body-related representations in response to repeated experience, training, altered feedback, or tool use.

XR rowing version:

> In XR rowing, brain plasticity is relevant as background for the idea that users may adapt to repeated tool-mediated action mappings, such as controlling virtual oars through a real ergometer handle. However, plasticity should be treated as a plausibility concept, not as evidence that virtual oars or offset avatar arms automatically become embodied.

## Body schema plasticity

Useful for offset oar/IK question:

> Body schema plasticity describes the ability of the brain’s action-oriented body representation to adapt to tools or altered movement mappings.

Mention only if needed; do not make it a central thesis unless supported.

---

# 16. Optic flow / vection / locomotion notes

## Optic flow vs vection

Keep clear:

- **Optic flow** = visual motion pattern.
- **Vection** = subjective feeling of self-motion that may arise from visual motion.

Stationary sport apps recreate optic-flow-like patterns while the user remains physically stationary.

## XR rowing use

In XR rowing:

- rowing effort drives virtual boat/world movement,
- shoreline/water/route move past,
- stationary erg work gains visible locomotion consequence.

Safe formula:

```text
stationary exercise
→ optic flow
→ vection / spatial presence
→ reduced awareness of being stationary
```

## Anti-Sisyphus effect

Working term only. Use carefully or not at all.

Meaning:

> stationary exercise stops feeling like repetitive effort in place and begins to feel like meaningful locomotion through a world.

Better to translate into established constructs:

- optic flow,
- vection,
- spatial presence,
- flow,
- action-outcome coupling.

---

# 17. VR motion sickness / stationary cardio notes

## Effort-coupled locomotion

Prototype observation:

- high virtual speeds may be tolerable when motion is coupled to rowing effort,
- discomfort reappears when motion is artificial/decoupled.

Use cautiously as prototype observation, not general scientific claim.

Safe thesis phrasing:

> In prototype testing, discomfort appeared more likely when visual motion was decoupled from rowing action than when forward movement was coupled to user effort. This observation is treated as design-relevant but not as a general claim about cybersickness.

## Wave/bobbing rule

Design rule:

> Rowing effort should produce forward motion, but wave motion should be treated carefully.

Possible implementation:

- keep user viewpoint/body stable,
- allow boat/water/world bob visually,
- avoid passive camera/head rocking.

---

# 18. Rowing-technique notes

## Keep rowing biomechanics narrow

Need only enough to explain:

- catch,
- drive,
- finish/release,
- recovery,
- feathering/squaring,
- erg vs boat distinction,
- oar/boat limitations.

Do not become a rowing biomechanics thesis.

## Erg vs boat

Useful point:

- ergometer uses simplified straight-line handle pull,
- boat rowing uses oar arcs around oarlocks,
- adds blade placement/extraction/feathering/squaring,
- force curves and rhythm can differ.

Use to justify why boat-centered IK is an approximation, not perfect replication.

## Prerecorded rowing animation + IK

Note:

You are tuning IK to rely partly on prerecorded rowing animation because pure IK from erg movement does not capture all boat-rowing rhythm, especially around finish/release.

Could mention in system chapter as implementation rationale if needed.

---

# 19. VR rowing related-work notes

## Keep VR rowing projects compressed

Do not narrate every project. Use a compact table/appendix.

Purpose of related-work pile:

> show that ergometer + VR / rowing simulators have been explored in the wild, but not this exact embodiment tradeoff.

Possible wording:

> Prior virtual rowing systems have investigated pacing, motivation, feedback, social rowing, and simulator training. These works demonstrate continued interest in rowing as a VR sport/exercise domain, but they do not isolate the embodiment tradeoff between physically congruent erg mapping and sport-faithful boat/oar depiction.

Then table.

## Yellow source use

Many sources are only:

- appendix,
- one-sentence lineage,
- “this has been done before,”
- future work.

Do not let them drive theory.

---

# 20. Reading/source priorities and status reminders

## Evaluation/questionnaire priority list

Read/use first:

1. Roth & Latoschik 2020 — VEQ
2. Gonzalez-Franco & Peck 2018 — Avatar Embodiment Questionnaire
3. Kilteni et al. 2012 — Sense of Embodiment
4. Kalckert & Ehrsson 2012 — ownership/agency dissociation
5. Kalckert & Ehrsson 2017 — onset/familiarization timing
6. Waltemate 2016 — latency/temporal congruence
7. Ma & Hommel 2013 — only if threat survives
8. Slater 2009 / Skarbez 2017 — if measuring presence/plausibility

## Theory stack sufficient

The current source base is sufficient. Do not keep expanding unless a specific sentence needs support.

Covered:

- embodiment theory,
- ownership/agency/self-location,
- RHI/moving RHI,
- VR embodiment reviews,
- temporal congruence,
- questionnaire methods,
- presence/plausibility,
- VR sport framing,
- rowing basics,
- erg vs boat mismatch.

Overloaded:

- VR rowing related projects,
- feedback/motor-learning sources,
- exergame/health sources.

---

# 21. Notes on “Change” in VEQ

## What Change means

VEQ Change is about perceived change in the participant’s own body schema/body image:

- body form/appearance changed,
- body weight changed,
- body height changed,
- body width changed.

For this thesis:

- not main outcome,
- maybe secondary/exploratory,
- useful if boat mode offset or avatar morphology creates perceived body transformation,
- not necessary if questionnaire length is an issue.

Safe phrasing:

> Change was treated as an exploratory subscale because the study primarily investigates ownership and agency rather than body-shape transformation.

---

# 22. Mottelson review notes

## Main findings to remember

Mottelson et al. 2023:

- systematic review/meta-analysis of VR body ownership illusions,
- large field-level overview,
- visuomotor synchrony is one of the strongest manipulations for body ownership,
- visuomotor asynchrony is especially strong for agency,
- agency often reports higher than ownership,
- first-person perspective matters,
- questionnaire practices are messy/non-standardized,
- field often underpowered,
- many studies use within-participant designs.

Use it to support:

- why visuomotor congruence matters,
- why your erg-centered condition is theoretically meaningful,
- why standardized measurement matters,
- why ownership and agency should be reported separately,
- why small-N conclusions should be cautious.

---

# 23. Source-inventory notes

## Master inventory created

A 37-bundle master inventory was created from `literature/Zips Papers/`.

Use it as the map for:

- all paper bundles,
- cluster,
- tag/priority,
- thesis-use note.

## Core writing spine from inventory

Use these to drive actual first theory draft:

- Kilteni 2012 — SoE conceptual spine.
- Botvinick & Cohen 1998 — RHI baseline.
- Kalckert & Ehrsson 2012 — ownership/agency dissociation.
- Ionta 2011 — self-location / bodily self-consciousness.
- Mottelson 2023 and/or Girondini 2025 — modern VR embodiment review.
- Waltemate 2016 — latency / temporal congruence.
- Roth & Latoschik 2020 VEQ and/or Gonzalez-Franco & Peck 2018 — questionnaire operationalization.
- Slater 2009 + Skarbez 2017 — presence/plausibility cleanup.
- Harris 2019 + Richlan 2023 + Neumann 2018 — VR sport/action realism/fidelity.
- Lamb 1989 + Flood/Simpson + Soper/Hume/Baca — rowing/erg-vs-boat support.

---

# 24. Drafting workflow notes

## Use this chat as argument brain

Because this chat is synced to project logic, use it for:

- section logic,
- paragraph-by-paragraph argument,
- claim strength,
- what to cut/footnote/appendix,
- danger-zone checks.

Use agentic account for:

- repo/file operations,
- LaTeX splitting,
- formatting,
- citation insertion,
- table generation,
- compile fixes.

## Snapshot habit

After each major section, export a small dated Markdown handoff like:

`theory_section_v01_argument_locked.md`

Then tell the agent:

- do not invent,
- do not rewrite core logic,
- do not change argument order,
- add TODO citations if needed.

---

# 25. Event / public-program description note

Test-event title:

> Vom Ergometer aufs Wasser: Virtuelles Rudern im Selbsttest

Accepted short public description:

> In diesem Selbsttest erleben Besucherinnen und Besucher, wie ein echtes Ruderergometer mittels eines Virtual-Reality-Headsets mit einer virtuellen Ruderumgebung verbunden wird. Dabei können zwei Varianten ausprobiert werden: Entweder wird man mitsamt Rudermaschine in ein virtuelles Boot versetzt und rudert durch eine Flusslandschaft, oder man bleibt sichtbar auf einem virtuellen 3D-Klon der eigenen Rudermaschine und gleitet damit durch virtuelle Welten.
>
> Die Anwendung untersucht, welche Darstellung sich überzeugender anfühlt: die sportlich realistischere Bootsumgebung mit virtuellen Rudern oder die genauere Übertragung der echten Körper- und Maschinenbewegung in die virtuelle Welt.
>
> Das Projekt verbindet Virtual Reality, Sporttechnologie und Forschung zur Körperwahrnehmung und zeigt, wie reale Bewegung und virtuelle Körperdarstellung zusammenwirken können.

---

# 26. File/conversion caution

For thesis material:

- Do not change wording unless explicitly requested.
- “Convert / format / clean layout” = formatting only.
- “Rewrite / polish” = only when explicitly asked.
- For exact wording, always preserve the original source-of-truth file.
- Avoid relying on earlier “cleaned” versions that may have smoothed content.

For paper bundles:

- `raw_page_marked.md` = source extraction.
- `clean_reading.md` = lightly cleaned extraction.
- `thesis_notes.md` = interpretive synthesis, not source text.

---

# 27. Small branding/design note

## Cyboats

Fictional boat manufacturer name “Cyboats” is amusingly on-theme because of:

- cybernetics,
- cyborg,
- feedback loops,
- machine-mediated rowing,
- body/device coupling.

Optional fun brand detail, not thesis-core.

---

# 28. Final thesis north star

Keep this as the final filter:

> I am not proving that VR rowing is good. I am using XR rowing as a precise design case to test whether embodied action congruence or sport-action depiction better supports ownership and agency.
