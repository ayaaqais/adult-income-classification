# Adult Income Classification Project

## Project Overview

This project uses the Adult Income dataset to build a classification model that predicts whether a person's income is `<=50K` or `>50K`.

The goal is to explore the dataset, build a machine learning model, evaluate its performance, and identify the most important features using permutation importance.

## Dataset

Each row represents one person.

The target variable is:

- `income`

Target classes:

- `<=50K`
- `>50K`

## Main Questions

This project answers:

- What factors are most related to income level?
- Can we predict whether someone earns more than 50K?
- Which features are most important for the model?
- Do the important features make sense from a stakeholder perspective?

## Methods Used

The project includes:

1. Data cleaning
2. Handling missing values marked as `?`
3. Exploratory Data Analysis
4. Preprocessing pipelines
5. Random Forest classification model
6. Model evaluation
7. Permutation importance
8. Explanatory visualizations

## Preprocessing

The preprocessing pipeline includes:

### Numeric Features

- Median imputation
- Standard scaling

### Categorical Features

- Most frequent value imputation
- One-hot encoding

Using a pipeline helps avoid data leakage.

## Model

The model used is:

- RandomForestClassifier

Random Forest was selected because it works well with tabular data and can capture non-linear relationships.

## Evaluation Metrics

The model is evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion matrix

## Key Findings

The most important features are expected to include factors such as:

- Education
- Occupation
- Age
- Hours per week
- Capital gain
- Marital status

The final notebook includes permutation importance to identify the actual top 10 features.

## Explanatory Visualizations

The notebook includes reporting-quality visualizations for important features such as:

- Percentage earning `>50K` by education level
- Percentage earning `>50K` by occupation

These visuals are designed to be understandable for a non-technical audience.

## Files in This Repository

- `adult_income_classification_project.ipynb`
- `adult.csv`
- `README.md`

## Conclusion

This project shows that income classification can be predicted using demographic and work-related features.  
It also demonstrates how feature importance can help explain model predictions to stakeholders.
