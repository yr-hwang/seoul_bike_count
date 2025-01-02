# Seoul Public Bike Demand Prediction Model

The goal of this project is to implement a machine learning model that can predict the demand for rental bicycles in Seoul based on various factors. This is important to overcome the rebalancing issue of the number of bicycles, hence providing the appropriate number of bicycles based on the demand at any certain time.

The task was evaluated on the following baseline models:
* Linear Regression
* Random Forest Regressor
* KNN Regressor
* SVR
* MLP Regressor

The results of the final model chosen using random search is as follows.
* Model with the best CV score: MLP Regressor
* Best CV Score: 0.9519
* Best Hyperparameters: {'solver': 'adam', 'learning_rate': 'adaptive', 'hidden_layer_sizes': (100, 100), 'alpha': 0.0001, 'activation': 'relu'}

The results of the final model evaluated on the test set is as follows:
* Test RMSE: 614683.5829
* Test MAE: 456453.3745
* Test R-squared: -906849.6396
