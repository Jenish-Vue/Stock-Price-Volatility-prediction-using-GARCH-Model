Volatility Modeling and Forecasting

Project Overview

This project focuses on modeling and forecasting the volatility of NIFTY 50 stock index using time series analysis. We apply ARIMA and GARCH models to analyze, predict, and evaluate market volatility, enabling better risk assessment and financial decision-making.

Objectives

Perform Exploratory Data Analysis (EDA) on NIFTY 50 closing prices.

Test for stationarity using the Augmented Dickey-Fuller (ADF) test.

Compute log returns for better time series modeling.

Fit ARIMA (2,0,2) and GARCH (1,1), GARCH (2,1), GARCH (1,2) models to capture volatility.

Compare models using AIC and BIC values to determine the best fit.

Forecast future volatility and evaluate model performance using Mean Absolute Error (MAE).

Visualize actual vs. forecasted volatility.

Dataset

Source: NIFTY 50 stock market index.

Timeframe: 2020 - 2025.

Key Columns: Date, Open, High, Low, Close, Volume.

Methodology

1. Data Preprocessing

Load NIFTY 50 stock market data into a pandas DataFrame.

Remove unnecessary columns and set date as index.

Convert closing price to a time series format.

2. Exploratory Data Analysis (EDA)

Plot the NIFTY 50 closing prices over time.

Compute log returns to stabilize variance.

Plot ACF and PACF for log returns to identify correlations.

3. Stationarity Check

Apply ADF test on closing prices and log returns.

Differencing applied if necessary to achieve stationarity.

4. Modeling

ARIMA Model

Fit ARIMA (2,0,2) to model time series trends.

Evaluate model using AIC and BIC values.

GARCH Models

Fit GARCH(1,1), GARCH(2,1), and GARCH(1,2) to capture volatility clustering.

Compare AIC and BIC values to determine the best model.

5. Forecasting and Evaluation

Forecast next 30 days volatility using the best GARCH model.

Compute Mean Absolute Error (MAE) for model evaluation.

Visualize Actual vs. Forecasted Volatility.

Results

AIC and BIC Comparison

Model

AIC Score

BIC Score

ARIMA(2,0,2)

-4860.10

-4829.29

GARCH(1,1)

-5383.61

-5363.07

GARCH(2,1)

-5385.38

-5359.70

GARCH(1,2)

-5368.13

-5342.45

Best Model: GARCH(2,1) due to the lowest AIC and BIC values.

Mean Absolute Error (MAE)

0.1094 (Small relative to the volatility range of 1-6).

Indicates a strong model fit.

Visualizations

Closing Price Over Time

Log Returns Plot

ACF and PACF of Log Returns

Actual vs. Forecasted Volatility Graph

How to Run the Project

Requirements

Install required Python libraries:

pip install numpy pandas matplotlib statsmodels arch

Run the Notebook

jupyter notebook

Execute the Jupyter Notebook cells to process data, fit models, and visualize results.

Conclusion

The GARCH(2,1) model was the best fit for volatility forecasting.

The model successfully captures volatility clustering and performs well within expected error margins.

The forecasted volatility closely follows actual values, making it useful for risk analysis and financial decision-making.

Future Work

Implement EGARCH and GJR-GARCH for asymmetry in volatility.

Test on alternative datasets (e.g., S&P 500, crypto markets).

Develop a real-time forecasting system using live market data.

Author

Your Name

Contact: [Your Email]

LinkedIn/GitHub: [Your Links]

