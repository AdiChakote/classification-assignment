# Cardiovascular Disease Prediction

## Project Overview

This project predicts whether a patient is likely to have cardiovascular disease using supervised machine learning techniques. The objective is to build an accurate binary classification model by applying an industry-standard machine learning workflow, including feature engineering, Weight of Evidence (WOE) encoding, Information Value (IV), multicollinearity analysis, and model evaluation.

---

## Problem Statement

Cardiovascular disease is one of the leading causes of mortality worldwide. Early prediction using patient health indicators can support timely diagnosis and preventive healthcare decisions.

---

## Dataset

The dataset contains demographic, lifestyle, and medical measurements of patients.

### Features

- Age
- Gender
- Height
- Weight
- BMI
- Systolic Blood Pressure (ap_hi)
- Diastolic Blood Pressure (ap_lo)
- Blood Pressure Category
- Cholesterol Level
- Glucose Level
- Smoking Status
- Alcohol Consumption
- Physical Activity

### Target Variable

- **cardio**
  - 0 → No Cardiovascular Disease
  - 1 → Cardiovascular Disease

---

## Project Workflow

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Weight of Evidence (WOE) Encoding
- Information Value (IV) Analysis
- Low IV Feature Removal
- Variance Inflation Factor (VIF) Analysis
- Train-Test Split
- Logistic Regression
- Decision Tree
- Model Evaluation
- Model Comparison

---

## Feature Selection

### Removed Features

- ID
- Age (measured in days)
- Height
- Gender
- Smoking Status
- Alcohol Consumption
- Physical Activity
- Duplicate Blood Pressure Encoded Feature

Features with Information Value less than 0.02 were removed before model training.

---

## Model Performance

### Logistic Regression

| Metric    | Score  |
| --------- | ------ |
| Accuracy  | 73.18% |
| Precision | 76.47% |
| Recall    | 65.98% |
| F1-Score  | 70.84% |

---

### Decision Tree

| Metric    | Score      |
| --------- | ---------- |
| Accuracy  | **73.52%** |
| Precision | 74.81%     |
| Recall    | **69.90%** |
| F1-Score  | **72.27%** |

---

## Final Model

The Decision Tree model was selected as the final model because it achieved the highest overall performance across Accuracy, Recall, and F1-Score.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- ScorecardPy
- Statsmodels
- Jupyter Notebook

---

## Project Structure

```
Cardiovascular_Disease_Prediction/
│
├── data/
│   └── cardiovascular_disease.csv
│
├── notebooks/
│   └── cardiovascular_disease_prediction.ipynb
│
├── README.md
```

---

## Future Improvements

- Hyperparameter optimization using GridSearchCV
- Random Forest Classifier
- XGBoost Classifier
- SHAP-based model interpretability
- Model deployment using Flask or FastAPI
- Interactive dashboard using Streamlit

---

## Author

**Aditya Sunil Chakote**

GitHub:
https://github.com/AdiChakote
