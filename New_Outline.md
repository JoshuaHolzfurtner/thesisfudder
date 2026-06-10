# Final Outline Candidate (locked-structure version)

## 1. Introduction

### 1.1 Motivation
* Indoor rowing = real exertion + real coordinated movement, but no physical travel through space.
* XR can transform indoor rowing into an embodied virtual sport experience.

### 1.2 The core representation conflict (thesis hook)
* In XR rowing, there is no single “correct” representation because:
    * the ergometer abstracts rowing into a straight-line handle movement
    * boat rowing uses oars rotating in an arc around oarlocks, including feathering/squaring
* This produces a design tradeoff:
    * Erg-centered / high congruence
    * Boat-centered / sport depiction

### 1.3 One visual “why you can’t match both” (in intro)
Diagram block (simple, immediate):
* Diagram A: Ergometer: straight handle path + seat rail
* Diagram B: Boat: oar arc around oarlock + blade feather/square cue
* Optional inset: feathering vs squaring (one image each)
This is where your Unity “filmed” visuals are perfect: a single composite figure that is instantly obvious.

### 1.4 Research question
* Does embodiment benefit more from:
    * direct physical congruence (erg-centered mapping), or
    * sport-action realism (boat/oar depiction with mismatch)?

### 1.5 Contributions
* Prototype enabling two modes under the same physical rowing task
* Fast/robust erg alignment (spatial congruence foundation)
* Full-body avatar control via IK and tracking scaffold
* Evaluation comparing ownership, agency, realism/plausibility, preference (+ optional drift probe)

---

## 2. Theoretical Background / Related Work

### 2.1 Rowing: minimum domain baseline (not a biomechanics thesis)
* Stroke phases: catch, drive, finish/release, recovery
* Erg vs on-water: straight handle vs oar arc + feather/square + oarlock pivot
* Why mismatch matters for representation (sets up the tradeoff)
(Keep tight — consistent with your own “don’t become rowing biomechanics thesis” reminder.)  

### 2.2 XR / VR baseline: minimum technical vocabulary
* XR / VR / HMD
* Tracking and latency (definitions only)
* Avatar / self-avatar; first-person view
* Embodied interaction (body as the interface)

### 2.3 XR rowing as an embodied interaction problem (bridge section)
* The physical-virtual action loop:
    * real body + real erg + real haptics → virtual body/action/world response
* Two representation strategies:
    * erg-centered vs boat-centered
* Different “realism” types (explicit disambiguation):
    * bodily/device congruence vs sport-action congruence vs visual realism vs plausibility

### 2.4 Presence and plausibility (only if you keep it)
* Presence / Place Illusion / Plausibility Illusion
* Why “being there” ≠ “owning the avatar”
* Use only as conceptual separator, not as a big thread
(You already noted these sections may be valuable but optional; keep them fenced and short.)

### 2.5 Embodiment framework (your core theory vocabulary)
* Sense of Ownership (SoO)
* Sense of Agency (SoA)
* Sense of Self-Location (SoL) (only if needed)
* Why ownership and agency can diverge (important for boat vs erg interpretation)

### 2.6 Body ownership illusion genealogy (condensed into ONE section)
This is where we fix the “2.6/2.7 crazy split” concern: merge the RHI-to-mVHI story into one clean block.
* Rubber Hand Illusion (RHI): root paradigm and measurement lineage
* Proprioceptive drift: classic marker (brief definition + caution)
* Moving RHI: ownership via synchronous movement (no brush required)
* Virtual Hand Illusion (VHI) / moving VHI (mVHI): VR movement-driven variants
* Key bridge claim relevant to your thesis:
    * active control + congruent feedback can support ownership/agency
    * incongruent/noisy feedback can reduce both
(Your “genealogy” sidebar image like your sketch can live here.)

### 2.7 Congruence variables (the mechanism map)
This is where you unify “bottom-up vs top-down” and where IK/alignment can be mentioned as variables, without turning the theory into implementation.
* Bottom-up cues:
    * visuomotor congruence
    * visuoproprioceptive congruence
    * visuotactile/haptic congruence (real handle grip)
    * temporal congruence (latency)
    * spatial congruence (alignment)
