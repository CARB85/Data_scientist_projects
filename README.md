# Sweet Lift Taxi - Taxi Order Prediction

## Project Description

Sweet Lift Taxi has collected historical data on taxi orders at airports. To attract more drivers during peak hours, we need to predict the number of taxi orders for the upcoming hour. Your task is to build a model to make this prediction.

The RECM (Root Mean Square Error) on the test set should not exceed 48.

## Data Description

The data is stored in the file `/datasets/taxi.csv`. 

The number of orders is in the column `num_orders`.

### Dataset Overview

The dataset provided by Sweet Lift Taxi contains historical information about taxi orders. The main features are:

- `datetime`: Date and time of the taxi order record.
- `num_orders`: The number of taxi orders in a specific hour.

## Prediction Objective

The goal is to predict the number of taxi orders per hour by adjusting the time intervals to full hours, using the features provided in the dataset.
