# Customer Churn Prediction Model

## Overview
This project implements a **Customer Churn Prediction Model** using machine learning(ANN) techniques. The aim is to predict whether a customer will churn (leave) based on various factors.

## Data Preprocessing
The following steps were carried out to prepare the data by using **pandas** for model training:

1. **Removed Customer ID**: 
   - The customer ID column was dropped as it is not relevant for prediction and does not contribute to the model.

2. **Converted String Values to Numeric**:
   - Categorical string columns were converted to numeric values using pandas.

3. **Replaced Boolean Values with 1 and 0**:
   - All boolean values in the dataset were replaced with binary representations, where `True` was converted to `1` and `False` to `0`.

4. **Converted Some Columns into Dummy Columns**:
   - Categorical columns with more than two values were converted into dummy/one-hot encoded columns. For binary columns, `True` was converted to `1` and `False` to `0`.

5. **Handled Missing Values**:
   - Any missing or NaN values were handled appropriately by either filling them with suitable values (e.g., mean or median) or by dropping the rows.

## Model Training
1. **Initial Model Training**:
   - After preprocessing, the data was split into training and testing sets.
   - Artificial Neural Network were used to train the model.
   
2. **Overfitting Detected**:
   - During the training process, overfitting was detected, where the model performed well on the training data but poorly on the testing data.
   
3. **Overfitting Mitigation**:
   - To address overfitting, techniques like dropout (for deep learning models) were employed.
  

## Results
The final model was tested on the test dataset and achieved an accuracy of **%94**
