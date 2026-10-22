# Stock Market Price Prediction using LSTM

This project predicts the next day's stock closing price using historical daily stock market data.

## Problem Statement

A financial analyst wants to predict future stock closing prices using historical market data.  
The model uses previous daily stock records to predict the next day's closing price.

## Dataset

The dataset contains daily stock market records with the following columns:

- Date
- Open
- High
- Low
- Close
- Volume

The `Close` price is used as the target variable.  
The previous 10 days of Open, High, Low, Close, and Volume values are used as input features.

## Tasks Completed

1. Loaded, cleaned, and normalized the stock dataset.
2. Generated input-output sequences using a window size of 10.
3. Selected and trained an LSTM model to predict the next day's closing price.
4. Evaluated the model using MAE and RMSE.
5. Plotted actual versus predicted prices and demonstrated prediction on unseen future data.

## Technologies Used

- Python
- TensorFlow
- Keras
- Scikit-learn
- Pandas
- NumPy
- Matplotlib
- Google Colab
- GitHub

## Model Architecture

- LSTM layer with 64 units
- Dropout layer
- LSTM layer with 32 units
- Dropout layer
- Dense layer with 16 neurons
- Dense output layer with 1 neuron

## Model Training

- Loss function: Mean Squared Error (MSE)
- Optimizer: Adam
- Learning rate: 0.001
- Batch size: 16
- Epochs: 100 with EarlyStopping

## Evaluation Metrics

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- Mean Absolute Percentage Error (MAPE)
- R2 Score

## Output Graphs

- Stock closing price trend
- Training and validation loss
- Actual versus predicted closing price
- Prediction on unseen next-day data
- Prediction for the next five days

## How to Run

1. Open the notebook in Google Colab.
2. Upload `random_stock_market_dataset.csv`.
3. Run all cells from top to bottom.
4. View the evaluation metrics and prediction graphs.

## Result

The LSTM model learns historical stock price patterns and predicts the next day's closing price.  
The model performance is evaluated using MAE, RMSE, MAPE, and R2 score.
