# Thesis AI Workflow: Prose, Citation Dossiers, Verification, and Cleanup

## Purpose

This workflow separates thesis writing into different AI-assisted roles. The goal is to keep high-quality thesis prose while using agentic tools for source grounding, citation checking, repetition detection, and repository maintenance.

The core principle is:

```text
ChatGPT = thesis voice, conceptual synthesis, prose quality
Codex = repository worker, citation clerk, source auditor, diff/checking tool
Git / VS Code = control surface and review layer
```

This avoids relying on one large chat context for everything and makes the thesis more auditable.

---

## Repository as Memory

The repository should be treated as the project memory. Important context should live in files, not only in chat history.

Recommended files:

```text
AGENTS.md
references.bib
notes/global/thesis_spine.md
notes/global/claims_register.md
notes/global/terminology.md
notes/global/contribution_hierarchy.md
notes/chapters/
MD Papers/
literature/
chapters/
ai_logs/
```

The `MD Papers/` folder acts as a lightweight, decomposed paper library. The PDFs are used for final checks, exact quotations, page verification, and ambiguous cases.

---

## Bibliography Strategy

`references.bib` is the controlled citation vocabulary.

Rules:

```text
citation key = stable internal source ID
BibTeX metadata = can be corrected later
```

The agent may use existing citation keys in dossiers and source checks, even if the BibTeX metadata still needs polishing. Once citation dossiers exist, avoid renaming keys unless absolutely necessary.

Preferred source triangle:

```text
references.bib key
↔ renamed PDF file
↔ decomposed .md paper bundle
```

Example:

```text
slater2009placePlausibility
literature/pdfs/slater2009placePlausibility.pdf
MD Papers/slater_2009_place_illusion_plausibility.../
```

Metadata verification can happen later during paper-first audit or final bibliography cleanup.

---

## Main Workflow

### 1. Prose scaffold or patch

Use ChatGPT for writing and polishing thesis prose.

Input should be small:

```text
- one chapter-wide .tex file or one target subsection
- relevant verified dossier excerpt
- chapter role note if needed
```

Prompt pattern:

```text
Patch only the currently open file or subsection.
Use the dossier only as source/citation support.
Do not rewrite unrelated sections.
Do not invent implementation details.
Do not over-explain concepts already introduced earlier.
Keep thesis prose clear, concise, and non-robotic.
```

---

### 2. Chapter-first citation dossier

Use Codex in a separate chat/thread.

Purpose: map existing chapter claims to source support.

Codex should not rewrite prose. It should create a dossier file such as:

```text
notes/01_introduction/dossier_section_1.md
```

Dossier entries should include:

```text
Claim
Location
Suggested source key
Evidence explanation
Markdown path and line range
PDF page if available
Confidence: verified / likely / needs manual check
Caution / overclaim note
```

The `Evidence` field is not just a quote. It should explain why the source supports the claim.

Example:

```md
## Evidence
The source distinguishes place illusion and plausibility illusion, which supports the Introduction's claim that scene plausibility and embodiment should not be collapsed into one construct.
```

---

### 3. Separate dossier verification

Use a second Codex chat/thread to verify the dossier.

Purpose: check whether the first dossier was accurate.

The verifier should check:

```text
- Does the cited source actually support the claim?
- Is the claim too broad?
- Is the source the best source, or only background?
- Are the MD line anchors real?
- Is the PDF page plausible?
- Is the confidence label correct?
```

Output file example:

```text
notes/01_introduction/dossier_section_1_verification.md
```

Verifier labels:

```text
verified
likely
needs manual check
unsupported
too broad
```

The verifier should not rewrite thesis prose or edit `.tex`.

---

### 4. Optional self-check of the verification

If the verification is important, ask the verifier to second-guess its own results.

Useful prompt:

```text
Review your verification file for overconfident verified labels, missing caveats, incomplete anchors, and places where a source supports only part of a claim. Make only small corrections. Do not rewrite the full file.
```

