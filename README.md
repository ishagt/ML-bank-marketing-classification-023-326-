# Bank-Marketing-Dataset-Classification-Project
Machine learning classification assignment
# Bank Marketing Term Deposit Prediction

An end-to-end Machine Learning classification project to predict whether a client will subscribe to a bank term deposit based on the **Bank Marketing Dataset**. 

---

##  Project Overview
This repository contains a comprehensive classification workflow evaluated on the Bank Marketing dataset. The goal is to build a predictive model that optimizes marketing campaigns by accurately identifying potential subscribers.

### **Key Tasks Completed:**
* **Exploratory Data Analysis (EDA):** Handled dataset checks, observed feature distributions, and evaluated target balance.
* **Data Preprocessing:** Imputed `'unknown'` missing values, encoded categorical strings via binary and One-Hot encoding, and handled feature scaling using `MinMaxScaler`.
* **Model Training:** Built and compared **Support Vector Machines (SVM)**, **k-Nearest Neighbors (kNN)**, and **Decision Tree** models.
* **Hyperparameter Tuning:** Optimized performance using `GridSearchCV`.

---

##  Evaluation & Model Performance

The classification models were evaluated using **Accuracy, Precision, Recall, and F1-Score**. 

| Model | Accuracy | Precision | Recall | F1-Score |
| :--- | :--- | :--- | :--- | :--- |
| **k-Nearest Neighbors (kNN)** | [Insert Score] | [Insert Score] | [Insert Score] | [Insert Score] |
| **Decision Tree (Baseline)** | [Insert Score] | [Insert Score] | [Insert Score] | [Insert Score] |
| **SVM (Baseline)** | [Insert Score] | [Insert Score] | [Insert Score] | [Insert Score] |
| **Tuned SVM (Best)** | [Insert Score] | [Insert Score] | [Insert Score] | [Insert Score] |

### **Key Findings & Insights:**
* **The Winner:** The **Tuned Support Vector Machine** yielded the highest performance metrics. 
* **Why it won:** SVM with an RBF kernel successfully mapped complex, non-linear boundaries in our high-dimensional, post-encoded feature space. 
* **The Runners-up:** kNN struggled slightly due to the *curse of dimensionality* (the distance metrics warp when handling numerous features), while the unpruned baseline Decision Tree showed signs of overfitting.

## 🛠️ Technologies & Libraries Used
* **Language:** Python
* **Libraries:** Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn, Kagglehub
