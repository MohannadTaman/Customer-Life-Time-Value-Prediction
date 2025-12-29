Customer Life Time Value Prediction

This repository contains a machine learning pipeline for predicting customer Lifetime Value (LTV) for a digital wallet dataset. The project demonstrates an end-to-end workflow from data preprocessing to model evaluation, including cross-validation and feature transformations.

Key Features

Data Preprocessing:

Numerical features transformed using Yeo-Johnson for normality and Standard Scaling

Income_Level encoded using Ordinal Encoding

Other categorical features encoded using One-Hot Encoding

Modeling:

XGBoost Regressor for regression

Preprocessing pipeline ensures consistent transformations

Evaluation:

Train/test metrics: MSE, RMSE, R²

K-Fold Cross-Validation for robust assessment

Feature importance can be extracted from the trained model

Results

Near-perfect performance: R² ≈ 0.9999, RMSE ≈ 4–5k

Consistent results across CV folds indicate pipeline stability

Purpose

Showcase an end-to-end regression pipeline

Demonstrate preprocessing for mixed numerical and categorical features

Provide an example of XGBoost regression with cross-validation


Install dependencies:

pip install pandas numpy scikit-learn xgboost seaborn matplotlib


Update the dataset path in the notebook.

Run the notebook to preprocess data, train the pipeline, and evaluate performance.

License

This project is open-source.
