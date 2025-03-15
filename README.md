# Heart Disease Prediction (Binary Classification)
This dataset was pulled from [Kaggle.com](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction)

#### -- Project Status: ✅ Completed

## Project Intro/Objective
Heart disease remains the leading cause of death among men, women, and most racial groups, according to the CDC. This project leverages healthcare data from five different clinics/datasets (Cleveland, Hungarian, Switzerland, Long Beach VA, Stalog (Heart) Data Set) to develop predictive models for heart disease, contributing to research efforts aimed at addressing this critical public health issue.

### Methods Used
* Exploratory Data Analysis (EDA) – Examined dataset structure, distributions, and potential patterns.
* Data Visualization – Used plots to explore relationships between variables.
* Statistical Analysis – Applied odds ratios to measure associations and variance inflation factors (VIF) to check for multicollinearity.
* Machine Learning – Built classification models (e.g., Random Forest, XGBoost) to predict heart disease.
* Predictive Modeling – Assessed model performance using metrics like AUC-ROC and F1 score.

### Technologies
* Python 🐍
* Seaborn & Matplotlib 🎨
* Sklearn & XGBoost 🚀⚡
* Statsmodels 📊

## Project Description
**Key Questions:** Can the available electronic health record (EHR) data effectively predict heart disease? Which features contribute most significantly?
### Workflow
1. Explore the Data
- Bar charts & KDE distributions with hue set to "Heart Disease" for breakdown.
2. Check for Multicollinearity 🔍
- Variance Inflation Factor (VIF) + heatmap analysis.
3. Identify Key Features
- Odds Ratios to determine statistically significant predictors.
4. Further Exploration
- EDA on the top four most significant features from the log odds ratios.
5. Preprocessing for Modeling 🔄
- Standardization + One-Hot Encoding.
6. Build models
- Random Forest 🌲🌲🌲
- Logistic Regression 🔀📈 
- XGBoost ⚡📈
- ADA Boost 🚀📈
- K Nearest Neighbors 📍
7. Evaluate Model Performance 
- Classification Report
- Confusion Matrix
- ROC-AUC Curve
- Precision & Recall vs Threshold
8. Extract Feature Importance 🔑
- Identified the Top 10 contributing factors.

## Best Performing Model 🏆
- Model: K-Nearest Neighbors (KNN)
- Hyperparameter: n_neighbors = 21
- Performance Metrics: 
    - AUC-ROC: 0.95
    - Accuracy: 0.90
    - Precision: 0.90
    - Recall: 0.92
    - F1 Score: 0.91

## Findings
### Feature Importance Across Models
Feature importance varied significantly across different models, highlighting the complexity of the dataset. The top four most influential features were:
- Resting BP (AdaBoost)
- ST_Slope (Up) (XGBoost & Random Forest)
- Cholesterol (KNN)
- Sex (Male) (Logistic Regression - adjusted and unadjusted for collinear features)


### Want to Clone & Experiment?

1. Clone this repository to your local machine.
2. Download dataset from [Kaggle](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction)
3. **Reach out!** Questions? Let’s connect on [LinkedIn](www.linkedin.com/in/davidgraham-cs)

