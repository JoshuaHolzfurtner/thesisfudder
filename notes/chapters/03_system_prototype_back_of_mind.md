# Chapter 3 — System and Prototype — Back of Mind

## Purpose

Document the design and implementation of the VR rowing system. Describe the hardware and software components, including the rowing ergometer, tracking setup (e.g., handle, seat, body), and VR headset. Explain the two embodiment modes:

1. **Ergometer‑based embodiment (erg mode):** High visuomotor congruence. Real handle and seat movements are mapped directly onto the avatar to maximize spatial and temporal alignment.
2. **Boat‑based embodiment (boat mode):** Sport‑realistic depiction. The avatar rows with virtual oars that follow realistic rowing animations. The user still rows on the ergometer, but the real handle motion is mapped indirectly to the oar motion, potentially sacrificing alignment for realism.

Provide details on avatar mapping and inverse kinematics (IK) for both modes, including how the virtual body is aligned with the user’s body (if at all). If a threat scene or heart‑rate integration is used, describe how it is implemented.

## Reader state before this chapter

The reader knows the research questions and the theoretical background but has not yet seen how the system is implemented.

## Reader state after this chapter

The reader should understand how the prototype works, what the two modes look like and feel like, and what technical decisions underpin them. This chapter sets the stage for the study design.

## Core claims

- The two modes differ primarily in their mapping strategies (direct vs indirect) and realism.
- The prototype faithfully captures and renders ergometer motion while supporting both modes.
- Technical details (e.g., sensor placement, IK) affect how congruence and realism are achieved.

## Allowed claims

- Describe technical decisions as design choices rather than absolute necessities.
- Note the intended trade‑offs (e.g., increased realism vs decreased congruence).

## Forbidden overclaims

- Do not claim that the system perfectly simulates rowing or embodiment. Emphasize limitations where relevant.
- Avoid presenting design decisions as inherently superior; present them as choices made for experimentation.

## Required sources

- References to similar VR rowing systems or interface designs (if any).
- Relevant technical literature on motion tracking, IK, and VR ergonomics.

## Required project details

- Hardware specifications (ergometer model, sensors, headset).
- Software stack (game engine, Netcode, network details if applicable).
- Mapping strategies for both modes (illustrations or diagrams could be added later).

## Open TODOs

- Finalize the description of how handle and seat motion are captured and mapped.
- Create diagrams or figures showing the mapping for each mode.
- Document calibration procedures (if needed).

## Tone

Technical and descriptive. Aim for clarity and transparency; acknowledge assumptions and limitations of the implementation.