# 📈 Telecom Customer Churn Prediction

A data science project to predict customer churn using behavioral metrics from a telecom provider. The project covers end-to-end steps from data exploration and feature engineering to model training and interpretation — with actionable business insights.

---

## 📌 Project Overview

Customer churn is a key concern in the telecom industry due to its direct impact on revenue and customer lifetime value. In this project, we developed a machine learning model that classifies customers as likely to churn or not, based on usage patterns, demographics, and service interactions.

---

## 🧠 Objectives

- Analyze telecom customer behavior through exploratory data analysis (EDA)
- Identify key drivers of churn
- Build and evaluate classification models
- Provide business recommendations based on model outputs
- Prepare the model for deployment and integration into CRM systems

---

## 🗂️ Dataset Overview

The dataset includes:
- Customer demographics
- Call duration and frequency
- SMS usage
- Account status and complaints
- Subscription length and customer value

📁 Source: Provided as `customer_churn.csv` (confidential)

---

## 🔍 Exploratory Insights

- Younger age groups favor SMS over calls
- Customers with complaints, short subscription history, and low usage are at higher churn risk
- High-value customers with stable, long-term usage patterns are more loyal

📊 Key Features Identified:
- `Status_1`, `Status_2` (account flags)
- `Seconds of Use`, `Frequency of Use`
- `Customer Value`, `Subscription Length`
- `Complaint`, `Distinct Called Numbers`

---

## 🤖 Model Comparison

| Metric (Churn Class) | Logistic Regression | Random Forest |
|----------------------|---------------------|---------------|
| Precision            | 51.0%               | **88.2%**     |
| Recall               | **89.9%**           | 81.1%         |
| F1-score             | 65.0%               | **84.5%**     |
| Accuracy             | 84.9%               | **95.3%**     |

✅ **Random Forest** chosen as final model for deployment due to its superior balance of precision and recall.

---

## 📊 Confusion Matrix (Random Forest)

![Confusion Matrix](path_to_your_confusion_matrix_image.png)

- **True Positives (120)**: Correctly predicted churners  
- **False Positives (16)**: Non-churners wrongly flagged  
- **False Negatives (28)**: Missed churners  
- **True Negatives (781)**: Correctly predicted non-churners

---

## 🧠 Feature Importance

![Feature Importance](path_to_your_feature_importance_plot.png)

Key predictors: service status, call duration, engagement level, and customer lifecycle.

---

## 🚀 Deployment Plan

- Save model using `joblib`
- Deploy with a simple Streamlit or Flask API
- Weekly scoring pipeline + CRM integration for automated retention targeting

---

## 💡 Business Recommendations

- Focus on customers with complaints, low recent usage, or short tenure
- Launch early-intervention campaigns for new users
- Use prediction scores to prioritize support and loyalty rewards

---

## 🧾 Tools Used

- Python (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn)
- Jupyter Notebook
- Machine Learning: Logistic Regression, Random Forest
- Streamlit (for future deployment)

---

## 📈 Results Summary

This project demonstrates how machine learning can turn raw behavioral data into real business impact. By predicting churn with high accuracy, companies can intervene earlier and reduce customer loss.

> 🔧 Ready to scale, interpret, and deploy in a business setting.

---
