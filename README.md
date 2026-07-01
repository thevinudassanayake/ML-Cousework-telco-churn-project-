# ML Coursework - Telco Churn Project

This repository contains two notebook-based machine learning exercises:

- `Telco_Churn_Project.ipynb` - customer churn prediction for a telecom dataset
- `Emotion_model.ipynb` - an additional audio emotion preprocessing and sequence-building notebook

## Telco churn workflow

The churn notebook cleans the telecom customer data, explores churn patterns, and trains models to predict customer attrition.

### Main steps

- Load and inspect the telecom dataset
- Fix missing or messy values, especially `TotalCharges`
- Remove the customer identifier column
- Encode the churn target
- Explore churn by tenure, monthly charges, and contract type
- Train a decision tree model with cross-validated tuning
- Train a small neural network with class weighting and early stopping

### Evaluation snapshot

- Test-set accuracy: `0.754`
- Precision: `0.525`
- Recall: `0.749`
- F1 score: `0.617`
- ROC AUC: `0.837`

## Emotion model notebook

The second notebook prepares fixed-length audio feature sequences and label arrays from a Drive-based dataset. It is a separate experiment but lives in the same repo.

## Project value

- Good example of a full churn-analysis pipeline
- Combines preprocessing, visualization, classical ML, and neural network experimentation
- Uses reproducible random seeds and explicit evaluation metrics

## Run notes

- The notebooks were built for Jupyter or Google Colab
- The churn notebook expects the telecom CSV file in the working directory
- The emotion notebook expects the dataset to be available in Google Drive paths defined inside the notebook
