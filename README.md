# Bank Churn Prediction

This project focuses on predicting whether a customer is likely to leave a bank within the next six months. It uses a tabular customer dataset and builds a machine learning model, with a neural network-based classifier used in the analysis.

## Project Objective

The main goal is to identify churn-prone customers so the bank can take preventive action and improve customer retention.

## Dataset

The project uses the dataset in `bank.csv`.

It contains customer information such as:

- Credit score
- Geography
- Gender
- Age
- Tenure
- Balance
- Number of products
- Credit card status
- Active member status
- Estimated salary
- Churn label (`Exited`)

The target variable is:

- `Exited = 0`: customer did not leave the bank
- `Exited = 1`: customer left the bank

## Files in this Repository

- `Bank_Churn_Prediction.ipynb` — notebook with data cleaning, EDA, preprocessing, model building, and evaluation
- `bank.csv` — customer dataset used for training and evaluation
- `README.md` — project overview and usage notes

## Workflow Covered in the Notebook

The notebook includes:

1. Loading and inspecting the dataset
2. Dropping irrelevant identifiers such as customer ID and surname
3. Exploratory data analysis (EDA)
4. Visualizing churn patterns across demographic and financial features
5. Splitting the data into train, validation, and test sets
6. Encoding categorical variables
7. Standardizing numerical features
8. Handling class imbalance with SMOTE
9. Training a neural network model
10. Evaluating performance using accuracy, confusion matrix, and ROC metrics

## Requirements

Use Python 3.9+ and install the following packages:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn tensorflow jupyter
```

## How to Run

### Option 1: Open the notebook

```bash
jupyter notebook
```

Then open `Bank_Churn_Prediction.ipynb` in the browser.

### Option 2: Run the notebook from the terminal

```bash
jupyter nbconvert --to notebook --execute Bank_Churn_Prediction.ipynb
```

## Model Notes

The notebook demonstrates a neural network classifier for binary classification, suitable for churn prediction tasks. It also evaluates model quality with business-relevant metrics, especially because churn is a minority class in the dataset.

## Insights Summary

The analysis highlights patterns such as:

- higher churn among inactive members
- more churn among older customers
- differences in churn rate by geography and gender
- the importance of modeling the minority class effectively

## License

This project is intended for educational and analytical use.
