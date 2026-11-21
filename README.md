# BFSI Financial Risk Modeling: Bankruptcy and Credit Default

Boston University OMDS | DX799 Data Science Capstone | Fall 2026
Author: Shuqin Ouyang

## Overview
Weekly notebooks that apply each week's modeling technique to two credit-risk problems:
predicting corporate bankruptcy and consumer credit card default. The goal is to see which
indicators signal risk, whether bankruptcy is harder to model than default, and whether the
findings hold across samples and models.

## Data
- [Taiwanese Bankruptcy Prediction](https://doi.org/10.24432/C5004D): 6,819 companies, 95 financial ratios, 3.2% bankrupt.
- [Default of Credit Card Clients](https://doi.org/10.24432/C55S3H): 30,000 clients, 23 predictors, 22.1% default.
Data files are not included. Download them from UCI and place them in [folder name].

## Methods by week
| Weeks | Topic |
|---|---|
| 1 | Polynomial and interaction terms |
| 2 | Ridge, Lasso, Elastic Net |
| 3 | Forward/backward selection, PCR, PLSR |
| 4 | Logistic regression and feature scaling |
| 5 | Support vector machines |
| 6 | Decision trees and random forests |
| 8 | K-nearest neighbors |
| 9 | Gradient boosting |
| 10 | K-Means clustering |
| 11 | DBSCAN and hierarchical clustering |
| 13 | Naive Bayes |

## Key results
- Failures are rare, so models were scored with F1 against an all-failure baseline instead of accuracy.
- Random forest test F1: 0.478 (bankruptcy) and 0.531 (credit card), about 7.7x and 1.5x baseline.
- Class-weighted gradient boosting raised recall (0.25 to 0.55 bankruptcy, 0.37 to 0.62 credit card) at the cost of precision (about 0.5).
- Repayment status was the strongest default signal; bankruptcy risk was spread across profitability, debt, and liquidity ratios.
- One K-Means cluster held 38 of the 44 bankruptcies in the test set.
- Feature scaling was essential for KNN and logistic regression.

## Limits
Results come from single train/test splits in places, the bankruptcy test set has only about 44 failures, and the two datasets differ in size, features, and failure rate, so comparisons between them are indicative, not proof.

## Running the notebooks
Python with pandas, NumPy, scikit-learn, statsmodels, matplotlib. Open the notebooks in order and update the data paths.
