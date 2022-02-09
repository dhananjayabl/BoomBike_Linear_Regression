# Project Name
> BoomBike - Multiple Linear Regression model is built on the BoomBikes data, to identity the significant variables in predicting the demand for shared bikes and also to understand the effect of these variables on the demand for the bikes


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
BoomBike offers a bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free.

BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state. 

**Analytical Objective**
- To understand which variables are significant in predicting the demand for the shared bikes
- How well those variables describe the bike demands

The dataset used in the time-series data of Total Bike Rentals recorded every day for the period of 2018 and 2019. 
The dataset is used a cross-sectional data by removing the temporal features from the data and by shuffling.
There are 730 rows and 16 columns, some are irrelevant columns, those are not considered in the analysis.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- The best fit model (OLS based MLR ) could only explain the 42% variance (Adjusted R-squared) in the test data as compared to 57% of variance in the train data, hence not recommended to be used for predicting the demand
- The model has high bias and high variance and underfit the data
- However the model can be used to explin the relationship between Independent Variable and Target Variable - 'cnt'
- The variables that are considered in best fit model are - `temp`, `windspeed`, `season_2`, `season_4`, `mnth_9`, `weekday_6`, `workingday_1`, `weathersit_2`, and `weathersit_3`
- While features  `temp`, `season_2`, `season_4`, `mnth_9`, `weekday_6`, `workingday_1` have positive relationships with demand, features -  `windspeed`, `weathersit_2`, and `weathersit_3` have negetive impact on the demand
- Best fit model:  
$$
count = 1295.4 + (5307.68 * temp) - (1153.59 * windspeed) + (745.78 * season_2) + (1228.76 * season_4) + (792.85 * mnth_9) + (592.63 * weekday_6) + (565.29 * workingday_1) - (685.62 * weathersit_2) - (2876.88 * weathersit_3)  
$$
- Using this model suitable promotional offerings / business plan can be deviced

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- python - 3.10.1
- pandas - 1.3.5
- numpy - 1.21.5
- matplotlib - 3.5.1
- seaborn - 0.11.2
- scikit-learn - 1.0.2
- scipy - 1.7.3
- statmodels - 0.13.1

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
Give credit here.
- This project was inspired by...
- References if any...
- This project was based on [this tutorial](https://www.example.com).


## Contact
Created by [@githubusername] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->