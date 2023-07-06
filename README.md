# Customer-Segmentation-Game-Mobile
User Segmentation in the Legends Mobile Game:  A Case Study of Shanghai Moonton Technology.
# Content:
## Data processing
### 1.1 Cleaning data
* No missing values
### 1.2 Merge data
* Information of dataset after merging: we have size of data is 799586 observations, 17 columns, and do not have any missing values

## Data mining
### 2.1 Descriptive statistic
### 2.2 EDA
* Correlation matrix
* Tableau for visualization:

## Pre-processing data for Segmentation
### 3.1 RFM (Recency/Frequency/Monetary
* The informative features in this dataset that tell us about customer buying behavior include “Online Date”, “Paid Frequency”, and “Paid Amount”. Using these variables, we are going to derive a customer’s RFM profile - Recency, Frequency, and Monetary Value.
RFM is commonly used in marketing to evaluate a client’s value based on their:
* Recency: How recently have they been online?
* Frequency: How often have they paid for the game?
* Monetary Value: How much money do they spend on the game?
* Then, we will calculate each customer’s recency, frequency, and monetary value. These RFM values will then be used to build the segmentation model.
* So here, we calculate recency, frequency, and monetary value:
* Firstly, Let’s start by calculating recency. To identify a customer’s recency,....
Recency = (max_day + 1) - date_online
* Secondly, let’s calculate frequency — how many times has each customer paid for the game:
Frequency = sum of paid_frequency follow group account_id
* Finally, we can calculate each user’s monetary value to understand the total amount they have spent on the game:
Monetary = sum of paid_amount follow group account_id
### 3.2 Outliers
* In this project, we will RFM data to build model segmentation.
* Before building the customer segmentation model, we first need to check the RFM data frame for outliers and remove them.
* To get a visual representation of outliers in the dataframe, we will create a boxplot of each variable.

## Model Clustering
### 4.1 KMean
### 4.2 Fuzzy c mean
### 4.3 Gaussian Mixture
### 4.4 OPTICS
### 4.5 Model evaluation
