# Credit-Card-Fraud-Detection
This project tackles the real-world problem of detecting fraudulent credit card transactions using machine learning. Given the extreme class imbalance (fraudulent transactions represent only 0.17% of the data), the project carefully preprocesses, analyzes, and models the data using various classification algorithms.

## 📌 Objective
Build and compare the performance of multiple machine learning models to accurately classify credit card transactions as fraudulent (1) or non-fraudulent (0).

## 📂 Dataset
1. Source: creditcard.csv (Kaggle)
2. Total records: 284,807
3. Fraudulent transactions: 492 (0.17%)
4. Features: 30 (V1–V28 are anonymized PCA components, plus Amount, Time, and Class)

## 🔧 Steps Followed
Data Import & Preprocessing
1. Removed Time column (not useful for modeling)
2. Scaled Amount feature using StandardScaler

Exploratory Data Analysis
1. Identified extreme class imbalance
2. Analyzed amount statistics across fraud and non-fraud cases

Feature Selection & Splitting
1. X: All features except Class
2. y: Target variable (Class)
3. Train-test split: 80% train / 20% test

## 🧪 Results Summary
Model	Accuracy Score	F1 Score
Decision Tree	99.94%	0.81
K-Nearest Neighbors	99.95%	0.86
Logistic Regression	99.92%	0.75
Support Vector Machine	99.93%	0.78
Random Forest	99.93%	0.77
XGBoost	99.96%	0.87

## ✅ Best Performing Model: XGBoost with the highest F1 score and accuracy.
