# Binary Classification with a Bank Churn Dataset 
![UTA-DataScience-Logo](https://github.com/user-attachments/assets/6d626bcc-5430-4356-927b-97764939109d)

## Project Objective
- Predict customer churn in a bank using historical customer data.
- The target variable `Exited` indicates:
  - `1`: Customer left the bank.
  - `0`: Customer remained with the bank.
- Identify patterns and key factors contributing to customer attrition.
- Enable proactive customer retention strategies based on predictions.

<img width="488" alt="Screenshot 2024-12-13 at 12 48 51 PM" src="https://github.com/user-attachments/assets/a9d8ab4b-337e-432a-8d03-a37b6e18763a" />


## Data Overview
- Initial dataset shape 165034 rows and 14 columns
- **After data cleaning:** 165034 rows and 12 columns 

## Model Performance
- **Accuracy:** `0.86`

## Tools and Techniques
- Machine learning model trained to predict customer churn.
- Data preprocessing and cleaning to ensure model reliability.

# Bank Churn Prediction Dataset


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
<img width="609" alt="Screenshot 2024-12-13 at 12 12 40 PM" src="https://github.com/user-attachments/assets/4ab01e0e-eb81-4932-8a8a-97ad2e867288" />
<img width="592" alt="Screenshot 2024-12-13 at 1 10 34 PM" src="https://github.com/user-attachments/assets/0ae5984c-3d8b-446a-9b74-d9733417568e" />

# ROC Curve 

<img width="578" alt="Screenshot 2024-12-13 at 1 28 13 PM" src="https://github.com/user-attachments/assets/d5eade03-d9ba-4173-a15c-20db3e1078ea" />


### Random Forest Classifier Performance
- **ROC Curve**:
  - The model achieved an **AUC (Area Under the Curve)** of **0.87**, indicating strong performance in distinguishing between customers who exited and those who stayed.
  - The curve is close to the top-left corner, showing an effective balance between True Positive Rate (TPR) and False Positive Rate (FPR).

- **Model Evaluation**:
  - The model effectively identifies churned customers while maintaining a low rate of false positives.
  - Results suggest the Random Forest classifier is well-suited for this dataset.

- **Threshold Adjustment**:
  - Depending on business needs, the threshold can be tuned to prioritize sensitivity (capturing more churned customers) or specificity (reducing false positives).

### Implications
- A high AUC score of **0.87** highlights the model's strong predictive capabilities.
- Features such as `Age`, `Balance`, and `NumOfProducts` are influential in predicting customer churn.
- Future work could involve hyperparameter tuning or feature engineering to further improve the model's performance.

