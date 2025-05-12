# Credit Card Fraud Detection

This project demonstrates how to detect fraudulent credit card transactions using machine learning techniques. It uses a dataset of anonymized transaction data and applies a Random Forest Classifier to identify suspicious activity.

## Project Structure

- `credit_card_fraud_detection.py` – Main script that performs data loading, preprocessing, model training, evaluation, and prediction.
- `creditcard.csv` – Dataset used for training and testing the model. (Not included here due to size and confidentiality.)
- `README.md` – Project overview and instructions.

## Dataset Overview

- **Source:** [Kaggle Credit Card Fraud Detection Dataset](https://www.kaggle.com/mlg-ulb/creditcardfraud)
- **Rows:** 284,807 transactions
- **Features:** 30 features including `Time`, `Amount`, and anonymized PCA-transformed variables `V1` to `V28`
- **Target:** `Class` (0 = Valid transaction, 1 = Fraudulent transaction)

## Process Overview

1. **Data Loading**
   - Reads the dataset from a CSV file.
2. **Exploratory Data Analysis**
   - Visualizes class imbalance and summary statistics.
   - Correlation heatmap to understand relationships.
3. **Data Preparation**
   - Splits dataset into features (`X`) and target (`Y`)
   - Train-test split (80/20)
4. **Model Training**
   - Random Forest Classifier from `scikit-learn`
5. **Model Evaluation**
   - Accuracy, Precision, Recall, F1 Score, Matthews Correlation Coefficient
   - Confusion Matrix visualization
6. **New Prediction**
   - Predicts whether a given transaction is fraudulent.

## 🛠️ Requirements

- Python 3.x
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn

Install dependencies using:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
