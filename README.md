# Time Series Demand Forecasting
The airline daily passengers are predicted by using LSTM model.

The dataset is based on the International Airline Passengers dataset [link](https://raw.githubusercontent.com/jbrownlee/Datasets/master/airline-passengers.csv).  
The link below  is the tutorial of the dataset [link](https://machinelearningmastery.com/time-series-prediction-lstm-recurrent-neural-networks-python-keras/).

<br>

## Stacked two-layer lstm regression model
* RMSE in test period: 22.66
* MAE is test period: 18.28
![](https://user-images.githubusercontent.com/30923675/78865607-dc5d7d00-7a78-11ea-95ea-13a8f25a57c0.png)

## Stacked two-layer gru regression model
* RMSE in test period: 22.47
* MAE is test period: 18.16
![](https://user-images.githubusercontent.com/30923675/78866401-41fe3900-7a7a-11ea-985f-75fdb9ddcd7b.png)

## Seq2se2 two-layer lstm model
### 1. When predicted next month passengers.
Note that the test period is diffrent from other models.
* RMSE in test period: 19.38
* MAE is test period: 15.97
![](https://user-images.githubusercontent.com/30923675/78984666-caa3d480-7b61-11ea-9f9e-78534a44cf8b.png)

### 2. When predicted passengers in five months.
Note that the test period is diffrent from other models.
* RMSE in test period: 21.51
* MAE is test period: 18.21
![](https://user-images.githubusercontent.com/30923675/78984671-cd9ec500-7b61-11ea-94dd-23def3eb7735.png)

## Prophet library
[Prophet](https://facebook.github.io/prophet/) is a procedure for forecasting time series data based on an additive model where non-linear trends are fit with yearly, weekly, and daily seasonality, plus holiday effects.
* RMSE in test period: 40.36
* MAE is test period: 31.17
![](https://user-images.githubusercontent.com/30923675/78988604-5f133480-7b6c-11ea-8285-d5e24401a5c7.png)