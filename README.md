# Final_Project_ML

# 📊 Bank Marketing Term Deposit Prediction

This project involves building a machine learning model to predict whether a customer will subscribe to a term deposit based on their personal, contact, and campaign-related information.

## 📌 Objective

To develop a predictive model using customer data that can classify whether a customer will subscribe to a term deposit.

---

## 🧩 Dataset Overview

- **Source**: UCI Bank Marketing Dataset (bank csv.csv)
- **Target Variable**: `subscribed` (yes/no)
- **Features**:
  - Personal: `age`, `job`, `marital`, `education`
  - Contact: `contact`, `day`, `month`, `duration`
  - Campaign-related: `campaign`, `pdays`, `previous`, `poutcome`

---

## 🔧 Steps Performed

### 1. **Data Cleaning & Preprocessing**
- Removed duplicates
- Handled missing values
- Detected and treated outliers
- Encoded categorical variables using Label Encoding and One-Hot Encoding

### 2. **Data Visualization**
- Bar plots and histograms to explore feature distributions
- Correlation heatmaps to analyze relationships
- Visual checks for class imbalance

### 3. **Balancing the Dataset**
- Addressed class imbalance using **SMOTE** (Synthetic Minority Over-sampling Technique)

### 4. **Model Building**
- Separated input features (`X`) and target (`y`)
- Split the data (80% training / 20% testing)
- Trained two models:
  - Logistic Regression
  - Random Forest Classifier

### 5. **Model Evaluation**
- Used the following metrics:
  - Accuracy Score
  - Confusion Matrix
  - Classification Report (Precision, Recall, F1-score)
  - ROC Curve
  - ROC-AUC Score

---

## ✅ Results Summary

- **Logistic Regression**:
  - Moderate accuracy
  - Lower recall for positive class (subscribed = yes)

- **Random Forest**:
  - Higher accuracy
  - Better balance between precision and recall
  - Higher ROC-AUC score

🔍 **Conclusion**:  
Random Forest performed better than Logistic Regression and is the recommended model for predicting customer subscription behavior.

---

## 📂 Files Included

- `Final_Project.ipynb` – Complete notebook with cleaning, visualization, model building, and evaluation
- `README.md` – This file

---

## 💡 Final Conclusion

This project shows how proper preprocessing, balancing, and model selection can lead to a reliable machine learning pipeline to predict real-world customer behavior.
