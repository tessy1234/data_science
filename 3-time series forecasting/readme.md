Auto Regression Analysis:
-------------------------
Problem statement: Given ice cream production data forecast production for a future time period.

Model:
------
ARIMA model of order (3,0,0). The first three lags in the PACF shows high statistical significance and 
therefore a three lag autoregression model has been chosen.

Conclusion:
-----------
The forecast for the time period 01.01.2017 until 01.12.2019 shows precise prediction at the beginning of the time period 
and a fading effect towards the end of the period (AR_Model_1). 
The plot exhibit the difference between ML prediction and time series forecasting. 
In time series time steps depend on previous time steps and this explains the fading effect for the prediction.

A rolling forecast of one month predicts only one month ahead, waits for the month to pass by, learns a new model, 
predict the next month and continue the process until to the end of the time period.
The plot shows a close fit between forecast and actual ice cream production even for the repeating seasonal time period (AR_Model_2).

The M-Lead Rolling Forecast is the same as the one-month forecast described above but with the difference that 
the prediction is done several months ahead. The result shows a deterioration of the forecast 
compared with the one-month solution (AR_Model_3). 

Moving Average Analysis:
------------------------
Synthetic random data from a Gaussian distribution has been generated in order to simulate the moving average process.
The ACF shows two lags that are statistical relevant and confirms the two-lags moving average process. 
Therefore an ARIMA model of order (0,0,2) has been chosen (MA Model).

The final plot shows the forecast of the last two days (2019.12.31 and 2020.01.01) of the time period.

Deep Learning Forecasting:
--------------------------
A deep learning model has been chosen to forecast air temperature 24 hours in the future (see deep learning forecasting folder)
