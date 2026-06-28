# Employee Attrition Prediction

## Project Overview

This project predicts whether an employee is likely to leave the organization using Machine Learning classification techniques.

The project follows an industry-level machine learning workflow including data preprocessing, roll rate bucket creation, target creation, Weight of Evidence (WOE) encoding, Information Value (IV), Variance Inflation Factor (VIF), Logistic Regression, Decision Tree, and hyperparameter tuning using GridSearchCV.

---

## Dataset Information

- Dataset: Employee Attrition
- Total Records: 1,470
- Target Variable: Employee Attrition

Target Classes:

- 0 → No Attrition
- 1 → Attrition

---

## Project Workflow

### 1. Data Loading

- Load dataset using Pandas
- Display first five records
- Display dataset information
- Check dataset shape

### 2. Data Cleaning

- Check duplicate records
- Remove duplicate records
- Check missing values
- Handle missing values (if any)

### 3. Exploratory Data Analysis (EDA)

- Statistical summary
- Numerical feature analysis
- Categorical feature analysis
- Target distribution

### 4. Roll Rate Bucket Creation

Created tenure-based buckets using the **YearsAtCompany** feature.

Example buckets:

- 0–2 Years
- 3–5 Years
- 6–10 Years
- 10+ Years

### 5. Target Creation

Created binary target variable.

- Attrition = No → Target = 0
- Attrition = Yes → Target = 1

### 6. Weight of Evidence (WOE)

- Performed WOE encoding for predictor variables.

### 7. Information Value (IV)

- Calculated Information Value for all features.
- Removed weak predictor variables based on IV analysis.

### 8. Multicollinearity Analysis (VIF)

- Calculated Variance Inflation Factor.
- Removed constant and highly correlated features.
- Recalculated VIF.

### 9. Train-Test Split

- Training Data: 75%
- Testing Data: 25%

### 10. Logistic Regression

Performed hyperparameter tuning using GridSearchCV.

Evaluation Metrics:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- Classification Report

### 11. Decision Tree

Performed hyperparameter tuning using GridSearchCV.

Evaluation Metrics:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- Classification Report

### 12. Model Comparison

Compared both models using:

- Accuracy
- Precision
- Recall
- F1 Score

---

## Model Performance

### Logistic Regression

- Accuracy: **86.68%**
- Precision: **63.16%**
- Recall: **40.68%**
- F1 Score: **49.48%**

### Decision Tree

- Accuracy: **82.07%**
- Precision: **41.03%**
- Recall: **27.12%**
- F1 Score: **32.65%**

---

## Final Conclusion

Both models were trained after performing data preprocessing, feature engineering, WOE encoding, IV-based feature selection, VIF analysis, and hyperparameter tuning.

Logistic Regression outperformed Decision Tree across all evaluation metrics, including Accuracy, Precision, Recall, and F1 Score. Therefore, Logistic Regression is selected as the final model for predicting employee attrition in this project.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- ScorecardPy
- Statsmodels

---

## Project Structure

```
04_Employee_Attrition/
│
├── data/
│   └── employee_attrition.csv
│
├── notebooks/
│   └── employee_attrition.ipynb
│
├── output/
│
└── README.md
```

---

## Learning Outcomes

- Data Cleaning
- Duplicate Removal
- Missing Value Handling
- Roll Rate Bucket Creation
- Target Creation
- Weight of Evidence (WOE)
- Information Value (IV)
- Variance Inflation Factor (VIF)
- Feature Selection
- Logistic Regression
- Decision Tree
- Hyperparameter Tuning using GridSearchCV
- Model Evaluation
- Decision Tree Visualization
- Feature Importance

## Author

**Aditya Sunil Chakote**

GitHub:
https://github.com/AdiChakote
