# 📊 Week 11 Challenge: Time Series Forecasting & Portfolio Optimization

## 🚀 Introduction
This repository contains the implementation and findings from the **Week 11 challenge** focused on **time series forecasting for portfolio management optimization**. The objective was to develop forecasting models for financial assets and use the insights to optimize portfolio allocations.

## 📌 Project Overview
- **Goal:** Predict future prices of key financial assets and optimize portfolio returns.
- **Assets Analyzed:**
  - **TSLA (Tesla Inc.)** – High-growth, high-volatility stock.
  - **BND (Vanguard Total Bond Market ETF)** – Low-risk bond ETF.
  - **SPY (S&P 500 ETF)** – Broad market index ETF.
- **Methodologies Applied:**
  - Data collection using **Yahoo Finance (YFinance API)**.
  - Exploratory Data Analysis (EDA) to identify trends and patterns.
  - Time series forecasting using **ARIMA, SARIMA, and LSTM**.
  - Portfolio optimization using **Sharpe Ratio Maximization**.

## 📂 Repository Structure
```
├── data/                     # Raw and processed financial datasets
├── notebooks/                # Jupyter Notebooks for analysis & modeling
│   ├── 01_data_preprocessing.ipynb
│   ├── 02_forecasting_models.ipynb
│   ├── 03_portfolio_optimization.ipynb
├── src/                      # Scripts for model training and optimization
├── results/                  # Plots and performance metrics
├── README.md                 # This file
└── report.pdf                # Final challenge report
```

## 📈 Key Findings
### 🔹 **Exploratory Data Analysis (EDA)**
- **Tesla’s stock price is highly volatile** compared to BND and SPY.
- **BND remains stable over time**, acting as a hedge against market downturns.
- **SPY follows a steady upward trend**, representing the general market movement.
- **Rolling mean & standard deviation confirmed** Tesla’s unpredictable fluctuations.

### 🔹 **Forecasting Model Performance**
| Model  | RMSE  | MAE  | Observations |
|--------|------:|------:|-------------|
| ARIMA  | 45.2  | 32.1  | Struggled with high volatility |
| SARIMA | 37.8  | 27.5  | Improved with seasonal trends |
| LSTM   | **28.3**  | **19.6**  | Best model, capturing long-term trends |

### 🔹 **Future Market Forecast (Next 12 Months)**
- **Tesla’s projected price range:** **$240 – $380** with potential fluctuations.
- **SPY and BND expected to remain stable**, reinforcing their role in risk management.
- **Volatility Analysis:** High uncertainty in TSLA, requiring a balanced investment approach.

### 🔹 **Portfolio Optimization Results**
- **Optimized Asset Allocation:**
  - **TSLA: 42%** (High return potential but risky)
  - **BND: 28%** (Low risk, stabilizing factor)
  - **SPY: 30%** (Diversification and steady growth)
- **Sharpe Ratio Improved to 1.42**, maximizing returns for the given risk.

## ⚙️ How to Run the Project
1. **Clone the repository**:
   ```bash
   git clone [https://github.com/your-repo/week11-challenge.git](https://github.com/amani387/10_ACADAMY_KAIM_W11.git)
   cd week11-challenge
   ```
2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```
3. **Run the Jupyter notebooks** in the `notebooks/` directory to:
   - Fetch and preprocess data (`01_data_preprocessing.ipynb`)
   - Train forecasting models (`02_forecasting_models.ipynb`)
   - Optimize portfolio (`03_portfolio_optimization.ipynb`)

## 📌 Conclusion
- **LSTM was the best model for Tesla’s price prediction**.
- **Portfolio optimization helped balance risk vs. return**.
- **Future improvements**: Fine-tune LSTM hyperparameters and explore ensemble models.

## 📜 References
- Data: **Yahoo Finance (YFinance API)**
- Libraries Used: `pandas`, `numpy`, `scipy.optimize`, `tensorflow`, `statsmodels`

---
🔹 **By completing this challenge, we gained hands-on experience in financial data analysis, forecasting, and portfolio management using AI-driven insights.** 🚀

