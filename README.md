 Predict Housing Prices using Advanced Regression Techniques
 Introduction

This project applies machine learning regression techniques to predict housing prices.
The workflow covers data preprocessing, feature engineering, multicollinearity analysis, and model evaluation.
Models used: Lasso Regression and XGBoost Regressor.

Dataset

Housing dataset (structured tabular data).

Features include lot area, number of rooms, garage details, year built, and more.

Target variable: SalePrice.

Methods
🔹 Data Preprocessing

Handling missing values (imputation).

Removing outliers.

Encoding categorical variables with One-Hot Encoding.

Feature scaling (where necessary).

🔹 Feature Engineering

Created new features such as HouseAge and GarageAge.

Checked correlations and removed highly collinear features.

Variance Inflation Factor (VIF) analysis to reduce multicollinearity.

🔹 Models Applied

Lasso Regression – to perform regression with feature selection.

XGBoost Regressor – to capture nonlinear relationships and boost performance.

Results
Lasso Regression

Train RMSE: 0.134

Train R²: 0.86

Test RMSE: 0.140

Test R²: 0.83

XGBoost Regressor

Train RMSE: 0.0103

Train R²: 0.9992

Test RMSE: 0.1394

Test R²: 0.8320

Key Insights

Lasso Regression performed well and reduced feature count effectively.

XGBoost fit the training set extremely well (risk of overfitting) but still generalized similarly to Lasso on test data.

Feature selection and proper preprocessing had a strong impact on model performance.

 How to Run
# Clone repo
git clone https://github.com/Himran13/housing-price-prediction.git  

# Install dependencies
pip install -r requirements.txt  

# Run notebook or script
jupyter notebook housing_price_prediction.ipynb

Future Improvements

Hyperparameter tuning with GridSearchCV / RandomizedSearchCV.

Try Ensemble Models (Stacking, Random Forest).

Deploy model as a web app using Streamlit or Flask.

Conclusion

This project demonstrates how advanced regression models can be applied to predict housing prices.
Through feature engineering, multicollinearity checks, and model evaluation, we improved prediction accuracy and gained insights into important housing features.
