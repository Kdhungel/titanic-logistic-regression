# Titanic Survival Prediction (Logistic Regression)

This project is a beginner-friendly machine learning baseline that predicts whether a passenger survived the Titanic disaster.

The goal of the project is not high accuracy, but **clear understanding of the full ML pipeline**.

## Dataset

- Titanic dataset (CSV format)
- Target variable: `Survived` (0 = did not survive, 1 = survived)

## Features Used

- `Pclass` — passenger ticket class
- `Sex` — encoded as 0 (male) and 1 (female)
- `Age` — passenger age

Only a small number of interpretable features were used to keep the model explainable.

## Model

- Logistic Regression (scikit-learn)

## Workflow

1. Load CSV data using pandas
2. Select relevant features and target
3. Handle missing values by removing incomplete rows
4. Encode categorical variables
5. Split data into training and testing sets
6. Train logistic regression model
7. Evaluate model accuracy on unseen test data

## Result

- Test accuracy: ~75%

This result is reasonable for a simple baseline model without feature engineering or hyperparameter tuning.

## Purpose

This project was built as a **learning-focused baseline**, with emphasis on:

- correctness
- clarity
- explainability

Every step can be explained line by line.

## Model Interpretation

After training the model, the learned coefficients were inspected to understand how each feature influences survival probability.

- A positive coefficient indicates that increasing the feature increases survival probability.
- A negative coefficient indicates that increasing the feature decreases survival probability.

In this model:

- Sex has the strongest positive influence on survival.
- Passenger class has a negative influence (lower class → lower survival probability).
- Age has a small negative influence on survival.
