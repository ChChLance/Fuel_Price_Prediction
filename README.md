# Fuel_Price_Prediction
### Use time series analysis skills like SARIMA model and deep learning RNN model to predict the fuel price, so we can decide whether we should fuel the car now or later 

### Steps:
### 1. Gathering "Weekly U.S. Regular All Formulations Retail Gasoline Prices  (Dollars per Gallon) data" from U.S. Energy Information Administration
### 2. Data preparation process such as filling null values and removing unnecessary rows & columns
### 3. Traning SARIMA and deep learning RNN models
### 4. Comparing thier results by using chart and metrics
### 5. Creating a function that predict fuel price for the following week by using the best model with lower MSE
### Use case examples:
#### - Assumption: SARIMA model's mse < RNN model's mse, and the predicted price of 2022-08-21 is $2.68
#####   1. If fuel price today is $4 --> Function will return "[SARIMA Model] Fuel price will go down to $2.68 in a week" --> we should fuel a car later
#####   2. If fuel price today is $2.5 --> Function will return "[SARIMA Model] Fuel price will go up to $2.68 in a week" --> we should fuel a car now
