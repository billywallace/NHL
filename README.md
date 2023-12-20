# NHL Shots on Goal Prediction Project

## Overview 
In this repository, I have created two .ipynb files: train_models will train the logistic regression models as well as scrape up to date NHL player data from the NHL's API, and make_predictions.ipynb will allow you to predict Shots on Goal (SoGs) outcomes given the most up to date data. 


## What are we trying to predict?
I am aiming to predict whether a given player will have Over/Under a specified number of shots on goal in a certain game. 


### Evaluation
We evaluate the models on their predictive power using accuracy, but more importantly precision and recall to truly understand the strength of the model.  With respect to our use case, precision is more important as we would like to avoid mistakes. 


## Sources
This work would not have been possible without the documentation built out by Drew Hynes here: https://gitlab.com/dword4/nhlapi

Link to video on youtube: https://youtu.be/PteTu1mr09s