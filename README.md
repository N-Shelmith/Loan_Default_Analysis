# Loan Default Prediction Project
## Overview

This project aims to build and evaluate machine learning models that can predict whether a borrower will default on a loan. This is important for financial institutions to minimize risk and make better lending decisions. Using supervised learning techniques like Logistic Regression, Random Forest, Decision Tree and Gradient Boosting, I analyzed borrower financial and demographic data to estimate default risk.

## Objective: 
To predict loan defaults using machine learning and reduce errors in loan approval.

## Dataset

**Source:** Kaggle (Loan Default dataset)

**Size:** 255,348 records × 18 features

**Key Variables:** Age, Income, Loan Amount, Credit Score, Interest Rate, DTI Ratio, Employment Duration etc.

## Methods

**Exploratory Data Analysis (EDA):** Trends, correlations and risk factor profiling

**Models Used:** Logistic Regression, Random Forest, Decision Tree, Gradient Boosting

**Evaluation Metrics:** Accuracy, ROC-AUC, Precision, Recall, Confusion Matrix

## Tools & Libraries

Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn

## Default Rate Insights
- **Lower** credit scores, **higher** DTI Ratio and **short** employment period are linked to **more defaults**.

- **Young** borrowers (18–30) default the most, while **older** groups show **lower risk**.

- Co-signers and longer work history **reduce default** rates.

- Loan purpose does not affect default as much, but business loans carry a **higher risk**.

- Loan term has **minimal effect** as the default rate is almost constant.

## Model Conclusion: 
After testing multiple classifiers, Logistic Regression and Gradient Boosting emerged as the strongest models.

**Logistic Regression**

Accuracy: 67.6%

ROC-AUC: 0.753

Precision: 22.0%

Recall: 69.9%

Insight: Best for catching defaulters. Has a higher recall hence fewer risky loans are missed, though at the cost of flagging many good customers.

**Gradient Boosting**

Accuracy: 88.7%

ROC-AUC: 0.757

Precision: 62.0%

Recall: 6.8%

Insight: Very precise but misses most defaulters. It is useful where false positives are costly, but not ideal as a standalone screening tool.

**Recommendation:**
Use Logistic Regression as the primary model when reducing default risk is the top priority and Gradient Boosting may be used in a secondary layer or when operational costs of false positives are a bigger concern.

## Key Insights

1. The strongest predictors of default are:
- Credit Score
- DTI Ratio
- Months Employed
- Age
- Co-signer status

2. These insights can help guide loan approval decisions and segment borrowers based on default risk.

3. Machine learning models can complement traditional risk scoring systems, providing faster and more nuanced borrower assessments.

4. The study highlights the balance between predictive performance and interpretability in financial modeling.
