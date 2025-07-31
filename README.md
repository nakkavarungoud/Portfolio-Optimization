##  Project Overview

Portfolio Optimization is a fundamental concept in finance that aims to maximize returns while minimizing risk. In this project, I applied Python-based data analysis and optimization techniques to identify the ideal allocation of funds among a set of financial assets.

The optimization is done using the **Sharpe Ratio**, which provides the best trade-off between risk and return.

##  Key Objectives

- Fetch historical stock data using `yfinance`
- Analyze return and risk metrics (volatility, correlation, covariance)
- Use mathematical optimization to **maximize the Sharpe Ratio**
- Determine the **optimal asset weights** in a portfolio
- Visualize the **Efficient Frontier**

## 📈 Tools & Technologies Used

| Category        | Tools/Technologies                     |
|----------------|----------------------------------------|
| Programming     | Python, Jupyter Notebook               |
| Libraries       | Pandas, NumPy, Matplotlib, SciPy, yFinance |
| Optimization    | SciPy (`minimize` function)            |
| Visualization   | Matplotlib, Efficient Frontier Plot    |

## Dataset

- Source: Fetched using `yfinance`
- Assets considered:  
  - `SPY` – S&P 500 ETF  
  - `BND` – Total Bond Market ETF  
  - `GLD` – Gold ETF  
  - `QQQ` – Nasdaq 100 ETF  
  - `VTI` – Total US Stock Market ETF  
- Timeframe: Last 5 years of daily adjusted close prices

## Insights

- Portfolio allocation was heavily favored toward **SPY (50%)**, **GLD (40.64%)**, and **VTI (9.36%)**.
- Bonds (`BND`) and Nasdaq (`QQQ`) were assigned 0% due to risk-return imbalance.
- The **Sharpe Ratio** was **0.6702**, indicating a favorable risk-adjusted return.
- Volatility was moderate at **12.87%**, with an expected annual return of **13.01%**.

## Results

```plaintext
Optimal Weights:
SPY: 50.00%
GLD: 40.64%
VTI: 09.36%
BND: 00.00%
QQQ: 00.00%

Expected Annual Return: 13.01%
Expected Volatility: 12.87%
Sharpe Ratio: 0.6702

## Project Structure

portfolio-optimization/
│
├── Portfolio_Optimization.ipynb   # Main Jupyter Notebook
├── efficient_frontier.png         # Final Plot
├── images/                        # Images used in README
├── README.md                      # Project Documentation

## Conclusion
This project demonstrates how historical data and statistical methods can be applied to build a balanced and high-performing investment portfolio. The optimized portfolio shows that diversification between equity (SPY, VTI) and commodities (GLD) leads to a strong risk-return profile.

## Future Improvements
Add dynamic rebalancing of portfolio

Use Monte Carlo simulation for stress testing

Add constraints like minimum/maximum investment or sector-based limits

Explore machine learning for return forecasting


