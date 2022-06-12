Problem Statement:
------------------
Predict whether it will rain today or not based on weather measurements.

Dataset:
--------
data source: https://www.kaggle.com/datasets/jsphyg/weather-dataset-rattle-package

Model:
------

Use XGBosst classifier, tune parameter using grid search, encode categorical variables with EmbeddingEncoder, OneHotEncoder and OrdinalEncoder.

Performance:
------------
The evaluation of the model on the test dataset using different encoding schemes:

| EmbeddingEncoder |          | OneHotEncoder    |          | OrdinalEncoder   |          |
| ---------------- | -------- | ---------------- | -------- | ---------------- | -------- |
| ROC AUC          | Accuracy | ROC AUC          | Accuracy | ROC AUC          | Accuracy |
| 0.8833           | 85.21%   | 0.8833           | 85.21%   | 0.8833           | 85.21%   |



