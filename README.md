# 📈 Portfolio Optimization Project

## Overview
This project explores **portfolio optimization and forecasting** to enhance investment decision-making. It combines **time-series forecasting (ARIMA)** with **quantitative portfolio construction**, aiming to determine optimal asset allocation strategies over time.

The project consists of:
- A **forecasting model** to predict stock market returns.
- A **portfolio optimization framework** applying **Markowitz's Efficient Frontier**.
- Analysis of **seven investment strategies** across a 10-year period.

## Project Setup
### Data
- **Time Frame:** October 2014 - October 2024
- **Assets:** FTSE 100 index & five selected UK companies
- **Risk-Free Asset:** 1-month UK GILTS

### Tools & Technologies
- **Python**
- **Pandas, NumPy, SciPy** for data handling
- **Statsmodels** for ARIMA forecasting
- **Matplotlib, Seaborn** for visualization

## Methodology

### 📊 1. Forecasting Model
- Implemented **ARIMA (1,1,1)** to predict FTSE 100 returns.
- Compared **forecasted returns** with risk-free rates.
- Allocated capital dynamically: **stocks if expected return > risk-free rate**, otherwise **risk-free assets**.

### 📈 2. Portfolio Construction
- Selected **5 UK stocks** based on **expected returns & low correlations**.
- Constructed two primary portfolios:
  - **Minimum Variance Portfolio:** Focused on risk minimization.
  - **Market Portfolio:** Maximized the **Sharpe Ratio**.
- Plotted the **Efficient Frontier** to visualize optimal risk-return trade-offs.

### 🔍 3. Investment Strategies
Evaluated **seven strategies** over the 10-year period:
1. **Market Portfolio (No Rebalancing)**
2. **Minimum Variance Portfolio (No Rebalancing)**
3. **Market Portfolio (Rebalanced Every 6 Months)**
4. **Minimum Variance Portfolio (Rebalanced Every 6 Months)**
5. **Risk-Free Asset**
6. **UK Stock Market (FTSE All-Share Index)**
7. **Forecasting Model Strategy** (Adaptive allocation based on ARIMA)

## Results
| Strategy | Terminal Wealth (£) | % Return |
|----------|------------------|----------|
| Market Portfolio (No Rebalancing) | £2360.93 | 136% |
| Min Variance Portfolio (No Rebalancing) | £2608.04 | 161% |
| Market Portfolio (Rebalancing) | **£3032.13** | **203%** |
| Min Variance Portfolio (Rebalancing) | £2536.47 | 154% |
| Risk-Free Asset | £1135.82 | 14% |
| UK Stock Market | £1264.99 | 26% |
| Forecasting Model Strategy | £2208.81 | 121% |

- **Best performing strategy:** Market Portfolio with rebalancing (**203% return**).
- **Most stable strategy:** Minimum Variance Portfolio.
- **Forecasting model performance:** 121% return, but sensitive to market shocks.

## Conclusion
- **Rebalancing** improves performance but increases **transaction costs**.
- **Passive investing (FTSE Index) underperforms** compared to optimized strategies.
- **Risk-averse investors** may prefer the **Minimum Variance Portfolio**, while **growth-focused investors** should consider **Market Portfolio with strategic rebalancing**.

## 📬 Contact
For any inquiries or collaboration, feel free to reach out:
- **Email:** [lollordp@gmail.com](mailto:lollordp@gmail.com)
- **LinkedIn:** [Lorenzo Rossi](https://www.linkedin.com/in/lorenzo-rossi01/)
