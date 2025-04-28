## High-Frequency-Price-Prediction
### Table of Contents  

[Project Overview](#1) 

[Data](#2) 

[ Data  Preprocessing](#5) 

[Feature Engineering](#6) 

<a name="1"/>
<a name="2"/>


<a name="5"/>
<a name="6"/>

<a name="8"/>

## Project Overview
This project aims to develop a robust predictive model using machine learning  to enhance trading strategies and optimize returns.

Challenges in High-Frequency Price Prediction:

**Noisy and Non-Stationary Data** – High-frequency market data is highly volatile and exhibits rapid fluctuations.

**Market Microstructure Effects** – Bid-ask spreads, order book depth, and transaction latency influence short-term price movements.

**Latency Constraints** – Predictions must be made in real-time to be actionable for trading strategies.

**Feature Engineering** – Extracting relevant features from vast amounts of financial time-series data is critical for accuracy.

### Data  Preprocessing

The dataset trades.csv is from Kaggle and can be downloaded here.

Timestamp: Exact time of each trade.
Price: Transaction price of the futures contract.
Volume: Number of contracts traded.

Clean the data by handling missing values and outliers.
Normalize features to ensure consistent scaling.

### Feature Engineering

Lagged Prices (past price movements to capture trends)

Rolling Averages (short-term trends)

Volatility Measures (standard deviation of prices)

Order Flow Imbalance (difference between buy and sell orders)


### Model Development

Split the data into training and testing sets.

Machine Learning Models: Train Random Forest, XGBoost, and Support Vector Machines (SVM) to identify patterns.

We used a Gradient Boosting Model (XGBoost) to predict future price movements.

### Backtesting and Evaluation

Simulate trading strategies using historical data.

Evaluate performance with Mean Squared Error (MSE), Sharpe Ratio, and Profit-Loss ratios.

Compare results with traditional models such as ARIMA and GARCH.

Perform backtesting to simulate trading strategies based on model predictions.

### Deployment and Optimization

Deploy models in a real-time trading environment with low-latency infrastructure.




