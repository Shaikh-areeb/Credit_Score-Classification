# 🏦 Credit Score Classification

This project predicts the **credit score category** of individuals (e.g., **Poor, Standard, Good**) based on financial and demographic factors.  
It involves **data preprocessing, exploratory data analysis (EDA), feature engineering, and machine learning model building** to accurately classify applicants’ creditworthiness.

---

## 📌 Project Overview
- **Objective**: Build a machine learning model to classify applicants into credit score categories.  
- **Approach**:
  - Performed **EDA** to understand distributions, correlations, and outliers.  
  - Conducted **feature engineering** (handling missing values, encoding categorical features, scaling numeric features).  
  - Trained and compared multiple models.  
  - Finalized **Random Forest** as the best-performing model.  

---

## 📊 Dataset Features
The dataset includes both **financial** and **demographic** attributes:

| Feature                  | Description |
|---------------------------|-------------|
| Annual_Income             | Yearly income of the applicant |
| Monthly_Inhand_Salary     | Monthly salary received |
| Num_Bank_Accounts         | Number of bank accounts held |
| Num_Credit_Card           | Number of credit cards owned |
| Interest_Rate             | Interest rate on loans |
| Num_of_Loan               | Total number of loans |
| Delay_from_due_date       | Average delay in payments (days) |
| Num_of_Delayed_Payment    | Number of delayed payments |
| Credit_Mix                | Type of credit (Good/Bad/Standard) |
| Outstanding_Debt          | Current outstanding debt |
| Credit_History_Age        | Age of credit history |
| Monthly_Balance           | Monthly account balance |

---

## 🔍 Exploratory Data Analysis (EDA)
- Distribution of **income, debt, and credit history age** was analyzed.  
- Relationship between **delayed payments and credit score** was identified.  
- Outliers were examined but retained as they represent real-world financial behavior.  

---

## 🤖 Model Building
- Various ML models were tested, including Logistic Regression, Decision Trees, and Random Forest.  
- **Random Forest Classifier** gave the best performance with balanced precision, recall, and f1-score.  

### ✅ Random Forest Performance

| Metric       | Good | Poor | Standard | Average |
|--------------|------|------|----------|---------|
| Precision    | 0.77 | 0.79 | 0.82     | 0.80    |
| Recall       | 0.76 | 0.83 | 0.81     | 0.80    |
| F1-Score     | 0.77 | 0.81 | 0.82     | 0.80    |
| **Accuracy** |      |      |          | **0.81** |

---

## 📈 Feature Importance (Top Predictors)

| Rank | Feature                | Importance (%) |
|------|-------------------------|----------------|
| 1    | Outstanding_Debt        | 15.0 |
| 2    | Credit_History_Age      | 13.4 |
| 3    | Monthly_Balance         | 10.9 |
| 4    | Interest_Rate           | 9.9 |
| 5    | Credit_Mix              | 9.3 |
| 6    | Delay_from_due_date     | 9.0 |
| 7    | Annual_Income           | 6.6 |
| 8    | Monthly_Inhand_Salary   | 6.7 |
| 9    | Num_of_Delayed_Payment  | 6.4 |
| 10   | Num_Credit_Card         | 5.2 |
| 11   | Num_Bank_Accounts       | 4.0 |
| 12   | Num_of_Loan             | 3.6 |

---

## 🚀 Tech Stack
- **Python**
- **Pandas, NumPy** (Data Processing)  
- **Matplotlib, Seaborn** (EDA & Visualization)  
- **Scikit-learn** (Modeling & Evaluation)  

---

## 📌 Key Insights
- **Outstanding debt** and **credit history age** are the strongest predictors of credit score.  
- **Payment delays** and **credit mix** significantly impact creditworthiness.  
- Achieved **81% accuracy** with a Random Forest model.  

---
