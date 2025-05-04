# Stock Price Prediction Using GRU and LSTM

## Overview
This project focuses on stock price prediction using deep learning models, specifically GRU and LSTM. It integrates two datasets: stock price data and financial news data. Sentiment analysis is performed on financial news using FinBERT, and the extracted sentiment scores are combined with stock price features to improve prediction accuracy.

## Features and Methodology
- **Datasets Used**:
  - Stock price data (historical prices)
  - Financial news data
- **Feature Engineering**:
  - Extracted sentiment scores from financial news using **FinBERT**
  - Added technical indicators: **Daily Return, EMA_100, RSI, Volatility_10**
  - Standardized data using **Robust Scaling**
- **Model Training**:
  - Implemented **GRU** and **LSTM** models
  - Combined stock price and sentiment data for training
  - Performance Metrics:
    - **GRU**: Train Loss - **0.1948**, Validation Loss - **0.24**, Test Loss - **0.35**
    - **LSTM**: Train Loss - **0.1933**, Validation Loss - **0.30**, Test Loss - **0.35**
- **Adversarial Training**:
  - Applied **Projected Gradient Descent (PGD)** adversarial training on a stacked GRU model
  - Found that adversarial training weakened performance compared to the standard GRU


## Results & Insights
- The **GRU** model outperformed **LSTM** in validation loss.
- Adversarial training using PGD did not improve the performance of the GRU model.
- Sentiment analysis using **FinBERT** contributed additional predictive power.
- Adding technical indicators improved overall model accuracy.



--------------------------------------------------------------------------
If you find this project useful, don't forget to ⭐ the repo!
![Uploading image.png…]()
