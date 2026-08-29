# Mod C Data Science Capstone — Fall 2026

Boston University Online Master's in Data Science (OMDS) — Module C, Semester 1
Course: DX799 Data Science Capstone

## Overview

This repository contains weekly Jupyter notebooks applying each week's modeling
techniques to the BFSI (banking, financial services, insurance) capstone project
carried forward from Module B, Semester 2. The project analyzes two datasets to
identify financial and behavioral patterns that predict financial failure, at
both the corporate level (bankruptcy) and the individual consumer level
(credit default).

## Datasets

- **Taiwanese Bankruptcy Prediction** — 6,819 observations, 95 financial ratios,
  binary bankruptcy outcome.
  https://doi.org/10.24432/C5004D
- **Default of Credit Card Clients** — 30,000 observations, 24 variables,
  binary default outcome.
  https://doi.org/10.24432/C55S3H

## Weekly Notebooks

| Week | Topic | Notebook |
|------|-------|----------|
| 1 | Polynomial terms, interaction terms, multicollinearity/VIF, categorical/continuous features | `week1_polynomial_interaction_vif.ipynb` |
| 2 | Lasso, Ridge, Elastic Net regression | `week2_lasso_ridge_elasticnet.ipynb` |
| 3 | Forward/backward selection, PCR, PLSR | `week3_pcr_plsr_selection.ipynb` |
| 4 | Logistic regression, feature scaling | `week4_logistic_regression.ipynb` |
| 5 | Support Vector Machines, kernel trick | `week5_svm.ipynb` |
| 6 | Decision trees, random forest | `week6_random_forest.ipynb` |

Weeks 2 and 6 are explored in greater depth per Milestone One's requirements,
connecting Week 1's multicollinearity findings to Week 2's regularization
results, and extending Module B's baseline Random Forest performance in Week 6.

## Milestone One

This work is compiled into a summary document for Milestone One (due Week 7),
per the course's Milestone One Guidelines and Rubric.

## Author

Shuqin Ouyang
