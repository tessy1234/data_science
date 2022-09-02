Auto Regression Analysis:
-------------------------
Problem statement: Given ice cream production data forecast production for a future time period.

Model:
------
ARIMA model

Conclusion:
-----------
The forecast for the time period 01.01.2017 until 01.12.2019 shows precise predition at the beginning of the time period and a fading effect towards the end of the period (AR_Model_1).

A rolling forecast of one month predicts only one month ahead, waits for the month to pass by, learns a new model, predict the next month and continue the process until to the end of the time period.
