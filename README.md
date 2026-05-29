# Customer Churn Prediction

Machine learning project for predicting telecom customer churn using classification models and customer behavior data.

## Project Overview

Customer churn is one of the most important business problems for subscription-based companies. This project aims to identify customers who are likely to leave a telecom service provider so that retention strategies can be applied proactively.

The project includes:

- Data cleaning and preprocessing
- Exploratory Data Analysis (EDA)
- Class imbalance handling with SMOTE
- Model training and comparison
- Performance evaluation
- Business insights extraction

## Dataset

**Source:** [Telco Customer Churn Dataset on Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

**Records:** 7,043 customers  
**Target Variable:** `Churn`

Features include:

- Customer demographics
- Account information
- Contract details
- Payment methods
- Internet services
- Monthly and total charges

## Machine Learning Pipeline

1. Data Cleaning
2. Exploratory Data Analysis
3. Feature Encoding
4. Feature Scaling
5. SMOTE Oversampling
6. Model Training
7. Model Evaluation
8. Final Model Selection

## Models Evaluated

| Model | Evaluated |
|---------|---------|
| Logistic Regression | ✓ |
| Random Forest | ✓ |
| XGBoost | ✓ |
| K-Nearest Neighbors | ✓ |
| Naive Bayes | ✓ |

## Final Model Performance

**Selected Model:** Logistic Regression

| Metric | Score |
|----------|---------:|
| Accuracy | 0.750 |
| Precision | 0.520 |
| Recall | 0.775 |
| F1 Score | 0.622 |
| ROC-AUC | 0.857 |

The model achieved strong recall while maintaining good overall discrimination performance, making it suitable for identifying customers at risk of churn.

## Key Business Insights

Higher churn likelihood was associated with:

- Fiber optic internet service
- Electronic check payment method
- Paperless billing
- Higher monthly charges

Lower churn likelihood was associated with:

- Longer customer tenure
- One-year and two-year contracts
- Online security services
- Technical support services

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Imbalanced-learn (SMOTE)
- Matplotlib
- Seaborn
- Jupyter Notebook

## Repository Structure

```text
customer-churn-prediction/
│
├── data/
│   └── data.csv
│
├── notebooks/
│   └── customer_churn_prediction.ipynb
│
├── README.md
├── requirements.txt
└── .gitignore
```

## Installation

```bash
git clone https://github.com/YOUR_USERNAME/customer-churn-prediction.git

cd customer-churn-prediction

pip install -r requirements.txt
```

## Run

```bash
jupyter notebook notebooks/customer_churn_prediction.ipynb
```

## Author

**Aram Atoyan**
