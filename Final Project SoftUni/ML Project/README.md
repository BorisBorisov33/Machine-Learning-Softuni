# Predict renewals of product for each customer

# Description:
    This is a time series project implemented in python with the help of the open-source Time Series library Darts
    (https://unit8co.github.io/darts/README.html).

    The goal of the project is to create a forecast/prediction on a specific company based on past values.
    The time aspect in this project is created manually. In the original data I had as time aspect a fiscal period(string) and I manually transformed it to a column called "time". The time column represent each month(timestamp).

    This time series is not a simple univariate time series project.
    My aim is to have multiple and multivariate time series. 
    The project:
        - multiple because I have many companies
        - multivariate because I have many "features"/ columns

    I will include here a column dictionary table as 'png' file in this folder. This files describes the available data.
    This table includes the name of the variable, the definition of it, source table and value range.
        
    In this project, the process made by me include preprocessing, handling null values, scaling the data,
    fit the data, predict the data, inverse transform and plot the results.

    I use three different models:
        - NBEATS model
        - TCN model - Temporal Convolutional Network
        - TFT model - Temporal Fusion Transformer

    For all the models, performance metrics such as mape, mae, r-squared,smape, marre and others were tested.

    A hyperparameter optimization was created using an open source hyperparameter optimization framework called Optuna.
    (https://optuna.org). 


Author: Boris Borisov