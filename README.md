# Telco Customer Churn Prediction

## Overview
This project predicts whether a customer will stop using a telecom service. It uses the Telco Customer Churn dataset and a Random Forest Classifier to identify at-risk customers before they leave.

## Problem Statement
Customer churn directly affects revenue. This project builds a model that flags churners early so businesses can act on retention.

## Dataset
- Source: Telco Customer Churn dataset
- Records: 7,043 customers
- Target variable: Churn (Yes/No)
- Key features: tenure, InternetService, PaymentMethod, Contract, TotalCharges

## Tech Stack
Python, pandas, NumPy, scikit-learn, seaborn, matplotlib

## Project Steps
1. Loaded and explored the dataset
2. Handled missing values in TotalCharges using median imputation
3. Encoded 16 categorical variables using LabelEncoder
4. Split data 80/20 for training and testing
5. Standardized features using StandardScaler
6. Trained a Random Forest Classifier
7. Evaluated performance using accuracy score and confusion matrix

## Results
| Metric | Value |
|--------|-------|
| Accuracy | 78% |
| True Positives | 181 |
| False Negatives | 187 |

## Known Limitation
The model misses a high number of actual churners. Future work will apply SMOTE to address class imbalance and optimize using F1-score instead of accuracy.

## How to Run
1. Clone this repository
2. Install dependencies: `pip install -r requirements.txt`
3. Run the notebook: `jupyter notebook churn_prediction.ipynb`
