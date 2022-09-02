Problem Statement:
------------------
Predict whether it will rain today or not based on weather measurements.

Dataset:
--------
Data source: https://www.kaggle.com/datasets/jsphyg/weather-dataset-rattle-package

Model:
------
Apply XGBosst classifier, tune parameter using grid search, encode categorical variables with EmbeddingEncoder, OneHotEncoder and OrdinalEncoder.

Performance:
------------
The evaluation of the model on the test dataset using different encoding schemes:

| EmbeddingEncoder |          | OneHotEncoder    |          | OrdinalEncoder   |          |
| ---------------- | -------- | ---------------- | -------- | ---------------- | -------- |
| ROC AUC          | Accuracy | ROC AUC          | Accuracy | ROC AUC          | Accuracy |
| 0.8830           | 85.16%   | 0.88326          | 85.23%   | 0.88332          | 85.21%   |



