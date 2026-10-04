# Optimal Portfolio of 10 Different‑Industry Stocks
This project builds **stock portfolio** across **10 stocks from different industries** starting from 01/01/2020, aiming to maximize the **Sharpe Ratio**.
## Overview
Using historical price data from 10 diversified stocks, the project applies:
- Equally Weighted Portfolio
- Optimal Random Portfolio using **Modern Portfolio Theory** developed by **Harry Markovitz**
## Optimal Portfolio Weights
Below are the optimal weights that maximize the Sharpe Ratio:
AMZN : 0.0000
GOOGL : 0.0962
JPM   : 0.0000
LIN   : 0.0000
LMT   : 0.0000
MSFT  : 0.0000
NVDA  : 0.5881
PG    : 0.0000
UNH   : 0.0000
XOM   : 0.3157
## Portfolio Performance
Expected Return: 49.66%
Standard Deviation: 35.33%
Sharpe Ratio: 1.2926
A Sharpe Ratio above **1.0** indicates strong risk‑adjusted performance.  
In this optimization, all weights were constrained between **0 and 1**, meaning the portfolio is **long‑only** with **no short selling allowed**. 
Because of this constraint, the optimizer allocates capital only to the assets that most improve the portfolio’s Sharpe Ratio. 
As a result, NVDA and XOM receive high weights while other stocks receive zero weight.
## How to Run
1. Download the notebook (`.ipynb`) from this repository.  
2. Open it in Jupyter Notebook, JupyterLab, or VS Code.  
3. Install required libraries:
   ```bash
   pip install numpy pandas matplotlib yfinance scipy
