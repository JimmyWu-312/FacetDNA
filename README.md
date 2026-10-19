# FacetDNA

<div align="center">

[![Language: R](https://img.shields.io/badge/Language-R-276DC3?logo=r&logoColor=white)](https://www.r-project.org/)
![Analysis: Linear regression](https://img.shields.io/badge/Analysis-Linear%20regression-497698)
[![Tools: ggplot2](https://img.shields.io/badge/Tools-ggplot2-1A162D)](https://ggplot2.tidyverse.org/)

![Diagnostics: car](https://img.shields.io/badge/Diagnostics-car-3B6B66)
![Model selection: MASS](https://img.shields.io/badge/Model%20selection-MASS-334155)

</div>

A comprehensive regression analysis of diamond prices using R. Includes data exploration, model fitting, assumption testing, transformation, model selection, and diagnostics with visualizations and interpretations.

### Linear Regression Analysis on Diamond Prices
This project investigates the factors influencing diamond prices through statistical modeling using R. Drawing from a dataset of 2,000 randomly sampled diamonds, the analysis explores how features such as carat, cut, color, clarity, and dimensions affect diamond pricing. The goal is to identify key predictors, build accurate models, and interpret results in a business-relevant context.

## Project Structure
- **Data Exploration**: Descriptive statistics, histograms, and correlation analysis to understand variable distributions and relationships.
- **Simple Linear Regression**: Initial model using `carat` to predict `price`, with assumption testing and diagnostics.
- **Model Refinement**: Logarithmic transformation to address normality and heteroscedasticity; model performance improves significantly.
- **Multiple Regression**: Incorporates additional predictors (cut, color, clarity, x, y, z, etc.) and assesses multicollinearity.
- **Stepwise AIC Model Selection**: Optimizes model using stepwise selection and evaluates performance.
- **VIF Analysis**: Addresses multicollinearity by removing highly correlated variables.
- **Prediction and Confidence Intervals**: Interprets results through interval estimates and assesses model accuracy.

## Key Results
- Simple model (`price ~ carat`) achieved R² of **0.85**, but violated assumptions.
- Log-transformed model improved to **R² = 0.93** and satisfied normality/equal variance conditions.
- Final multiple regression model (after AIC and VIF filtering) had an **R² = 0.92**, suggesting strong explanatory power.
- Some prediction intervals had **unrealistic negative lower bounds**, highlighting limitations and need for further model refinement.

## Technologies
- **Language**: R
- **Libraries**: `ggplot2`, `car`, `MASS`, `knitr`, `kableExtra`
- **Outputs**: Tables, plots, regression summaries, confidence and prediction intervals


## Insights
This project demonstrates how to construct, refine, and evaluate linear models with real-world implications. It emphasizes the importance of checking regression assumptions and thoughtfully selecting predictors to avoid multicollinearity.


