# Life Expectancy Prediction

## Overview
The Life Expectancy Prediction project aims to develop a machine learning model that predicts life expectancy based on various socioeconomic and health-related factors. This model assists in understanding key contributors to life expectancy and aids policymakers in making data-driven decisions.

## Key Features
- Predicts life expectancy based on multiple country-specific indicators.
- Implements data preprocessing to handle missing values and optimize model performance.
- Uses machine learning techniques to improve accuracy and minimize error.
- Provides insights into key factors influencing life expectancy.

## Dataset
The dataset consists of multiple health and economic variables:

| Variable                         | Description                                         |
|----------------------------------|-----------------------------------------------------|
| Country                          | Name of the country                                |
| Year                             | Year of data collection                           |
| Status                           | Developing/Developed status of the country        |
| Life expectancy                  | Life expectancy in years                          |
| Adult Mortality                  | Probability of dying between 15 and 60 years     |
| Infant deaths                    | Number of infant deaths per 1000 live births      |
| Alcohol                          | Alcohol consumption per capita                    |
| Percentage expenditure            | Government health expenditure as % of GDP        |
| Hepatitis B                      | Immunization coverage (%)                         |
| Measles                          | Number of reported measles cases                 |
| BMI                              | Average Body Mass Index (BMI)                    |
| Under-five deaths                | Number of deaths of children under 5 years old   |
| Polio                            | Immunization coverage for polio (%)              |
| Total expenditure                 | Total healthcare expenditure as % of GDP         |
| Diphtheria                       | Immunization coverage for DTP (%)                |
| HIV/AIDS                         | Death rate due to HIV/AIDS per 1000              |
| GDP                              | Gross Domestic Product per capita                |
| Population                        | Total population of the country                  |
| Thinness 1-19 years               | % of thin individuals aged 1-19 years            |
| Thinness 5-9 years                | % of thin individuals aged 5-9 years             |
| Income composition of resources   | Human Development Index-based income composition |
| Schooling                         | Average number of years of schooling             |

### Observations:
- Countries with higher GDP and healthcare expenditure tend to have higher life expectancy.
- Infant and under-five mortality rates are negatively correlated with life expectancy.
- Immunization rates (Hepatitis B, Polio, Diphtheria) show a strong influence on life expectancy.
- Higher schooling years correlate with improved life expectancy.

## Workflow Overview
1. **Data Preprocessing**
   - Checking for missing values using heatmaps.
   - Handling missing values through appropriate imputation methods.
   - Normalizing/transforming data to improve model performance.

2. **Exploratory Data Analysis (EDA)**
   - Understanding feature distributions and correlations.
   - Identifying outliers and extreme values.
   
3. **Feature Engineering**
   - Selecting the most relevant features impacting life expectancy.
   - Removing unnecessary or redundant features.

4. **Model Building**
   - Using **RandomForestRegressor** for prediction.
   - Hyperparameter tuning to optimize model accuracy.

5. **Model Evaluation**
   - Accuracy achieved: **96.45%**
   - Mean Squared Error (MSE): **1.75**
   - Cross-validation score: **96.03%**

6. **Prediction & Deployment**
   - Using the trained model to predict life expectancy.
   - Deploying the model for real-world applications in policy-making and healthcare analysis.

## Model Performance
- The best-performing model is **RandomForestRegressor**, achieving an accuracy of **96.45%**.
- **GDP, Schooling, and Healthcare expenditure** were found to be strong predictors of life expectancy.
- The model effectively handles missing data and ensures reliable predictions.

This project provides valuable insights into global life expectancy trends, supporting informed decision-making in healthcare and policy development.