This can catch small improvements without restarting the whole workflow.

---

### 5. ChatGPT prose/citation patch

After dossier and verification, use ChatGPT to patch the actual chapter.

Input:

```text
- target chapter or subsection
- relevant dossier excerpt
- relevant verification excerpt
```

Goal:

```text
- improve prose
- insert minimal citations where useful
- avoid citation stuffing
- narrow overbroad claims
- keep thesis voice
```

Important rule:

```text
The Introduction should use a minimal source spine, not cite every sentence.
```

---

### 6. Redundancy / repetition audit

Use Codex for folder-wide or chapter-wide repetition detection.

Purpose: find repeated definitions, repeated framing, and concepts introduced too many times.

Output file example:

```text
notes/01_introduction/redundancy_audit.md
```

The audit should not rewrite prose. It should list:

```text
Repeated concept
Locations
Why it repeats
Keep / merge / cut suggestion
```

ChatGPT can then do the final prose reduction.

---

### 7. Paper-first audit

After the chapter is stable, run paper-first checks for core papers.

Purpose: ask whether important papers are underused or incorrectly used.

For each core paper, Codex checks:

```text
Where does this paper support an existing thesis claim?
Are we missing a useful citation?
Is this paper being overused?
Is a weaker source being used where this source would be better?
Does the BibTeX entry match the paper?
```

This should happen after the chapter-first pass, not before, to avoid citation stuffing.

---

### 8. Final cleanup

Before submission:

```text
- remove unnecessary SOURCE-CHECK comments or move them into dossiers
- verify direct quotes against PDFs
- verify page numbers for critical claims
- clean references.bib metadata
- check terminology consistency
- compile PDF
- run final redundancy pass
- update AI assistance statement / ai_logs
```

---

## Recommended Order for a Chapter

For each chapter:

```text
1. Stabilize prose scaffold.
2. Generate chapter-first dossier.
3. Verify dossier in separate chat.
4. Optionally self-check verification.
5. Patch prose/citations with ChatGPT.
6. Run redundancy audit.
7. Run paper-first audit for core sources.
8. Clean citations and comments.
```

---

## Chapter 1 Lessons

The Chapter 1 dossier and verification showed that the workflow works.

Strongly supported source spine:

```text
Rowing / erg vs boat:
- lamb1989kinematicComparison
- soperHume2004rowingTechnique
- rauterEtAl2013rowingTransfer

VR rowing / VR sport:
- murrayEtAl2016vrRowingPresence
- arndtEtAl2018vrRowingWorkouts
- neumannEtAl2018interactiveVrSport

Embodiment:
- kilteniEtAl2012senseEmbodiment
- botvinickCohen1998rubberHand
- kalckertEhrsson2012movingRubberHand

Presence / plausibility / self-motion:
- slater2009placePlausibility
- niehorster2021opticFlowHistory
- kooijmanEtAl2024measuringVection
- palmisanoEtAl2015vectionChallenges

VR action caution:
- harrisEtAl2019visionForAction
```

Main caution points:

```text
- "Whole-body rowing" needs Rauter or a stronger Lamb anchor.
- "Design problem" is thesis synthesis, not a direct source claim.
- "Sport depiction and visuomotor congruence come apart in indoor rowing" needs both rowing sources and embodiment/action sources.
- "No exact comparison exists" must remain a reviewed-material / underexplored claim unless a formal search table is added.
- Commercial app examples need separate sources or should be removed from academic gap framing.
- Preference is exploratory, not an embodiment construct.
```

---

## File Structure Recommendation

Use chapter-wide `.tex` files or generated chapter-wide review files for ChatGPT prose work.

Recommended practical structure:

