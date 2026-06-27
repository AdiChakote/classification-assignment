# Adult Income Census Classification

## Project Overview

This project predicts whether an individual's annual income is less than or equal to $50K or greater than $50K using Machine Learning classification techniques.

The project follows an industry-level credit risk style workflow including data preprocessing, target creation, Weight of Evidence (WOE) encoding, Information Value (IV), multicollinearity analysis using VIF, Logistic Regression, and Decision Tree with hyperparameter tuning using GridSearchCV.

---

## Dataset Information

- Dataset: Adult Income Census
- Records: 32,537
- Features: 15
- Target Variable: Income Level

Target Classes:

- 0 → Income ≤ 50K
- 1 → Income > 50K

---

## Project Workflow

### 1. Data Loading

- Load dataset using Pandas
- Display dataset information
- Check shape and data types

### 2. Data Cleaning

- Removed duplicate records
- Replaced '?' values with NaN
- Handled missing values
- Verified missing values

### 3. Exploratory Data Analysis (EDA)

- Statistical summary
- Distribution analysis
- Categorical feature analysis

### 4. Roll Rate Bucket Creation

Created income-based buckets using working hours.

Example:

- 0–20 Hours
- 21–40 Hours
- 41–60 Hours
- 60+ Hours

### 5. Target Creation

Created binary target variable.

- Income ≤ 50K → Target = 0
- Income > 50K → Target = 1

### 6. Weight of Evidence (WOE)

- Performed WOE encoding on all predictor variables.

### 7. Information Value (IV)

- Calculated IV for all features.
- Removed weak predictor variables based on IV.

### 8. Multicollinearity Analysis (VIF)

- Calculated Variance Inflation Factor.
- Removed constant features.
- Removed highly correlated features.
- Recalculated VIF.

### 9. Train-Test Split

- 75% Training Data
- 25% Testing Data

### 10. Logistic Regression

- Hyperparameter tuning using GridSearchCV
- Model Evaluation

Metrics:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- Classification Report

### 11. Decision Tree

- Hyperparameter tuning using GridSearchCV
- Decision Tree Visualization
- Feature Importance

Metrics:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- Classification Report

### 12. Model Comparison

Compared Logistic Regression and Decision Tree using:

- Accuracy
- Precision
- Recall
- F1 Score

---

## Model Performance

### Logistic Regression

- Accuracy: 73.93%
- Precision: 61.35%
- Recall: 30.83%
- F1 Score: 41.03%

### Decision Tree

- Accuracy: 74.49%
- Precision: 59.84%
- Recall: 40.52%
- F1 Score: 48.32%

---

## Final Conclusion

Both models were trained using WOE-transformed features after feature selection through Information Value (IV) and multicollinearity analysis using VIF.

Although Logistic Regression achieved slightly higher Precision, the Decision Tree model produced higher Accuracy, Recall, and F1 Score. Since F1 Score provides a balanced measure of Precision and Recall, Decision Tree demonstrated better overall classification performance.

Therefore, Decision Tree is selected as the final model for this project.

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
03_Adult_income_Census/
│
├── data/
│   └── adult.csv
│
├── notebooks/
│   └── adult_income_census.ipynb
│
├── output/
│
└── README.md
```

---

## Learning Outcomes

- Data Cleaning
- Missing Value Treatment
- Duplicate Removal
- Roll Rate Target Creation
- Weight of Evidence (WOE)
- Information Value (IV)
- Variance Inflation Factor (VIF)
- Feature Selection
- Logistic Regression
- Decision Tree
- Hyperparameter Tuning using GridSearchCV
- Model Evaluation
- Feature Importance
- Decision Tree Visualization

## Author

**Aditya Sunil Chakote**

GitHub:
https://github.com/AdiChakote
