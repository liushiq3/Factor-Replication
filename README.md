# Project: Investment Factor Replication and Analysis

In this project, I developed a comprehensive framework to replicate and analyze key investment factors that are widely used in hedge fund strategies. The objective was to deepen my understanding of asset pricing anomalies and the construction of long-short portfolios by recreating several popular factors—similar to those found in the Capital IQ Alpha Factor Library—using historical stock data.

## Overview & Objectives

- **Replication of Investment Factors:**  
  I focused on replicating seven fundamental factors including Price Momentum, Analyst Expectations, Long-Term Momentum, Valuation (Book-to-Price), CAPM Beta, Size (Log Market Cap), and 12-Month Realized Price Volatility. The goal was to recreate these factors over a sample period from 1970 to 2019, ensuring the results correlated strongly (targeting correlations of 0.9 or higher) with benchmark data.

- **Data-Driven Approach:**  
  Utilizing a well-organized dataset sourced from major financial databases (Compustat-Capital IQ and I/B/E/S Thomson Reuters), I processed historical stock returns and firm-level characteristics. The dataset included extensive information on S&P 500 constituents, acknowledging the dynamic nature of the index over time.

## Methodology

- **Data Processing & Organization:**  
  I standardized the data to a monthly frequency and transformed individual variables into matrix forms, where each row represented a date and each column a firm. This allowed for efficient computation and portfolio construction.

- **Portfolio Sorting & Construction:**  
  Stocks were sorted into quintiles based on the specific characteristics relevant to each factor. I constructed equal-weighted portfolios, rebalancing them monthly, and calculated the quantile spread (difference between the top and bottom quintile returns) as a measure of factor performance.

- **Performance and Risk Analysis:**  
  In addition to plotting the time series of the factor spreads, I computed key performance statistics—mean, standard deviation, Sharpe ratio, skewness, kurtosis, and maximum drawdown. I also performed hypothesis testing to assess whether the mean returns of these factors were statistically significant.
