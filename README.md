# Churn-Prediction


## 📌 Project Overview
Customer churn occurs when customers stop doing business with a company. Discovering that a customer is about to leave allows businesses to take proactive measures (e.g., targeted offers, discounts, or feedback loops) to retain them. 

This repository contains an end-to-end Machine Learning pipeline designed to predict customer churn based on historical customer data (demographics, account information, and usage patterns).

---

## 📊 Dataset
The model is trained on a typical customer retention dataset (e.g., Telco Churn Dataset). Key features included:
* **Demographics:** Gender, age, partner, and dependent status.
* **Services:** Phone service, multiple lines, internet service, online security, streaming, etc.
* **Account Info:** Contract type, payment method, paperless billing, monthly charges, and total charges.
* **Target Variable:** `Churn` (Yes/No).

---

## 🛠️ Tech Stack & Libraries
* **Language:** Python
* **Data Analysis:** Pandas, NumPy
* **Visualization:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-Learn, XGBoost / LightGBM (Optional)
* **Environment:** Jupyter Notebook / Google Colab

---

## 🚀 Key Features & Workflow

### 1. Data Preprocessing & EDA
* Handled missing values and corrected data types (e.g., converting `TotalCharges` to numeric).
* Encoded categorical variables using **One-Hot Encoding** and **Label Encoding**.
* Addressed class imbalance using techniques like **SMOTE** (Synthetic Minority Over-sampling Technique).
* Visualized feature correlations and churn distributions.

### 2. Feature Engineering
* Scaled numerical features using `StandardScaler`.
* Selected high-impact features using correlation matrices and feature importance rankings.

### 3. Model Training & Evaluation
Multiple classification models were trained and compared:
* Logistic Regression
* Random Forest Classifier
* XGBoost Classifier

Models were evaluated using **ROC-AUC**, **Precision**, **Recall**, and **F1-Score** to ensure minimizing false negatives (missing actual churning customers).

---

## 📈 Results Summary

| Model | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Logistic Regression | 79.2% | 0.65 | 0.58 | 0.61 | 0.83 |
| Random Forest | 81.5% | 0.71 | 0.62 | 0.66 | 0.85 |
| **XGBoost (Best)** | **83.1%** | **0.74** | **0.68** | **0.71** | **0.88** |

*Note: Replace these numbers with your actual project results.*

---

## ⚙️ Installation & Usage

### Prerequisites
Make sure you have Python 3.8+ installed.
