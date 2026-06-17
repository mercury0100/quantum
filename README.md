# The Black Book of Quantum Physics
### *or: Bad Maths that Gets the Right Answer*

**Cooper Doyle**

---

A derivation of the most important laws of quantum physics using nothing but a pen, a few thought experiments, and two experimental results.

This book began as graduate lecture notes and became something else: an argument that quantum mechanics is not a collection of weird facts imposed on us by experiment, but the inevitable destination of classical mechanics taken seriously enough. Starting from a mass on a spring, and following the logic wherever it goes, we arrive at the Dirac equation in seven steps.

## The argument

Two experimental inputs — Planck's quantisation and Born's rule — and everything else follows. A spring becomes a field. A field becomes a wave. A wave becomes a particle. A particle becomes a spinor. Spin and antimatter appear unrequested.

This is not what a mathematician would consider rigorous. But we are physicists, and infinity, to us, is just a large number.

## Contents

| Part | Topic |
|---|---|
| I | Introduction |
| II | The Mechanics of Heaven and Earth |
| III | Light |
| IV | The Jacobi Conspiracy |
| V | The Ultraviolet Catastrophe |
| VI | The Born Ultimatum |
| VII | Creation and Annihilation |
| VIII | Dirac's Coup |

## Compiling

The book is written in LaTeX using the `krantz` document class.

```bash
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

Figures are in `/img` as SVG files. Convert to PDF before compiling:

```bash
for f in img/*.svg; do inkscape "$f" --export-pdf="${f%.svg}.pdf"; done
```

Or switch to `xelatex`, which handles SVG natively via the `svg` package.

A compiled PDF is included in the repository for those who just want to read it.

## Prerequisites

- A LaTeX distribution (TeX Live or MiKTeX)
- The `krantz` class (included in most distributions)
- Inkscape (for SVG to PDF conversion) or `xelatex`

## Status

Work in progress. The core derivation is complete. Remaining work is polish and figures.

## License

© Cooper Doyle. All rights reserved. Please do not reproduce without permission.
