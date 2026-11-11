# Quantitative Analysis of an SME Credit Portfolio Using Python

## Project Overview

This project demonstrates the application of Python, statistical analysis, and econometric techniques to an illustrative SME credit portfolio.

The analysis uses a synthetic dataset of eight SME borrowers with a combined credit exposure of ₦54 million. It examines repayment capacity, arrears behaviour, portfolio concentration, and the relationship between Debt Service Coverage Ratio (DSCR) and arrears days.

**Data disclaimer:** All borrower records and financial figures are synthetic. They are not actual bank customer records.

## Objectives

- Assess borrower repayment capacity using DSCR.
- Examine credit exposure across economic sectors.
- Identify borrowers with elevated arrears.
- Analyse the relationship between DSCR and arrears days.
- Apply correlation analysis and OLS regression.
- Evaluate model assumptions and diagnostic results.
- Compare regression specifications and prediction errors.
- Communicate findings and limitations.

## Tools and Technologies

- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- SciPy
- Statsmodels
- Scikit-learn
- Google Colab

## Methodology

1. Dataset creation and preparation.
2. Data-quality checks and descriptive statistics.
3. Exploratory data analysis.
4. Borrower risk classification.
5. Pearson correlation analysis.
6. Multiple linear regression.
7. Variance Inflation Factor (VIF) assessment.
8. Residual and heteroscedasticity diagnostics.
9. Regression model comparison.
10. MAE and RMSE evaluation.
11. Interpretation and recommendations.

## Key Findings

| Metric | Result |
|---|---:|
| Number of borrowers | 8 |
| Total portfolio exposure | ₦54 million |
| Average DSCR | 1.121 |
| 90+ day arrears exposure | ₦11 million |
| 90+ day arrears exposure share | 20.37% |
| Multiple regression R² | 0.883 |
| DSCR-only regression R² | 0.809 |
| DSCR-only MAE | 15.41 days |
| DSCR-only RMSE | 18.89 days |

The Pearson correlation between DSCR and arrears days was approximately -0.899, indicating a strong negative association within this synthetic sample.

The multiple regression model had an R² of 0.883. Neither DSCR nor cash flow was individually statistically significant at the 5% level in that specification.

The DSCR-only model produced an in-sample MAE of 15.41 days and RMSE of 18.89 days. These are not independent estimates of predictive performance.

## Model Diagnostics and Limitations

The analysis considered multicollinearity, residual patterns, normality diagnostics, and heteroscedasticity.

Key limitations:

- Very small sample size (eight borrowers).
- Synthetic rather than observed banking data.
- Potential multicollinearity between DSCR and cash flow.
- Possible nonlinearity.
- Negative predictions from unconstrained linear regression.
- No independent holdout or out-of-time validation.

The fitted models are exploratory and should not be deployed for real credit decisions.

## Conclusion

This project demonstrates practical application of data preparation, exploratory analysis, statistical inference, econometric modelling, model diagnostics, and quantitative interpretation using Python.
---

## Project 2: Statistical Inference and Hypothesis Testing Using Python

**Objective:** Analyse SME revenue performance and examine differences between trained and untrained businesses using statistical inference.

**Tools:** Python, Pandas, NumPy, SciPy, Statsmodels, Matplotlib and Seaborn.

**Methods demonstrated:**
- Descriptive statistics and confidence intervals
- Independent and paired-sample t-tests
- Welch's t-test and confidence interval for mean differences
- Chi-square tests of independence
- One-way ANOVA and diagnostic testing
- Effect-size analysis using Cohen's d, eta-squared and Cramér's V
- Data-quality checks and statistical interpretation

**Key finding:** The synthetic sample showed a statistically significant difference in mean post-training revenue between the trained and untrained groups (Welch's t-test, p = 0.0461).

**Important limitation:** The dataset is synthetic, and group-level revenue increments were programmed into the data generator. The results demonstrate statistical methods and interpretation, not evidence that training caused revenue growth in real businesses.

**Notebook:** `STEM_Quant_Statistical_Inference.ipynb`
It also highlights the importance of distinguishing statistical significance from predictive reliability and communicating model limitations responsibly.

## Project Notebook

`STEM_Quant_SME_Credit_Risk_Analysis.ipynb`
