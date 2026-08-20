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
Main effect of PEG treatment
Main effect of imbibition time
PEG × imbibition time interaction

2. Coefficient of variation

3. Assumption tests
Shapiro–Wilk test for normality of residuals
Levene's test for homogeneity of variances

4. Multiple comparisons

Student-Newman-Keuls (SNK) test
Duncan's multiple range test
Estimated marginal means (emmeans) with appropriate p-value adjustment

5. Principal Component Analysis

Repository structure
├── introduction data/
│   
│
├── R/
│   ├── data_preparation.R
│   ├── ANOVA.R
│   ├── figures.R
│   ├── posthoc_tests.R
│   └── PCA.R
│
└── README.md

#The analyses were performed using R.

#Main R packages used include:
car
agricolae
emmeans
ggplot2
FactoMineR
factoextra
Reproducibility

#The experimental dataset and analysis scripts are provided in this repository for transparency and reproducibility.

Variable names and factor levels should be checked before running the scripts, particularly for PEG treatment and imbibition time.
