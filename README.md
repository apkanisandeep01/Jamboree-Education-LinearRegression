Below is a **clean, simple, easy-to-understand `README.md`** that you can **copy and paste directly into GitHub**.

---

# Graduate Admission Prediction (Jamboree Case Study)

## Project Overview

This project builds a **machine learning regression model** to predict the **probability of admission to Ivy League universities** based on a student's academic profile.

The analysis is based on a dataset provided by **Jamboree Education**, which helps students estimate their chances of getting admission to top universities abroad. 

The goal of the project is to understand **which factors influence admission chances** and build a **predictive model** using regression techniques.

---

# Problem Statement

Students applying for graduate programs often want to know their **probability of admission**.

Using student profile data such as:

* GRE Score
* TOEFL Score
* University Rating
* SOP Strength
* LOR Strength
* CGPA
* Research Experience

we build a model that predicts the **Chance of Admit (0–1 probability)**.

---

# Dataset Information

The dataset contains **500 student records and 9 features**. 

### Features

| Feature           | Description                                |
| ----------------- | ------------------------------------------ |
| GRE Score         | Graduate Record Exam score (out of 340)    |
| TOEFL Score       | English proficiency score (out of 120)     |
| University Rating | Rating of university (1–5)                 |
| SOP               | Strength of Statement of Purpose           |
| LOR               | Strength of Letters of Recommendation      |
| CGPA              | Undergraduate GPA (out of 10)              |
| Research          | Research experience (0 = No, 1 = Yes)      |
| Chance of Admit   | Probability of admission (Target variable) |

---

# Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* Statsmodels

---

# Project Workflow

1. Data Loading
2. Data Cleaning
3. Exploratory Data Analysis (EDA)
4. Feature Engineering
5. Correlation Analysis
6. Model Training
7. Model Evaluation
8. Model Interpretation

---

# Exploratory Data Analysis (EDA)

EDA was performed to understand relationships between variables.

### Key Findings

* **GRE Score, TOEFL Score, and CGPA** show strong positive correlation with admission chances.
* **CGPA is the most influential predictor**.
* Students with **research experience** have higher admission probability.
* Higher **university ratings and stronger LOR/SOP** also increase admission chances.

The dataset contains **no missing values and no duplicate records**, making it clean and reliable for modeling. 

---

# Model Building

Three regression models were trained:

* Linear Regression
* Ridge Regression
* Lasso Regression

The dataset was split into:

* **70% Training Data**
* **30% Testing Data**

Data was also **standardized using StandardScaler** before model training.

---

# Model Performance

| Metric      | Value |
| ----------- | ----- |
| MAE         | 0.05  |
| RMSE        | 0.07  |
| R² Score    | 0.81  |
| Adjusted R² | 0.81  |

All three models performed similarly, indicating **stable and reliable predictions**. 

---

# Feature Importance

After handling **multicollinearity using VIF**, the most important predictors were identified as:

1. **CGPA (Strongest Predictor)**
2. **Research Experience**

Other features such as GRE and TOEFL were correlated but less impactful after removing redundancy.

---

# Key Insights

* **CGPA has the strongest impact on admission chances.**
* Students with **research experience have higher admission probability.**
* Strong **letters of recommendation and university ratings** improve chances.
* GRE and TOEFL scores positively influence admission probability.

---



# Final Conclusion

The regression model successfully predicts the **chance of admission** with an **R² score of 0.81**, indicating strong predictive capability.

Among all factors, **CGPA and Research Experience are the most important predictors** for graduate admissions.

---

