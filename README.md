# Credit-Risk-Classification

## Overview of the Analysis

This analysis is focused on training a model to evaluate and assess the risk associated with a list of loans in a dataset. The dataset is based on the history of a peer-to-peer lending company so that the risk of borrowers can be analysed. The most important values to count were "0" and "1" within the "loan_status" column of the dataset. This is a direct indicator of the health of a loan and the creditworthiness of an individual, since "0" means healthy and "1" means a high risk of defaulting. A logistic regression model was created and trained on a small subset of the data using `LogisticRegression` from scikit_learn. The model then tested the entire dataset and its performance was evaluated using a confusion matrix and classification report.


## Results

* Machine Learning Model:
    * Accuracy: 99%
    * Precision: 100% in detecting low risk, 87% in detecting high risk
    * Recall: 100% in low risk, 89% in high risk

## Summary

The model is able to successfully predict the healthy loans within the dataset with 100% precision. Additionally, as the f1-score is 1, the model is able to successfully predict loans which can be classified as healthy. With regards to high-risk loans, the model is not as precise, but still maintains a very good precision of 87%. Due to the reduced precision (and recall score), the f1-score does suffer somewhat. With an f1-score of 0.88, the model is very good at predicting high-risk loans, but it is not perfect.
