# Loan Default / Credit Risk Prediction — Logistic Regression

## Project Overview

This project develops a Machine Learning model to predict whether a loan applicant is likely to default. The model uses **Logistic Regression**, an interpretable binary-classification approach for credit-risk scoring.

The notebook demonstrates an end-to-end workflow: synthetic data generation, exploratory analysis, preprocessing, model training, evaluation, feature-impact analysis, and prediction for a new applicant.

> **Data note:** The dataset is synthetic (artificially generated) and designed to resemble real credit-risk data without using private customer information.

## Business Problem

Lenders need to assess the risk that an applicant may default on a loan. A predictive model can provide a default-probability score that can support loan approval, pricing, and risk-management workflows.

## Features Used

- **Age** — applicant age
- **Annual income** — annual income in ₹ thousands
- **Credit score** — credit bureau score on a 300–900 scale
- **Loan amount** — requested amount in ₹ thousands
- **Loan term** — repayment period in months
- **Employment length** — years in the current job
- **Debt-to-income ratio** — existing debt relative to income
- **Previous defaults** — number of past missed/defaulted payments

**Target:** `default` — `1` indicates default and `0` indicates normal repayment.

## Machine Learning Workflow

1. Generate a synthetic credit-risk dataset
2. Perform exploratory analysis
3. Split data into training and testing sets
4. Standardize features
5. Train a Logistic Regression model
6. Evaluate using accuracy, confusion matrix, classification report, and ROC-AUC
7. Analyze model coefficients
8. Predict default risk for a new applicant
9. Test predictions through an interactive slider-based demo

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook / Google Colab
- IPyWidgets

## Model Details

**Algorithm:** Logistic Regression  
**Problem Type:** Binary Classification  
**Dataset Size:** 2,000 synthetic applicants  
**Train/Test Split:** 75% / 25% with stratification  
**Preprocessing:** StandardScaler

## Evaluation

The notebook evaluates the model using:

- Accuracy
- ROC-AUC
- Confusion Matrix
- Classification Report
- ROC Curve

The model coefficients are also visualized to show the direction and relative effect of features on predicted default risk.

## Interactive Demo

The notebook includes an interactive applicant-risk demo using sliders for income, credit score, loan amount, debt-to-income ratio, employment length, and previous defaults. The model updates the predicted class and estimated probability of default.

## Responsible AI Considerations

A real-world credit-risk system should include bias testing across relevant groups, transparency around model decisions, human review for borderline or high-value cases, and regular monitoring and retraining as the market changes.

The model should support responsible lending decisions rather than automatically replace appropriate human oversight.

## Learning Outcomes

This project demonstrates practical experience with:

- Credit-risk modelling
- Data preprocessing
- Exploratory data analysis
- Logistic Regression
- Model evaluation
- Feature interpretation
- Probability-based prediction
- Interactive Machine Learning demonstrations
- Responsible AI considerations in financial applications

## Author

**Aditya Thakur**  
BBA Fintech and AI
