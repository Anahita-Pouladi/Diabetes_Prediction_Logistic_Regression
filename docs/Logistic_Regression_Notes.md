# Logistic Regression Notes

## Overview

Logistic Regression is a classification algorithm used to estimate the
probability of a binary outcome.

Unlike regression models that predict continuous values, Logistic
Regression predicts the probability that an observation belongs to a
specific class.

------------------------------------------------------------------------

## Probability Output

The model produces a probability score representing the likelihood of
belonging to the positive class.

This probability is converted into a final class label using a
classification threshold.

------------------------------------------------------------------------

## Classification Threshold

The default classification threshold is commonly 0.5.

Changing the threshold affects the balance between:

-   Precision
-   Recall
-   F1 Score

In medical prediction tasks, threshold selection can be important
because identifying positive cases may have higher priority.

------------------------------------------------------------------------

## Model Evaluation Metrics

Important classification metrics include:

-   Accuracy
-   Precision
-   Recall
-   F1 Score
-   ROC-AUC
-   Confusion Matrix

Accuracy alone may not provide enough information, especially when the
cost of false negatives and false positives is different.

------------------------------------------------------------------------

## Hyperparameter Tuning

GridSearchCV can be used to evaluate different model configurations and
identify suitable hyperparameters.

However, tuning does not always guarantee better performance.
Improvements should always be validated using appropriate evaluation
metrics.

------------------------------------------------------------------------

## Threshold Optimization

A model can sometimes achieve better practical results by adjusting the
decision threshold rather than changing the algorithm.

This approach allows the prediction strategy to be aligned with the
objective of the problem.
