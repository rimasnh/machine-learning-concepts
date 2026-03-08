Bias–Variance Tradeoff in Machine Learning
Overview

The Bias–Variance Tradeoff is one of the most important concepts in machine learning. It explains the balance between a model’s ability to learn patterns from training data and its ability to generalize to unseen data.

In this project, we explore:

Bias

Variance

Underfitting

Overfitting

How model complexity affects prediction performance

Understanding this concept helps in building models that generalize well instead of memorizing training data.

What is Bias?

Bias refers to the error caused by overly simplistic assumptions in the learning algorithm.

High bias models:

Are too simple

Fail to capture underlying patterns

Lead to underfitting

Example models with high bias:

Linear regression on nonlinear data

Very shallow decision trees

Characteristics of high bias:

Poor performance on training data

Poor performance on test data

Model too simple to learn patterns

What is Variance?

Variance refers to how sensitive a model is to changes in the training data.

High variance models:

Learn noise from training data

Perform well on training data

Perform poorly on unseen data

This leads to overfitting.

Examples of high variance models:

Very deep decision trees

High-degree polynomial regression

Complex neural networks

Mathematical Representation

The prediction error of a machine learning model can be decomposed into three parts:

Bias²

Variance

Irreducible Error

Error = Bias^2 + Variance + Irreducible Error

Goal of machine learning is to minimize total error by balancing bias and variance.

Underfitting vs Overfitting
Model Behavior	Cause	Result
Underfitting	High Bias	Model too simple
Overfitting	High Variance	Model memorizes data
Good Fit	Balanced Bias & Variance	Best generalization
Bias–Variance Tradeoff

Increasing model complexity usually:

Decreases bias

Increases variance

This creates a tradeoff where we must find the optimal model complexity.

Typical behavior:

Model Complexity	Bias	Variance
Simple model	High	Low
Medium complexity	Balanced	Balanced
Complex model	Low	High

The best model lies in the middle of this curve.

Example Models
High Bias Model

Linear regression on complex data

Underfits the dataset

Balanced Model

Polynomial regression with appropriate degree

Captures patterns without overfitting

High Variance Model

Deep neural network

Memorizes training data

Techniques to Reduce Bias

Methods to reduce bias include:

Using more complex models

Adding more features

Using ensemble methods

Increasing training time

Techniques to Reduce Variance

Methods to reduce variance include:

Increasing training data

Regularization (L1 / L2)

Cross validation

Pruning decision trees

Dropout in neural networks

Practical Example

In this notebook we demonstrate:

Training a regression model

Observing underfitting

Increasing model complexity

Observing overfitting

Finding a balanced model

Technologies Used

Python

NumPy

Scikit-Learn

Matplotlib

Jupyter Notebook

Repository Structure
machine-learning
│
└── 01_bias_variance
    │
    ├── bias_variance_demo.ipynb
    └── README.md
Key Takeaways

Bias represents model simplicity

Variance represents model sensitivity to data

Increasing complexity reduces bias but increases variance

The goal is to find a balance that minimizes prediction error

Understanding the bias–variance tradeoff is essential for building robust machine learning models that generalize well to new data.
