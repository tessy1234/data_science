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
 
file 				GRU-units 	dropout-regularized	dropout		recurrent_dropout	GRU-stacked	densely connected network	epochs
temperature_forecasting_02_*	8		n			-		-			n		n				20
temperature_forecasting_18_*	8		n			-		-			n		n				40
temperature_forecasting_19_*	8		n			-		-			n		n				60

results:
--------
file 				mean absolute error (MAE) [degree celsius]
temperature_forecasting_01_*	2.37
temperature_forecasting_02_*	2.31
temperature_forecasting_03_*	2.32
temperature_forecasting_04_*	2.31
temperature_forecasting_05_*	2.31
temperature_forecasting_06_*	2.35
temperature_forecasting_07_*	2.36
temperature_forecasting_08_*	2.33
temperature_forecasting_09_*	2.36
temperature_forecasting_10_*	2.43
temperature_forecasting_11_*	2.37
temperature_forecasting_12_*	2.37
temperature_forecasting_13_*	2.45
temperature_forecasting_14_*	2.37
temperature_forecasting_15_*	2.33
temperature_forecasting_16_*	2.33
temperature_forecasting_17_*	2.35
temperature_forecasting_18_*	2.35
temperature_forecasting_19_*	2.33

analysis:
---------
file 				GRU-units 	dropout-regularized	dropout		recurrent_dropout	GRU-stacked	densely connected network	epochs
temperature_forecasting_01_*	4		n			-		-			n		n				20
temperature_forecasting_02_*	8		n			-		-			n		n				20
temperature_forecasting_03_*	12		n			-		-			n		n				20
temperature_forecasting_04_*	16		n			-		-			n		n				20
temperature_forecasting_05_*	32		n			-		-			n		n				20
temperature_forecasting_06_*	64		n			-		-			n		y				20
temperature_forecasting_07_*	32		y			0.2		0.2			n		n				40
temperature_forecasting_08_*	32		y			0.1		0.3			n		n				20
temperature_forecasting_09_*	32		y			0.1		0.5			n		n				20
temperature_forecasting_10_*	32		y			0.4		0.4			n		n				20
temperature_forecasting_11_*	64		y			0.2		0.2			n		n				40
temperature_forecasting_12_*	64		y			0.2		0.2			n		y				40
temperature_forecasting_13_*	64		y			0.5		0.5			n		y				40
temperature_forecasting_14_*	8		n			-		-			n		y				20
temperature_forecasting_15_*	8		n			-		-			y (1x)		n				20
temperature_forecasting_16_*	8		n			-		-			y (1x)		n				40
temperature_forecasting_17_*	8		n			-		-			y (2x)		n				40
temperature_forecasting_18_*	8		n			-		-			n		n				40
temperature_forecasting_19_*	8		n			-		-			n		n				60
