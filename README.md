# DS3000_fraud-detection-model

Machine learning model for detecting fraudulent financial transactions.

## Team Members
- Brayden
- Ethan
- Waddah

## Dataset

[Financial Transactions Dataset for Fraud Detection](https://www.kaggle.com/datasets/aryan208/financial-transactions-dataset-for-fraud-detection) (Kaggle)

- 5,000,000 synthetic transactions, 18 columns
- Target column: `is_fraud` (179,553 fraud cases, about 3.59%)
- File: `financial_fraud_detection_dataset.csv` (about 800 MB)

The dataset is too large for GitHub, so it is not stored in this repository. The notebook downloads it automatically from Kaggle with `kagglehub` the first time it runs.

## How to Run

### Option 1: Google Colab (easiest)
1. Open `notebooks/notebook1_model_training_faster.ipynb` in Google Colab.
2. Click **Runtime → Run all**. The dataset downloads automatically.

### Option 2: On your own computer
1. Install Python 3.10 or newer.
2. Install the libraries:
   ```bash
   pip install -r requirements.txt
   ```
3. Start Jupyter and open `notebooks/notebook1_model_training_faster.ipynb`:
   ```bash
   jupyter notebook
   ```
4. Run all cells. The dataset downloads automatically on the first run.

If the Kaggle download asks you to sign in, see the [kagglehub instructions](https://github.com/Kaggle/kagglehub#authenticate).

## Completed

- Data loading and exploratory data analysis
- Data cleaning and feature selection
- Train/validation/test split
- Preprocessing pipeline
- Baseline model
- Model training and hyperparameter tuning
- Model evaluation
- Best model selection and threshold optimization
- Final model training and testing
- Final report completed

## Models
- Logistic Regression (baseline)
- Decision Tree
- Random Forest
- XGBoost (with decision-threshold tuning)

## Libraries
- Pandas
- Polars
- NumPy
- Scikit-learn
- XGBoost
- Matplotlib
- kagglehub

## File Structure
- `notebooks/notebook1_model_training_faster.ipynb`: final notebook (data loading, cleaning, all models, XGBoost and threshold tuning)
- `notebooks/notebook1.ipynb`: earlier draft of the notebook
- `Final_Report_Formatted.pdf`: final project report
- `requirements.txt`: Python libraries needed to run the notebook
- `.gitignore`: files excluded from version control
