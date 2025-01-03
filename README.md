# Customer Churn Prediction for Interconnect

## Project Overview
This project aims to build a machine learning model for Interconnect, a telecommunications company, to predict customer churn. The goal is to identify customers likely to cancel their services and offer them incentives, such as promotions, to retain them. Multiple classification models, including logistic regression and random forests, will be used, with AUC-ROC as the primary evaluation metric. The target is to achieve an AUC-ROC between 0.85 and 0.88.

## Objectives
- **Build a predictive model** to identify customers likely to churn.
- **Evaluate model performance** using AUC-ROC.
- **Compare multiple models** to find the best performing one.

## Dataset
The dataset consists of the following files:
- **contract.csv**: Information about customer contracts (type, start/end dates).
- **personal.csv**: Customer personal details (ID, gender, age, marital status).
- **internet.csv**: Internet service details (connection type, speed).
- **phone.csv**: Phone service details (landline status).

The target variable is **EndDate**, which indicates if a customer has canceled their service (value 'No').

## Evaluation Metrics
- **Primary Metric**: AUC-ROC (0.85 ≤ AUC-ROC ≥ 0.88).
- **Secondary Metric**: Accuracy.
