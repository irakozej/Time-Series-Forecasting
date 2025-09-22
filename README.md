# Air Quality Forecasting Assignment

## Overview
This project focuses on predicting air pollution levels (PM2.5) using machine learning techniques. The goal is to forecast air quality based on historical data and environmental features, and to generate predictions suitable for submission to Kaggle.

## Dataset
- **Training Data:** Contains historical air quality measurements along with features like temperature, humidity, wind speed, etc.
- **Test Data:** Contains similar features but without the target variable (`PM2.5`) for which predictions are to be made.
- **Target Variable:** `PM2.5` (Particulate Matter 2.5 concentration)

## Methodology
1. **Data Preprocessing**
   - Handled missing values
   - Dropped irrelevant columns (e.g., `datetime` if not needed for modeling)
   - Split data into features (`X`) and target (`y`)
2. **Feature Engineering**
   - Selected relevant features
   - Encoded categorical variables if any
3. **Modeling**
   - Trained **Random Forest Regressor** and **Linear Regression**
   - Compared models based on training metrics (MSE, RMSE, MAE, R²)
4. **Evaluation**
   - Evaluated models on training set
   - Selected the best-performing model (Random Forest) for final predictions
5. **Submission**
   - Generated `submission.csv` with predictions for the test set

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/irakozej/Time-Series-Forecasting-copy.git


**Usage**
  - Run the notebook Air_Quality_Forecasting.ipynb cell by cell.

  - After training and evaluation, a submission file submission.csv will be generated.

  - Submit submission.csv to Kaggle for evaluation.

**Metrics**

  - The models were evaluated using:

  - Mean Squared Error (MSE)

  - Root Mean Squared Error (RMSE)

  - Mean Absolute Error (MAE)

  - R² Score

**Conclusion**

Random Forest outperformed Linear Regression on training data.

The final submission uses predictions from the Random Forest model.

This workflow provides a clear pipeline from data preprocessing to model evaluation and submission.
