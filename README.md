# Exploratory_Project-powertheftdetection
Approach for Project
The  dataset  used  is  found  on  Kaggle  about  Smart Meters  in 
London :https://www.kaggle.com/jeanmidev/smart-meters-in-london
For data cleaning few techniques were used to remove outliers and Nan values.As energy consumption depends on type of user clustering was done using appropriate number of clusters and small amount of data was manipulated from each cluster to create data for electricity theft and added to given dataset. Some other features having correlation with energy consumption were added in dataset. This dataset is then tested upon few model and model with best accuracy was chosen for prediction.
It has following files
Data Preprocessing :- It contain all techniques applied to clean the data , forming clusters, creating fake data and adding extra features to the power consumption data.

Number_Of_Cluster:- It contain Elbow and Silhouette Method used to find appropriate number of clusters according to the dataset.

Check_Correlation:- It contain method used to link electricity consumption and weather condition of each day. Then correlation matrix was formed to find dependent features.

Feature_Selection:- In this file some extra features such as month , day , season etc. were generated to daily consumption data. Also precipitation type and holiday features were added. Then correlation matrix was formed to find dependent features. 

Model_Selection:- In this file dataset is split in training and testing set and various methods were applied to find accuracy and one with highest accuracy was selected for final training.

Accuracy given by Random Forest model is ~80% in prediction of power theft by training it on 70% data set and testing on 30% dataset.

In this model other factors like temperature, uv index, season, month, holidays and precipitation type are taken in consideration with energy consumption to predict power theft. Some factors like Acorn Details, hourly dataset are not used and all customers were considered honest, focusing on these factors can further help in increasing accuracy of model in future.
