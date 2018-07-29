# The problem
A company wants to automate the loan eligibility process (real time) based on customer detail provided while filling online application form. These details are Gender, Marital Status, Education, Number of Dependents, Income, Loan Amount, Credit History and others. To automate this process, they have given a problem to identify the customers segments, those are eligible for loan amount so that they can specifically target these customers.

# Data
The training set can be found [here](./data/train.csv)  
The test set to validate your model can be found [here](./data/test.csv)
| Variable | Description|
|----------|------------|
| Loan_ID  | Unique Loan ID |
| Gender   | Male / Female |
| Married  | Applicant married (Y/N) |
| Dependents | Number of dependents |
| Education | Applicant Education (Graduate/ Under Graduate) |
| Self_Employed | Self employed (Y/N) |
| ApplicantIncome | Applicant income |
| CoapplicantIncome | Coapplicant income |
| LoanAmount | Loan amount in thousands |
| Loan_Amount_Term | Term of loan in months |
| Credit_History | Credit history meets guidelines |
| Property_Area | Urban / Semi Urban / Rural |
| Loan_Status | Loan approved (Y/N) |