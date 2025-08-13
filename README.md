Loan Approval Prediction Project Description
Overview
This project focuses on building a machine learning model to predict whether a loan application will be approved based on the Kaggle Loan Approval Prediction Dataset. The goal is to develop a robust binary classification model, addressing challenges such as missing values, categorical feature encoding, and class imbalance. Two models—Logistic Regression and Decision Tree—are trained and evaluated, with performance metrics emphasizing precision, recall, and F1-score. Additionally, SMOTE is used to handle class imbalance, and a visualization of the target variable's distribution is included to highlight the dataset's characteristics.
Objectives

Data Preprocessing: Handle missing values using median imputation for numerical features and most frequent imputation for categorical features. Encode categorical variables using LabelEncoder.
Class Imbalance: Apply SMOTE to balance the training data, ensuring better model performance on minority classes.
Model Training: Train and compare Logistic Regression and Decision Tree models.
Evaluation: Assess model performance using precision, recall, and F1-score to account for imbalanced data.
Visualization: Generate a bar chart to visualize the distribution of the target variable (' loan_status').

Dataset
The dataset used is the Loan Approval Prediction Dataset from Kaggle, containing features such as loan_id, no_of_dependents, education, self_employed, income_annum, loan_amount, loan_term, cibil_score, residential_assets_value, commercial_assets_value, luxury_assets_value, bank_asset_value, and the target variable  loan_status (with values ' Approved' and ' Rejected').
Key Features

Preprocessing: Handles missing values and encodes categorical features.
Imbalanced Data Handling: Uses SMOTE to oversample the minority class.
Model Comparison: Evaluates Logistic Regression and Decision Tree models.
Visualization: Includes a bar chart to display the distribution of loan approval statuses.

Tools and Libraries

Python
pandas: Data manipulation
scikit-learn: Machine learning models and preprocessing
imblearn: SMOTE for class imbalance
matplotlib: Visualization

Outcomes
The project provides insights into the performance of Logistic Regression and Decision Tree models on an imbalanced dataset, with detailed metrics to guide model selection. The visualization highlights the distribution of loan approvals, aiding in understanding class imbalance.
