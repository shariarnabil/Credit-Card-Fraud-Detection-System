# Credit-Card-Fraud-Detection-System

Credit Card Fraud Detection System

Overview

This project demonstrates a machine learning-based fraud detection system using a logistic regression model trained on credit card transaction data. The model predicts whether a transaction is legitimate or fraudulent based on 30 transaction features (including anonymized V1-V28 features, Time, and Amount).

dataset link = https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud#machinelearning


Features

    Trained logistic regression model on PCA-transformed credit card dataset.

    Prediction of transaction legitimacy based on user input or uploaded data.

    CSV-compatible output for easy data logging.

    Fraud probability displayed for each transaction.

Requirements

    Python 3.7+

    Required Libraries:

        numpy

        pandas

        sklearn (for preprocessing and model training)


Usage

1. Manual Transaction Input

You can input a single transaction manually (with 30 values):

# Run the script
python fraud_detection.py

# When prompted, enter 30 comma-separated values (e.g.)
Enter transaction data (30 comma-separated values): 0, -1.359807, -0.072781, ..., 0.133558

The script will output whether the transaction is legitimate or fraudulent, along with the fraud probability.
2. Batch Transaction Prediction via CSV

You can also prepare a CSV file with multiple rows of transaction data (each row should have 30 comma-separated values):


Example:

0,-1.359807,-0.072781,2.536346,1.378155,-0.338321,0.462388,0.239599,0.098698,0.363787,0.090794,-0.551600,-0.617801,-0.991390,-0.311169,1.468177,-0.470400,0.207971,0.025791,0.403993,0.251412,-0.018307,0.277838,0.373200,0.086295,0.324211,-0.042999,0.118070,0.133558
...

Update and run the script to read and process the CSV file.

Notes

    A fraud probability above 50% is flagged as fraudulent.

    You may adjust the threshold for more sensitivity or specificity depending on use case.

