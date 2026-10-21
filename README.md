
# Telco Customer Churn Prediction Using Machine Learning

## 1. Project Overview

This project predicts whether a telecommunications customer is likely to leave the company (churn) using machine learning algorithms.

The project implements and compares three classification models to identify the most suitable model for customer churn prediction based on multiple evaluation metrics.

The objective is to help telecom companies identify customers at risk of leaving and support data-driven customer retention strategies.

## 2. Dataset

**Dataset Name:** Telco Customer Churn

**Source:** Kaggle

**Dataset Link:** https://www.kaggle.com/datasets/blastchar/telco-customer-churn/data

The dataset contains customer information, including demographics, services, contract details, billing information, and churn status.

- Records: Approximately 7,043 customers
- Features: Customer demographics, account details, services, and billing
- Target Variable: `Churn`
- Problem Type: Binary Classification

### Target Variable

- `Yes`: Customer churned
- `No`: Customer did not churn

The target variable is encoded as:
- `Yes` = 1
- `No` = 0

## 3. Machine Learning Algorithms

Three machine learning algorithms are implemented and compared.

### 1. Logistic Regression

A supervised classification algorithm used as a baseline model. It estimates the probability of customer churn and provides a useful benchmark for more complex models.

### 2. Random Forest Classifier

An ensemble learning algorithm that combines multiple decision trees to capture complex relationships between customer characteristics and churn behavior.

### 3. HistGradientBoosting Classifier

A gradient boosting algorithm that builds decision trees sequentially to improve predictive performance by learning from previous trees.

## 4. Technologies and Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## 5. Project Workflow

1. Load the dataset.
2. Explore the data and examine missing values.
3. Remove duplicate records.
4. Convert `TotalCharges` into a numeric format.
5. Encode the target variable.
6. Separate numerical and categorical features.
7. Split the data into training and testing sets.
8. Impute missing values and preprocess features.
9. Train three machine learning models.
10. Evaluate each model using multiple performance metrics.
11. Compare model performance.
12. Visualize confusion matrices and ROC curves.
13. Analyze Random Forest feature importance.
14. Generate a sample customer churn prediction.

## 6. Model Evaluation Metrics

The following metrics are used to evaluate the models.

| Metric | Purpose |
|---|---|
| Accuracy | Measures overall classification correctness |
| Precision | Measures how many predicted churners actually churned |
| Recall | Measures how many actual churners were identified |
| F1-Score | Balances precision and recall |
| ROC-AUC | Measures the model's ability to distinguish between churn classes |
| Confusion Matrix | Shows correct and incorrect classifications |
| Training Time | Measures the time required to train each model |

ROC-AUC is used to rank the models in the final comparison. However, the best model for deployment should also consider recall, precision, business costs, and customer retention objectives.

## 7. Installation

Install the required Python libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## 8. How to Run the Project

1. Download the dataset from Kaggle.
2. Extract the CSV file.
3. Place the CSV file in the project directory.
4. Ensure the filename is:

   `WA_Fn-UseC_-Telco-Customer-Churn.csv`

5. Save the Python implementation as `churn_prediction.py`.
6. Run the script:

```bash
python churn_prediction.py
```

The script trains the models, prints evaluation metrics, generates visualizations, and saves the model comparison results.

## 9. Project Outputs

The script generates the following files:

- `model_comparison_results.csv` — Evaluation metrics for all models.
- `model_comparison.png` — Comparison of performance metrics.
- `confusion_matrices.png` — Confusion matrices for the three models.
- `roc_curves.png` — ROC curve comparison.
- `feature_importance.png` — Top 15 Random Forest features.

## 10. Expected Outcome

The project produces a comparative evaluation of three machine learning algorithms for predicting customer churn.

The final results help identify a model that offers a suitable balance between detecting customers at risk of leaving and minimizing incorrect predictions.

Actual performance scores depend on the dataset, preprocessing, model configuration, and test results. No specific accuracy or winning algorithm is assumed in advance.

## 11. Future Improvements

- Hyperparameter tuning using GridSearchCV or RandomizedSearchCV.
- Cross-validation for more reliable model comparisons.
- Threshold optimization based on customer retention costs.
- SHAP-based model explainability.
- Class imbalance analysis and resampling experiments.
- Deployment through a Streamlit web application.
- Saving the best-performing model for future predictions.

## 12. Conclusion

This project demonstrates an end-to-end machine learning workflow for telecommunications customer churn prediction, including data preprocessing, model training, evaluation, visualization, and feature importance analysis.

By comparing multiple algorithms using appropriate evaluation metrics, the project provides a foundation for developing data-driven customer retention solutions.

## Author

**Rapol Rahul Reddy**

Machine Learning | Data Analysis | Predictive Modeling
