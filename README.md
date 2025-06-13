# Multiple Linear Regression Analysis: Predicting Sales with Promotion Data

This project aims to build and analyze a multiple linear regression model to predict sales (`Sales`) based on TV and Radio advertising budgets.

---

## Contents

- [Project Overview](#project-overview)  
- [Data Preparation](#data-preparation)  
- [Model Setup](#model-setup)  
- [Model Results](#model-results)  
- [Assumptions and Checks](#assumptions-and-checks)  
- [Methods Used](#methods-used)  
- [Conclusions and Interpretations](#conclusions-and-interpretations)  
- [Usage](#usage)  
- [License](#license)  

---

## Project Overview

This analysis investigates factors affecting sales and models the impact of TV and Radio advertising budgets on sales. The model's performance and validity are assessed through various statistical techniques.

---

## Data Preparation

- `TV` and `Radio` are used as independent variables.  
- Categorical and ordinal variables are properly encoded into numerical values.  
- Column names with spaces in the dataset have been corrected.

---

## Model Setup

- The model formula `Sales ~ TV + Radio` is used for multiple linear regression.  
- The model is fitted using the Ordinary Least Squares (OLS) method.

---

## Model Results

- The model’s $R^{2}$ value is 0.904, indicating it explains 90.4% of the variance in sales.  
- Model coefficients:  
  - $\beta_0 = 64.9254$ (Intercept)  
  - $\beta_{TV} = 77.3156$  
  - $\beta_{Radio} = 2.9558$  
- All coefficients have p-values of 0.000, indicating statistical significance at the 0.05 level.  
- 95% confidence intervals should be reported for each coefficient; for example, the slope of $\beta_{TV}$ is within $[72.497, 82.135]$ with 95% confidence.

---

## Assumptions and Checks

- Residual analysis, homoscedasticity, and multicollinearity checks were performed to validate model assumptions.  
- VIF was not applied due to the ordinal nature of the `TV` variable, to avoid misleading interpretations.  
- Fitted values group into three clusters corresponding to the categorical variable, with similar variance distribution validating the assumptions.

---

## Methods Used

- Multiple Linear Regression (OLS)  
- Ordinal Encoding of categorical variables  
- $R^{2}$ analysis for explanatory power  
- p-value for coefficient significance  
- Residual analysis and assumption validation

---

## Conclusions and Interpretations

The model shows that TV and Radio advertising expenditures have significant positive effects on sales, with TV being the strongest predictor. The model is reliable and effective for sales prediction.

---

## Usage

You can use the provided Python code to build the model, perform analysis, and interpret results.

---

## License

This project is prepared for educational purposes.

---

## Language Versions

This README is available in both English and Turkish.  
You can find the Turkish version in the `README_tr.md` file or request it if needed.
