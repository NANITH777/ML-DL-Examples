# Credit Card Fraud Detection

## Overview

This project focuses on detecting fraudulent credit card transactions using machine learning and deep learning techniques. The primary goal is to accurately classify transactions as "Normal" or "Fraud" using a combination of data preprocessing, model training, and evaluation.

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Modeling](#modeling)
- [Results](#results)

## Dataset

The dataset used in this project is the [Kaggle Credit Card Fraud Detection dataset](https://www.kaggle.com/mlg-ulb/creditcardfraud). It contains transactions made by European cardholders over two days in September 2013. The dataset is highly imbalanced, with fraudulent transactions constituting a very small percentage of the total.

- **Total transactions**: 284,807
- **Fraudulent transactions**: 492

## Installation

 **Clone the repository**:

    ```bash
    git clone https://github.com/yourusername/credit-card-fraud-detection.git
    ```


## Usage

1. **Preprocessing and EDA**: 
    - Load and inspect the dataset.
    - Check for missing values and perform scaling on numerical features.
    - Visualize the distribution of transaction classes and amounts.

2. **Model Training**:
    - Build and train an autoencoder to detect anomalies in transaction data.
    - Use logistic regression for final classification of transactions.

3. **Model Evaluation**:
    - Evaluate model performance using metrics like accuracy, precision, recall, and F1 score.

## Modeling

### Autoencoder

The autoencoder is used to compress and reconstruct transaction data, identifying anomalies based on reconstruction errors. This approach helps in distinguishing between normal and fraudulent transactions.

### Logistic Regression

A logistic regression model is trained on the compressed data from the autoencoder to classify transactions. This model provides a final prediction on whether a transaction is fraudulent or not.

## Results

The model's performance is evaluated based on:

- **Accuracy**: Measures overall correctness.
- **Precision**: Indicates the proportion of true positives among the predicted positives.
- **Recall**: Indicates the proportion of true positives among actual positives.
- **F1 Score**: Balances precision and recall, providing a single metric for evaluation.

The model effectively identifies fraudulent transactions while minimizing false positives and negatives.