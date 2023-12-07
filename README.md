# Long-term fairness in predicting default for loan applications.
Evaluating long-term fairness in mortgage applications when predicting default.

The "year_approved_only.csv" files contain US mortgage applications which were approved per year by Freddie Mac and were able to be matched with applicant data (race, age, gender, etc.) from HMDA and the loan performance data, including whether the applicant defaulted on their loan, and when. 

We have added binary indicators for whether the applicant defaulted on their mortgage (failed to pay 3 or more consecutive mortgage payments) in the first six months or year of their mortgage.

Data features:
['credit_score', 'first_payment_date', 'total_units', 'occupancy_type',
       'debt_to_income_ratio', 'loan_amount', 'interest_rate', 'postal_code',
       'loan_purpose', 'loan_term', 'defaulted', 'default_month',
       'loan_to_value_ratio', 'income', 'applicant_race', 'applicant_sex',
       'applicant_age', 'hmda_index', 'defaulted_in_six_months',
       'defaulted_in_one_year', 'six_month_interval_label']

## Sensitive attributes
Race: White, Hispanic/Latino, Black/African American, Asian, Native, Pacific Islanders. \\
Sex of principal applicant: male, female \\
Age
