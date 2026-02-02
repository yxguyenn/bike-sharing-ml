# Bike Sharing Demand Prediction

## Overview
This project builds and evaluates supervised machine learning models to predict **hourly bike rental demand** using weather and temporal features from the UCI Bike Sharing Dataset.

## Dataset
- Source: UCI Machine Learning Repository
- Granularity: Hourly
- Target variable: total bike rentals per hour

## Methods
- Data cleaning and preprocessing
- Feature engineering using temporal and weather variables
- Model comparison:
  - Linear Regression (baseline)
  - Random Forest Regressor
  - Gradient Boosting Regressor
- Evaluation metrics: RMSE and R²

## Results
Tree-based models significantly outperformed linear regression, indicating strong non-linear relationships in the data.
- **Best model:** Random Forest  
- **R²:** ~0.95  
- **RMSE:** ~41  

## Tools
Python, NumPy, Pandas, scikit-learn, Jupyter Notebook


