# Sure Tomorrow Insurance Project

The insurance company **Sure Tomorrow** wants to solve several tasks using machine learning, and they have asked you to evaluate the possibility of achieving this. Below are the details of the tasks and project instructions:

## Tasks

### Task 1: Find Similar Clients
You need to find clients that are similar to a given client. This will help the company's agents in their marketing efforts.

### Task 2: Predict Insurance Benefits Probability
Predict whether a new client is likely to receive an insurance benefit. Can a trained prediction model outperform an untrained dummy model? Can it perform worse? Please explain your answer.

### Task 3: Predict the Amount of Insurance Benefits
Predict the amount of insurance benefits a new client will likely receive using a linear regression model.

### Task 4: Protect Client Data
Protect the personal data of clients without affecting the model developed in Task 3. You are required to develop a data transformation algorithm that makes it difficult to recover personal information if the data falls into the wrong hands. This is known as **data masking** or **data obfuscation**. However, the data must be protected in such a way that the quality of the machine learning models is not compromised. You do not need to select the best model; it is sufficient to demonstrate that the algorithm works correctly.

## Data Description

The dataset is stored in the file `/datasets/insurance_us.csv`

### Features
- Sex
- Age
- Salary
- Number of family members insured

### Target
- Number of insurance benefits received by the insured person in the last five years.
