# Customer Churn Prediction using Machine Learning

## Project Overview

This project predicts whether a telecom customer is likely to **churn (leave the service)** using multiple machine-learning classification algorithms.

The objective is to help businesses identify **high-risk customers** and improve customer retention strategies through data-driven insights.

---

## Business Problem

Customer churn directly affects revenue, customer acquisition costs, and long-term profitability. By identifying customers who are likely to leave, companies can:

* Reduce revenue loss
* Improve customer retention campaigns
* Increase customer lifetime value
* Prioritize high-risk customer segments

---

## Dataset Information

* **Dataset:** Telco Customer Churn Dataset
* **Records:** 7,032 customer records
* **Features:** 20+ customer demographic and service-related attributes
* **Target Variable:** `Churn` (0 = No, 1 = Yes)

---

## Technologies Used

| Category                | Tools                 |
| ----------------------- | --------------------- |
| Programming             | Python                |
| Data Analysis           | Pandas, NumPy         |
| Visualization           | Matplotlib, Seaborn   |
| Machine Learning        | Scikit-learn, XGBoost |
| Development Environment | Jupyter Notebook      |

---

## Project Workflow

### 1. Data Cleaning

* Converted `TotalCharges` from object to numeric datatype
* Handled missing values and removed invalid records
* Verified column datatypes and data consistency

### 2. Exploratory Data Analysis (EDA)

* Churn distribution analysis
* Tenure vs churn relationship
* Monthly charges vs churn behavior
* Service-level customer behavior analysis

### 3. Feature Engineering

* Encoded categorical variables using **Label Encoding**
* Prepared feature matrix (`X`) and target variable (`y`)
* Split data into **training and testing sets**

---

## Machine Learning Models Implemented

### Decision Tree Classifier

* Baseline interpretable classification model

### Random Forest Classifier

* Ensemble bagging approach
* Improved stability and reduced overfitting
* **Hyperparameter tuning performed using GridSearchCV**

### AdaBoost Classifier

* Boosting-based ensemble model
* Enhanced classification performance compared to the baseline model

### XGBoost Classifier

* Gradient boosting implementation
* Evaluated for comparison with other ensemble methods

---

## Hyperparameter Tuning

Random Forest was optimized using **GridSearchCV** to improve predictive performance. Tuned parameters included:

* `n_estimators`
* `max_depth`
* `min_samples_split`
* `min_samples_leaf`

---

## Model Evaluation

The models were evaluated using:

* **Accuracy Score**
* **Precision**
* **Recall**
* **F1-Score**
* **Confusion Matrix**
* **Classification Report**

---

## Final Result

### Best Performing Model: **Tuned Random Forest**

Key observations from the experiment:

* **Random Forest achieved the highest accuracy** of 80.64% after hyperparameter tuning with GridSearchCV.
* **AdaBoost also produced competitive performance** and performed better than the baseline Decision Tree model with a accuracy score of 79.03%.
* **XGBoost did not outperform the tuned Random Forest** on this dataset and configuration and produced a accuracy of 77.61%.

This demonstrates that a well-tuned Random Forest can provide **strong predictive performance with simpler tuning complexity** for telecom customer churn prediction.

---

## Key Business Insights

* Customers with **shorter tenure** showed a higher probability of churn.
* Customers with **higher monthly charges** were more likely to leave the service.
* Certain **internet and support service combinations** were associated with increased churn risk.
* Retention efforts should focus on **new customers with high monthly billing and limited support engagement**.

---

## Repository Structure

```
customer-churn-prediction-ml/
│
├── data/
│   └── customer_churn.csv
│
├── notebooks/
│   └── customer_churn_prediction.ipynb
│
├── images/
│   ├── churn_distribution.png
│   ├── confusion_matrix.png
│   └── model_comparison.png
│
├── requirements.txt
└── README.md
```

---

## How to Run the Project

```bash
git clone https://github.com/ds-learner-akki/customer-churn-prediction-ml.git
cd customer-churn-prediction-ml
pip install -r requirements.txt
jupyter notebook
```

Open:

```
notebooks/customer_churn_prediction.ipynb
```

---

## Future Improvements

* Perform **cross-validation** for more robust evaluation
* Apply **SMOTE** for class imbalance handling
* Use **feature importance analysis** for interpretability
* Deploy the model using **Streamlit** or **Flask**
* Build a **real-time churn prediction dashboard** integrating Power BI insights


---

## Author

**Abhishek Singh Bisht**

QA Analyst (BFSI) | SQL | Power BI | Python | Aspiring Data Analyst

GitHub: https://github.com/ds-learner-akki
