# Difference-in-Differences and Shift-Share Designs

Materials for a short course at the **University of Louisiana at Lafayette**, September 18, 2026.

**Brantly Callaway**
John Munro Godfrey, Sr. Department of Economics, University of Georgia
<brantly.callaway@uga.edu>

## Sessions

| | Topic | Slides |
|---|---|---|
| 1 | Difference-in-Differences with a Continuous Treatment | [`01_continuous-treatment.qmd`](01_continuous-treatment.qmd) |
| 2 | Assessing the Plausibility of Strong Parallel Trends using Close Comparison Groups | [`02_comparison-groups.qmd`](02_comparison-groups.qmd) |
| 3 | Shift-Share Instruments | [`03_shift-share.qmd`](03_shift-share.qmd) |

## Building the slides

Slides are written in Quarto and render to self-contained `revealjs` HTML
(`embed-resources: true`, so each `.html` is a single portable file).

```bash
quarto render
```

or, for a single set of slides,

```bash
quarto render 01_continuous-treatment.qmd
```

Rendering requires the [`revealEquations`](https://github.com/bcallaway11/revealEquations)
package, which is used for incremental equation reveals:

```r
remotes::install_github("bcallaway11/revealEquations")
```

## Repository layout

```
├── index.qmd                    landing page for the course website
├── 01_continuous-treatment.qmd  session 1 slides
├── 02_comparison-groups.qmd     session 2 slides
├── 03_shift-share.qmd           session 3 slides
├── united.scss                  slide theme
├── _extensions/clean/           Quarto revealjs extension
├── refs.bib, extra-refs.bib     bibliography
└── img/                         figures used in the slides
```

## Related materials

* "Difference-in-Differences: A Practitioner's Guide" ([arXiv](https://arxiv.org/pdf/2503.13323)), forthcoming at the *Journal of Economic Literature*
* [`did`](https://bcallaway11.github.io/did) — R package for DiD with multiple periods
* [`contdid`](https://github.com/bcallaway11/contdid) — R package for DiD with a continuous treatment
