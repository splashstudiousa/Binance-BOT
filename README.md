# Binance RSI Bot 🤖

A browser-based contrarian RSI trading bot dashboard with live Binance price feeds. No backend, no installation — just open `index.html` in any browser.

![Bot Status](https://img.shields.io/badge/status-live-brightgreen)
![License](https://img.shields.io/badge/license-MIT-blue)

## 🚀 Live Demo
👉 **[splashstudiousa.github.io/Binance-BOT](https://splashstudiousa.github.io/Binance-BOT/)**

---

## ✨ Features

| Feature | Details |
|---|---|
| **Live price feed** | WebSocket stream from Binance (auto-fallback to polling) |
| **RSI signals** | Configurable oversold (BUY) and overbought (SELL) thresholds |
| **Auto-execute** | Opens trades automatically on RSI signal |
| **Take profit / Stop loss** | Auto-closes position when TP or SL is hit |
| **Spot + Futures** | Both modes supported with leverage control |
| **Trade log** | Full history with entry, exit, P&L, and running balance |
| **Open position banner** | Live P&L tracking while trade is open |
| **No server needed** | Pure HTML + JS, runs entirely in the browser |

---

## 📖 How to use

1. Open the live demo or download `index.html` and open it locally
2. Select your **symbol** (BTC, ETH, SOL, BNB, XRP, ADA, DOGE)
3. Choose **Spot** or **Futures** mode
4. Adjust **RSI thresholds**, **Take profit %**, and **Stop loss %**
5. Enable **Auto-execute** to let the bot trade on signals
6. Watch live trades execute in the **Trade log**

---

## ⚙️ Strategy

This bot uses a **contrarian reversal** approach:

- **RSI ≤ 30 (oversold)** → Everyone is selling → Bot goes **LONG** (BUY)
- **RSI ≥ 70 (overbought)** → Everyone is buying → Bot goes **SHORT** (SELL)
- Position closes automatically at **Take Profit** or **Stop Loss**

---

## 🔑 API Keys (for live order execution)

> ⚠️ Current version tracks signals and simulates P&L. Live order execution requires a Python backend.

To connect your Binance API keys for live data:
1. Go to Binance → Account → API Management
2. Create API key (enable Spot + Futures trading, **disable withdrawals**)
3. Paste keys into the sidebar — stored in your browser only, never transmitted

---

## 📊 Recommended settings

| Setting | Conservative | Aggressive |
|---|---|---|
| RSI Oversold | 25 | 30 |
| RSI Overbought | 75 | 70 |
| Take profit | 3–5% | 2–3% |
| Stop loss | 2% | 1.5% |
| Leverage (Futures) | 2–3x | 5–10x |

---

## ⚠️ Disclaimer

This tool is for **educational and simulation purposes only**. Trading cryptocurrency carries significant financial risk. Past performance does not guarantee future results. Never trade with money you cannot afford to lose.

---

## 🛠️ Built with

- Vanilla HTML / CSS / JavaScript
- Chart.js for price and RSI charts
- Binance Public REST API + WebSocket

---

*Built with ❤️ — Open source, free to use and modify*
