# Stock Price Movement Prediction using Machine Learning

## Project Overview

This project predicts whether a stock’s closing price will increase or decrease the next day using machine learning classification models. The goal is to classify price movement direction:

- 1 → Price goes up  
- 0 → Price goes down  

This project demonstrates an end-to-end ML pipeline including data preprocessing, feature engineering, model training, and evaluation.

## Dataset Description

The dataset contains historical stock data with **1009 rows and 7 columns**:

- Date
- Open
- High
- Low
- Close
- Adj Close
- Volume

### Data Preprocessing Steps

- Checked for missing values (none found)
- Created new engineered features
- Standardized features before training

## Feature Engineering

Two additional features were created:

- `open-close` = Open − Close  
- `low-high` = Low − High  

### Target Variable

The target is defined as:

1 → If next day’s Close price > Today’s Close  
0 → Otherwise  

This converts the task into a binary classification problem.

## Models Implemented

The following models were trained and compared:

- Logistic Regression
- Support Vector Classifier (Polynomial Kernel)
- XGBoost Classifier

### Data Split

- 90% Training Data
- 10% Validation Data

## Libraries Used
- numpy  
- pandas  
- matplotlib  
- seaborn  
- scikit-learn  
- xgboost  


