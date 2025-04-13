# Module 20: Credit Risk Classification Analysis

## Overview

This project focuses on building and evaluating a machine learning model to classify loan risk as either **healthy (low risk)** or **high-risk (likely to default)**. Using historical data from a peer-to-peer lending service, the goal was to identify the creditworthiness of borrowers through logistic regression, a classification algorithm.

The analysis includes:
- **Exploration of financial data**: Loan size, interest rate, and borrower characteristics.
- **Model training and evaluation**: Developing a logistic regression model and assessing its performance with key metrics.
- **Insights and recommendations**: Leveraging model performance to guide its applicability for real-world decision-making.

---

## Dataset

The dataset consists of historical loan information, with the following key variables:
- **Features (X)**:
  - Loan size
  - Interest rate
  - Borrower metrics such as total debt, derogatory marks, accounts, and more.
- **Target (y)**: `loan_status`
  - `0`: Healthy loan (low risk).
  - `1`: High-risk loan (likely to default).

The dataset is imbalanced, with more healthy loans (`0`) than high-risk loans (`1`), which influenced the model's evaluation metrics.

---

## Machine Learning Process

1. **Data Preparation**:
   - Separated the target variable (`loan_status`) and features.
   - Split the data into training (75%) and testing (25%) sets.
2. **Model Training**:
   - Trained a logistic regression model on the training dataset.
3. **Prediction**:
   - Used the trained model to predict loan statuses in the test dataset.
4. **Evaluation**:
   - Analyzed model performance using metrics like accuracy, precision, recall, F1-score, and confusion matrix.

---

## Results

### Performance Metrics:
- **Accuracy**: 99% - The model correctly classified 99% of loans.
- **Precision**:
  - Class `0` (Healthy loans): 100% - All loans predicted as healthy were truly healthy.
  - Class `1` (High-risk loans): 84% - 84% of loans predicted as high-risk were truly high-risk.
- **Recall**:
  - Class `0` (Healthy loans): 99% - 99% of actual healthy loans were correctly identified.
  - Class `1` (High-risk loans): 94% - 94% of actual high-risk loans were correctly identified.
- **F1-Scores**:
  - Class `0`: 100%.
  - Class `1`: 89%.

### Confusion Matrix:
- **True Positives (TP)**: 619 high-risk loans correctly identified.
- **True Negatives (TN)**: 18,765 healthy loans correctly identified.
- **False Positives 
