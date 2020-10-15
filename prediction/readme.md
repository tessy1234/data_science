weather forecasting:
--------------------
forecast air temperature 24 hours in the future.

dataset:
--------
weather timeseries dataset recorded at the Weather Station at the Max Planck Institute
for Biogeochemistry in Jena, Germany (https://www.bgc-jena.mpg.de/wetter/).
In this dataset, 14 different quantities (such as air temperature, atmospheric pressure,
humidity, wind direction, and so on) were recorded every 10 minutes, from 2009–2016.

repository location: 			data_science\data\jena_climate
dataset: 				jena_climate_2009_2016.csv
size:					420,551 lines of data
header:					date and 14 weather-related values

model:
------
GRU model in different complexity and regularization.

best-of-breed model:
--------------------
GRU model with 8 GRU-units. Best compromise between mean absolute error and overfitting.
