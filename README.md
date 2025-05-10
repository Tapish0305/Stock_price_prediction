# Stock Price Prediction Using GRU and LSTM

## Overview
This project focuses on stock price prediction using deep learning models, specifically GRU and LSTM. It integrates two datasets: stock price data and financial news data. Sentiment analysis is performed on financial news using FinBERT, and the extracted sentiment scores are combined with stock price features to improve prediction accuracy.

## Features and Methodology
- **Datasets Used**:
  - Stock price data taken via kaggle
  - Financial news data taken via alphavantage API
- **Feature Engineering**:
  - Extracted sentiment scores from financial news using **FinBERT**
  - Added technical indicators: **Daily Return, EMA_100, RSI, Volatility_10**
  - Standardized data using **Robust Scaling**
- **Model Training**:
  - Implemented **GRU** and **LSTM** models
  - Combined stock price and sentiment data for training
  - Performance Metrics:
    - **GRU**: Train Loss - **0.2694**, Validation Loss - **0.9557**, Test Loss - **0.39**
    - **LSTM**: Train Loss - **0.2475**, Validation Loss - **0.9265**, Test Loss - **0.3954**
- **Adversarial Training**:
  - Applied **Projected Gradient Descent (PGD)** adversarial training on a stacked GRU model
  - Found that adversarial training performance better compared to the standard GRU
    - **Adversinal Training**: Train Loss - **0.0495**, Validation loss - **0.0459**, Test loss - **0.02414**


## Results & Insights
- The **Adversinal Trained** model outperformed **GRU**,**LSTM** in validation loss and Test loss.
- The **LSTM** model outperform **GRU** model.
- Sentiment analysis using **FinBERT** contributed additional predictive power.
- Adding technical indicators improved overall model accuracy.



--------------------------------------------------------------------------
If you find this project useful, don't forget to ⭐ the repo!
![Uploading image.png…]()
