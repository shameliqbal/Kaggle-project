# Binary Classification with a Bank Churn Dataset 
![UTA-DataScience-Logo](https://github.com/user-attachments/assets/6d626bcc-5430-4356-927b-97764939109d)
# Overview
The primary objective of this project is to predict customer churn in a bank using historical customer data. The target variable, Exited, indicates whether a customer left the bank (1) or remained (0). By training a machine learning model.The goal is to identify patterns and key factors contributing to customer attrition, enabling proactive customer retention strategies.Initial data shape (165034, 14) and after cleaning: (165034, 12). The acurracy of the model Accuracy: 0.86

# Bank Churn Prediction Dataset

## Overview
This dataset contains customer data for a bank, aiming to predict customer churn (whether a customer will leave the bank). The target variable, `Exited`, indicates customer churn status:
- `1`: Customer exited.
- `0`: Customer stayed.

## Data Summary

### Initial Dataset
- **Total Rows**: [Initial record count- 165,034]
- **Total Columns**: [Initial feature count - 14]
- **Key Features**:
  - `CustomerId`: Unique identifier for customers.
  - `Surname`: Customer surname (dropped during cleaning).
  - `Geography`: Customer's country (e.g., France, Germany, Spain).
  - `Gender`: Male or Female.
  - `Age`: Customer age.
  - `Balance`: Account balance.
  - `CreditScore`, `Tenure`, `NumOfProducts`, `EstimatedSalary`.
  - `Exited`: Target variable for churn prediction.

### Cleaning and Preprocessing
- **Dropped Columns**:
  - `id` and `Surname` were removed as they do not contribute to churn prediction.
- **Categorical Encoding**:
  - `Geography` and `Gender` were converted into numerical values using label encoding.
- **Duplicates**:
  - Identified and removed duplicate rows.
- **Final Dataset Shape**:
  - **Rows**: [Cleaned record count- 165,004]
  - **Columns**: [REMAININg features- 12

## Key Features
- **Numerical Features**:
  - `CreditScore`, `Age`, `Tenure`, `Balance`, `NumOfProducts`, `EstimatedSalary`.
- **Categorical Features**:
  - `Geography`, `Gender`.

## Class Distribution
- `Exited = 0`: Majority class (customers who stayed).
- `Exited = 1`: Minority class (customers who left).

## Insights from Data
- Features such as `Age`, `Balance`, and `NumOfProducts` show distinct patterns between customers who stayed and those who exited.
- The dataset can be used to train a machine learning model to predict customer churn and identify significant factors influencing it.

## Usage
- Suitable for binary classification tasks.
- Can be used to develop predictive models using algorithms like Random Forest, Logistic Regression, or Neural Networks.

## Visualization Highlights
- Histograms reveal how each feature varies between the classes (`Exited = 0` and `Exited = 1`).
- 

