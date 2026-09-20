# Diabetes Prediction \| Logistic Regression

An end-to-end binary classification workflow covering data analysis,
Logistic Regression modeling, model evaluation, hyperparameter tuning,
and threshold optimization.

------------------------------------------------------------------------

## Project Overview

This project develops a classification workflow to predict diabetes
outcomes using Logistic Regression.

The focus is not only on model performance, but also on understanding
the dataset, validating data quality, exploring relationships between
features, preparing the data correctly, evaluating the model, and
interpreting the results.

------------------------------------------------------------------------

## Key Highlights

-   Interpretable Logistic Regression baseline
-   Evaluation using Accuracy, Precision, Recall, F1 Score, and ROC-AUC
-   Hyperparameter tuning with GridSearchCV
-   Classification threshold optimization
-   Focus on reproducible and explainable ML workflow

------------------------------------------------------------------------

## Project Structure

``` text
Diabetes_Prediction_Logistic_Regression/

├── data/
│   └── diabetes.csv

├── docs/
│   └── Logistic_Regression_Notes.md

├── images/
│   ├── correlation_matrix.png
│   ├── roc_curve.png
│   ├── threshold_optimization.png
│   └── confusion_matrix.png

├── notebooks/
│   └── Diabetes_Prediction_Logistic_Regression.ipynb

├── README.md
├── requirements.txt
└── .gitignore
```

------------------------------------------------------------------------

## Dataset

The dataset contains medical measurements and demographic information
used to predict diabetes outcomes.

Target Variable:

-   Outcome
    -   0 → No Diabetes
    -   1 → Diabetes

------------------------------------------------------------------------

## Model Improvement

GridSearchCV was applied to evaluate different Logistic Regression
configurations.

The tuned model was compared with the baseline model. The results showed
that hyperparameter tuning does not always guarantee better performance.

Threshold optimization was also evaluated by testing different
classification thresholds to improve the strategy for identifying
positive cases.

------------------------------------------------------------------------

## Model Insights

## Correlation Analysis

![Correlation Matrix](images/correlation_matrix.png)

## Threshold Optimization

![Threshold Optimization](images/threshold_optimization.png)

## Final Confusion Matrix

![Confusion Matrix](images/confusion_matrix.png)

## ROC Curve

![ROC Curve](images/roc_curve.png)

------------------------------------------------------------------------

## Future Improvements

Possible future improvements:

-   Compare additional algorithms:
    -   Random Forest
    -   Gradient Boosting
    -   XGBoost
    -   Support Vector Machines
-   Advanced feature engineering
-   More extensive hyperparameter optimization
-   Ensemble modeling

------------------------------------------------------------------------

## Technologies & Libraries

-   Python
-   Pandas
-   NumPy
-   Matplotlib
-   Seaborn
-   Scikit-learn

------------------------------------------------------------------------

## What I Learned

The main lesson from this project was that improving a machine learning
model is not only about achieving a higher metric value.

Building a Logistic Regression baseline provided an interpretable
starting point and helped evaluate how different metrics reflect model
performance. This project showed that in medical classification
problems, recall, precision, and the cost of prediction errors are as
important as accuracy.

GridSearchCV was useful for testing different model configurations, but
the results showed that more complex tuning does not always lead to
better performance. The biggest improvement came from optimizing the
classification threshold and aligning the decision strategy with the
goal of identifying positive cases.

This project reinforced the importance of building reproducible
workflows, validating improvements with evidence, and making every
modeling decision clear and explainable.
