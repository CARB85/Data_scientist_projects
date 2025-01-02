# Video Game Sales Prediction Project

## Project Description

You are working for the online store *Ice*, which sells video games worldwide. User and expert reviews, game genres, platforms (such as Xbox or PlayStation), and historical sales data are available from open sources. Your task is to identify patterns that determine whether a game is successful or not. This will allow you to detect promising projects and plan advertising campaigns.

You have data going back to 2016. Imagine it's December 2016, and you are planning a campaign for 2017.

The important part of the project is to gain experience working with data. It doesn't really matter whether you are forecasting 2017 sales based on 2016 data or 2027 sales based on 2026 data.

The dataset contains a "rating" column, which stores the ESRB rating of each game. The Entertainment Software Rating Board (ESRB) evaluates the content of a game and assigns an age rating such as Teen or Adult.

## Instructions for Completing the Project

### Step 1: Open the data file and explore the general information

File path:  
`/datasets/games.csv` — Download the dataset.

### Step 2: Prepare the data

- Rename the columns (convert to lowercase).
- Convert the data to the necessary types.
- Describe the columns where data types have been changed and explain why.
- If necessary, decide how to handle missing values:
  - Explain why you filled in the missing values the way you did or why you chose to leave them blank.
  - Why do you think the values are missing? Provide possible explanations.
  - Pay attention to the abbreviation "TBD" (To Be Determined). Specify how you plan to handle these cases.
- Calculate the total sales (sum of sales in all regions) for each game and place these values in a separate column.

### Step 3: Analyze the data

- Look at how many games were released in different years. Are the data from each period significant?
- Observe how sales vary across different platforms. Choose the platforms with the highest total sales and build a distribution based on data from each year. Look for platforms that used to be popular but now have no sales. How long do new platforms generally take to emerge, and how long do old platforms take to disappear?
- Determine for which period you should collect data. To do this, look at your answers to the previous questions. The data should allow you to build a model for 2017.
- Work only with the data that you consider relevant. Ignore data from earlier years.
- Which platforms are leading in sales? Which ones are growing, and which ones are declining? Choose several potentially profitable platforms.
- Create a box plot for global sales of all games, broken down by platform. Are the sales differences significant? What happens with average sales across various platforms? Describe your findings.
- Look at how user and critic reviews affect sales on a popular platform (your choice). Create a scatter plot and calculate the correlation between reviews and sales. Draw conclusions.
- Considering your findings, compare sales of the same games on different platforms.
- Take a look at the general distribution of games by genre. What can be said about the most profitable genres? Can you generalize about genres with high or low sales?

### Step 4: Create a user profile for each region

For each region (NA, EU, JP), determine:

- The top five platforms. Describe the variations in their market share from one region to another.
- The top five genres. Explain the differences.
- Whether ESRB ratings affect sales in individual regions.

### Step 5: Test the following hypotheses:

- The average user ratings for Xbox One and PC platforms are the same.
- The average user ratings for Action and Sports genres are different.

Set the alpha threshold yourself.

Explain:
- How you formulated the null and alternative hypotheses.
- The criteria you used to test the hypotheses and why.

### Step 6: Write a general conclusion

### Format:

Complete the task in Jupyter Notebook. Insert the programming code in code cells and the text explanations in markdown cells. Apply formatting and add headings.

## Data Description

- **Name**: Game name
- **Platform**: Platform (e.g., Xbox, PlayStation)
- **Year_of_Release**: Year of release
- **Genre**: Game genre
- **NA_sales**: Sales in North America (in millions of USD)
- **EU_sales**: Sales in Europe (in millions of USD)
- **JP_sales**: Sales in Japan (in millions of USD)
- **Other_sales**: Sales in other countries (in millions of USD)
- **Critic_Score**: Critic score (maximum of 100)
- **User_Score**: User score (maximum of 10)
- **Rating**: ESRB rating

Note: The 2016 data might be incomplete.
```
