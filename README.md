This repository contains the statistical analysis of experimental data related to seed imbibition under different PEG treatments and imbibition times (hours). The analyses were performed in R and include descriptive statistics, analysis of variance (ANOVA), assumption tests, post hoc comparisons,graphical analysis, and principal component analysis (PCA).

#The experiment evaluated the effect of:
PEG concentration (treatments): 4 levels (PEG0, PEG1, PEG2, PEG3)
Imbibition time: 24 levels (1–24 hours)
Replicates: 3 

#The main response variables include measurements such as:
Fresh weight
Turgid weight
pH
Electrical conductivity (EC)
Relative Water Content (RWC)
Imbibition Rate (IMB)

#The following analyses were performed:

1. Analysis of variance (ANOVA)

Two-way ANOVA models were used to evaluate:

Main effect of PEG treatment
Main effect of imbibition time
PEG × imbibition time interaction

2. Assumption tests

The assumptions of the ANOVA models were evaluated using:

Shapiro–Wilk test for normality of residuals
Levene's test for homogeneity of variances
Diagnostic plots of model residuals

3. Multiple comparisons

When significant differences were detected, post hoc analyses were performed using methods such as:

Student-Newman-Keuls (SNK) test
Duncan's multiple range test
Estimated marginal means (emmeans) with appropriate p-value adjustment
4. Coefficient of variation

The coefficient of variation (CV) was calculated from the residual mean square of the ANOVA:

[
CV = \frac{\sqrt{MS_{error}}}{\bar{Y}} \times 100
]

5. Principal Component Analysis

Principal Component Analysis (PCA) was performed to explore relationships among measured variables and identify patterns in the experimental data.

Repository structure
├── data/
│   └── Official Database.xlsx
│
├── R/
│   ├── data_preparation.R
│   ├── ANOVA.R
│   ├── posthoc_tests.R
│   ├── PCA.R
│   └── figures.R
│
├── figures/
│   └── ...
│
└── README.md
Software and packages

The analyses were performed using R.

Main R packages used include:

car
agricolae
emmeans
ggplot2
FactoMineR
factoextra
Reproducibility

To reproduce the analyses:

Clone or download this repository.
Open the R scripts in the R/ directory.
Make sure the required packages are installed.
Set the working directory to the repository location.
Run the scripts in the indicated order.
Data availability

The experimental dataset and analysis scripts are provided in this repository for transparency and reproducibility.

Notes

Variable names and factor levels should be checked before running the scripts, particularly for PEG treatment and imbibition time.
