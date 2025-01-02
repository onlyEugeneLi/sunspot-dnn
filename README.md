Predicting Sunspots with DNN, Simple RNN and LSTM
=================================================

***Time Series Data Analysis***

# Introduction

![sunpots-nasa-photo](https://spaceplace.nasa.gov/solar-activity/en/solar-activity2.en.jpg)

Topic (Background):

Sunspots are temporary dark regions on the sun's surface. They are a key measure of solar activity, which affects many aspects of human society on Earth, such as navigation systems, power systems, and spacecrafts etc. Predicting the number of sunspots helps scientists to minimise its negative impact. 

Problem (Issues): 

This project aims to devise a robust Deep Learning (DL) model to predict sunspot numbers by recognising patterns in sunspot time series data. 

Objectives (Outline project):

1. Time series analysis of sunspots with statistics tool

1. Baseline prediction - moving average and data shifting

1. Use DNN to make sunspot number prediction
    - Hyperparameter tuning

1. Use RNN to make sunspot number prediction
    - Hyperparameter tuning

1. Use LSTM to make sunspot number prediction
    - Hyperparameter tuning

1. Compare performance

Source of data: [Kaggle Sunspots](https://www.kaggle.com/datasets/robervalt/sunspots/data)

## Time Series Analysis with Statistical Tools

![Stationary and Nonstationary time series](https://www.machinelearningplus.com/wp-content/uploads/2019/02/stationary-and-non-stationary-time-series-865x569.png?ezimgfmt=ng:webp/ngcb1)

## Hyperparameter Tuning

<!-- Data Preprocessing Methods

- Data windowing
- Data Slicing with Tensorflow -->

Table: The list of hyperparameter combinations

Tools

- `keras-tuner` - this works!
- `Sklearn.model_selection.GridSearchCV` and `scikeras`

Issues

- Data input errors when fitting training data into model. 
- Limited flexibility to tune batch size, window size and number of layers. 
- Need more randomness and wider coverage on learning rate. 

Trivial questions

- What's the difference between shape (30,) and shape (30, 1)?

# Reference

# Logs

2024-12-30

- Debug kerastuner function for hyperparameter tuning. It is necessary to tune learning rate separately or deploy a continuous range in the search space. 