# Loan Default Prediction Using EDA

## Problem Statement

Loan providers often face challenges in granting loans to individuals with insufficient or non-existent credit history, leading to potential defaults. Suppose you work for a consumer finance company that specializes in lending various types of loans to urban customers. This project aims to use Exploratory Data Analysis (EDA) to analyze patterns in loan application data, ensuring that applicants capable of repaying the loan are not rejected.

When the company receives a loan application, it must decide whether to approve the loan based on the applicant’s profile. Two types of risks are associated with this decision:

1. **Business Loss**: If a potentially reliable applicant is rejected, the company loses a business opportunity.
2. **Financial Loss**: If a risky applicant is approved and defaults, the company incurs financial losses.

The dataset contains information about loan applications, including clients with payment difficulties and others who have paid on time. The four possible decisions regarding loan applications are:

- **Approved**: Loan application approved.
- **Cancelled**: Client canceled the application.
- **Refused**: Loan application rejected by the company.
- **Unused Offer**: Loan canceled by the client at different stages.

## Business Objectives

The objective is to identify patterns indicating whether a client might have difficulty paying installments. This analysis can inform actions such as denying loans, reducing loan amounts, or lending at higher interest rates. The ultimate goal is to ensure that consumers capable of repaying loans are not rejected. Understanding the driving factors behind loan defaults will help the company in portfolio and risk assessment.

## Data Insights

- **Customer Segmentation**:
  - Repeated customers outnumber new ones.
  - Female applicants outnumber males, but both genders show similar payment difficulties (~7% for females, ~10% for males).
  
- **Loan and Payment Trends**:
  - No significant difference in payment difficulties between those with or without car/house ownership (~8% difficulty).
  - Payment difficulties are similar for cash loans (8%) and revolving loans (5%).
  - Working-class customers face the highest payment difficulties, while pensioners and commercial associates are more timely with payments.

- **Demographic Factors**:
  - Singles and those not married face more payment difficulties.
  - Retired customers have the highest loan approval rates, followed by laborers.
  - Applicants with academic degrees and those aged 30-45 or 65-70 have higher approval rates.

- **Loan Characteristics**:
  - Customers with EMIs less than 15,000 receive more approvals, while those with EMIs between 15,000-30,000 face more refusals.
  - Loans with shorter repayment durations (<10 years) have higher approval rates.
  - Applicants requesting more than 160k in loans or those employed for less than 5 years face more refusals.

## Recommendations for the Company

**Target for Providing Loans**:
- Customers in occupations such as accountants, retirees, and students.
- Applicants with higher education or academic degrees.
- Customers employed for over 10 years.
- Reliable borrowers aged over 40.

**Avoid for Providing Loans**:
- Occupations like drivers and low-skill laborers.
- Customers with lower secondary education.
- Working-class and unemployed customers.
- Customers employed for less than 10 years.
- Applicants under the age of 30.

## Data Understanding

Download the dataset from the link below:

[Download Dataset](https://drive.google.com/drive/folders/1vebQ4_NZe3xiZCgZbNCr4t-F4ugTBtoD?usp=drive_link)

This dataset contains three files:

1. **application_data.csv**: Contains client information at the time of application, including whether the client has payment difficulties.
2. **previous_application.csv**: Contains information about the client’s previous loan applications (Approved, Cancelled, Refused, or Unused offers).
3. **columns_description.csv**: A data dictionary describing the meaning of the variables.
