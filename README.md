# Customer Life Time Value Prediction

This repository contains a **machine learning pipeline** to predict **customer Lifetime Value (LTV)** for a digital wallet dataset. It demonstrates an end-to-end workflow from data preprocessing to model evaluation, including cross-validation, feature transformations, and explainable AI using SHAP.

## Key Features

### Data Preprocessing
- Numerical features transformed using **Yeo-Johnson** for normality and **Standard Scaling**  
- `Income_Level` column encoded using **Ordinal Encoding**  
- Other categorical features encoded using **One-Hot Encoding**

### Modeling
- **XGBoost Regressor** used for regression  
- Pipeline ensures consistent preprocessing and model fitting

### Explainability
- **SHAP (SHapley Additive exPlanations)** used to interpret model predictions  
- Provides feature-level contribution for each prediction  
- Helps understand which features **increase or decrease predicted LTV**, improving trust in the model

### Evaluation
- Train/test metrics: **MSE**, **RMSE**, **R²**  
- **K-Fold Cross-Validation** for robust performance assessment  
- Feature importance extraction supported

## Results

| Metric | Train | Test |
|--------|-------|------|
| MSE    | 17,045,086.63 | 23,433,368.69 |
| RMSE   | 4,128.57      | 4,840.80      |
| R²     | 0.9999        | 0.9999        |

- Near-perfect performance, indicating features are highly predictive of LTV  
- Stable results across CV folds  

## Purpose
- Showcase an **end-to-end regression pipeline**  
- Demonstrate preprocessing for **mixed numerical and categorical features**  
- Example of **XGBoost regression with cross-validation and explainability**

## Usage

1. Clone the repository:

```bash
git clone https://github.com/<your-username>/Customer-Life-Time-Value-Prediction.git
```
Install dependencies:
```bash
pip install pandas numpy scikit-learn xgboost shap seaborn matplotlib
```

Update the dataset path in the notebook.

Run the notebook to preprocess data, train the pipeline, evaluate performance, and generate SHAP explainability plots.
