# Bank-Marketing-Dataset-Classification-Project
Machine learning classification assignment

# Bank Marketing Term Deposit Prediction

An end-to-end Machine Learning classification project to predict whether a client will subscribe to a bank term deposit based on the **Bank Marketing Dataset**. 

## Project Overview
This repository contains a comprehensive classification workflow evaluated on the Bank Marketing dataset. The goal is to build a predictive model that optimizes marketing campaigns by accurately identifying potential subscribers.

### **Key Tasks Completed:**
* **Exploratory Data Analysis (EDA):** Evaluated data distributions, verified client age groupings, and checked for class balance.
* **Data Preprocessing:** Handled missing data by imputing `'unknown'` values, removed structural duplicates, encoded categorical features using One-Hot encoding, and applied `MinMaxScaler`.
* **Model Training:** Constructed and benchmarked **Support Vector Machines (SVM)**, **k-Nearest Neighbors (kNN)**, and a **Decision Tree** baseline.
* **Hyperparameter Tuning:** Tuned and optimized parameters using `GridSearchCV`.


## Evaluation & Model Performance

The classification models were evaluated using **Accuracy, Precision, Recall, and F1-Score** on the testing set.

| Model | Accuracy | Precision | Recall | F1-Score |
| :--- | :---: | :---: | :---: | :---: |
| **Tuned Support Vector Machine** | **0.8339** | **0.8166** | **0.8374** | **0.8269** |
| **Support Vector Machine (Baseline)** | 0.8245 | 0.8165 | 0.8119 | 0.8142 |
| **Decision Tree** | 0.7716 | 0.7528 | 0.7713 | 0.7619 |
| **k-Nearest Neighbors (kNN)** | 0.7053 | 0.7193 | 0.6200 | 0.6660 |

### **Key Findings & Insights:**
* **The Winner:** The **Tuned Support Vector Machine** performed best across all primary performance indicators, achieving the highest accuracy (~83.4%) and a balanced F1-Score (~82.7%).
* **Why it won:** SVM with an RBF kernel handles non-linear boundaries smoothly, finding an optimal dividing boundary in high-dimensional feature spaces created during One-Hot encoding.
* **The Runners-up:** * **k-Nearest Neighbors** struggled noticeably (62% Recall), primarily due to the *curse of dimensionality* where distance metrics break down when too many columns are involved.
  * The untuned **Decision Tree** suffered from slight overfitting and rigid boundaries, reducing its capacity to generalize effectively on unseen test entries.
