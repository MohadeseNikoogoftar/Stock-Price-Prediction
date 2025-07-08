# 📈 Stock Price Prediction using Machine Learning

This project presents a complete machine learning pipeline to analyze and predict the stock prices of Apple Inc. (AAPL) using historical market data. It includes data collection, preprocessing, feature engineering, multiple ML model implementations, and evaluation of predictive performance. The objective is to build models that can either **predict the closing price** of the stock (regression) or **classify price movement trends** (classification), and to analyze patterns in the market behavior using clustering.

---

## 🔍 Project Goals

- Fetch historical AAPL stock data from Yahoo Finance.
- Analyze and visualize trends in historical price and volume data.
- Perform extensive data preprocessing and feature engineering.
- Train and evaluate several models:
  - Regression: Linear Regression
  - Classification: K-Nearest Neighbors (KNN), Decision Tree, Support Vector Machine (SVM), Artificial Neural Network (ANN)
  - Clustering: DBSCAN, K-Means, Agglomerative Clustering
- Compare the performance of each model and identify the best-performing algorithm for the task.

---

## 🧠 Why ANN Was the Best Model

The Artificial Neural Network (ANN) model outperformed other classifiers in both accuracy and generalization ability. ANN achieved the highest accuracy and F1-score in predicting price movement (i.e., whether the stock price would increase or decrease). This is due to its strong capability to model nonlinear patterns and complex relationships in time series data, which traditional algorithms like SVM or Decision Tree struggle to capture effectively. While simpler models performed adequately, the ANN model demonstrated superior performance and consistency across both training and testing data.

---

## 🗂️ Dataset Description

- **Data Source:** Yahoo Finance via `yfinance` API
- **Stock Ticker:** AAPL (Apple Inc.)
- **Time Period:** 2020-01-01 to 2024-12-31
- **Features Used:** Open, High, Low, Close, Volume
- **Target Variables:**
  - For regression: Close price
  - For classification: Binary price movement (Up/Down based on Close)

---

## 📦 Libraries and Dependencies

Ensure the following libraries are installed in your environment:

```bash
keras
matplotlib
numpy
pandas
seaborn
sklearn
tensorflow
yfinance

