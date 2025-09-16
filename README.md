# 📊 Statistical Arbitrage: Pairs Trading Strategy

This project implements a **statistical arbitrage (pairs trading) strategy** on a basket of large-cap US tech stocks.  
The goal is to identify **mean-reverting pairs** using econometric tests, backtest a systematic trading strategy,  
and evaluate its performance under realistic assumptions (including transaction costs).

---

## 🚀 Project Overview

Pairs trading is a **market-neutral strategy** that profits from the relative movement of two correlated assets.  
We scan stock pairs, test for cointegration, estimate hedge ratios, and generate trading signals based on **z-scores of spreads**.

The workflow covers:

1. **Data Loading** – Adjusted daily close prices for 12 tech stocks.  
2. **Pair Selection** –  
   - Engle-Granger cointegration test (ADF).  
   - Rolling beta estimation.  
   - Stability scoring.  
3. **Signal Generation** – Entry when |z-score| ≥ threshold, exit when z-score ≈ 0.  
4. **Backtesting** – Trade simulation with transaction costs & PnL accounting.  
5. **Performance Evaluation** –  
   - CAGR, volatility, Sharpe ratio, max drawdown.  
   - Train vs Out-of-Sample (OOS) Sharpe for robustness.  
6. **Visualization** – Publication-quality plots for LinkedIn/GitHub showcase.

---

## 📂 Dataset

- Universe: 12 U.S. tech stocks (AAPL, MSFT, GOOG, META, NVDA, AMD, INTC, ADBE, ORCL, CRM, CSCO, QCOM).  
- Period: 2020-01-01 → 2025-09-01 (≈1400 trading days).  
- Frequency: Daily adjusted close prices.  

---

## 🔑 Key Results

- **Scanned Pairs:** 66 total  
- **Top 5 Pairs (by stability & train Sharpe):**  
  - MSFT–AMD  
  - MSFT–NVDA  
  - META–NVDA  
  - MSFT–GOOG  
  - MSFT–ORCL  

- **Portfolio Backtest (Top 5 Pairs):**  
  - CAGR: **2.41%**  
  - Annualized Volatility: **3.78%**  
  - Sharpe Ratio: **0.64**  
  - Max Drawdown: **-4.38%**  
  - Transaction cost assumption: **10 bps round-trip**  

- **Robustness Check:**  
  - Train vs OOS Sharpe scatterplot confirms generalization.  
  - Strategy profitable under multiple thresholds (1.5σ–2.5σ).

---

## 📈 Visualizations


1. **Adjusted Prices Timeseries** – Universe of 12 tech stocks.  
2. **Spread & Z-Score Plot (Best Pair)** – Mean-reverting spread, entry/exit signals.  
3. **Cumulative PnL Curve** – Trade equity for the best pair.  
4. **Sharpe Ratio Ranking** – Top 5 pairs ranked by train Sharpe.  
5. **Train vs OOS Scatterplot** – Robustness check across all pairs.  
6. **Trade Returns Histogram (Best Pair)** – Risk distribution view.  


---

## ⚙️ Tech Stack

- **Python**: `pandas`, `numpy`, `matplotlib`, `seaborn`, `statsmodels`  
- **Quant Methods**: Cointegration tests (ADF), rolling hedge ratios, Sharpe analysis, backtesting engine  
- **Backtesting**: Custom trade simulator with PnL tracking and transaction costs  

---


---

## 🔮 Next Extensions

- Kalman filter for dynamic hedge ratio.  
- Regime detection (volatility clustering).  
- Multi-pair portfolio optimization.  
- Risk-adjusted capital allocation across pairs.  


---


## 🙌 About Me

If you're working on financial risk modeling, machine learning, or applied deep learning — let’s connect!

👤 **Surajit Biswas, Ph.D.**  

🔗  [![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?logo=linkedin)](https://www.linkedin.com/in/surajit-biswas-phd/)

📫 surajitbiswas.iiserb@gmail.com

---

## 🏷️ Tags

`Pairs Trading` `Cointegration` `Statistical Arbitrage` `Quant Finance` `Backtesting` `Sharpe Ratio`
