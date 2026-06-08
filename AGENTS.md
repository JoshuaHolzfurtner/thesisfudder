# AGENTS.md — Thesis Assistance Rules

This repository contains a master's thesis project. AI tools may assist with drafting, reviewing, restructuring, LaTeX maintenance, citation-gap detection, and code/documentation review. The author remains fully responsible for the final thesis.


## Core thesis framing

This thesis develops and evaluates an XR/VR rowing system as a testbed for embodiment in sport-specific virtual interaction. The central design tension is between two representation strategies:

1. **Ergometer-congruent mode**  
   This mode prioritizes close spatial and temporal alignment between the user's real ergometer movement and the virtual avatar. The real handle and seat motion are mapped as directly as possible to the virtual body. The design goal is high visuomotor congruence and a strong sense that the visible stroke is caused by the user’s own bodily action.

2. **Boat-realistic mode**  
   This mode prioritizes a more sport-faithful depiction of rowing on water. The user still rows on an ergometer, but the virtual representation shows a rowing body using oars in a boat-like environment. Because real ergometer handle motion and realistic oar motion do not match exactly, this mode may sacrifice some visuomotor congruence in favor of recognizable rowing realism.

The thesis does not assume in advance that one mode is better. Instead, it asks how spatial alignment, temporal congruence, movement mapping, and avatar realism influence embodiment-related experience in XR rowing.

The main empirical focus is on sense of ownership, sense of agency, and broader sense of embodiment. The system and study are used to investigate whether embodiment is better supported by precise movement correspondence with the real ergometer or by a more realistic sport depiction.

The primary contribution is the developed XR rowing mechanism and its evaluation. The theoretical concepts are used as lenses for interpretation, not as claims that the thesis resolves embodiment theory in general.


## Primary responsibility

Do not invent, assume, or silently add thesis content. The author provides the scientific contribution, implementation details, study data, interpretation, and final wording.

AI assistance may help with:

- drafting scaffolds from provided notes
- improving clarity and structure
- identifying unsupported claims
- detecting citation gaps
- reviewing LaTeX consistency
- suggesting missing sections as TODOs
- checking terminology consistency
- proposing cautious academic phrasing

AI assistance must not:

- invent sources
- invent results
- invent participant numbers
- invent implementation details
- invent citations or BibTeX entries
- fabricate author names, years, DOIs, page numbers, or quotations
- overstate findings
- turn hypotheses into conclusions
- add theory as if it were already established without evidence

## Files to read before editing

Before editing any chapter, read these files first:

1. `AGENTS.md`
2. `notes/global/thesis_spine.md`
3. `notes/global/claims_register.md`
4. `notes/global/terminology.md`
5. `notes/global/contribution_hierarchy.md`
6. The relevant chapter back-of-mind file in `notes/chapters/`
7. The chapter `.tex` file being edited

For literature-heavy sections, also read relevant files from:

- `literature/summaries/`
- `literature/txt/`

Prefer `literature/summaries/` first. Use raw text files only when direct verification is needed.

## Citation rules

Use only citation keys that already exist in `references.bib`, unless explicitly asked to add a new source.

If a claim needs evidence and no source is available, write:

`TODO:CITE`

If a source may support a claim but must be checked manually, write:

`TODO:VERIFY`

If a paper text contains useful evidence, add a LaTeX comment near the relevant claim, for example:

```tex
% SOURCE-CHECK: smith2020example, p. 4, body ownership vs agency
