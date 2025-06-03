# 📈 RSI-EMA and EMA Crossover Strategy Backtest

This project implements two popular technical trading strategies — **RSI with EMA**, and **EMA Crossover (MACD-like)** — using Python. It fetches real-time historical crypto price data from the CryptoCompare API and simulates trading logic based on indicator conditions.

> ⚠️ Binance API access is region-blocked, so CryptoCompare is used as a fallback.

---

## 🔍 Features

- 📊 **Fetch OHLCV data** (minute-level) from CryptoCompare
- ⚙️ **RSI + EMA Strategy**: Buy when RSI > 30 and price > EMA(21), sell when RSI > 70 or price < EMA(21)
- 📈 **EMA Crossover Strategy**: Buy on EMA(5) crossing above EMA(20), sell on crossover below
- 🧠 Trades are logged with timestamps, prices, PnL, and strategy used
- 📁 Can be run on **Google Colab** or **Jupyter Notebook**

---

## 🛠 Requirements

- Python 3.7+
- `pandas`
- `numpy`
- `requests`
- Internet connection (for API data)

Install requirements (if running locally):

```bash
pip install pandas numpy requests
