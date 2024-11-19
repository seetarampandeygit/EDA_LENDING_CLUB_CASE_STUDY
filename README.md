# Lending Club Case Study
> This exploratory data analysis study seeks to explore how consumer characteristics and loan features affect the likelihood of loan default.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Dataset Reading](#dataset-reading)
* [Data Cleaning](#data-cleaning)
* [Data_Filtering](#data-filtering)
* [Data Standardization](#data-standardization)
* [Univariate Analysis](#univariate-analysis)
* [Bivariate Analysis](#bivariate-analysis)
* [Derived Metrics](#derived-metrics)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- This exploratory data analysis study was conducted with two participants.
  
- When the company gets a loan application, it must evaluate whether to approve the loan based on the applicant's profile. There are two categories of risks related to the bank's decision:
- 1. If the applicant is deemed likely to repay the loan, not granting the loan could result in a loss of business for the company.
- 2. If the applicant is considered unlikely to repay the loan, meaning they may default, then approving the loan could lead to a financial loss for the company.
   
- The aim of this research is to investigate how the characteristics of consumers and the specifics of loans affect the likelihood of defaulting on a loan.
  
- We utilized the dataset referred to as 'Loan Data Set'. It includes comprehensive loan information for all loans granted from 2007 to 2011.


## Technologies Used
- numpy - version 1.26.4
- matplotlib - version 3.8.4
- seaborn - version 0.13.2
- pandas - version 2.2.2

## Dataset Reading
- Headers and Top-5 rows
- Shape
- Index Range and Column's datatype

## Data Cleaning
- Null values processing

## Data Filtering
- Data Duplicacy Check
- Segragating and Analysing variable type (Categorical, Numerical)

## Data Standardization
- Converting variables 'int-rate' and 'revol_util' to numeric

## Univariate Analysis
### Numerical Variables
- Loan Amount Distribution
- Interest Rates
- Revolving Utilities
- Installments
### Categorical Variables
- Unique Member Check
- Loan Term
- Customer Grade
- Employment Length
- Verification Status
- Loan Purpose
- Home Ownership

## Bivariate Analysis
- Loan Term Vs Loan Status
- Grade vs Loan_status
- Subgrade Vs Loan_Status
- Purpose vs Loan_Status
- Employment Length Vs Loan_Status
- House Ownership Vs Loan Status

## Derived Metrics
- emp_len&Term vs loan status
- purpose&emp_len vs loan status
- credit_enquiry vs loan status
- public_record vs loan status
- bankruptcy vs loan status
- delinq_record vs loan status
- perc_util vs loan status
- interest vs loan status
- dti_buck vs loan status

## Conclusions
- Loan Term: The organization offers a 36-month loan repayment period for approximately 78% of its clients. However, customers with a 60-month loan repayment term are generally more prone to default. This was further confirmed when analyzed alongside the length of employment. Regardless of how long a customer has been employed, those with a 60-month tenure have a greater likelihood of defaulting. Therefore company should have a stringent policy to minimize lending for 60 months tenure.

- Customer Grade: Most customers fall into grades A or B. However, those in grades G, F, and E have a higher probability of defaulting. Therefore, the company should refrain from extending loans to customers in grades G, F, and E.

- Purpose of Loan: The company should be wary or exercise additional caution when providing loans for small business ventures or renewable energy projects, as these are more prone to default. This was further confirmed when analyzed in conjunction with the length of employment.

- Customer Collateral: It is noted that individuals whose home ownership status is labeled as unknown (other) tend to have a higher likelihood of default. The company should make sure to obtain appropriate collateral guarantees before providing loans.

- Credit History: The company needs to exercise extreme caution when lending to customers who have any credit inquiries within the past six months, those with any public record entries, or individuals with a history of bankruptcy.

- Customer Behaviour: The company should also make sure to review the delinquency history of a customer for at least two years before issuing loans. The analysis indicated that individuals with any delinquency history are more likely to default.

- Customer Financial Situation: The organization needs to thoroughly evaluate the Debt-to-Income (DTI) ratio before making decisions on loan approvals or setting interest rates. The interest rates should not be excessively high. It has been noted that as both the DTI and interest rates rise, the likelihood of default also escalates.

- Customer Credit Limit: Customers who make greater use of credit lines are at a higher risk of default. Consequently, the company should focus on this significant variable as well.

- Institution Research: The lending institution has failed to consider crucial factors before granting loans. It appears that there is almost no correlation between aspects such as bankruptcy records and loan amounts, debt-to-income ratios and loan amounts, delinquency records and loan amounts, and so forth.

- Institution Loss: Typically, around 14% to 15% of members default, which is quite significant.


## Acknowledgements

- This project was inspired by ML-AI couse at UpGrad and IIIT-B
- References: UpGrad and IIIT-B
- This project was based on [Exploratory Data Analysis]([https://learn.upgrad.com/course/5811/segment/53276/316330/957989/4783435]).


## Contact
Created by [@seetarampandeygit] - feel free to contact me!
