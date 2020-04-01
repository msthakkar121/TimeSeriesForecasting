# TimeSeriesForecasting
Performing forecasting on univariate time series data. 

### Dataset
The dataset describes the cumulative power produced by solar panels from 26th October 2011 to 27th July 2018. There are 2470 recorded observations which gives us the data for a period of six years and ten months. The unit of the observations is kWh. The source of the dataset is credited to Frank (https://www.kaggle.com/fvcoppen).

Below is a sample of the first 5 rows of data.

| 26/10/2011 |  0.1 |
|:----------:|:----:|
| 27/10/2011 | 10.2 |
| 28/10/2011 | 20.2 |
| 29/10/2011 | 29.6 |
| 30/10/2011 | 34.2 |

### Task
On the basis of univariate data provided, predict the power generation for the next three months, i.e. from 1st August 2018 to 31st October 2018.

### Approach 1 - Using ARIMA

ARIMA, short for 'Auto Regressive Integrated Moving Average' is a class of models that 'explains' a given time series based on its own past values, that is, its own lags and the lagged forecast errors, so that equation can be used to forecast future values.

### Approach 2 - Using LSTM (Neural Network)

LSTM, short for 'Long Short Term Memory' is a special kind of RNN (Recurring Neural Network) composed of a set of cells with features to memorize the sequence of data. The cell captures and stores the data streams. Further the cells inter-connect one module of past to another module of present one to convey information from several past time instants to the present one. Due to the use of gates in each cell, data in each cell can be disposed, filtered, or added for the next cells. The following image presents the unfolding of an LSTM unit. 

![RNN-LSTM.png](https://github.com/msthakkar121/TimeSeriesForecasting/blob/master/Images/RNN-LSTM.png)

In terms of working, the LSTM model provides considerably more options for fine-tuning compared to ARIMA.
