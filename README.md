# Stroke Risk Prediction & Logistic Regression
## Project Overview
This repository contains a statistical analysis and predictive model focused on identifying patient stroke risk. Built using R, the project demonstrates data preprocessing, exploratory data analysis (EDA), and the development of a Logistic Regression model to perform binary classification on health data.

## Key Analyses
### 1. Exploratory Data Analysis & Preprocessing
Objective: Clean demographic and health data and identify strong predictive features.

Findings: Processed categorical variables (like gender and smoking status) using one-hot encoding and consolidation. Visualizations revealed that stroke risk is notably higher among individuals with hypertension. Age presented a unimodal distribution peaking around 55 years old, while average glucose levels were right-skewed and bimodal.

### 2. Model Selection & Diagnostics
Objective: Build and evaluate a classification model to predict the binary outcome of experiencing a stroke.

Methodology: Implemented a generalized linear model (GLM) with a logit link function using age, average glucose level, and hypertension as predictors.

Evaluation: Utilized DHARMa residual simulations to confirm the model met necessary assumptions (linearity and constant variance). A direct comparison proved that Logistic Regression was strictly superior to standard Linear Regression, as linear models violate core statistical assumptions when predicting binary outcomes.

### 3. Statistical Findings & Interpretation
Age: Identified as the most significant predictor. Every additional year of age is associated with an estimated 7.5% increase in the odds of having a stroke, holding other variables constant.

Hypertension: High-risk individuals with hypertension experience an estimated 58% increase in the odds of having a stroke compared to those without it.

Glucose Levels: Increases in average glucose levels were also found to be statistically significant contributors to elevated stroke risk.

## Tech Stack
Language: R

Libraries: tidyverse, MASS, DHARMa (residual diagnostics), car

Techniques: Logistic Regression, Binary Classification, Residual Diagnostics, One-Hot Encoding
