# Monte Carlo VaR / CVaR Engine  

[![Live Demo – Streamlit](https://img.shields.io/badge/Live%20Demo-Streamlit-FF4B4B?logo=streamlit&logoColor=white)](https://bad-day-bingo-var-calculator.streamlit.app/)  

**Try it live:** [bad-day-bingo-var-calculator.streamlit.app](https://bad-day-bingo-var-calculator.streamlit.app/)  

## Overview

**Bad Day Bingo** is a Value-at-Risk (VaR) and Conditional VaR (CVaR) engine that answers one critical question:

> *“If the market throws a tantrum, how much could I lose?”*

Upload a portfolio, simulate alternate scenarios, and estimate losses across horizons. The app supports stress tests, fat-tail risk modeling, and rolling backtests — giving you an interactive way to quantify portfolio risk.

## Features

* **Monte Carlo Simulations**: Gaussian & Student-t (fat-tail) distributions
* **Multi-Horizon Support**: 1 / 5 / 10 / 20-day horizons
* **Stress Testing**: ±σ shocks for crash-day scenarios
* **Backtesting**: Rolling 95% exceedance checks
* **Automation**: GitHub Actions generate daily plots + JSON reports
* **Interactive UI**: Streamlit dashboard for toggling assumptions

## Example Results (NIFTY Portfolio Demo)

* **95% VaR (10-day)**: −₹1.2L
* **99% VaR (10-day)**: −₹2.5L
* **CVaR 99%**: −₹3.4L

## 🛠️ Tech Highlights

* Python: `NumPy`, `Pandas`, `SciPy`, `yfinance`
* Risk Models: Monte Carlo, Student-t, Bootstrap Simulations
* Visualization: `matplotlib`, `Streamlit`
* Automation: GitHub Actions (auto-reports)

## Live Demo

[Streamlit App]([https://your-streamlit-demo-link.com](https://bad-day-bingo-var-calculator.streamlit.app/))
Or run locally:
python var_engine.py --mode t --df 6 --horizon 1 --scenarios 20000 --kde
streamlit run app.py


## Use Cases

* Portfolio risk management for equities
* Stress testing during high volatility
* Academic/industry benchmarking against Basel III norms
* Training tool for risk analytics students

## Closing Note

This project is part of my exploration into **quantitative finance and risk modeling**.
Feedback and collaboration are welcome — feel free to connect!

