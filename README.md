# Lending Club Case Study
> Case Study on exploring the lending club dataset and suggesting feedback to the client to minimize loan defaults.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
Case study for a consumer finance company **Lending Club** which specializes in lending various types of loans to urban customers. This company is the largest online loan marketplace, facilitating personal loans, business loans, and financing of medical procedures. Borrowers can easily access lower interest rate loans through a fast online interface. When the company receives a loan application, the company has to **decide for loan approval based on the applicant’s profile.**
When a person applies for a loan, two types of decisions could be taken by the company:

**1. Loan accepted:** If the company approves the loan, there are 3 possible scenarios described below:

**Fully paid:** Applicant has fully paid the loan (the principal and the interest rate)

**Current:** Applicant is in the process of paying the installments, i.e. the tenure of the loan is not yet completed. These candidates are not labelled as 'defaulted'.

**Charged-off:** Applicant has not paid the installments in due time for a long period, i.e. he/she has defaulted on the loan

**2. Loan rejected:** The company had rejected the loan (because the candidate does not meet their requirements etc.). Since the loan was rejected, there is no transactional history of those applicants with the company and so this data is not available with the company (and thus in this dataset)

### Business Objectives:
Like most other lending companies, lending loans to ‘risky’ applicants is the largest source of financial loss (called credit loss). The credit loss is the amount of money lost by the lender when the borrower refuses to pay or runs away with the money owed. In other words, borrowers who default cause the largest amount of loss to the lenders.


The objective is to **identify the risky loan applicants at the time of loan application** so that such loans can be reduced thereby cutting down the amount of credit loss. Identification of such applicants using EDA is the aim of this case study.

In other words, **to understand the driving factors (or driver variables) behind loan default, i.e. the variables which are strong indicators of default.**  The company can utilize this knowledge for its portfolio and risk assessment. And thus minimize the risk of losing money while lending to customers.

### Dataset:
The dataset used has been uploaded in the repository.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- Customers with long-term loans tend to default more, the recommendation is to encourage shorter-term loans (36 months) as the interest
rates are also higher in long-term loans and customers fail to repay the loans.
- Higher LC Grade Loans have an impact on default rate as the interest rates also increase from grade A to grade G. Nearly 33% of all loans
in Grades F and G see a default. A recommendation is to prefer Grades A, B, C over D, E, F, G. This is a Loan Attribute influencing the tendency to
default.
- Purpose of the loan is also a strong indicator; the recommendation is to scrutinize more small business and renewable energy-related loans.
Weddings, cars, and big purchases remain safe bets. Also one can provide small business loans at lower interest rates to reduce defaults. This is
a consumer Attribute influencing the tendency to default.
- Loan amounts of 30% of annual income or higher see a high rate of default. As long as the loan amount is less than 20% of annual income,
defaults are low. This could be considered if other risk factors are higher to provide large loan amounts.
- Loan Default tendency driving variables are **Loan Purpose, Emp length, Grade, Interest rate, Annual Income, Term of Loan.**




## Technologies Used
- numpy - version 1.23.5
- pandas - version 1.5.3
- seaborn - version 0.12.2
- plotly - version 5.15.0


## Acknowledgements
- This project was inspired by the case study assigned as a group project from UpGrad. Thanks to Saksham Gupta for all the contributions. 

