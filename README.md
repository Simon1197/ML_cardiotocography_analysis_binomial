# ML_cardiotocography_analysis_binomial

## Data source
Cardiotocography data set from the UCI website. 
Here is the link for the dataset https://archive.ics.uci.edu/ml/datasets/cardiotocography. 

## Variables and observations
In the dataset, it has 2126 observations and 23 variables such as minimum, mean, maximum value of histogram, beats accelerate, and decelerate times, etc. The percentage of time with abnormal for the long and short term are also included. 

## Purposes
Our goal in analyzing this dataset is to use logistic and lasso regression and KNN, decision tree and random forrest to tune our models and provide a higher accuracy prediction model to predict NSP based on these variables. The original response variable of our dataset is NSP which is fetal state class code (N=normal; S=suspect; P=pathologic) and we switch the three classifications into two (1 = normal, 2 = abnormal).

## Procedure
There has no missing value in the dataset. Thus, we remove 0 and remain 2126 observations for our full dataset. After cleaning the data, we divide our original to training (90%) and testing (10%) dataset and use ten-fold cross validation with three times repeated to train our data. 
