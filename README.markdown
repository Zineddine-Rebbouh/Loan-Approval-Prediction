# Loan Approval Prediction

## Overview
This repository contains a machine learning project to predict loan approval outcomes using the Kaggle Loan Approval Prediction Dataset. The project implements binary classification models (Logistic Regression and Decision Tree), handles missing values, encodes categorical features, addresses class imbalance with SMOTE, and visualizes the target variable's distribution. Performance is evaluated using precision, recall, and F1-score.

## Dataset
The dataset is sourced from Kaggle's Loan Approval Prediction Dataset. It includes features like `loan_id`, `no_of_dependents`, `education`, `self_employed`, `income_annum`, `loan_amount`, `loan_term`, `cibil_score`, and the target variable ` loan_status` (' Approved' or ' Rejected'). Download the dataset from [Kaggle](https://www.kaggle.com/datasets/architsharma01/loan-approval-prediction-dataset) and place it in the `data/` folder as `loan_data.csv`.

## Requirements
To run the scripts, install the required Python libraries:
```bash
pip install pandas matplotlib scikit-learn imblearn
```

## Project Structure
- `loan_approval_prediction.py`: Main script for preprocessing, training Logistic Regression and Decision Tree models, applying SMOTE, and evaluating performance.
- `plot_loan_status_distribution.py`: Script to generate a bar chart visualizing the distribution of the ` loan_status` column.
- `data/`: Directory to store the dataset (`loan_data.csv`).
- `README.md`: This file.

## Usage
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/loan-approval-prediction.git
   cd loan-approval-prediction
   ```

2. **Place the Dataset**:
   - Download the dataset from Kaggle.
   - Save it as `data/loan_data.csv`.

3. **Run the Prediction Script**:
   ```bash
   python loan_approval_prediction.py
   ```
   This script:
   - Preprocesses the data (handles missing values, encodes categorical features).
   - Applies SMOTE to address class imbalance.
   - Trains and evaluates Logistic Regression and Decision Tree models.
   - Outputs precision, recall, and F1-score for both models.

4. **Run the Visualization Script**:
   ```bash
   python plot_loan_status_distribution.py
   ```
   This script generates a bar chart showing the distribution of ` loan_status` (' Approved' vs. ' Rejected').

## Notes
- Ensure the dataset file is named `loan_data.csv` and placed in the `data/` folder.
- The target column is ` loan_status` (with a leading space). If your dataset has a different column name or values, update the scripts accordingly.
- The visualization assumes ` loan_status` has values ' Approved' and ' Rejected'. Check the unique values using the script's output and adjust the `xticks` labels if needed.

## Results
- The prediction script outputs performance metrics (precision, recall, F1-score) for both models, allowing comparison of their effectiveness on imbalanced data.
- The visualization script displays a bar chart to highlight the class distribution of loan approvals.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments
- Dataset provided by Kaggle user [Archit Sharma](https://www.kaggle.com/datasets/architsharma01/loan-approval-prediction-dataset).
- Built with Python, scikit-learn, pandas, matplotlib, and imblearn.