# Next-Generation Time-Series Forecasting Using Machine Learning and Deep Learning

## Overview
This project explores NIFTY 50 stock price prediction using traditional machine learning and deep learning techniques. Historical Open, Close, High, and Low prices are transformed into supervised learning datasets using sliding windows. Multiple models are trained and evaluated to compare prediction errors across different input-window sizes and target price columns.

## Objectives
- Predict stock prices using historical NIFTY 50 data.
- Generate input-output sequences using sliding windows of different lengths.
- Compare traditional machine learning regressors with deep learning models.
- Evaluate model performance using MAE and RMSE.
- Identify promising model configurations and save trained models for reuse.

## Technologies Used
- **Programming Language:** Python
- **Data Processing:** Pandas, NumPy
- **Machine Learning:** Scikit-learn, XGBoost, LightGBM
- **Deep Learning:** TensorFlow, Keras
- **Visualization:** Matplotlib
- **Progress Tracking:** tqdm
- **Model Persistence:** Joblib

## Models Implemented

### Machine Learning Models
- Linear Regression
- Ridge Regression
- Lasso Regression
- Random Forest Regressor
- Gradient Boosting Regressor
- Support Vector Regression (SVR)
- K-Nearest Neighbors (KNN)
- XGBoost Regressor
- LightGBM Regressor

### Deep Learning Models
- Simple Recurrent Neural Network (RNN)
- Long Short-Term Memory (LSTM)
- Gated Recurrent Unit (GRU)
- Bidirectional LSTM

## Project Workflow

### 1. Data Loading
Load historical stock price data from `data.csv` using Pandas. The project analyzes the `Open`, `Close`, `High`, and `Low` columns.

### 2. Data Preparation
Create supervised learning datasets using a sliding-window function. The previous 30, 45, 60, 90, 120, 150, 200, or 250 price observations are used as inputs to predict the next value for the selected price column.

### 3. Model Development
Build a collection of machine learning regressors and neural networks. The RNN, LSTM, GRU, and Bidirectional LSTM models use 50 recurrent units and a dense output layer for regression.

### 4. Model Training
Train the models on the generated datasets. The code uses a 90% training and 10% testing split through `train_test_split`. Deep learning models are trained for 50 epochs with a batch size of 8.

### 5. Model Evaluation
Calculate the following metrics for both training and testing data:
- **MAE (Mean Absolute Error):** Measures the average absolute difference between actual and predicted prices.
- **RMSE (Root Mean Squared Error):** Measures prediction errors while giving larger errors more weight.

### 6. Model Comparison and Visualization
Rank the trained model configurations by test MAE and examine the top 50 results. Visualizations compare training and testing errors and show the frequency of different input-window sizes, target columns, and model types among the top-performing configurations.

### 7. Model Saving and Inference
Save the evaluation results to `models.csv` and the trained model objects and their metrics to `trained_models.joblib`. Reload a saved model and use it to generate a prediction from a prepared input sequence.

## Key Findings

In the reported experiment, KNN, Ridge Regression, Linear Regression, and Random Forest appeared frequently among the top 50 configurations ranked by test MAE. The 30-, 90-, and 120-day windows were frequently represented, and models predicting the `High` price appeared prominently.

These observations describe the reported experiment; they do not establish that the same models will perform best on future market data.

## Files Generated
- `data.csv` — Input stock price dataset.
- `models.csv` — Model evaluation results.
- `trained_models.joblib` — Saved models and evaluation metrics.
- Jupyter Notebook — Data preparation, training, evaluation, visualization, and inference workflow.

## Future Improvements
- Apply hyperparameter tuning to the most promising model configurations.
- Use chronological train-test splitting and time-series cross-validation.
- Compare results with simple baseline forecasting methods.
- Evaluate performance across different forecast horizons and market conditions.

## Disclaimer
This project is intended for educational purposes. Stock prices are uncertain, and model predictions should not be treated as financial advice.

