# 🐳 A Whale Portfolio analysis

<img src="https://c.tenor.com/jr1MtHkypYUAAAAC/nature-whaleshark.gif" alt="drawing" width="100%"/>

# Table of Contents
1. [Background](#-1-background)
2. [Instructions](#-2-instructions)
3. [Results](#%EF%B8%8F-3-results)

## [🚧 1. Background](#🚧-1-background)

* Using Python and Pandas, determine which portfolio is performing the best across multiple areas:
    * volatility
    * returns
    * risk 
    * Sharpe ratios
* This python code compares [my custom portfolio](/custom_portfolio/) to [the whales](/Resources/whale_returns.csv) and [two alogorithmic trading strategies](/Resources/algo_returns.csv)
* This code compares if my custom portfolio: 
    * Outperforms
    * Underperforms 
    * Or Equally perfroms 

## [🚦 2. Instructions](#🚦-2-instructions)
* Analyze whale Returns of Soros, Paulson,Tiger and Berkshire 
    * Read the Whale Portfolio daily returns and clean the data 
    ![Whale Data Analysis](./images/whale_portfolio.png)
* Analyze Algorithm 1 and Algorithm 2 Daily Returns
    * Read the algorithmic daily returns and clean the data
    ![Algorithm Data Analysis](./images/algorithm_portfolio.png)
* S&P 500 Returns
    * Read the S&P 500 historic closing prices and create a new daily returns DataFrame from the data.
    ![S & P 500 Data Analysis](./images/sp500_portfolio.png)
* Combined Returns
    * Performance Analysis
    * Calculate and Plot the daily returns.
    * Calculate and Plot cumulative returns.
    ![Daily Returns](./images/daily_returns.png)
* Determine the risk of each portfolio:
    * Create a box plot for each portfolio.
    * Calculate the standard deviation for all portfolios
    * Determine which portfolios are riskier than the S&P 500
    * Calculate the Annualized Standard Deviation
    ![Risk Analysis](./images/risk_analysis.png)
* Analyze the rolling statistics for Risk and Beta.
    * Calculate and plot the rolling standard deviation for all portfolios using a 21-day window
    * Calculate the correlation between each stock to determine which portfolios may mimick the S&P 500
    ![Correlation Stats](./images/correlation_stats.png)
    * Choose one portfolio, then calculate and plot the 60-day rolling beta between it and the S&P 500
    * Calculate and Plot Beta for a chosen portfolio and the S&P 500
        *  Try calculating the `ewm` with a 21-day half life for each portfolio, using standard deviation (std) as the metric of interest. 
        ![Beta Plot 60 day Window](./images/beta_portfolio_60day.png)
* Using the daily returns, calculate and visualize the Sharpe ratios using a bar plot ![Sharpe Ratio Bar](./images/sharpe_ratio_bar.png)
    * Determine whether the algorithmic 1 strategies outperform both the market (S&P 500) and the whales portfolios.
    * Determine whether the algorithmic 2 strategies outperform both the market (S&P 500) and the whales portfolios. ![Algo_vs_whales](./images/algo_vs_whales.png)
* Create Custom Portfolio
    * Choose 3-5 custom stocks with at last 1 year's worth of historic prices and create a DataFrame of the closing prices and dates for each stock.
    ![Custom Stocks](./images/custom_stocks.png)
    * Calculate the weighted returns for the portfolio assuming an equal number of shares for each stock
        * Join your portfolio returns to the DataFrame that contains all of the portfolio returns
        ![Joined Portfolios](./images/joined_portfolios.png)
    * Calculate the Annualized Standard Deviation.
    * Calculate and plot rolling `std` with a 21-day window.
    * Calculate and plot the correlation.
        ![Joined Correlations](./images/joined_correlations.png)
    * Calculate and plot beta for your portfolio compared to the S&P 60 TSX.
    * Calculate the Sharpe ratios and generate a bar plot.
        ![Joined Beta Sharpe](./images/joined_beta_sharpe.png)
* How does my portfolio do?
    ![My Portfolio Results](./images/my_results.png)
## [🛣️ 3. Results](#🛣️-3-results)
* **File:** [Whale Analysis](./whale_analysis.ipynb)