```text
chapters/
  01_introduction.tex
  02_theory.tex
  03_system.tex
  04_study_design.tex

notes/
  01_introduction/
    dossier_section_1.md
    dossier_section_1_verification.md
    redundancy_audit.md

review_context/
  01_introduction_full_context.tex
  02_theory_full_context.tex
  full_thesis_context.tex
```

The cleanest rule:

```text
Merged/chapter-wide files = better context for ChatGPT
Split files or Git diffs = safer editing control
```

If using VS Code plugin with surgical patches, chapter-wide files are acceptable because the diff remains small as long as the prompt is scoped.

---

## Prompt: Chapter-First Dossier

```text
You are creating a chapter-first citation dossier for a master's thesis. Follow AGENTS.md strictly.

Do not rewrite thesis prose.
Do not edit .tex files.
Do not add BibTeX entries.
Use only existing keys from references.bib.

Read:
1. AGENTS.md
2. references.bib
3. relevant global notes
4. relevant chapter notes
5. target chapter .tex
6. relevant MD Papers bundles

Create:
notes/[chapter]/dossier_[chapter].md

For each citation-relevant claim, include:
- Claim
- Location
- Suggested citation key
- Evidence explanation
- Markdown path and line range
- PDF page if available
- Confidence: verified / likely / needs manual check
- Caution / overclaim note
- Source role: best / supporting / background / weak

Do not try to cite every sentence.
Do not invent page numbers, line numbers, quotes, citation keys, or metadata.
Flag unsupported claims as TODO:CITE or TODO:VERIFY.
```

---

## Prompt: Dossier Verification

```text
You are verifying a citation dossier for a master's thesis. Follow AGENTS.md strictly.

Task:
Double-check the existing citation dossier. Do not rewrite thesis prose. Do not edit .tex files. Do not add new citations to the thesis.

Read:
1. AGENTS.md
2. references.bib
3. the dossier file
4. the chapter .tex files referenced by the dossier
5. the relevant markdown source files cited in the dossier
6. raw page-marked markdown or PDFs only when needed

Create:
notes/[chapter]/dossier_[chapter]_verification.md

For each dossier entry, check:
- Does the cited source actually support the claim?
- Is the claim too broad?
- Is the suggested citation the best source or only background?
- Are the .md path and line range real and relevant?
- Is the PDF page anchor plausible if given?
- Is the evidence snippet/paraphrase accurate?
- Is the confidence label correct?

Use this format:

## Entry [number or claim title]

### Verdict
verified / likely / needs manual check / unsupported / too broad

### Claim checked
...

### Source checked
...

### Evidence check
...

### Anchor check
- MD path: valid / invalid / missing
- Line range: valid / invalid / missing
- PDF page: valid / invalid / missing / not checked

### Source role
best / supporting / background / weak / wrong source

### Required action
...

At the end, add:
- Keep
- Downgrade
- Replace
- Remove or TODO
- Dossier quality rating

Do not invent page numbers, line numbers, quotes, or citation keys.
Do not mark anything verified unless the cited evidence was actually checked.
```

---

## Prompt: Verification Self-Check

```text
Review your verification file for overconfident verified labels, missing caveats, incomplete anchors, and places where a source supports only part of a claim.

Make only small corrections.
Do not rewrite the full file.
Do not edit thesis prose.
Do not add new citations.
Show a concise diff.
```

---

## Prompt: Redundancy Audit

```text
You are auditing repetition and conceptual overlap in a master's thesis chapter.

Do not rewrite prose.
Do not edit .tex files.

Read:
1. AGENTS.md
2. target chapter .tex or merged review context
3. relevant notes/dossiers if needed

Create:
notes/[chapter]/redundancy_audit.md

For each repeated topic:
- Topic
- Locations
- What is repeated
- Which occurrence should stay
- Which occurrence should be shortened, merged, or removed
- Risk if removed

Focus on:
- repeated definitions
- repeated thesis framing
- repeated construct explanations
- repeated methodological justification
- terminology drift

Keep the audit concise and actionable.
```
