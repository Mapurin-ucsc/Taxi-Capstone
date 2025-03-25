## Data Set Information

This dataset is taken from Kaggle and includes data taken from the NYC Taxi and Limo Commission (TLC). This data includes key information about the date and time a particular ride took place, the number of passengers and the duration of the trip which would be vital to our business goals.

## Problem Statement 

The taxi business is an extremely lucrative one, depending on where it is based, taxis end up being one of the most important modes of transportation. It is especially important for firms in the business to optimize the location at which they have the most availability to ensure they retain the largest number of customers. To this end, understanding taxi demand patterns is crucial for optimizing the allocation of resources. This project uses predictive modeling techniques that consider factors such as time, precise location to determine the ideal conditions to maximize operational availability, and by extension, revenue.
## Model Outcomes or Predictions
This project uses a regression model to predict taxi demand, the model measures number of rides at any given time or location and uses supervised learning to analyze historical trip records and devise potential future demand patterns.
## Data Acquisition
The dataset used for this project is the NYC Yellow Taxi Trip Dataset from Kaggle. The data includes timestamps, pickup and drop off coordinates, trip durations, fare amounts and passenger counts. This provides the necessary critical information to train the requisite predictive models to judge taxi usage patterns.
## Data Preprocessing/Preparation
I had to complete several steps to ensure that the dataset was ready to use for modeling purposes. I first took in the data into a separate dataframe, I then analyzed the data to check for, and remove, all null values from the dataset. I then went ahead and removed all duplicates from the data to ensure that the results of the modeling process were not skewed by duplicate data. For this purpose, I used these specific commands df.drop_duplicates(inplace=True) and df.dropna(inplace=True).
I then split the cleaned dataset into a training and testing set to use for modeling using the train_test_split(X, y, test_size=0.2, random_state=42) method. This made it so that 20% of the dataset was used for testing and the remaining 80% was used for the training process.
## Modeling
For the modeling part of this project, I first created a baseline linear regression model using the LinearRegression() function. I then fit the baseline model with the X_train and y_train sets and finally used the mode.predict() function to generate some predictions upon completion. 

## Model Evaluation
I used the root_mean_squared_error function on the test set and the predicted values to determine the rmse value which was determined to be 8.87, which was relatively low given the context of the dataset. 
 