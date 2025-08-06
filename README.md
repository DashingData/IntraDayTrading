# 📊 Intra-day Stock Price Prediction using GRU + MCP Server

## 🚀 Project Overview

This project aims to build an intelligent **intra-day stock trading system** using a **GRU (Gated Recurrent Unit)** deep learning model. It uses a centralized **MCP server** to fetch, clean, and prepare data from **Yahoo Finance** before feeding it into the GRU model for training and prediction.

This architecture simulates a production-ready trading pipeline using modular components.

---

## 📦 Components of the Project

### 🧠 GRU Model (Deep Learning)
- Used to capture sequential patterns in stock prices.
- Predicts short-term price movement based on historical data.
- More efficient than LSTM for many financial time series problems.

### 🖥️ MCP Server (Data Handling Layer)
- Acts as a centralized backend to fetch and preprocess stock data.
- Fetches data from Yahoo Finance using `yfinance`.
- Cleans the data, handles missing values, and returns a ready-to-use dataset.
- Optional: Can also compute indicators like RSI, SMA etc.

---

## 📈 Features Used (Input to GRU)

For each timestamp, the following features can be used:

- Open
- High
- Low
- Close (or Current Price)
- Volume
- RSI (optional)
- SMA (optional)
- Price Change %

---

## 🛠️ Tech Stack

| Component | Tool |
|----------|------|
| Data Source | Yahoo Finance |
| Data Handling | MCP Server (Flask/FastAPI) |
| ML/DL Framework | TensorFlow / PyTorch |
| Data Processing | Pandas, Numpy |
| Visualization | Matplotlib, Seaborn |
| Deployment Ready | Yes |

---

## 📂 Project Structure

