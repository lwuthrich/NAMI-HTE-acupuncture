# Acupuncture Trial Analysis

Reproducible demonstration of the nonparanormal framework for **joint estimation of marginal and heterogeneous treatment effects**, applied to a publicly available randomized clinical trial on acupuncture for chronic headache (Vickers et al., 2004, *BMJ*, <https://doi.org/10.1136/bmj.38029.421863.EB>).

This analysis accompanies the paper:

> Wüthrich, L. & Hothorn, T. (2026). *Joint Estimation of Marginal and Heterogeneous Treatment Effects*. Department of Biostatistics, University of Zurich.

## Background

The trial randomized 401 patients to acupuncture (*n* = 205) or usual care (*n* = 196) to assess whether acupuncture reduces chronic headache burden. The primary outcome was a patient-reported headache severity score (6-point Likert scale) summed over four weeks, measured at baseline and at 12 months.

The analysis reproduces the original trial findings and progressively extends them by:

-   Adjusting for prognostic and predictive covariate effects
-   Incorporating all 401 observations (vs. 301 complete cases in the original)
-   Relaxing the normality assumption
-   Treating the outcome as ordinal

## Files

| File                        | Description                                |
|-----------------------------|--------------------------------------------|
| `acupuncture_analysis.Rmd`  | R Markdown source for the full analysis    |
| `acupuncture_analysis.html` | Rendered HTML report                       |

## Requirements

To re-run the `.Rmd`, you need R with the following packages:

``` r
install.packages(c("tram", "multcomp", "lattice"))
```

## Usage

Open `acupuncture_analysis.html` directly in a browser to view the report, or knit `acupuncture_analysis.Rmd` to reproduce it.

## Authors

Leticia Wüthrich and Torsten Hothorn\
Department of Biostatistics, University of Zurich
