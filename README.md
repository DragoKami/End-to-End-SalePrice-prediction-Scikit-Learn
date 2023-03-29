# Predicting the Sale Price of Bulldozers using Machine Learning
This is an end to end SalePrice prediction of Buldozers, based on Blue Book for Bulldozers dataset on Kaggle

<img src = "bulldozer-new.jpg">

**In this notebook, we're going to go through an example machine learning project with the goal of predicting the sale price of bulldozers.**

## 1. Problem definition

> How well we can predict the future sale price of a bulldozer, given its characteristics and previous examples of how much similar bulldozers have been sold for?

## 2. Data

The data is downloaded from  Kaggle Bluebook for Bulldozers competition!
https://www.kaggle.com/competitions/bluebook-for-bulldozers/data

Data is split into three parts:

* `Train.csv` is the training set, which contains data through the end of 2011.
* `Valid.csv` is the validation set, which contains data from January 1, 2012 - April 30, 2012 You make predictions on this set throughout the majority of the competition. Your score on this set is used to create the public leaderboard.
* `Test.csv` is the test set, which won't be released until the last week of the competition. It contains data from May 1, 2012 - November 2012.

## 3. Evaluation

The evaluation metric for this project is the RMSLE (root mean squared log error) between the actual and predicted auction prices.

https://www.kaggle.com/competitions/bluebook-for-bulldozers/overview/evaluation

**Note:** The goal for most regression evalution metrics is to minimize the error. For example, our goal for this project will be to build a machine learning model which minimizes RMSLE.

## 4. Features

The features can be seen below alog with their description:

<img src="feat-img1">
<img src="feat-img2">
<img src="feat-img3">


## Steps to run:
* Create a conda environment with scikit-learn, numpy, matplotlib, jupyter, pandas, seaborn
* Clone this repo
* Run the notebook

## License
This notebook is created by Abhishek Gautam and is licenced under MIT.

