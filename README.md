# Google Stock Price Forecasting

This project explores the use of Long Short Term Memory(LSTM) to forecast Google's stock prices over time(from 2021). By leveraging historical stock data, a Long Short-Term Memory (LSTM) model is trained to predict future stock prices based on historical trends. The project demonstrates time-series forecasting with the help of LSTMs. This project is intended solely for educational and exploratory purposes.

## Project Overview

The project involves the following steps:
1. **Data Loading**: Data was loaded from the CSV file.
2. **Feature Engineering**: Data normalization was applied to optimize model performance.
3. **Modeling with LSTM**: A Long Short-Term Memory (LSTM) model was implemented suing Pytorch, given its effectiveness in capturing time-series patterns. The model was trained on the processed dataset to learn from historical trends.
4. **Evaluation**: The model's performance was evaluated using training and testing error metrics to ensure predictive accuracy.

## Dataset

- **Source**: The dataset was obtained from Kaggle.
- **Attributes**:
    - `Date`: Date of the stock record.
    - `Open`: Opening price of the stock on that day.
    - `High`: Highest price during the day.
    - `Low`: Lowest price during the day.
    - `Close`: Closing price of the stock.
    - `Adj Close`: Adjusted closing price, taking into account dividends and stock splits.
    - `Volume`: Volume of stock traded on that day.

The data spans from 2004-08-19, capturing the historical trends of Google's stock performance.
Dataset Link: https://www.kaggle.com/datasets/henryshan/google-stock-price

## Model & Training
We chose an LSTM neural network for time-series forecasting due to its ability to capture sequential dependencies in data. The model was trained over multiple epochs with an optimized learning rate to minimize the Mean Squared Error (MSE).

### Key Model Details:
- **Model Architecture**: A simple LSTM model with hidden layers designed to capture stock price trends.

- **Evaluation Metrics**: Mean Squared Error (MSE) and R-squared score was used to evaluate the model.

## Results
The LSTM model demonstrated the capability to capture and predict stock price movements with reasonable accuracy, although financial forecasting remains inherently challenging. Key insights include:

- **Predictive Performance**: While the model performed well on historical data, it highlighted the volatility and unpredictability of stock prices, especially in shorter time frames.
- **Evaluation**: The training and testing error metrics showed that the model could generalize on unseen data, though further tuning could improve results.
- **The model obtained a mean-squared-error of 4.988 and R-squared score of 0.982**

## Conclusion
This project underscores the potential and challenges of using LSTM models for financial forecasting. The results are promising for historical trend analysis, but stock prediction remains a highly volatile task. Future work could involve experimenting with additional features, using more advanced architectures, or combining models to enhance predictive accuracy.
