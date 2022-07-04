## Detection of Erroneous Weather Data

This project aims to predict erroneous measurements in the data received from North Carolina State Climate office.

## EcoNet Dataset 

The NC Climate Office receives measurements from various(23) sensors across 45 stations each day. This amounts to around 544 million samples of data each year. First, these data points get automatically flagged by quality control sensors. Then these flagged samples have to be manually reviewed by experts at the Climate Office to check if any of samples are erroneous(which would mean the sensors need to be looked at). Since the number of samples is huge, this would take a considerable amount of time and effort. 

## Problem Statement

This is a supervised, binary classification problem, where we need to predict whether different measures from weather stations are erroneous(instead of manual flagging).

**The project report can he found [here](/ProjectReport)**

## Libraries Used for the Project
1) pandas 
2) tqdm 
3) numpy 
4) datetime
5) sklearn
6) imblearn
7) scipy
8) tensorflow 
9) os


## Project Flow
1) All the preprocessing steps like one hot encoding, Normalization and feature engineering are performed in "PreProcessing.ipynb". This will generate two csv files, Train_updated.csv and Test_updated.csv
2) Now all the model (Decision Tree, Random Forest, Logistic Regression) training and hyperparameter tuning is performed in the file, "ModelRandomSearch.ipynb" file, this also generates a prediction.csv file which was submitted as part of the competition.
3) A ANN Model is trained and later tuned in the file, "NeuralNetwork.py".


## Commands to Run
1) After Installing all the libraries mentioned in the above list.
2) Run the Jupiter Notebooks mentioned above in the respective order.
3) Also, Run the python file NeuralNetwork.py using `python3 NeuralNetwork.py`
