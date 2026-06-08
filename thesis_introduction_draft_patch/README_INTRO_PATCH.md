# Thesis Introduction Draft Patch

This zip contains a drop-in Introduction draft organized as subsection-level LaTeX files.

## Integration

In `main.tex`, replace the old introduction input, if needed, with:

```tex
\input{chapters/01_introduction/00_chapter}
```

## Notes

- Citations are deliberately left as `\cite{TODO}` placeholders where source keys need verification.
- Chapter references assume labels such as `chap:theoretical_background`, `chap:system_prototype`, `chap:study_design`, `chap:results`, `chap:discussion`, and `chap:conclusion`.
- Adjust labels if your current chapter files use different names.
