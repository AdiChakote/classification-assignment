# 📊 Bank Marketing Classification

## 📌 Project Overview

This project predicts whether a customer will subscribe to a term deposit based on demographic, financial, and campaign-related information.

The project follows a complete machine learning classification workflow including:

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Weight of Evidence (WOE) Encoding
- Information Value (IV) Analysis
- Multicollinearity Check (VIF)
- Logistic Regression Modeling
- Model Evaluation

---

## 📂 Project Structure

```
02_Bank_Marketing/
│
├── data/
│   └── bank-marketing.csv
│
├── notebooks/
│   └── bank_marketing.ipynb
│
├── output/
│
└── README.md
```

---

## 📊 Dataset

The dataset contains customer information collected during direct marketing campaigns conducted by a Portuguese banking institution.

Target Variable

- **Target = 1** → Customer subscribed to a term deposit
- **Target = 0** → Customer did not subscribe

---

## 🛠 Technologies Used

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

- Loaded dataset
- Checked dataset shape
- Verified data types

---

### 2. Data Cleaning

- Checked missing values
- Removed unnecessary columns (if applicable)
- Converted target variable into binary format

---

### 3. Exploratory Data Analysis (EDA)

Performed:

- Dataset information
- Summary statistics
- Class distribution
- Numerical feature analysis
- Categorical feature analysis
- Correlation analysis

---

### 4. Feature Engineering

Applied:

- Weight of Evidence (WOE) Encoding
- Information Value (IV) Calculation

Removed weak predictor variables based on IV.

---

### 5. Multicollinearity Check

Calculated Variance Inflation Factor (VIF) for all WOE encoded features.

Removed features only if necessary based on:

- High VIF
- Constant features
- Duplicate information

---

### 6. Model Building

Built Logistic Regression classifier.

Performed:

- Train-Test Split
- Model Training
- Prediction

---

### 7. Model Evaluation

Evaluated model using:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- Classification Report
- ROC Curve
- AUC Score

---

## 📌 Key Concepts Used

- Binary Classification
- Weight of Evidence (WOE)
- Information Value (IV)
- Logistic Regression
- Multicollinearity
- Variance Inflation Factor (VIF)
- Feature Selection
- Model Evaluation Metrics

---

## 📊 Results

The model was evaluated using multiple classification metrics to measure predictive performance and business usefulness.

---

## 🚀 Future Improvements

- Hyperparameter Tuning
- Decision Tree
- Random Forest
- XGBoost
- Feature Importance Analysis
- Model Deployment using Flask or FastAPI

---

## 👨‍💻 Author

**Aditya Sunil Chakote**

GitHub:
https://github.com/AdiChakote
