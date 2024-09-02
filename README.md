# Phase_3_project
morigaschool phase 3 project

---

## Overview
This project aims to build a binary classification model using logistic regression to predict a target outcome based on financial data from various global organizations. The goal is to leverage gradient descent for model training and evaluate the model's performance using ROC and AUC curves.

## Business and Data Understanding

### Stakeholder Audience
The primary stakeholders for this project include:
- **Financial Analysts**: Interested in understanding the financial health and performance of organizations based on key metrics like revenue, profits, assets, and market value.
- **Investors**: Seeking insights into which companies are likely to be profitable and stable, aiding investment decisions.
- **Corporate Executives**: Focused on benchmarking their organizations against industry leaders to identify areas for improvement.

### Dataset Choice
The dataset used in this project includes financial data from a variety of global organizations across multiple industries. The data contains the following features:
- **Revenue (Billions)**: Annual revenue of the organization.
- **Profits (Billions)**: Annual profit of the organization.
- **Assets (Billions)**: Total assets owned by the organization.
- **Market Value (Billions)**: The market value of the organization.

Additionally, a binary target variable is created to classify organizations based on their revenue, where organizations with revenue greater than a specific threshold are classified as `1` (high revenue) and others as `0` (low revenue).

## Modeling
The project employs a logistic regression model to classify the organizations. The steps involved include:

1. **Data Preprocessing**: Standardizing the features and splitting the data into training and test sets.
2. **Model Initialization**: Setting up initial weights and biases.
3. **Gradient Descent Implementation**: Using gradient descent to optimize the logistic regression model.
4. **Training**: Running the gradient descent algorithm for a specified number of iterations.
5. **Prediction**: Using the trained model to predict outcomes on the test dataset.

## Logistic Regression and Classification Metrics
Logistic regression is a powerful method for binary classification. In this project, we utilized the following metrics to evaluate the performance of the logistic regression model:

- **Accuracy**: The ratio of correctly predicted observations to the total observations. It measures the overall effectiveness of the model in making accurate predictions.
  
- **Precision**: The ratio of true positive predictions to the total positive predictions made by the model. It indicates how many of the predicted positives are actually positive.
  
- **Recall (Sensitivity)**: The ratio of true positive predictions to all actual positives in the dataset. It measures the model's ability to correctly identify positive cases.
  
- **F1 Score**: The harmonic mean of precision and recall, providing a balance between the two metrics. It is especially useful when the class distribution is imbalanced.
  
- **ROC (Receiver Operating Characteristic) Curve**: A graphical representation of the model’s performance across different thresholds. It plots the true positive rate (sensitivity) against the false positive rate (1-specificity).
  
- **AUC (Area Under the Curve)**: A scalar value summarizing the ROC curve. A higher AUC value indicates better model performance, with 1 being the perfect model and 0.5 representing a model that performs no better than random guessing.

The ROC curve was plotted and saved as a PNG file, allowing stakeholders to visualize the trade-off between true positives and false positives at various thresholds.

## Conclusion
This project demonstrates the effectiveness of logistic regression, optimized via gradient descent, in classifying organizations based on financial metrics. The ROC and AUC analysis, along with other classification metrics, provide a comprehensive evaluation of model performance, highlighting its potential applications for financial analysts, investors, and corporate executives. Future improvements could include expanding the dataset, exploring additional features, or applying more complex models to enhance prediction accuracy.

---
