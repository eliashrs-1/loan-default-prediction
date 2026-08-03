# Loan Default Prediction Using Machine Learning

## Project Report

View the full interactive report here:
https://eliashrs-1.github.io/loan-default-prediction/loan_default_prediction.html

## Overview

This project develops a machine learning pipeline to predict loan defaults using the LendingClub loan dataset containing 9,578 borrower records. The goal was to build models that identify borrowers at higher risk of default while balancing the tradeoff between identifying defaults and minimizing false positives.

This project applies statistical modeling, machine learning, and ensemble techniques to explore how predictive models can support credit risk assessment and lending decisions.

## Objectives

- Predict whether a borrower will fail to fully repay a loan
- Compare multiple machine learning approaches for credit risk classification
- Address challenges caused by class imbalance in financial datasets
- Evaluate models using accuracy, precision, recall, and F1 score

## Methods

The project includes:

### Data Preparation
- Data cleaning and validation
- Exploratory data analysis
- Outlier analysis
- Feature scaling
- Categorical variable encoding
- Train/validation/test splitting

### Exploratory Analysis
- Summary statistics
- Correlation analysis
- Multicollinearity testing using VIF
- PCA dimensionality analysis
- K-means clustering to identify borrower profiles

### Predictive Models

Single models:
- Logistic Regression
- Decision Tree
- k-Nearest Neighbors (kNN)
- Gradient Boosting Machine (GBM)

Ensemble models:
- Random Forest
- Bootstrap Logistic Regression ensembles
- Bootstrap kNN ensembles
- Heterogeneous probability blending ensembles

### Model Improvements
- SMOTE oversampling for class imbalance
- Hyperparameter tuning
- Probability threshold optimization
- Ensemble weighting based on validation performance

## Results

The project compared 11 different modeling approaches.

The strongest individual model was Logistic Regression, which achieved:

- Accuracy: 58.3%
- Precision: 22.7%
- Recall: 69.2%
- F1 Score: 0.342

The best-performing heterogeneous ensemble achieved:

- Accuracy: 84.7%
- Precision: 61.5%
- Recall: 5.4%
- F1 Score: 0.099

While accuracy-based models performed well overall, Logistic Regression-based approaches provided the strongest balance between detecting defaults and maintaining predictive reliability.

## Business Application

Accurately identifying borrowers likely to default is an important challenge in lending and financial risk management. This project demonstrates how machine learning models can support credit evaluation by identifying risk patterns, comparing modeling strategies, and evaluating the tradeoffs between missed defaults and false alarms.

## Tools & Technologies

- R
- R Markdown
- caret
- randomForest
- gbm
- tidyverse
- Data visualization
- Statistical modeling
- Machine learning

## Files

- `loan_default_prediction.Rmd` — Complete analysis, code, and methodology
- `loan_default_prediction.html` — Rendered report containing results and visualizations

## Dataset

The project uses the LendingClub loan dataset containing borrower financial information and loan repayment outcomes.

Dataset source:
LendingClub publicly available loan data via Kaggle.
