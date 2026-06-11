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
```

### Strict source-audit protocol

For literature-heavy thesis sections, prefer a two-layer citation audit:

1. **Inline `SOURCE-CHECK` comments** near the relevant LaTeX claim.
2. **Chapter citation dossier files** in `notes/chapters/` or `ai_logs/` when a larger source audit is being performed.

A `SOURCE-CHECK` comment should be used for citation-relevant claims when the source support has been checked or partially checked. Use the richest available form without inventing missing details:

```tex
% SOURCE-CHECK:
%   key: kalckertEhrsson2017ownershipOnset
%   md: literature/summaries/kalckert_ehrsson_2017.md, lines 42-58
%   pdf: p. 6
%   evidence: active synchronous movement produced stronger/faster ownership than passive synchronous movement
%   confidence: verified
```

If only partial support is known, mark it clearly:

```tex
% SOURCE-CHECK:
%   key: TODO:CITE
%   md: unknown
%   pdf: unknown
%   evidence: claim needs source support
%   confidence: needs manual check
```

Use these confidence labels:

- `verified` — source file, evidence, and page/line anchor were checked.
- `likely` — source appears relevant, but exact page, line, or wording still needs human verification.
- `needs manual check` — the claim needs evidence or the proposed source has not been checked closely enough.

When adding source-audit comments:

- Prefer `references.bib` keys that already exist.
- Include a supporting `.md` path and line range when available.
- Include the original PDF page when available.
- Include a short evidence snippet or paraphrase so the comment remains useful if line numbers shift.
- Do not invent page numbers, line numbers, quotation text, citation keys, authors, years, DOIs, or results.
- If a source is useful but not yet verified, use `TODO:VERIFY` or `confidence: likely` instead of presenting it as checked.
- Keep source-audit comments in LaTeX comments so they do not appear in the compiled PDF.

### Chapter-first and paper-first citation workflow

Use the citation workflow in this order unless the author asks otherwise:

1. **Chapter-first pass.** Read the target chapter and identify claims that need sources. Add citation keys, `TODO:CITE`, `TODO:VERIFY`, and `SOURCE-CHECK` comments near the relevant claims. This keeps the thesis argument driven by the chapter text rather than by citation stuffing.
2. **Paper-first audit.** After the chapter is stable, review core papers against the chapter to find missed source opportunities, stronger source anchors, or claims that should be corrected.
3. **Final cleanup.** Keep only useful LaTeX citation commands in the final text. Leave `SOURCE-CHECK` comments only if the author wants an auditable draft; otherwise remove or move them into a dossier before final submission.

For chapter dossiers, create or update a human-readable Markdown file such as:

```md
# Chapter 4 Citation Dossier

## Claim
Ownership and agency are measured separately because they can diverge.

## Location
chapters/04_study_design.tex, Section 4.5

## Source
kalckertEhrsson2012movingRHI

## Evidence
Short paraphrase or quote-sized snippet from the decomposed `.md` or source text.

## Anchors
- MD: literature/summaries/example.md, lines 42-58
- PDF: p. 6

## Confidence
verified / likely / needs manual check
```

Do not use dossiers to add new claims to the thesis. Use them only to audit, support, or flag claims already present in the chapter.
