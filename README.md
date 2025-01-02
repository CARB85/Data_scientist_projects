# Beta Bank Customer Churn Prediction

## Project Description

Beta Bank is experiencing gradual customer churn every month. Bankers have discovered that it is cheaper to retain existing customers than to acquire new ones.

The goal of this project is to predict whether a customer will leave the bank soon based on historical customer behavior and contract termination data.

You need to build a model with the highest possible F1 score. To pass the review, you need to achieve an F1 score of at least 0.59. Verify the F1 score on the test set.

Additionally, you should measure the AUC-ROC metric and compare it to the F1 score.

## Data Description

The dataset is available in the file `/datasets/Churn.csv`. Download the dataset and examine its contents.

### Features:

- **RowNumber:** Data index
- **CustomerId:** Unique customer identifier
- **Surname:** Customer's surname
- **CreditScore:** Credit score of the customer
- **Geography:** Country of residence
- **Gender:** Gender of the customer
- **Age:** Age of the customer
- **Tenure:** Number of years the customer has had a fixed deposit with the bank
- **Balance:** Account balance of the customer
- **NumOfProducts:** Number of banking products used by the customer
- **HasCrCard:** Whether the customer has a credit card (1 = Yes; 0 = No)
- **IsActiveMember:** Whether the customer is active (1 = Yes; 0 = No)
- **EstimatedSalary:** Estimated salary of the customer

### Target:
- **Exited:** Whether the customer has exited (1 = Yes; 0 = No)
