# Car Evaluation Classification

Educational machine learning project by Nivedha Sivakumar.

## Changes from the saved notebook
- Fixed reversed classification-report and confusion-matrix arguments
- Replaced arbitrary category numbers with one-hot encoding
- Added fixed stratified holdout, training-only stratified CV and majority baseline
- Removed deprecated multi_class argument and raw fold-index dumps

## Run locally
Use Python 3.12, install `pip install -r requirements.txt`, and place an authorized copy of `car_evaluation.csv` beside the notebook (or in `data/` as shown). Dataset redistribution rights have not been established, so input data is not included. Run all notebook cells in order.

## Validation
Executed successfully top-to-bottom on the local source data using Python 3.12. Exact tested package versions are recorded in requirements-lock.txt. Saved charts were visually reviewed. Historical output claims have been removed; new conclusions must follow the revised evaluation.

## Limits
This is a learning project, not a deployed decision system. Holdout scores do not establish external validity, fairness, or causal effects. 

## Observed results

Training-only cross-validation selected XGBoost by macro F1. On the untouched 519-row holdout it correctly classified 514 rows (99.0%). This result applies to this benchmark split, not real-world vehicle safety or market suitability. No test-set hyperparameter search was performed.
