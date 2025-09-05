# LSTM-Based Apple Stock Price Predictor

This project demonstrates how to use a **Long Short-Term Memory (LSTM)** neural network to forecast stock prices, focusing on **Apple Inc. (AAPL)**. The model leverages historical stock data to predict future trends in stock prices.

---

## Project Highlights

The project workflow includes the following key steps:

1. **Data Acquisition and Preprocessing**
   - Download historical AAPL stock data using Yahoo Finance (`yfinance`) from 2015 to present.
   - Compute moving averages (e.g., MA5, MA10, MA20, MA50) for trend analysis.
   - Normalize data to prepare it for the LSTM model.

2. **Dataset Preparation**
   - Transform time series data into a supervised learning format using a **sliding window** approach.
   - Each input sequence consists of `n` past days of stock features to predict the next day's prices.

3. **LSTM Model Development**
   - Build a **multi-layer LSTM network** for sequential prediction.
   - Incorporate **Dropout layers** to reduce overfitting.
   - Use **Early Stopping** to halt training when performance plateaus.

4. **Prediction and Evaluation**
   - Predict stock prices for both training and testing datasets.
   - Evaluate the model using:
     - **Mean Squared Error (MSE)**
     - **Root Mean Squared Error (RMSE)**
     - **Mean Absolute Percentage Error (MAPE)**
   - Visualize **Actual vs Predicted** prices to assess model performance.

5. **Future Price Forecasting**
   - Use the trained model to predict prices for upcoming dates (e.g., a specific week in September).
   - Sliding window method ensures predictions are based on the latest historical data.

---
