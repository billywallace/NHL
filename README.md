# NHL Shots on Goal Prediction Project

## Overview 
In this repository, I have created two .ipynb files: train_models will train the logistic regression models as well as scrape up to date NHL player data from the NHL's API, and make_predictions.ipynb will allow you to predict Shots on Goal (SoGs) outcomes given the most up to date data. 


### How to use
    1. Update END_DATE variable to desired date in train_models.ipynb
    2. Run all cells in train_models.ipynb
        2a. This will take ~5 minutes to scrape all player data over all games year to date. 
    3. Run all cells in make_predictions.ipynb
    4. Investigate SoGs predictions for various Over/Unders that are predicted in cells. 
    5. Compare against predicted Over/Under SoGs outcome markets manually


### Evaluation
We evaluate the models on their predictive power using accuracy, but more importantly precision and recall to truly understand the strength of the model.  With respect to our use case, precision is more important as we would like to avoid mistakes. Evaluation against SoGs markets is challenging given I have not pulled in SoGs odds from live sports books. One assumption I made in evaluating my models is backtesting against players who currently have desired odds for SoGs lines -- most commonly I look for o2.5 at -150 or shorter. My thought process is that if we can achieve over 60% precision for test data, then -150 or shorter would be a profitable wager.

I have recorded my prediction history in make_predictions.ipynb


### Sources
This work would not have been possible without the documentation built out by Drew Hynes here: https://gitlab.com/dword4/nhlapi

Link to video on youtube: https://youtu.be/PteTu1mr09s