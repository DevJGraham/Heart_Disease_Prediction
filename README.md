# Project Overview
> This project aimed to develop a binary classification model for predicting heart disease using a dataset from Kaggle. The dataset underwent extensive exploratory data analysis (EDA) and feature engineering to ensure robust model performance.

## Exploratory Data Analysis and Feature Engineering
- Multicollinearity Analysis: Visual Inspection of a correlation heatmap and Variance Inflation Factors (VIF) were used to detect collinear features. Two highly collinear features were identified and later tested in logistic regression models with and without their inclusion.
- Visualization: Pandas, Matplotlib, and Seaborn were used to identify trends in both numerical and categorical data.
- Odds Ratios & Log Odds Ratios: These were calculated for each feature to assess their statistical significance in predicting heart disease. Additional EDA was explored among the most significant features.

## Data Preprocessing
- Continuous Features: Standardized to ensure uniform scaling.
- Categorical Features: One-hot encoded for proper model interpretation.
- Binary Features: Left unchanged to preserve their original structure.

## Model Training & Evaluation
Multiple machine learning models were trained and compared, including:
- Random Forest
- Logistic Regression (with and without collinear features)
- K-Nearest Neighbors (KNN)
- XGBoost
- AdaBoost

## Best Performing Model
- Model: K-Nearest Neighbors (KNN)
- Hyperparameter: n_neighbors = 21
- Performance Metrics: 
    - AUC-ROC: 0.95
    - Accuracy: 0.90
    - Precision: 0.90
    - Recall: 0.92
    - F1 Score: 0.91

## Feature Importance Across Models
Feature importance varied significantly across different models, highlighting the complexity of the dataset. The top four most influential features were:
- Resting BP (AdaBoost)
- ST_Slope_Up (XGBoost & Random Forest)
- Cholesterol (KNN)
- Sex_M (Logistic Regression - adjusted and unadjusted for collinear features)

