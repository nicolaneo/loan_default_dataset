# Long-term fairness in predicting default for loan applications.
Evaluating long-term fairness in mortgage applications when predicting default.

The "year_approved_only.csv" files contain US mortgage applications which were approved per year by Freddie Mac and were able to be matched with applicant data (race, age, gender, etc.) from HMDA and the loan performance data, including whether the applicant defaulted on their loan, and when. 
The year indicates the year the loan was originated (when the mortgage was approved and granted). 

We have added binary indicators for whether the applicant defaulted on their mortgage (failed to pay 3 or more consecutive mortgage payments) in the first six months or year of their mortgage. \
Percentage of approved mortgage applicants who defaulted, 2020: 1.7%, 2021: 1.4%, 2022: 1.7%

Data features:
- 'credit_score': applicant credit score at application stage
- 'first_payment_date': agreed date of first mortgage payment
- 'total_units': number of units on the property for the mortgage
- 'occupancy_type': P - Principal residence, S - Second residence, I - Investment property
- 'debt_to_income_ratio': applicants debt to income ratio
- 'loan_amount': amount of mortgage loan
- 'interest_rate': original interest rate
- 'postal_code': postcode of property for mortgage
- 'loan_purpose': P - home purchase, R - refinancing, C - cash-out refinancing
- 'loan_term': original agreed total loan period
- 'defaulted': binary indicator for defaulting any time before the end of 2022
- 'default_month': month of default if appropriate
- 'loan_to_value_ratio': original loan to value ratio
- 'income': applicant income
- 'applicant_race'
- 'applicant_sex',
- 'applicant_age',
- 'hmda_index': a label used for hmda files
- 'defaulted_in_six_months': binary indicator of defaulting in six months
- 'defaulted_in_one_year': binary indicator of defaulting in one year
- 'six_month_interval_label': a label to associate the morgage start time with a six month interval

## Sensitive attributes
Race: White, Hispanic/Latino, Black/African American, Asian, Native, Pacific Islanders.\
Sex of principal applicant: male, female \
Age
