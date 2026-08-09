## Customer Churn Prediction using Machine Learning

### Overview

This project predicts whether a telecom customer is likely to **churn** using ensemble machine-learning algorithms.

### Business Objective

Reduce customer attrition by identifying customers with high churn probability and understanding the factors influencing churn behavior.

### Dataset

* **Rows:** 7,032
* **Target:** `Churn`

### Technologies Used

* Python
* Pandas
* NumPy
* Seaborn
* Scikit-learn
* XGBoost

### Workflow

1. Data Cleaning
2. Missing Value Handling
3. Exploratory Data Analysis
4. Label Encoding
5. Train-Test Split
6. Model Training
7. Hyperparameter Tuning
8. Model Evaluation

### Models Implemented

* Decision Tree
* Random Forest
* AdaBoost
* XGBoost

### Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

### Key Insight

XGBoost achieved the best predictive performance among the evaluated models, while Random Forest provided strong interpretability and stable classification performance.

### How to Run

```bash
git clone https://github.com/your-username/customer-churn-prediction-ml.git
cd customer-churn-prediction-ml
pip install -r requirements.txt
jupyter notebook
```
