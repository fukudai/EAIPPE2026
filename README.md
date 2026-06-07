# Empirical Analysis for Infrastructure Project / Policy Evaluation — Lecture Notebooks (Lectures 2–8)

Interactive Jupyter notebooks (R) for the graduate course *Empirical Analysis for Infrastructure Project/Policy Evaluation* (University of Tokyo, Dept. of Civil Engineering). Topics: linear regression, causal effect analysis, instrumental variables, panel data, matching, quasi-experimental methods, and applications.

## ▶ Run online (no installation)

Click the Binder badge to launch a live R environment in your browser. Replace `fukudai/EAIPPE2026` with the actual GitHub path after you upload this repository.

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/fukudai/EAIPPE2026/HEAD)

The first launch builds the environment (a few minutes); later launches are cached and faster. When the notebook opens, the kernel is **R**.

## Contents

| File | Topic |
|---|---|
| `2_Basics_of_Linear_Regression_enriched.ipynb` | Linear regression — full lecture version (recommended) |
| `2_Basics_of_Linear_Regression.ipynb` | Linear regression — concise version |
| `3_Basics_of_Causal_Effect_Analysis.ipynb` | Causal effect analysis |
| `4_Instrumental_Variable_Method.ipynb` | Instrumental variables |
| `5_Panel_Data_Analysis.ipynb` | Panel data |
| `6_Matching_Method.ipynb` | Matching |
| `7_Causal_Inference_under_Quasi_Experimental_Conditions.ipynb` | Quasi-experimental methods |
| `8_Applications_of_Causal_Inference_Methods.ipynb` | Applications |
| `figures/` | Figures and equation images referenced by the notebooks |
| `*.csv`, `mroz.txt` | Datasets used by the R code cells |

> **Keep the folder structure intact.** Notebooks reference images via relative paths (`figures/<lecture>/...`) and the R code reads the datasets by file name from the working directory.

## Run locally (alternative)

Requires R and the Jupyter R kernel:

```r
install.packages(c("IRkernel", "AER", "Matching", "plotrix"))
IRkernel::installspec()   # register the "R" kernel for Jupyter
```

Then `jupyter notebook` (or open the folder in VS Code) and select the **R** kernel.

## Environment

- `runtime.txt` pins the R version and a dated package snapshot for Binder.
- `install.R` lists the required R packages (`AER`, `Matching`, `plotrix`).
