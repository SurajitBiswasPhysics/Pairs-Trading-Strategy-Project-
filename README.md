# 🔗 Pairs Trading Strategy using Cointegration  

Can we exploit temporary price divergences between cointegrated stocks?  

This project implements a **statistical arbitrage (pairs trading) strategy** using **cointegration analysis** and **z-score–based trading signals**. The idea is to identify stock pairs that move together in the long run, and trade on their short-term deviations.  

---

## 🧠 Project Highlights  

- 📂 Dataset: Daily stock price data (multiple tickers)  
- 🧮 Methodology: Engle–Granger cointegration test + rolling window analysis  
- 🎯 Strategy: Long/short based on z-score thresholds  
- 📈 Output: Trade logs, portfolio NAV curve, performance metrics  
- ✅ Evaluation: CAGR, Annualized Volatility, Sharpe Ratio, Max Drawdown  

---

## 🧪 Features & Workflow  

- **Data Preprocessing** – load & clean stock price data  
- **Pairs Selection** – find cointegrated stock pairs  
- **Signal Generation** – z-score–based entry & exit rules  
- **Backtesting** – simulate trades with transaction costs  
- **Performance Metrics** – CAGR, Sharpe, Drawdown, Volatility  
- **Visualization** – NAV curves, spread charts, trade annotations  

---

## 📊 Visual Results  

### 📈 Portfolio NAV Curve  
![NAV Curve](outputs/portfolio_nav.png)  

### 🔍 Example Cointegrated Pair Spread  
![Pair Spread](outputs/pair_spread_example.png)  

### 📑 Sample Trade Log  
![Trades](outputs/trades_example.png)  

---


## 🙌 About Me

If you're working on financial risk modeling, machine learning, or applied deep learning — let’s connect!

👤 **Surajit Biswas, Ph.D.**  

🔗  [![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?logo=linkedin)](https://www.linkedin.com/in/surajit-biswas-phd/)

📫 surajitbiswas.iiserb@gmail.com

---

## 🏷️ Tags

`Pairs Trading', `Cointegration', `Statistical Arbitrage', `Quant Finance', `Backtesting', `Sharpe Ratio'
