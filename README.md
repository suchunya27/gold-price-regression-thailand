# Multiple Regression Analysis on Factors Affecting Gold Prices in Thailand
Multiple regression analysis of economic factors influencing gold prices in Thailand
___

## Project Overview

This study aims to identify the key factors influencing gold prices in Thailand and to develop the best-fit multiple linear regression model to forecast the average monthly gold price in Thailand for the upcoming year. The analysis considers independent variables including crude oil price (THB), average monthly exchange rate (THB/USD), policy interest rate (%), and average global gold price (THB), based on secondary data from January 2015 to December 2022.
___

## Objectives

1. To investigate the factors affecting gold prices in Thailand.  
2. To develop an optimal regression equation for forecasting Thailand’s gold price in the coming year.

___

## Scope of Study

The study uses average monthly gold price data (THB) along with related factors: crude oil price, average exchange rate of Thai Baht to US Dollar, policy interest rate, and global average gold price. The dataset covers 96 months from January 2015 to December 2022. The goal is to construct a regression model that can estimate and forecast gold prices in Thailand effectively.
___

## Data Description

- **Dependent Variable:**  
  - Average monthly gold price in Thailand (Price, THB)  
- **Independent Variables:**  
  - Crude oil price (Oil, THB)  
  - Average monthly exchange rate (USD, THB/USD)  
  - Policy interest rate (IR, %)  
  - Global average gold price (GoldSpot, THB)  
- **Period Covered:** January 2015 – December 2022 (96 months)

## Methodology

- Variable selection was performed using Stepwise Selection and All Possible Regression methods at a significance level of 0.05.  
- Assumptions of regression were thoroughly tested:  
  - **Linearity:** Residual plots showed no violation.  
  - **Constant Variance (Homoscedasticity):** Residual analysis and Szroeter’s test confirmed the assumption.  
  - **Normality:** Initial violation corrected by removing outliers; assumption then met.  
  - **Independence:** Durbin-Watson test indicated autocorrelation; attempts to correct with lag variables were not significant, so original model was retained.  
  - **Multicollinearity:** Moderate multicollinearity detected; removing correlated variables worsened model fit, so original model was retained.  
- Dummy variables representing months (Q1 to Q11, with December as baseline) were tested but found insignificant.  
- Interaction terms between independent variables improved model fit by reducing standard errors and increasing R-squared.

## Final Regression Model

\[
\text{Price} = 22322 + 8.088 \times \text{Oil} + 716.3 \times \text{USD} + 15.847 \times \text{GoldSpot} + 0.3305 \times (\text{GoldSpot} \times \text{IR})
\]

Where:  
- Price = Average monthly gold price in Thailand (THB)  
- Oil = Crude oil price (THB)  
- USD = Average exchange rate (THB/USD)  
- GoldSpot = Global average gold price (THB)  
- IR = Policy interest rate (%)

## Conclusion

The study successfully identified key factors impacting gold prices in Thailand and developed a robust multiple linear regression model incorporating interaction effects. This model can accurately forecast gold prices, and the inclusion of interaction terms notably improved model performance, highlighting their importance in economic modeling.
