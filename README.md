# Megaline Tariff Analysis Project

## Project Description

You work as an analyst for the telecommunications operator Megaline. The company offers its customers two prepaid plans, **Surf** and **Ultimate**. The commercial department wants to know which plan generates more revenue in order to adjust the advertising budget.

You will conduct a preliminary analysis of the tariffs based on a relatively small sample of customers. You will have data from 500 Megaline customers: who they are, where they live, which tariff they use, as well as the number of calls they made and text messages they sent in 2018. Your task is to analyze customer behavior and determine which prepaid plan generates more revenue. Later, you will find more details in the project instructions regarding the specific customer behavior aspects to analyze. Determining which plan, on average, generates more revenue will be addressed through statistical testing. More information on this will be found in the project instructions section.

## Tariff Description

Note: Megaline rounds seconds to minutes and megabytes to gigabytes. For calls, each individual call is rounded up: even if the call lasted only one second, it will count as one minute. For web traffic, individual web sessions are not rounded. Instead, the total for the month is rounded up. If someone uses 1025 megabytes in a month, they will be charged for 2 gigabytes.

### Surf

- **Monthly payment**: $20.
- **500 minutes per month**, 50 SMS, and 15 GB of data.
- If the plan limits are exceeded:
  - 1 minute: 3 cents.
  - 1 SMS: 3 cents.
  - 1 GB of data: $10.

### Ultimate

- **Monthly payment**: $70.
- **3000 minutes per month**, 1000 SMS, and 30 GB of data.
- If the plan limits are exceeded:
  - 1 minute: 1 cent.
  - 1 SMS: 1 cent.
  - 1 GB of data: $7.

## Data Dictionary

In this project, you will work with five different tables.

### The `users` table (user information):

- `user_id`: Unique user identifier.
- `first_name`: User's first name.
- `last_name`: User's last name.
- `age`: User's age (in years).
- `reg_date`: Subscription date (dd, mm, yy).
- `churn_date`: The date when the user stopped using the service (if absent, the plan was still active when the data was extracted).
- `city`: User's city of residence.
- `plan`: The name of the plan.

### The `calls` table (call data):

- `id`: Unique call identifier.
- `call_date`: Date of the call.
- `duration`: Duration of the call (in minutes).
- `user_id`: The user identifier who made the call.

### The `messages` table (SMS data):

- `id`: Unique SMS identifier.
- `message_date`: Date of the SMS.
- `user_id`: The user identifier who sent the SMS.

### The `internet` table (web session data):

- `id`: Unique session identifier.
- `mb_used`: Amount of data consumed during the session (in megabytes).
- `session_date`: Date of the web session.
- `user_id`: User identifier.

### The `plans` table (plan information):

- `plan_name`: Name of the plan.
- `usd_monthly_fee`: Monthly payment in US dollars.
- `minutes_included`: Minutes included per month.
- `messages_included`: SMS included per month.
- `mb_per_month_included`: Data included per month (in megabytes).
- `usd_per_minute`: Price per minute after exceeding the plan limits (e.g., if the plan includes 100 minutes, the operator will charge for minute 101 onward).
- `usd_per_message`: Price per SMS after exceeding the plan limits.
- `usd_per_gb`: Price per gigabyte for additional data after exceeding the plan limits (1 GB = 1024 megabytes).
