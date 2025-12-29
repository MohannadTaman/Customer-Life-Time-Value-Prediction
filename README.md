# Customer Life Time Value Prediction

This repository contains a **machine learning pipeline** to predict **customer Lifetime Value (LTV)** for a digital wallet dataset. It demonstrates an end-to-end workflow from data preprocessing to model evaluation, including cross-validation and feature transformations.

## Key Features

### Data Preprocessing
- Numerical features transformed using **Yeo-Johnson** for normality and **Standard Scaling**  
- `Income_Level` column encoded using **Ordinal Encoding**  
- Other categorical features encoded using **One-Hot Encoding**

### Modeling
- **XGBoost Regressor** used for regression  
- Pipeline ensures consistent preprocessing and model fitting

### Evaluation
- Train/test metrics: **MSE**, **RMSE**, **R²**  
- **K-Fold Cross-Validation** for robust performance assessment  
- Feature importance extraction supported

## Results

| Metric | Train | Test |
|--------|-------|------|
| MSE    | 16,958,199 | 23,547,085 |
| RMSE   | 4,118      | 4,853 |
| R²     | 0.9999     | 0.9999 |

- Near-perfect performance, indicating features are highly predictive of LTV  
- Stable results across CV folds

## Purpose
- Showcase an **end-to-end regression pipeline**  
- Demonstrate preprocessing for **mixed numerical and categorical features**  
- Example of **XGBoost regression with cross-validation**

## Usage

1. Clone the repository:

```bash
git clone https://github.com/<your-username>/Customer-Life-Time-Value-Prediction.git

Install dependencies:

pip install pandas numpy scikit-learn xgboost seaborn matplotlib


Update the dataset path in the notebook

Run the notebook to preprocess data, train the pipeline, and evaluate performance
