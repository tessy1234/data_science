Application:
------------
Classify persons having diabetes or not using classical machine learning techniques. It is a typical binary classification problem.

Dataset:
--------
A dataset consists of 768 instances and nine features with eight clinical features and one outcome feature.

The eight clinical features, also called predictor variables, are:  Pregnancies, Glucose, Blood Pressure, Skin Thickness, Insulin, BMI, Diabetes Pedigree Function, Age.

The target variable is called Outcome with values zero or one.

Model:
------
A K-Nearest Neighbors classifier (KNN) is used to accomplish the task. KNN is based on feature similarity and is mostly used for classification. It classifies a new instance based on how its neighbors are classified. Neighbors are found by calculating the Euclidean distance from all the points in the dataset to the unknown data point. The classification is done by taking the classes of the nearest neighbors to determine the majority vote which provides the class to be predicted.

Performance:
------------
The evaluation of the model on the test dataset results in the following confusion matrix:

|               |              | Prediction              |                          |
| ------------- | ------------ | ----------------------- | ------------------------ |
|               |              | <b>Negative</b>         | <b>Positive</b>          |
| <b>Actual</b> | <b>False</b> | TN= 94  [True Negative] | FP= 13  [False Positive] |
|               | <b>True</b>  | FN= 15  [False Negative]| TP= 32  [True Positive]  |

From the confusion matrix we get the following metrics:

| F1 score | accuracy |
| -------- | -------- |
| 69.56%   | 82%      |



