# Recurrent Neural Network

This repository contains code for a Recurrent Neural Network (RNN) designed to predict Google stock prices. 

## Part 1 - Data Preprocessing

In this section, I preprocess the data to prepare it for training the RNN. This involves importing necessary libraries such as NumPy, Matplotlib, and Pandas, and loading the training dataset from a CSV file. Then, I scale the data using MinMaxScaler to normalize it between 0 and 1. After that, I create a data structure with 60 timesteps and 1 output, which helps the RNN learn patterns in the data.

## Part 2 - Building the RNN

Here, I construct the RNN model using Keras. Firstly, I import the required Keras modules - Sequential, Dense, LSTM, and Dropout. Then, I initialize the RNN as a sequential model and add LSTM layers with dropout regularization to prevent overfitting. The LSTM layers are stacked to create a deep RNN architecture. Finally, I compile the RNN with the Adam optimizer and mean squared error loss function.

## Part 3 - Making Predictions and Visualizing Results

In this part, I make predictions using the trained RNN model and visualize the results. I load the test dataset, preprocess it in a similar manner as the training data, and generate predictions for the stock prices. Then, I inverse scale the predicted prices to get them back to their original scale. Finally, I plot the real and predicted stock prices using Matplotlib to visually compare the model's performance.
