# OilyGiant Oil Extraction Project

## Project Description

You are working for OilyGiant, an oil extraction company. Your task is to identify the best locations to open 200 new oil wells.

To complete this task, you will need to follow these steps:

1. **Read Data Files**: Load the data with the parameters collected from oil wells in the selected region: crude oil quality and reserve volume.
2. **Model Development**: Create a model to predict the reserve volume in new oil wells.
3. **Select Top Wells**: Choose the oil wells that have the highest estimated values.
4. **Region Selection**: Choose the region with the highest total benefit from the selected oil wells.
5. **Benefit and Risk Analysis**: You have data from crude samples from three regions. Known parameters for each well in the region are available. Create a model to help select the region with the greatest profit margin. Analyze potential benefits and risks using the bootstrapping technique.

### Conditions:
- Only linear regression should be used to train the model.
- A study is conducted with 500 points, and the best 200 points are selected for benefit calculation.
- The budget for developing 200 oil wells is 100 million dollars.
- A barrel of raw materials generates 4.5 USD in revenue. The income from one unit of product is 4500 USD (reserve volume is expressed in thousands of barrels).
- After risk evaluation, only regions with a risk of loss lower than 2.5% should be kept. From those, select the region with the highest average profit.
- The data is synthetic: contract details and well features are not published.

## Data Description

The geological exploration data for the three regions are stored in the following files:

- **geo_data_0.csv**
- **geo_data_1.csv** 
- **geo_data_2.csv** 

### Columns in the Data:
- `id`: Unique identifier of the oil well.
- `f0, f1, f2`: Three features of the points (their specific meaning is not important, but the features themselves are meaningful).
- `product`: Reserve volume in the oil well (thousands of barrels).
