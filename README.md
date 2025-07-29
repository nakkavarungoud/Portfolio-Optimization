# Portfolio-Optimization
This project focuses on optimizing a portfolio of financial assets to achieve the **maximum Sharpe Ratio**, representing the best risk-adjusted return. It uses historical market data, calculates key portfolio metrics, and applies optimization techniques to determine the ideal asset allocation.

##  Objective

The main objective of this project is to determine the optimal portfolio weights among selected financial assets by maximizing the Sharpe Ratio. This helps in identifying the most efficient combination of assets for investment.

##  Tools & Technologies Used

- Python 
- NumPy
- Pandas
- Matplotlib
- yFinance (for financial data)
- SciPy (for optimization)

##  Assets Used

The portfolio includes the following ETFs:
- `SPY` – S&P 500 ETF
- `BND` – Total Bond Market ETF
- `GLD` – Gold Trust ETF
- `QQQ` – Nasdaq-100 ETF
- `VTI` – Total Stock Market ETF

## Methodology

1. **Data Collection** – Downloaded historical adjusted close prices using `yfinance`.
2. **Return Calculation** – Calculated daily and annual returns.
3. **Covariance & Risk** – Estimated the annualized volatility using the covariance matrix.
4. **Optimization** – Applied SciPy’s `minimize` function to maximize the Sharpe Ratio.
5. **Result Evaluation** – Output optimal weights, expected return, volatility, and Sharpe Ratio.
6. **Visualization** – Plotted the Efficient Frontier for better understanding.

## Results

**Optimal Portfolio Allocation**:

