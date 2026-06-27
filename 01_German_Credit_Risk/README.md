# 🏦 German Credit Risk Classification

## 📌 Project Overview

This project predicts whether a loan applicant is a **Good Risk** or **Bad Risk** using the German Credit dataset. The objective is to build a reliable credit risk classification model following an industry-standard machine learning workflow.

The project includes:

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Target Variable Creation
- Weight of Evidence (WOE) Encoding
- Information Value (IV) Analysis
- Multicollinearity Check (VIF)
- Logistic Regression Model
- Decision Tree Model
- Model Evaluation and Comparison

---

## 📂 Project Structure

```
01_German_Credit_Risk/
│
├── data/
│   └── german_credit_data.csv
│
├── notebooks/
│   └── german_credit.ipynb
│
├── output/
│
└── README.md
```

---

## 📊 Dataset

The dataset contains customer demographic and financial information used to assess credit risk.

### Target Variable

- **0 → Good Risk**
- **1 → Bad Risk**

The target variable was created based on the Risk column.

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- ScorecardPy
- Statsmodels
- Scikit-learn

---

## 📈 Project Workflow

### 1. Data Loading

- Loaded the dataset
- Checked dataset shape
- Verified data types

---

### 2. Data Cleaning

- Checked missing values
- Removed unnecessary columns
- Verified duplicate records

---

### 3. Exploratory Data Analysis (EDA)

Performed:

- Dataset information
- Summary statistics
- Target variable distribution
- Numerical feature analysis
- Categorical feature analysis
- Correlation analysis

---

### 4. Feature Engineering

Applied:

- Weight of Evidence (WOE) Encoding
- Information Value (IV) Calculation

Removed weak predictor variables based on Information Value.

---

### 5. Multicollinearity Check

Calculated Variance Inflation Factor (VIF) for all WOE encoded features.

Removed constant or problematic features where necessary before model training.

---

### 6. Model Building

Implemented:

- Logistic Regression
- Decision Tree Classifier

Performed:

- Train-Test Split
- Model Training
- Hyperparameter Tuning using GridSearchCV

---

### 7. Model Evaluation

Compared models using:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- Classification Report

Also analyzed:

- Decision Tree Feature Importance
- Decision Tree Visualization

---

## 📌 Machine Learning Concepts Covered

- Binary Classification
- Feature Engineering
- Weight of Evidence (WOE)
- Information Value (IV)
- Multicollinearity
- Variance Inflation Factor (VIF)
- Logistic Regression
- Decision Tree
- GridSearchCV
- Model Evaluation

---

## 📊 Model Performance

Both Logistic Regression and Decision Tree models were evaluated and compared using multiple classification metrics to identify the most effective model for credit risk prediction.

---

## 🚀 Future Improvements

- Random Forest Classifier
- XGBoost Classifier
- ROC Curve & AUC Analysis
- Probability-Based Credit Scoring
- Model Deployment using Flask or FastAPI

---

## 👨‍💻 Author

**Aditya Sunil Chakote**

GitHub: https://github.com/AdiChakote
