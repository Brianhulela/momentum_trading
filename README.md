# Momentum Trading Strategy with EWMA and RSI

![Cover Image](https://placeholder.com/your-cover-image-link)

This project implements a momentum-based trading strategy using **Exponential Weighted Moving Averages (EWMA)** and the **Relative Strength Index (RSI)**. The primary goal is to simulate the strategy and evaluate its performance on historical stock price data.

## Overview
In this trading strategy:
- We calculate two EWMAs (short-term and long-term) for the stock’s closing price.
- A buy signal is generated when the **short-term EWMA** crosses above the **long-term EWMA** and the **RSI** is below a specified overbought threshold (70).
- A sell signal is generated when the **short-term EWMA** crosses below the **long-term EWMA** and the **RSI** is above a specified oversold threshold (30).
- Each trade considers brokerage fees, and the portfolio value is updated based on these transactions.

## Key Components
- **Data Preparation**: The data includes closing prices with a date index. EWMAs and RSI are calculated on this data.
- **Trading Signals**: The code generates buy and sell signals based on EWMA crossovers and RSI thresholds.
- **Transaction Tracking**: Each buy/sell transaction includes a brokerage fee, and positions are calculated using fractional shares.
- **Portfolio Performance**: The final portfolio value and individual transactions (date, closing price, net investment, fees, total shares, and portfolio value) are tabulated and displayed.

## Results
The simulation calculates key metrics such as:
- Final portfolio value after all trades.
- Number of buy and sell transactions.
- A detailed transaction table showing each trade’s specifics, including fees and portfolio value.

## Visualizations
The simulation includes two main plots:
- **Price Chart**: Displays closing prices, EWMAs, and buy/sell signals.
- **RSI Chart**: Shows the RSI values over time, indicating overbought/oversold levels.

## Requirements
- **Python Libraries**: `pandas`, `matplotlib`, and `tabulate` are required to run the code.

## Usage
To run the simulation, set up the data with date-indexed closing prices, define the EWMA and RSI windows, and run the code to see the portfolio's performance based on the trading strategy.

