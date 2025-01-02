# Zuber Rideshare Data Analysis Project

## Project Description

You are working as an analyst for Zuber, a new rideshare company launching in Chicago. Your task is to find patterns in the available data. You want to understand passenger preferences and the impact of external factors on trips.

While working with the database, you will analyze competitor data and test a hypothesis about the impact of weather on trip frequency.

## Data Description

The database contains information about taxi rides in Chicago:

### Table: neighborhoods
Data about the city's neighborhoods.

- `name`: Name of the neighborhood
- `neighborhood_id`: Neighborhood ID code

### Table: cabs
Data about the taxis.

- `cab_id`: Vehicle code
- `vehicle_id`: Vehicle technical ID
- `company_name`: The company that owns the vehicle

### Table: trips
Data about the trips.

- `trip_id`: Trip code
- `cab_id`: Vehicle code operating the trip
- `start_ts`: Start time of the trip (rounded to the hour)
- `end_ts`: End time of the trip (rounded to the hour)
- `duration_seconds`: Duration of the trip in seconds
- `distance_miles`: Distance of the trip in miles
- `pickup_location_id`: ID code of the pickup neighborhood
- `dropoff_location_id`: ID code of the dropoff neighborhood

### Table: weather_records
Data about the weather.

- `record_id`: Weather record ID
- `ts`: Timestamp of the record (rounded to the hour)
- `temperature`: Temperature when the record was taken
- `description`: A brief description of the weather conditions, e.g., "light rain" or "scattered clouds"

### Table Schema
![Database Schema](image_url)

Note: There is no direct connection between the `trips` and `weather_records` tables in the database. However, you can use JOIN and link them using the trip start time (`trips.start_ts`) and the weather record timestamp (`weather_records.ts`).

## Instructions to Complete the Project

### Step 1: Analyze Weather Data

Write code to analyze the weather data from Chicago in November 2017 from the following website:

[Chicago Weather November 2017](https://practicum-content.s3.us-west-1.amazonaws.com/data-analyst-eng/moved_chicago_weather_2017.html)

### Step 2: Exploratory Data Analysis

### Step 3: Hypothesis Testing

Test the hypothesis that the duration of trips from the Loop to O'Hare International Airport changes on rainy Saturdays.

### Step 4: Exploratory Data Analysis (Python)

In addition to the data you retrieved in the previous tasks, you now have two CSV files. The files are:

- `project_sql_result_01.csv`: Contains the following data:
  - `company_name`: Name of the taxi company
  - `trips_amount`: Number of trips for each taxi company from November 15 to 16, 2017.

- `project_sql_result_04.csv`: Contains the following data:
  - `dropoff_location_name`: Chicago neighborhoods where the trips ended
  - `average_trips`: Average number of trips that ended in each neighborhood in November 2017.

### Step 5: Hypothesis Testing (Python)

`project_sql_result_07.csv`: The result of the last query. Contains data about trips from the Loop to O'Hare International Airport. The fields in the table are:

- `start_ts`: Pickup date and time
- `weather_conditions`: Weather conditions when the trip started
- `duration_seconds`: Duration of the trip in seconds

Test the hypothesis:
"The average duration of trips from the Loop to O'Hare International Airport changes on rainy Saturdays."

Set the significance level (alpha) by yourself.

Explain:

- How you formulated the null and alternative hypotheses.
- What criteria you used to test the hypotheses and why.

