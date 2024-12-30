This project is an extension of a Coursera course "Sequence, Time Series and Prediction" assignemnt. 

More work is yet to be published and updated here.

Time series features and their visualisation

## Time Series Analysis with Statistical Tools

![Stationary and Nonstationary time series](https://www.machinelearningplus.com/wp-content/uploads/2019/02/stationary-and-non-stationary-time-series-865x569.png?ezimgfmt=ng:webp/ngcb1)

## Hyperparameter Tuning

<!-- Data Preprocessing Methods

- Data windowing
- Data Slicing with Tensorflow -->

Tools

- `keras-tuner` - this works!
- `Sklearn.model_selection.GridSearchCV` and `scikeras`

Issues

- Data input errors when fitting training data into model. 
- Limited flexibility to tune batch size, window size and number of layers. 
- Need more randomness and wider coverage on learning rate. 

Trivial questions

- What's the difference between shape (30,) and shape (30, 1)?

## Logs

2024-12-30

- Debug kerastuner function for hyperparameter tuning. It is necessary to tune learning rate separately or deploy a continuous range in the search space. 