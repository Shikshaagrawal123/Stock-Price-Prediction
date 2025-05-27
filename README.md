# Stock-Price-Prediction
# Stock Price Prediction (Next-Day) Using Linear Regression

## Project Overview

This project aims to predict the **next-day closing price** of a stock using historical stock market data. By leveraging regression analysis on features such as the previous day's closing price and a 5-day moving average, the model forecasts short-term price trends to assist in informed investment decisions.

The project is implemented in Python using popular libraries such as pandas, NumPy, matplotlib, and scikit-learn. The data is uploaded and processed in Google Colab.

---

## Problem Statement

Predicting stock prices accurately is a challenging task due to market volatility and numerous influencing factors. This project focuses on building a **regression-based model** to predict the next-day closing price of a stock using historical pricing data, providing valuable insights for traders and investors.

---

## Methodology

1. **Data Preprocessing**  
   - Convert the `Date` column to datetime format and sort data chronologically.  
   - Create features: previous closing price (`Prev_Close`) and 5-day moving average (`5day_MA`).  
   - Define the target variable as the next-day closing price (`Next_Close`).  
   - Remove missing values resulting from rolling calculations and shifting.

2. **Model Training**  
   - Split data into training (80%) and testing (20%) sets without shuffling to preserve time order.  
   - Train a Linear Regression model using `Prev_Close` and `5day_MA` as predictors.

3. **Evaluation**  
   - Predict next-day prices on the test set.  
   - Evaluate model accuracy using Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R² score.  
   - Visualize actual vs predicted prices and the historical price trend.

---

## Requirements

- Python 3.x  
- pandas  
- numpy  
- matplotlib  
- scikit-learn  
- Google Colab (for file upload and execution) or any Python IDE

You can install the required Python libraries via pip:

```bash
pip install pandas numpy matplotlib scikit-learn
