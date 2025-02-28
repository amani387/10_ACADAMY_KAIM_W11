# Time Series Forecasting for Portfolio Management Optimization

## Task 1: Week 11 Challenge
**Date:** 26 Feb – 04 Mar 2025  

## Overview
This project focuses on leveraging time series forecasting techniques to optimize portfolio management. We analyzed historical data for three key assets—Tesla (TSLA), Vanguard Total Bond Market ETF (BND), and S&P 500 ETF (SPY)—to forecast future trends and optimize asset allocation strategies.

## Data Acquisition and Preprocessing
- **Data Source:** Yahoo Finance
- **Period:** January 1, 2015 – January 31, 2025
- **Preprocessing Steps:**
  - Addressed missing values and formatted timestamps
  - Normalized data for comparability
  - Conducted exploratory data analysis (EDA), including trend analysis, volatility assessment, and seasonal decomposition

## Time Series Forecasting
- **Model Used:** ARIMA for TSLA forecasting
- **Optimization:** Parameter tuning using `auto_arima`
- **Evaluation Metrics:** MAE, RMSE, MAPE
- **Forecast Horizon:** 6–12 months
- **Results:**
  - Predicted upward trend for TSLA with confidence intervals
  - Residual analysis confirmed model reliability

## Portfolio Optimization
- **Assets Considered:** TSLA, BND, SPY
- **Key Metrics Computed:**
  - Expected returns, portfolio volatility, Sharpe Ratio
  - Covariance matrix for inter-asset correlations
- **Optimization Approach:**
  - Maximized Sharpe Ratio through risk-adjusted allocation
  - Suggested allocation: TSLA (45%), BND (30%), SPY (25%)

## Insights & Recommendations
- **Investment Strategy:**
  - Increase TSLA exposure in growth phases, shift to BND in volatile periods
  - Implement dynamic portfolio rebalancing based on updated forecasts
- **Further Improvements:**
  - Incorporate real-time data for adaptive decision-making
  - Explore advanced deep learning models (e.g., LSTM) for improved accuracy

## References
- ARIMA for Time Series Forecasting – Machine Learning Mastery
- Portfolio Optimization with Modern Portfolio Theory – PyPortfolioOpt
- Time Series Analysis – Analytics Vidhya

## How to Run the Project
1. Install dependencies:
   ```bash
   pip install yfinance pandas numpy pmdarima matplotlib seaborn
   ```
2. Run the forecasting model:
   ```bash
   python forecast.py
   ```
3. Perform portfolio optimization:
   ```bash
   python optimize_portfolio.py
   ```

---
**Author:** Amanuel Nega  
**Project:** GMF Investments - Time Series Forecasting & Portfolio Optimization
