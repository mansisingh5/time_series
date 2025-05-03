Time Series Analysis of UPI Transaction.

Overview

This project explores Time Series Analysis using UPI transaction data from the Reserve Bank of India (RBI). The goal is to analyze trends, seasonality, and patterns in the dataset and develop predictive models using ARIMA and SARIMA techniques.
Dataset
The dataset consists of UPI transactions with the following attributes:
Date of transaction
Volume (in Lakhs)
Value (in INR Crores)
The dataset is sourced from RBI’s official website.
Key Analysis & Methods
1. Exploratory Data Analysis (EDA)
Data Cleaning: Handling missing values and formatting dates.
Trend Visualization: Monthly and yearly transaction trends using Matplotlib and Seaborn.
Seasonality Detection: Fourier Transform-based Periodogram analysis.
Feature Engineering: Differencing to make the data stationary.
2. Statistical Tests
Dickey-Fuller Test for stationarity check.
Autocorrelation & Partial Autocorrelation (ACF & PACF) to determine time-dependent relationships.
3. Time Series Modeling
ARIMA (AutoRegressive Integrated Moving Average) model for short-term forecasting.
SARIMA (Seasonal ARIMA) model to account for seasonal effects.
Hyperparameter tuning using pmdarima.auto_arima.
Residual Analysis: Checking model assumptions and performance.
4. Model Validation & Forecasting
Train-Test Split (80-20).
Ljung-Box test for residual independence.
Forecasting future UPI transaction volumes and values.
Results
ARIMA(3,1,1) and ARIMA(2,1,1) were the best models for transaction Volume and Value, respectively.
SARIMA(1,0,3)(1,1,1,30) captured seasonality in UPI transactions.
Ljung-Box test confirmed residual independence, indicating a good model fit.
Technologies Used
Python (Pandas, NumPy, Statsmodels, Matplotlib, Seaborn)
Time Series Modeling (ARIMA, SARIMA)
Jupyter Notebook for analysis
