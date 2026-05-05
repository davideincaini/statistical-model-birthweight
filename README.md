# Statistical Model for Newborn Weight Prediction

## Problem
Predict newborn weight from maternal and clinical variables — a regression problem with a real medical dataset requiring rigorous statistical modeling and assumption validation.

## Notable Aspect
This project is implemented in **R**, demonstrating statistical modeling beyond the Python ecosystem — relevant for environments where R is the standard for statistical analysis (clinical, academic, quality engineering contexts).

## Approach

### Exploratory Analysis
- Descriptive statistics and distribution checks per variable group
- Visualization: ggplot2 for distributional analysis, boxplots by categorical predictors
- Correlation structure analysis before model building

### Modeling
- Linear regression baseline (MASS::lm)
- Assumption validation: residual normality (Shapiro-Wilk), homoscedasticity, leverage/influence analysis
- Stepwise variable selection to identify significant predictors

### Key Predictors Identified
Maternal smoking status, gestational age, and maternal age show the strongest associations with birth weight — consistent with clinical literature.

## What I Would Do Differently
- Test Box-Cox transformation on the response variable — birth weight distributions are often slightly right-skewed
- Add interaction terms: smoking × gestational age interaction is clinically plausible

## Stack
`R` · `ggplot2` · `dplyr` · `MASS` · `rstatix` · `patchwork`

---
*Part of [Davide Incaini's data science portfolio](https://github.com/davideincaini)*
