# Volatility Modeling and Forecasting

## Project Overview

This project focuses on modeling and forecasting the volatility of NIFTY 50 stock index using time series analysis. We apply ARIMA and GARCH models to analyze, predict, and evaluate market volatility, enabling better risk assessment and financial decision-making.

## Objectives

Fetch and visualize  NIFTY 50 closing prices  using Yahoo Finance.

Test for stationarity using the Augmented Dickey-Fuller (ADF) test.

Compute log returns for better time series modeling.

Fit ARIMA (2,0,2) and GARCH (1,1), GARCH (2,1), GARCH (1,2), EGARCH(1,1) , GJR-GARCH(1,1) models to capture volatility.

Compare models using AIC and BIC values to determine the best fit.

Forecast future volatility and evaluate model performance.

## Dataset

Source: NIFTY 50 stock market index.

Timeframe: 2018 - 2024.

Key Columns: Date, Open, High, Low, Close, Volume.

## Methodology

### 1. Data Preprocessing

Load NIFTY 50 stock market data into a pandas DataFrame.

Remove unnecessary columns and set date as index.

Convert closing price to a time series format.

### 2. Stationarity Check

Apply ADF test on closing prices and log returns.

Differencing applied if necessary to achieve stationarity.

### 3. Modeling

ARIMA Model

Fit ARIMA (1,0,1) to model time series trends.

Evaluate model using AIC and BIC values.

GARCH Models

Fit GARCH(1,1), GARCH(2,1), GARCH(1,2), EGARCH(1,1) and GJR-GARCH(1,1) to capture volatility clustering.

Compare AIC and BIC values to determine the best model.

### 2. Forecasting and Evaluation

Forecast next 30 days volatility using the best GARCH model.

Compute Mean Absolute Error (MAE), Root Mean Error(RME) and Root Mean Square Error(RMSE) for model evaluation.

## Conclusion

The GARCH(2,1) model was the best fit for volatility forecasting.

The model successfully captures volatility clustering and performs well within expected error margins.

The forecasted volatility closely follows actual values, making it useful for risk analysis and financial decision-making.

## Future Work

Test on alternative datasets (e.g., S&P 500, crypto markets).

Develop a real-time forecasting system using live market data.



