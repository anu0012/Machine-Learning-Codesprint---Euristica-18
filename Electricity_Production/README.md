## Problem Statement

An engineer at a power generation plant anticipates that power generated in the plant can be calculated only from ambient variables of the plant i.e. without knowledge of the machines and their efficiencies. He has data of ambient variables and electricity generated for several days, so to check if his anticipations are correct he asks you to predict Net daily generated electrical energy (E) MW for 200 days. 

The ambient variables of the power plant are:

Temperature (T) in °C
Ambient Pressure (P) in millibar
Relative Humidity (RH)
Exhaust Vacuum (V) in cm Hg
The training data includes ambient variables along with Net daily electrical energy (E) MW.

The variables are given without normalization.

## Approach

1. I started with some exploratory data analysis.
2. Split the training data to cross validate the model.
3. Train the data on different models i.e. LinearRegression, Lasso, XGB etc.
4. Best result got by averaging of 4 models(LassoCV, LinearRegression, XGB and GradientBoostingRegressor)
5. Got 0.958 r2_score.
