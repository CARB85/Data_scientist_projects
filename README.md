# Rusty Bargain Project

## Project Description

Rusty Bargain is a second-hand car selling service that is developing an app to attract new customers. Through this app, users can quickly determine the market value of their car. The app provides access to the car's history, technical specifications, equipment versions, and prices. The objective is to create a model that predicts the market value of the cars.

Rusty Bargain is interested in:

- Prediction quality
- Prediction speed
- Time required for training

## Project Instructions

1. **Download and examine the data.**
2. **Train different models with various hyperparameters.** (At least two models are required, but more is better. Remember, multiple gradient boosting implementations do not count as different models.) The main point of this step is to compare gradient boosting methods with random forest, decision tree, and linear regression.
3. **Analyze the speed and quality of the models.**

### Observations:
- Use the **RMSE** (Root Mean Squared Error) metric to evaluate the models.
- Linear regression may not perform well for hyperparameter tuning but is perfect for sanity checking other methods. If gradient boosting performs worse than linear regression, something has gone wrong.
- Learn on your own about the LightGBM library and its tools for creating gradient boosting models.
- Ideally, your project should include:
  - Linear regression for sanity checking.
  - A tree-based algorithm with hyperparameter tuning (preferably random forest).
  - LightGBM with hyperparameter tuning (try a couple of setups).
  - CatBoost and XGBoost with hyperparameter tuning (optional).
- Take note of categorical feature encoding for simple algorithms. LightGBM and CatBoost have their own implementations, but XGBoost requires One-Hot Encoding (OHE).
- You can use a special command to find the execution time of a cell in Jupyter Notebook. Look for that command.
- Since training a gradient boosting model can be time-consuming, try changing only a few parameters of the model.
- If Jupyter Notebook stops working, delete excessive variables using the `del` operator:

  ```python
  del features_train
