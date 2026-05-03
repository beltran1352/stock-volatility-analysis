# stock-volatility-analysis
Analysis of stock market volatility across sectors using 2 years of Yahoo Finance data
# Stock Market Volatility & Sector Performance Analysis

## Project Overview
Analysis of 2 years of historical stock data to identify which market sectors exhibit the highest volatility and why.

## Key Findings
- **Most Volatile Stock:** UNH (Healthcare) at 2.66% volatility
- **Least Volatile Stock:** JNJ (Healthcare) at 1.12% volatility
- **Most Volatile Sector:** Healthcare (1.89% average)
- **Least Volatile Sector:** Finance (1.59% average)

## Data
- **Source:** Yahoo Finance
- **Stocks:** 9 companies across 4 sectors (Tech, Finance, Healthcare, Consumer)
- **Time Period:** May 3, 2024 - May 3, 2026 (2 years)
- **Total Observations:** 4,500 daily closing prices

## Files in This Repository
- `analysis_v2.R` - Complete R analysis script
- `Findings` - Summary of key insights
- `chart1_volatility_by_stock.png` - Bar chart of volatility by individual stock
- `chart2_volatility_by_sector.png` - Bar chart of volatility by sector
- `chart3_price_trends.png` - Line chart of price trends for top 3 volatile stocks
- `chart4_return_distribution.png` - Histogram comparing return distributions

## Methodology
1. Downloaded 2 years of daily stock prices from Yahoo Finance using `getSymbols()`
2. Calculated daily returns (percent change day-to-day)
3. Computed volatility as standard deviation of returns
4. Aggregated metrics by sector
5. Created visualizations with ggplot2

## Tools & Libraries
- **Language:** R 4.5.3
- **IDE:** RStudio
- **Libraries:** tidyverse, quantmod, ggplot2, dplyr, lubridate

## Key Insights
- Healthcare sector has extreme volatility (UNH: 2.66%, JNJ: 1.12%)
- Finance sector is the most stable (1.59% average)
- Tech and Consumer sectors have moderate volatility (~1.74%)
- UNH experienced a -22.4% day (worst single day in dataset)
- JNJ is the most resilient with only -7.59% worst day

## Next Steps
- Analyze volatility trends over time
- Compute correlations between sectors
- Build predictive model for future volatility
