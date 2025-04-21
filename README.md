# 💸 Financial Fraud Detection Using Machine Learning

Detecting fraudulent financial transactions is a critical task in the age of digital payments. This project uses **EDA** and **supervised machine learning** techniques to analyze transaction data and build models that can effectively detect fraud.

---

## 📁 Dataset

The dataset used in this project is from Kaggle:  
🔗 [PaySim Fraud Simulation Dataset](https://www.kaggle.com/datasets/ealaxi/paysim1)

This dataset simulates mobile money transactions and includes both fraudulent and non-fraudulent cases.

---

## 📊 Project Objectives

- Perform **Exploratory Data Analysis (EDA)** to understand transaction patterns.
- Detect and handle **outliers** using IQR and Z-score methods.
- Apply **data cleaning** techniques: remove duplicates, encode categorical features, and scale numerical values.
- Evaluate and compare **multiple machine learning models**:
  - K-Nearest Neighbors (KNN)
  - Support Vector Machine (SVM)
  - Decision Tree
  - Logistic Regression
- Identify the best-performing model and extract insights on fraud behavior.

---

## 🔍 Key EDA Insights

- **Highly Skewed Distributions**: Most transactions are small, but some large amounts skew the data.
- **Fraud Patterns**: Fraudulent transactions usually bring the sender’s balance close to zero.
- **Recipient Anomalies**: Recipient balances in fraud cases often behave unnaturally, indicating possible money laundering or scams.
- **Correlations**:
  - Transaction type has a strong positive correlation with fraud.
  - Some balance columns are highly correlated and can be dropped to reduce redundancy.

---

## 🧹 Data Cleaning & Preprocessing

- ✅ No missing values
- ✅ Duplicates removed
- ✅ Outliers handled using **Winsorization**
- ✅ Label Encoding used for transaction type
- ✅ Feature scaling using **Min-Max** and **Z-score normalization**

---

## 📈 Model Performance

| Model            | Accuracy | Precision | Recall | F1 Score |
|------------------|----------|-----------|--------|----------|
| KNN (k=5)        | 96.07%   | 95.8%     | 95.6%  | 95.7%    |
| SVM (RBF Kernel) | 96.10%   | 96.0%     | 95.9%  | 96.0%    |
| Decision Tree    | 96.30%   | 96.5%     | 96.2%  | 96.3%    |
| Logistic Reg (L2)| 95.50%   | 95.3%     | 95.0%  | 95.1%    |

🔑 **Best Accuracy**: Decision Tree  
⚖️ **Best Balanced**: SVM (RBF Kernel)  
⚡ **Most Efficient**: Decision Tree (fast training & high performance)

---

## 📌 Conclusion

This project demonstrates how effective data analysis and machine learning can be in detecting suspicious transactions and preventing fraud. By analyzing patterns, optimizing models, and identifying high-risk features, this approach can help build smarter fraud detection systems in real-world financial platforms.
