# Telco Churn Project Insights

## Executive summary

- The churn dataset is imbalanced, so recall matters almost as much as accuracy.
- The notebook uses both tree-based and neural-network approaches, which gives a useful comparison of simpler versus deeper models.
- The decision tree model reaches about `75.4%` accuracy and a strong `0.837` ROC AUC, while recall on churners is especially useful for retention analysis.

## What the notebook shows

- Tenure is a strong churn signal: shorter-tenure customers are more likely to leave.
- Monthly charges and contract type also appear to separate churners from retained customers.
- Preprocessing is handled carefully, including numeric conversion of `TotalCharges` and target encoding for `Churn`.
- The pipeline uses `ColumnTransformer`, scaling, encoding, `GridSearchCV`, and class weighting.

## Practical takeaways

- Retention campaigns should prioritize low-tenure customers and those on short-term contracts.
- Model selection should favor recall when the goal is to catch likely churners early.
- The notebook structure is a strong base for trying logistic regression, random forest, or gradient boosting next.

## Extra notebook note

- `Emotion_model.ipynb` suggests the repo is also being used as a home for other ML coursework, not only churn prediction.