* Top-down cues:
    * anatomical plausibility
    * avatar morphology plausibility
    * sport-action plausibility (rowing logic)
* Map explicitly to modes:
    * Erg-centered: maximizes bodily/device congruence
    * Boat-centered: maximizes sport-action congruence (tool-mediated action) but introduces hand/oar offset

### 2.8 Related XR rowing systems (main text = tiny, appendix = big)
* One paragraph: “many projects exist; most are yellow for this thesis”
* Purpose: show your two strategies occur “in the wild”
* Push details into Appendix island/table
(This matches our earlier “compress VR rowing projects; don’t let them drive theory” note.)  

### 2.9 Research gap and thesis framing
* The gap is not “VR rowing exists”
* The gap is: same real rowing task, two competing embodiment strategies, evaluated through ownership/agency + realism/preference
* Leads directly into system chapter

---

## 3. System / Prototype (technical chapter)

### 3.1 Design goals and constraints
* Fair comparison: same physical rowing, different representation mapping
* Comfort: avoid decoupled motion where possible
* Keep congruence stable enough to evaluate

### 3.2 Hardware and software
* HMD
* Tracking approach
* Unity pipeline

### 3.3 IK and hand tracking (explicitly reinstated)
* What is tracked
* What is inferred
* What IK solves in your system (full-body plausibility from sparse signals)

### 3.4 Ergometer alignment and calibration (explicitly reinstated)
* Your fast alignment method (3s-ish)
* What is aligned (erg model, handle, seat reference frame, user pose baseline)

### 3.5 Ergometer as tracking scaffold (the “hardware from 5 years in the future” claim)
* Why alignment + erg constraints let you infer full-body pose plausibly
* Why this is an enabling contribution for embodied sport tasks

### 3.6 Erg-centered mode
* How mapping works
* What congruence it prioritizes
* Expected subjective outcomes

### 3.7 Boat-centered mode
* How retargeting works (oar handles, oarlock arc, feather/square)
* What sport-action plausibility it prioritizes
* Expected subjective outcomes and mismatch risks

### 3.8 Environment and locomotion (minimal)
* Stroke-coupled locomotion basics
* Any comfort design choices (camera stability, etc.)

---

## 4. Study Design / Method

### 4.1 Design
* Within-subject erg vs boat
* Counterbalancing order (if possible)
* Standardized exposure time/intensity

### 4.2 Participants
* Non-technical participant-friendly
* Capture rowing experience, VR experience, sickness susceptibility

### 4.3 Procedure
* Consent + safety
* Calibration/alignment
* Condition A → short questionnaire
* Condition B → short questionnaire
* Preference/comparison + open comment

### 4.4 Measures (lean, non-technical friendly)
* Ownership (few items)
* Agency (few items)
* Perceived realism/plausibility (few items)
* Movement match / timing (few items)
* Preference (post both)
* Discomfort/cybersickness safety check (short)
* Optional: hand-location/drift-style probe (exploratory)
(Consistent with your concern: don’t make them feel like they deserve an hourly rate.)

---

## 5. Results

* Ownership
* Agency
* Realism/plausibility
* Movement match/timing
* Preference
* Discomfort
* Exploratory drift probe

---

## 6. Discussion

* Answer the core question first
* Interpret divergences: agency vs ownership vs realism
* Tool-mediated boat action vs bodily congruence
* Alignment + tracking scaffold implications
* Limitations (small-N, prototype fidelity, etc.)
* Future work (optional, controlled)

---

## 7. Conclusion

* What was built
* What was compared
* What was learned

---

## Quick reminders of “what changed” vs your earlier state

1. Rowing basics moved earlier as a reader prerequisite (but kept minimal).
2. RHI → mRHI → VHI/mVHI collapsed into one genealogy block (instead of two big sections), because you correctly flagged that as crazy/over-academic.
3. IK + hand tracking explicitly reinstated (in System chapter; theory mentions them only as variables).
4. Alignment explicitly reinstated, and “ergometer as tracking scaffold” becomes a named contribution. (This was also present in our chat notes.)  
5. Related XR rowing projects demoted to appendix/table island (main text: short).  
6. Presence/optic flow/motion sickness are fenced: allowed, but must stay short unless you truly evaluate them.
