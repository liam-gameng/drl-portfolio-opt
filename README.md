# Deep Reinforcement Learning for Portfolio Optimization

---

## Overview
This repository implements portfolio optimization using **Deep Reinforcement Learning (DRL)**, specifically focusing on the **Deep Deterministic Policy Gradient (DDPG)** algorithm. The project aims to evaluate the performance of DRL-based portfolio strategies against traditional portfolio optimization techniques such as **Markowitz Portfolio**, **Minimum Variance Portfolio**, and **Equal Weight Portfolio**.

The repository includes training, testing, and analysis scripts, along with helper modules for data processing, feature extraction, and visualization. It provides comparisons of DRL strategies across multiple periods and evaluates them based on metrics such as Sharpe Ratio, Calmar Ratio, Annualized Return, and Volatility.

---

## Repository Structure

### Folders and Files
- `DRL_init_train.ipynb`: Training code for DRL-based portfolio optimization (base single period).
- `DRL_forward.ipynb`: Training DRL portfolios for walk-forward periods.
- `DRL_all_test.ipynb`: Testing and analysis of DRL-based portfolio performance for all periods.
- `DRL_init_test.ipynb`: Testing code with visualization for portfolio allocations and cumulative returns of base period.
- `DRL_forward_test.ipynb`: Testing code with visualization for portfolio allocations and cumulative returns for walk-forward periods.
- `rolling_markowitz_window.ipynb`: Implementation of traditional rolling **Markowitz Portfolio**, **Minimum Variance Portfolio**, **Equal Weight Portfolio**

---

## Key Features
1. **Deep Deterministic Policy Gradient (DDPG)**:
   - Actor-Critic architecture for continuous action spaces.
   - Integrated Ornstein-Uhlenbeck Noise for exploration.

2. **Portfolio Optimization Benchmarks**:
   - Rolling Markowitz Portfolio.
   - Minimum Variance Portfolio.
   - Equal Weight Portfolio.

3. **Customizable Training and Testing**:
   - Adjustable rolling windows, rebalancing periods, and time frames.
   - Scalable architecture with modularized actor and critic networks.

4. **Comprehensive Visualization**:
   - Stacked area plots for portfolio allocations.
   - Cumulative return plots comparing DRL to benchmarks.

---

### Prerequisites
- Python 3.8+
- Required Libraries:
  - `torch`
  - `numpy`
  - `matplotlib`
  - `pandas`
  - `yfinance`
  - `gym`
