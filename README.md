# Regression Tree for Predicting Mean Temperature in London
This project is to use a Regression Tree to predict the mean temperature on a given day in London, given information on the Month, Cloud Cover, Sunshine, Global Radiation, Precipitation and Pressure on the day. 

## DATA
The data used in this project is 'london_weather.csv' from https://www.kaggle.com/datasets/emmanuelfwerr/london-weather-data?resource=download, which in turn was sourced from https://www.ecad.eu/dailydata/index.php

## MODEL 
The model is a Regression Tree. This was chosen as the aim was to produce not only a model with accurate results, but also a model that could be easily interpreted and understood. The use of a Regression Tree allows easy insight into how the model is making its predictions and which variables it believes are the most important in estimating the temperature.

## HYPERPARAMETER OPTIMSATION
There are two steps in the hyperparameter optimisation process. The first is a grid search method for the parameters:
- criterion
- splitter
- max_depth
- min_samples_split
- min_samples_leaf

Bayesian Optimisation is then used to optimise the min_impurity_decrease.

## RESULTS
The final tree got a score of 73.99% on the validation data. It found that the month and the global radiation were the two most important variables in determining the mean temperature.

This is the resulting tree:
![tree](https://user-images.githubusercontent.com/131019698/232862360-fb8649bb-7e17-4b21-9e8a-73545fe3fa2b.png)
