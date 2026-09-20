# Diabetes Prediction | Logistic Regression

## Project Overview

This project presents an end-to-end binary classification workflow to
predict diabetes outcomes using Logistic Regression.

The objective was not only to build a predictive model, but also to
understand the complete machine learning workflow: data validation,
exploratory analysis, preprocessing, model evaluation, optimization
strategies, and decision-making based on model objectives.

------------------------------------------------------------------------

## Problem Statement

Diabetes prediction is a binary classification problem where the goal is
to identify whether a patient is likely to have diabetes based on
medical-related features.

In healthcare-related machine learning tasks, evaluating a model
requires more than accuracy alone. Understanding false positives, false
negatives, recall, and precision is essential when making prediction
decisions.

------------------------------------------------------------------------

## Dataset

The dataset contains medical measurements and demographic information
used to predict diabetes outcomes.

### Target Variable

**Outcome**

-   0 → No Diabetes
-   1 → Diabetes

------------------------------------------------------------------------

# Project Workflow

## 1. Data Understanding & Validation

Performed:

-   Dataset structure review
-   Feature inspection
-   Data quality checks
-   Missing value analysis
-   Duplicate review
-   Initial statistical analysis

The purpose was to understand the dataset before applying machine
learning techniques.

------------------------------------------------------------------------

## 2. Exploratory Data Analysis

The following analyses were performed:

-   Target distribution analysis
-   Numerical feature distributions
-   Feature relationship analysis
-   Pearson correlation analysis
-   Outlier review

Key observations from EDA were used to guide preprocessing and modeling
decisions.

------------------------------------------------------------------------

## 3. Data Preparation

Preparation steps included:

-   Separating features and target
-   Train/test split
-   Feature scaling
-   Preparing data for Logistic Regression

------------------------------------------------------------------------

# Modeling

## Baseline Logistic Regression

Logistic Regression was selected as an interpretable baseline
classification model.

Reasons for selecting this model:

-   Provides probability-based predictions
-   Allows feature coefficient interpretation
-   Creates a clear and explainable baseline

The baseline model was evaluated using multiple metrics rather than
accuracy alone.

------------------------------------------------------------------------

# Model Evaluation

Metrics used:

-   Accuracy
-   Precision
-   Recall
-   F1 Score
-   ROC-AUC
-   Confusion Matrix

For medical classification problems, recall is especially important
because it reflects the model's ability to identify positive cases.

------------------------------------------------------------------------

# Model Improvement

## Hyperparameter Tuning with GridSearchCV

GridSearchCV was applied to evaluate different Logistic Regression
configurations.

Parameters explored:

-   Regularization strength (`C`)
-   Penalty type
-   Solver

The tuned model was compared with the baseline model.

### Result

The GridSearchCV model did not outperform the baseline model.

This demonstrates that increasing model complexity or tuning parameters
does not always guarantee better performance.

------------------------------------------------------------------------

## Threshold Optimization

Logistic Regression produces probabilities before assigning final class
labels.

Different classification thresholds were evaluated:

-   0.3
-   0.4
-   0.5
-   0.6

### Selected Decision Strategy

A threshold of **0.3** improved the model's ability to identify positive
diabetes cases.

Compared with the default threshold:

-   Recall improved significantly
-   F1 Score improved
-   More positive cases were detected

This improvement came from adjusting the decision strategy rather than
changing the algorithm.

------------------------------------------------------------------------

# Final Insights

This project demonstrated that improving a machine learning system
involves more than selecting a more complex model.

Important lessons:

-   Understand the data before modeling
-   Select evaluation metrics based on the problem objective
-   Validate improvements using evidence
-   Consider decision thresholds as part of the modeling process

------------------------------------------------------------------------

# Future Improvements

Possible future improvements:

## Algorithm Comparison

Evaluate additional algorithms:

-   Random Forest
-   Gradient Boosting
-   XGBoost
-   Support Vector Machines

## Feature Engineering

Potential improvements:

-   Creating new meaningful features
-   Feature selection
-   Feature transformation

## Advanced Optimization

Further approaches:

-   More extensive hyperparameter tuning
-   Ensemble modeling
-   Advanced validation strategies

------------------------------------------------------------------------

# Technologies & Libraries

## Programming Language

-   Python

## Libraries

-   Pandas
-   NumPy
-   Matplotlib
-   Seaborn
-   Scikit-learn

------------------------------------------------------------------------

# What I Learned

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
