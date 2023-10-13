# Project-Loan-Delinquency-Prediction-Model
This is an End to End project on how to build a Machine Learning model that helps to predict if the Borrower will end up becoming delinquent towards his loan repayment plan.

Loan Delinquency Prediction model
Loan delinquency refers to a situation where a borrower fails to make scheduled payments towards their loan obligations. This typically occurs when a borrower misses one or more payments and extends beyond the agreed-upon due date. A loan becomes delinquent when the borrower is unable to make the payment within a specified grace period.
About Dataset
XYZ Corporation is currently experiencing a period of adversity. Their Non-Performing Assets (NPAs) have seen a notable increase in recent times, with a significant portion stemming from loans extended to individual borrowers. To address this pressing issue, the bank's Chief Risk Officer has taken the initiative to establish a data-driven framework for the approval of loans to individual borrowers, with the aim of mitigating the risk of these loans transitioning into NPAs.

Link: https://www.kaggle.com/datasets/wajidsaleem/loan-delinquent

Features
ID:
Customer ID

Delinquent :
Indicates whether the customer is delinquent or not (1 => Yes, 0 => No)

Term:
Loan term in months

Gender:
The borrower's Gender (Male or Female).

Purpose:
Borrower's purpose of taking the loan.

Home_Ownership:
Home ownership status of the borrower

Age:
Age of the borrower.

FICO:
The Fico score of the customer (Credit score issued by the Bureau)

How can these factors potentially affect the loan delinquency?
Loan term: The length of the loan term can affect a borrower's ability to repay the loan. Longer loan terms may result in higher chances of delinquency, as borrowers have more time to encounter financial difficulties.

Gender: While gender should not be a factor in determining loan delinquency, some studies have shown that there may be statistically significant differences in delinquency rates between genders. However, it's important to note that these differences may be influenced by other factors like income, employment stability, or loan amount.

Purpose of loan: The purpose for which the borrower is taking the loan can have an impact on delinquency. For example, loans taken for education or medical expenses may have lower delinquency rates compared to loans taken for high-risk ventures like starting a business.

Home ownership status: Home ownership status can be an indicator of stability and financial responsibility. Homeowners may have lower delinquency rates compared to renters, as they have an asset and are more likely to have stable income.

Age: Age can be a factor in delinquency, as younger borrowers may have less financial stability and experience compared to older borrowers. However, it's important to assess age in conjunction with other factors like employment stability, income, and credit history.

FICO score: FICO score is a widely used credit scoring system that assesses a borrower's creditworthiness. Lower FICO scores indicate higher risk, and borrowers with lower scores may have higher delinquency rates. FICO score is considered one of the most important factors in predicting loan delinquency.

These factors are not exhaustive, and other variables like income, employment stability, debt-to-income ratio, and previous delinquency history may also be important in predicting loan delinquency. It's important to analyze and assess multiple factors together to get a comprehensive understanding of a borrower's risk profile.

The dataset can also be found within this repository.

Data Preprocessing is done by using label encoding, one hot encoding, imbalance data treatment by using Random Over Sampling technique.

Exploratory Data Analysis (EDA) has been performed to understand the distribution and behaviour of all the input features.

Concluding: Since the model is showing great performance in the ROC-AUC Curve, the model using Random Forest with Train accuracy of 83% and Test accuracy of 82% and 10 Fold Cross Validation mean Accuracy scores for training and test data is 82% and 81% respectively, Hence the model can be said to be performing very well and can be used for deployment in production.

Usage: The model can be trained as shown in the .ipynb file and relevant input variables can be given to predict the output by using the following example code: prediction = rfc.predict([[Loan_term, Gender, Age, Fico_score, Loan_purpose_House, Loan_purpose_Medical, Loan_purpose_Other, Loan_purpose_Personal, Loan_purpose_Wedding, Home_ownership_Own, Home_ownership_Rent]])

Outcome: Caution!!! The likelihood of the borrower being delinquent is very high.
                                          OR
          The likelihood of the borrower being delinquent is negligibly low.
