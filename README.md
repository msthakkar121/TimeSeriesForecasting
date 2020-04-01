# TimeSeriesForecasting
Performing forecasting on univariate time series data. 

### Dataset
The dataset describes the number of daily female births in California, USA in the year 1959. There are 365 recorded observations which gives us the data for a period of one year. The units are a count and there are 365 observations. The source of the dataset is credited to Newton (1988).

Below is a sample of the first 5 rows of data including the header row.

|    Date    | Daily total female births in California, 1959 |
|:----------:|:---------------------------------------------:|
| 1959-01-01 |                       35                      |
| 1959-01-02 |                       32                      |
| 1959-01-03 |                       30                      |
| 1959-01-04 |                       31                      |
| 1959-01-05 |                       44                      |

### Task
On the basis of univariate data provided, predict the number of births for the next six months, i.e. from 1960-01-01 to 1960-06-30.

### Approach 1 - Using ARIMA

ARIMA, short for 'Auto Regressive Integrated Moving Average' is a class of models that 'explains' a given time series based on its own past values, that is, its own lags and the lagged forecast errors, so that equation can be used to forecast future values.

### Approach 2 - Using LSTM (Neural Network)

LSTM, short for 'Long Short Term Memory' is a special kind of RNN (Recurring Neural Network) composed of a set of cells with features to memorize the sequence of data. The cell captures and stores the data streams. Further the cells inter-connect one module of past to another module of present one to convey information from several past time instants to the present one. Due to the use of gates in each cell, data in each cell can be disposed, filtered, or added for the next cells. The following image presents the unfolding of an LSTM unit. 

![RNN-LSTM.png](https://github.com/msthakkar121/TimeSeriesForecasting/blob/master/Images/RNN-LSTM.png)

In terms of working, the LSTM model provides considerably more options for fine-tuning compared to ARIMA.
