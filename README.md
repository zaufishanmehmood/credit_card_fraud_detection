# Credit Card Fraud Detection Using Machine Learning

## Project Overview
This project uses Machine Learning to identify fraudulent credit card transactions. It uses the Credit Card Fraud Detection dataset and compares Logistic Regression and Random Forest classifiers.

The main goal is to detect fraudulent transactions while reducing false alarms.

## Dataset
- **Source:** [Kaggle – Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- Original records: 284,807
- Features: 30
- Target column: `Class`
- `0` = Normal transaction
- `1` = Fraudulent transaction

The dataset contains anonymized features V1–V28, along with Time and Amount.

## Machine Learning Models
1. Logistic Regression
2. Random Forest Classifier

## Data Preprocessing
- Removed duplicate records.
- Checked missing values.
- Separated features and target.
- Used stratified training, validation and testing splits.
- Applied StandardScaler for Logistic Regression.
- Used class weights to address class imbalance.
- Selected the Random Forest classification threshold using validation data.

## Model Performance

| Metric | Logistic Regression | Random Forest |
|---|---:|---:|
| Accuracy | 97.53% | 99.95% |
| Precision | 5.64% | 93.67% |
| Recall | 87.37% | 77.89% |
| F1 Score | 10.59% | 85.06% |
| Average Precision | 67.19% | 80.84% |

Random Forest used a classification threshold of 0.2 for its final evaluation.

## Final Random Forest Results
- Accuracy: 99.95%
- Precision: 93.67%
- Recall: 77.89%
- F1 Score: 85.06%
- Average Precision: 80.84%

Confusion Matrix:

| | Predicted Normal | Predicted Fraud |
|---|---:|---:|
| Actual Normal | 56,646 | 5 |
| Actual Fraud | 21 | 74 |

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab

## How to Run
1. Download the notebook from this repository.
2. Download the dataset from Kaggle.
3. Upload `creditcard.csv` to Google Colab.
4. Open the notebook in Google Colab.
5. Run the cells step by step.

## Conclusion
Random Forest achieved better precision, F1 Score and Average Precision than Logistic Regression in this experiment. It provides a stronger balance between detecting fraudulent transactions and reducing false alarms.

This project is for educational and machine learning practice purposes.

## Author
Machine Learning Portfolio Project
