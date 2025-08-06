# IntraDayTrading



# 📊 Intra-day Stock Price Movement Prediction (Phase 1)

## 🚀 Project Overview

This project aims to build a basic machine learning model to predict **next-day or intra-day stock price movement** using historical market data. The goal is to help identify potential short-term trading opportunities based on selected technical and basic fundamental indicators.

For Phase 1, we are focusing on **5 Indian defense companies**, and using **daily historical stock data** from **Yahoo Finance**.

---

## 📌 Phase 1 Goals

- ✅ Fetch historical stock data from Yahoo Finance using Python.
- ✅ Select a limited set of indicators for simplicity and speed.
- ✅ Apply basic data cleaning logic to prepare the data for modeling.
- ✅ Train a basic machine learning model to predict price movement (up/down).
- ✅ Evaluate model performance on historical data.

---

## 📈 Selected Indicators (Features)

We will use the following features for each stock:

1. **Volume** – total traded volume of the day  
2. **Previous Close** – close price from the previous day  
3. **Current Price** – today's close price  
4. **RSI (Relative Strength Index)** – to capture overbought/oversold signals  
5. **SMA (10)** – 10-day simple moving average to track price trend  
6. **Price Change %** – percentage change in price from previous day

---

## 📦 Data Source

We are using the [Yahoo Finance API](https://pypi.org/project/yfinance/) via the `yfinance` Python package.

- Interval: Daily (1d)
- Date Range: Jan 2024 to Aug 2024 (example)
- Example Ticker: `HAL.NS`, `BEL.NS`, `BEML.NS`, etc.

---

## 🤖 ML Model (Basic)

We will use a simple **classification model** (e.g., Random Forest or Logistic Regression) to predict:

> Will the stock go **Up (1)** or **Down (0)** the next day?

- Input: Technical indicators as features
- Output: Binary classification (up/down)

---

## 🧹 Data Cleaning

- Handle missing values (NaNs)
- Remove invalid data (e.g., zero volume)
- Normalize/scale features if needed
- Ensure date-wise sorting

Data cleaning will eventually be moved to a **central MCP server** that preprocesses data before it is used locally.

---

## 🔮 Future Scope

After Phase 1, we plan to:

- Add more technical indicators (VWAP, MACD, Bollinger Bands)
- Use intraday (15-min) interval data
- Connect with live APIs (e.g., Zerodha) for real-time prediction
- Integrate a logic-based MCP Server for smart data routing and cleaning
- Auto-trade based on model predictions

---

## 👨‍💻 Technologies Used

- Python  
- yfinance  
- pandas  
- scikit-learn  
- ta (technical analysis)  
- MCP Server (in later phases)

---

## 📁 Folder Structure (Planned)

