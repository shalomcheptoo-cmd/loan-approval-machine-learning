# Machine Learning Model for Loan Approval

## FinTech Innovations — Data-Driven Loan Risk and Approval Analysis

### Project Overview

This project uses machine learning to support FinTech Innovations in improving its loan approval process.

The project follows the **CRISP-DM** process, covering:

* Business Understanding
* Data Understanding
* Data Preparation
* Modeling
* Evaluation and Conclusion

### Dataset

The dataset contains **20,000 loan applications and 35 columns** covering financial, demographic, employment, credit, and loan-related information.

The target variable is **LoanApproved**, which indicates whether a loan application was approved.

### Machine Learning Models

Three classification models were evaluated:

* Logistic Regression
* Decision Tree
* Random Forest

GridSearchCV with 5-fold cross-validation was used to tune the Random Forest model.

### Evaluation

The tuned Random Forest achieved the following results on the test set:

* Accuracy: **93.23%**
* Precision: **89.23%**
* Recall: **81.49%**
* F1-score: **85.18%**
* ROC-AUC: **97.81%**

The analysis also examined confusion matrix results, feature importance, business cost, and performance across applicant segments.

### Business Impact

The case assigns a cost of **$50,000** to approving a bad loan and **$8,000** to denying a creditworthy applicant.

Based on the test-set confusion matrix, the estimated cost was **$6.116 million** under these assumptions.

### Key Features

The Random Forest feature importance analysis identified several influential features, including:

* LoanToIncomeRatio
* TotalDebtToIncomeRatio
* MonthlyIncome
* AnnualIncome
* InterestRate

### Limitations

The dataset records historical loan approval decisions rather than actual loan defaults. Therefore, the model should not be interpreted as a direct prediction of whether a borrower will repay a loan.

Further testing with real repayment and default data would be needed before deployment.

### Files

* `finanicial_loan_risk.ipynb` — Complete analysis and machine learning project
* `Loan Approval Projetc Banner.png` — Project banner
