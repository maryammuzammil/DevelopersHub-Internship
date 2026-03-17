# DevelopersHub Corporation — Data Science & Analytics Internship

**Intern:** Maryam Muzammil  
**Program:** Data Science & Analytics Internship  
**Organization:** DevelopersHub Corporation  

---

## Overview

This repository contains all 5 tasks completed as part of the Data Science & Analytics Internship at DevelopersHub Corporation. Each task involves real-world datasets, data cleaning, exploratory data analysis, machine learning model building, and evaluation.

**Tools & Libraries:** Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, KaggleHub

---

## Task 1: Exploring and Visualizing a Simple Dataset

**Objective:**
Understand how to read, summarize, and visualize a dataset using the Iris dataset.

**Approach:**
- Loaded the Iris dataset using Seaborn
- Performed data inspection using `.shape`, `.info()`, and `.describe()`
- Created scatter plots, histograms, box plots, and a correlation heatmap
- Trained a Random Forest Classifier to evaluate feature separability

**Results & Insights:**
- Dataset is perfectly balanced with 50 samples per species and no missing values
- Petal length and petal width are the strongest features for classification
- Setosa is clearly separable from the other two species
- Random Forest achieved high classification accuracy on this dataset

---

## Task 2: Credit Risk Prediction

**Objective:**
Predict whether a loan applicant is likely to default on a loan.

**Dataset:** Loan Prediction Dataset (Kaggle)

**Approach:**
- Handled missing values using mode (categorical) and median (numerical)
- Visualized loan amounts, income distribution, and approval rates
- Trained Logistic Regression and Decision Tree classifiers
- Evaluated using accuracy score and confusion matrix

**Results & Insights:**
- Credit history is the most important factor for loan approval
- Graduates have a significantly higher loan approval rate
- Applicants with higher income tend to receive higher loan amounts
- Logistic Regression performed consistently well on this dataset

---

## Task 3: Customer Churn Prediction (Bank Customers)

**Objective:**
Identify customers who are likely to leave the bank.

**Dataset:** Churn Modelling Dataset (Kaggle)

**Approach:**
- Dropped irrelevant columns (RowNumber, CustomerId, Surname)
- Applied Label Encoding for Gender and One-Hot Encoding for Geography
- Trained Logistic Regression and Random Forest classifiers
- Analyzed feature importance to understand churn drivers

**Results & Insights:**
- Overall churn rate is around 20%
- Age is the most important predictor — older customers churn more
- Customers from Germany have a noticeably higher churn rate
- Customers with higher balance but fewer products are more likely to leave
- Random Forest outperformed Logistic Regression due to non-linear patterns

---

## Task 4: Predicting Insurance Claim Amounts

**Objective:**
Estimate medical insurance claim amounts based on personal data.

**Dataset:** Medical Cost Personal Dataset (Kaggle)

**Approach:**
- Encoded categorical features (sex, smoker, region) using Label Encoding
- Visualized how BMI, age, and smoking status affect charges
- Trained Linear Regression and Random Forest Regressor
- Evaluated using MAE, RMSE, and R2 Score

**Results & Insights:**
- Smoking status is the single most influential factor — smokers pay far higher charges
- Age and BMI both have a strong positive relationship with insurance charges
- Customers who are both obese (BMI > 30) and smokers have the highest charges
- Region and gender have relatively little impact on charges
- Random Forest achieved a better R2 score and lower error than Linear Regression

---

## Task 5: Personal Loan Acceptance Prediction

**Objective:**
Predict which customers are likely to accept a personal loan offer.

**Dataset:** Bank Marketing Dataset — UCI Machine Learning Repository (Kaggle)

**Approach:**
- Performed data exploration on age, job, marital status, and education
- Applied Label Encoding to all categorical features
- Trained Logistic Regression and Decision Tree classifiers
- Analyzed feature importance to identify key customer groups

**Results & Insights:**
- The dataset is imbalanced — most customers did not accept the loan offer
- Students and retired customers showed higher acceptance rates
- Customers contacted via cellular responded better than telephone
- Duration of last contact and number of previous contacts are strong predictors
- Logistic Regression performed well given the linear nature of the decision boundary

---

## Repository Structure

```
DevelopersHub-Internship/
├── Task1_Iris_EDA.ipynb
├── Task2_Credit_Risk_Prediction.ipynb
├── Task3_Customer_Churn_Prediction.ipynb
├── Task4_Insurance_Claims_Prediction.ipynb
├── Task5_Loan_Acceptance_Prediction.ipynb
└── README.md
```

---

## How to Run

1. Open any notebook in Google Colab or Jupyter Notebook
2. Install required library if not already available:
   ```
   pip install kagglehub
   ```
3. Run all cells from top to bottom
4. Datasets are downloaded automatically via `kagglehub` (Tasks 2–5) or loaded via `seaborn` (Task 1)

---

*Completed as part of the DevelopersHub Corporation Data Science & Analytics Internship Program.*
