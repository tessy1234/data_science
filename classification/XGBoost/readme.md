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
The evaluation of the model on the test dataset results in the following confusion matrix:

|               |              | Prediction              |                          |
| ------------- | ------------ | ----------------------- | ------------------------ |
|               |              | <b>Negative</b>         | <b>Positive</b>          |
| <b>Actual</b> | <b>False</b> | TN= 94  [True Negative] | FP= 13  [False Positive] |
|               | <b>True</b>  | FN= 15  [False Negative]| TP= 32  [True Positive]  |

From the confusion matrix we get the following metrics:

| EmbeddingEncoder |          |
| ---------------- | -------- |
| ROC AUC          | Accuracy |
| 0.8833           | 85.21%   |



