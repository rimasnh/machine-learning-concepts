# Hospital Readmission Prediction using Machine Learning

## Project Overview
Hospital readmissions are a major challenge for healthcare systems, increasing costs and indicating potential gaps in patient care. This project develops machine learning models to predict whether a patient will be **readmitted within 30 days** after discharge.

Accurate prediction of high-risk patients allows healthcare providers to implement preventive strategies, improve patient outcomes, and reduce hospital costs.

This project implements a complete machine learning workflow including **data exploration, preprocessing, model training, evaluation, and fairness analysis**.

---

## Problem Statement
Hospital readmissions are expensive and often preventable. Identifying patients at high risk of readmission can help hospitals:

- Improve patient monitoring
- Reduce healthcare costs
- Provide targeted interventions
- Improve overall patient outcomes

The objective of this project is to **build predictive models that classify whether a patient will be readmitted**.

---

## Dataset Description

The dataset contains patient information including demographic details, clinical data, and healthcare utilization metrics.

### Target Variable
| Variable | Description |
|--------|-------------|
| readmitted | 1 = patient readmitted within 30 days, 0 = not readmitted |

### Demographic Features
- race
- sex
- age

### Clinical Features
- admission_source
- blood_glucose
- insurer

### Healthcare Utilization Features
- duration
- n_previous_visits
- n_diagnoses
- n_procedures
- n_medications

---

## Machine Learning Workflow

The project follows a structured machine learning pipeline:

1. Import Required Libraries  
2. Data Loading  
3. Exploratory Data Analysis (EDA)  
4. Data Preprocessing  
5. Model Training  
6. Model Evaluation  
7. Model Comparison  
8. Fairness Metrics Analysis  
9. Model Deployment Testing

---

## Exploratory Data Analysis (EDA)

EDA was performed to understand the dataset characteristics including:

- Distribution of the target variable
- Feature relationships
- Missing values
- Data imbalance

Visualization and summary statistics were used to better understand the dataset before training the models.

---

## Data Preprocessing

Data preprocessing steps included:

- Handling missing values
- Encoding categorical variables
- Feature selection
- Data transformation
- Preparing the dataset for machine learning algorithms

Proper preprocessing ensures that models receive clean and structured input data.

---

## Machine Learning Models

### Logistic Regression

Logistic Regression is a linear classification algorithm used for binary outcomes.

Advantages:
- Simple and interpretable
- Works well for linearly separable data
- Provides probability estimates

Use Case in Project:
Predict whether a patient will be readmitted based on clinical and demographic features.

---

### Random Forest

Random Forest is an ensemble learning method that combines multiple decision trees.

Advantages:
- Handles nonlinear relationships
- Reduces overfitting compared to single decision trees
- Provides feature importance scores

Random Forest helps capture complex relationships between patient characteristics and readmission risk.

---

## Model Evaluation

Model performance was evaluated using standard classification metrics such as:

- Accuracy
- Precision
- Recall
- F1 Score

These metrics help determine how well the models predict patient readmissions.

---

## Model Comparison

Both models were compared to determine which performs better in predicting hospital readmissions.

Key aspects evaluated:

- Prediction accuracy
- Model generalization
- Interpretability
- Robustness

---

## Fairness Metrics Analysis

Fairness analysis was included to evaluate whether model predictions are unbiased across demographic groups.

Fairness metrics help identify potential bias related to:

- Race
- Gender
- Age

Ensuring fairness is critical in healthcare machine learning applications.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-Learn
- Matplotlib
- Seaborn
- Jupyter Notebook
---

## Key Insights

- Machine learning can help identify patients at risk of hospital readmission.
- Healthcare utilization variables often play a significant role in prediction.
- Ensemble models such as Random Forest can capture complex patterns in healthcare data.
- Fairness analysis is important when deploying models in sensitive domains such as healthcare.

---

## Future Improvements

Potential improvements to this project include:

- Testing additional models such as Gradient Boosting or XGBoost
- Use the computed feature importance list to train a linear model (e.g. logistic regression) as a means of feature selection.
