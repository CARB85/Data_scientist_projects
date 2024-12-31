# Project: Instacart Data Analysis

## Project Description

This project utilizes data provided by the grocery delivery platform Instacart, which allows users to place orders for home delivery. The dataset has been modified to simplify analysis by reducing its size and introducing common issues such as missing values and duplicates. Your task is to clean the data and perform exploratory analysis to understand the shopping habits of Instacart customers.

The analysis should include clear, well-labeled visualizations to explain the results. All answers must be accompanied by a brief markdown explanation.

## Data Dictionary

### `instacart_orders.csv`
- **order_id**: Unique ID for each order.
- **user_id**: Unique ID for each customer.
- **order_number**: Number of orders placed by the customer.
- **order_dow**: Day of the week the order was placed (0: Sunday).
- **order_hour_of_day**: Hour of the day the order was placed.
- **days_since_prior_order**: Days since the customer's previous order.

### `products.csv`
- **product_id**: Unique ID for each product.
- **product_name**: Name of the product.
- **aisle_id**: ID of the grocery aisle.
- **department_id**: ID of the grocery department.

### `order_products.csv`
- **order_id**: Unique ID for each order.
- **product_id**: Unique ID for each product.
- **add_to_cart_order**: Sequential order in which the product was added to the cart.
- **reordered**: Indicates if the product was ordered previously (1: Yes, 0: No).

### `aisles.csv`
- **aisle_id**: Unique ID for the aisle.
- **aisle**: Name of the aisle.

### `departments.csv`
- **department_id**: Unique ID for the department.
- **department**: Name of the department.

## Instructions for Completing the Project

### Step 1: Initial Exploration
1. Load the datasets (`instacart_orders.csv`, `products.csv`, `aisles.csv`, `departments.csv`, `order_products.csv`).
2. Review the content of each table and adjust arguments as needed to read the files correctly.

### Step 2: Data Preprocessing
- **Validation and Corrections**: Adjust incorrect data types.
- **Handling Missing Values**: Identify, analyze, and impute missing values.
- **Removing Duplicates**: Identify and remove duplicate rows, explaining the methods used.

### Step 3: Data Analysis
#### [A] Validation and Initial Visualizations
1. Validate `order_hour_of_day` and `order_dow` column values.
2. Create visualizations for:
   - Orders by hour of the day.
   - Orders by day of the week.
   - Time between consecutive orders.

#### [B] Comparisons and Frequencies
1. Compare the distribution of `order_hour_of_day` for Wednesdays and Saturdays.
2. Plot the distribution of the number of orders per customer.
3. Identify the 20 most frequently ordered products.

#### [C] Order and Product Analysis
1. Analyze the average number of items per order.
2. Identify the 20 most reordered products.
3. Calculate the reorder ratio for each product and customer.
4. Identify the 20 most frequently first-added products to the cart.

### Visualization Requirements
All visualizations must include:
- Clear titles.
- Labeled axes.
- Legends if needed.
- Use of `plt.show()` at the end of each visualization cell.
