# TSMC Stock Price Direction Prediction using LSTM

## Overview
This project implements a Long Short-Term Memory (LSTM) neural network to predict
the direction (up/down) of TSMC (2330) stock prices using daily trading data from 2024.

## Dataset
- Source: Yahoo Finance
- Stock Symbol: 2330.TW
- Features:
  - Open
  - High
  - Low
  - Close
  - Volume
- Target:
  - 1 = Next day's closing price is higher
  - 0 = Next day's closing price is lower or equal

## Methodology
1. Data preprocessing and normalization using Min-Max scaling
2. Sequence creation using a 10-day look-back window
3. LSTM model with dropout regularization
4. Binary classification using sigmoid activation
5. Model evaluation using accuracy and confusion matrix

## Technologies Used
- Python
- TensorFlow / Keras
- NumPy
- Pandas
- Scikit-learn

## Results
The LSTM model achieved approximately 55–60% accuracy on test data, which is
reasonable for financial time-series direction prediction.

## Disclaimer
This project is for academic and educational purposes only and does not constitute
financial advice.
