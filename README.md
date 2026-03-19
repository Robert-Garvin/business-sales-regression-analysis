# business-sales-regression-analysis
Excel-based regression analysis identifying key drivers of sales performance

# Sales Regression Analysis in Excel 📊

## Overview

This project explores the relationship between business operational factors and sales performance across multiple franchise locations using Excel-based statistical analysis.

The objective was to determine which variables significantly impact sales and to evaluate different regression models for best fit.

---

## Dataset

The dataset includes:

* Sales (dependent variable)
* Overhead Costs
* Square Footage
* Number of Employees

---

## Statistical Analysis

### Linear Regression (Overhead vs Sales)

Model:
Sales = -1741.57 + 32.25 × Overhead

* p-value: ~0.000000015
* t-statistic: 6.32
* 95% Confidence Interval: (22.09, 42.41)

**Interpretation:**

* Extremely low p-value → strong evidence of a real relationship
* Overhead is a statistically significant predictor of sales
* For every unit increase in overhead, sales increase by ~22 to 42 units (95% confidence)

---

### Model Limitations

* Residual spread increases with overhead
* Indicates **non-linearity (heteroscedasticity)**
* Linear regression alone may not be the best model

---

### Polynomial Regression

Model:
Sales = 1042.42 − 47.40(Overhead) + 0.56(Overhead²)

* Captures nonlinear behavior
* Provides improved fit over simple linear regression

---

### Logarithmic Model

Model:
Sales = -8929.41 + 2226.68 × ln(Overhead)

* Alternative nonlinear transformation
* Helps model diminishing returns

---

### Multiple Linear Regression

Model:
Sales = -1036.95 + 9.50(Sq Ft) − 8.12(Employees) + 29.12(Overhead)

**Results:**

* Overhead → statistically significant (p < 0.05)
* Square Footage → not significant
* Employees → not significant

---

## Key Insights

* Overhead is the strongest and only statistically significant predictor of sales
* Increasing store size or staffing does not guarantee higher sales
* The relationship between overhead and sales is likely nonlinear
* Polynomial regression provided the best overall model fit

---

## Tools Used

* Microsoft Excel

  * Regression Toolpak
  * Correlation Analysis
  * Statistical Testing (p-values, confidence intervals)

---

## What I Learned

* How to interpret regression outputs (p-values, t-stats, confidence intervals)
* Identifying when linear models are insufficient
* Comparing multiple models to determine best fit
* Understanding statistical significance in a business context

---

## Future Improvements

* Recreate analysis in Python (pandas, statsmodels)
* Add visualizations (scatter plots, residual plots)
* Build an interactive dashboard (Power BI or Tableau)

---

