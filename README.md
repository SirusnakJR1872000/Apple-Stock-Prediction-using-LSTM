# Apple-Stock-Prediction-using-LSTM

Project Overview
The project tries to forecast future stock values for Apple (AAPL) using deep learning techniques, notably Long Short-Term Memory (LSTM) neural networks. 
The objective is to use previous stock price data to create a predictive model capable of forecasting prices for a specific number of days in the future.

Key Components and Steps:

Data Collection:

I used the Tiingo API to retrieve daily historical stock price data for Apple over the course of five years.
The data contains open, high, low, and close prices, as well as volume.

Data preprocessing:

Preprocessed the raw data by scaling numerical characteristics with MinMaxScaler to normalise them between 0 and 1.
The data was organised into sequences appropriate for training the LSTM model.
Model Development:

I used TensorFlow and Keras to build an LSTM model architecture.
The LSTM layers were configured using dropout regularisation to reduce overfitting and increase generalisation.
The model was constructed using the Adam optimizer and the mean squared error loss function.

Model Training:

I trained the LSTM model using preprocessed historical data.
The model's performance was assessed using measures such as Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and Mean Absolute Percentage Error (MAPE).
Model Evaluation:

I evaluated the model's accuracy and performance on both training and testing datasets.
The model's ability to forecast actual stock prices was measured using assessment measures.
Future Price Predictions:

Using the trained LSTM model, I implemented a function that predicts future stock values for a set number of days.
Inverse scaling was used to bring anticipated values back to their original scale, allowing for meaningful interpretation.

The project's goal is to give a realistic application of deep learning to financial forecasting, especially predicting Apple stock prices. utilising LSTM networks and extensive assessment procedures, the research aims to provide insights into the feasibility and usefulness of utilising sophisticated machine learning techniques to anticipate stock market movements.
