# Megaline Customer Plan Recommendation Model

## Project Description

Megaline, a mobile company, is dissatisfied with the number of customers still using legacy plans. They want to develop a model that can analyze customer behavior and recommend one of Megaline's new plans: Smart or Ultra.

You have access to data on the behavior of subscribers who have already switched to the new plans (from the Statistical Data Analysis sprint project). For this classification task, you should create a model that chooses the correct plan. Since the data preprocessing step has already been completed, you can jump straight into building the model.

The goal is to develop a model with the highest possible accuracy. The accuracy threshold for this project is 0.75. Use the provided dataset to evaluate the model's accuracy.

## Data Description

Each observation in the dataset contains monthly behavioral information about a user. The given information is as follows:

- **calls** — number of calls
- **minutes** — total call duration in minutes
- **messages** — number of text messages
- **mb_used** — internet traffic used in MB
- **is_ultra** — plan for the current month (Ultra - 1, Smart - 0)

