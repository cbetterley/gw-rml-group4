<div align="center">

# Predicting High Mortgage Rates Using Explainable Boosted Machines

Chip B., Charlotte G., Chengkai J., Abenezer T.

2021-06-26

</div>


## Intended Use

This model was developed to predict whether a borrower has been charged a high interest rate for a home mortgage.  "High" is defined as any APR that is at least 1.5 percentage points above a survey-based estimate for similar mortgages.  

**Primary Use:**  The primary purpose of this model is to aid lenders in validating lending decisions, from the perspectives of both fairness and also default risk.  For example:  

- If a lender's systems finds that a non-high interest rate is appropriate but the model predicts a borrower would receive a high interest rate, a lending specialist can intervene by evaluating if any default risks have been missed, and potentially override the original APR with something higher.  This creates business value by collecting more annual interest from high-risk borrowers to offset the risk of default.  

- In the opposite case where the model predicts non-high APR, then a lending specialist can intervene to assess whether the APR should be reduced.  This creates business value for the lender by protecting them from discrimination lawsuits, and also by increasing conversion among borrowers who might walk away from higher interest rates.  

**Other Uses:**  Outside auditors could use this model to assess a lender's practices for discrimination by examining cases where the model predicts non-high APR for borrowers that received a high APR from the lender.  

**Not In Scope:**  The model does not output interest rates.  It cannot be used directly by lenders to set a borrower's interest rate.  



## Training Data

**Source of training data:** https://github.com/jphall663/GWU_rml/tree/master/assignments/data

**Data split:** 70% of the training data are used for training and 30% of the training data are used for validation.

**General view:** There are 112253 rows and 23 columns in training data and 48085 rows and 23 columns in validation data.

**Column meanings:** 

- high priced: Binary target, whether (1) or not (0) the annual percentage rate (APR) charged for a mortgage is 150 basis points (1.5%) or more above a survey-based estimate of similar mortgages. 

- conforming: Binary numeric input, whether the mortgage conforms to normal standards (1), or whether the loan is different (0), e.g., jumbo, HELOC, reverse mortgage, etc.

- debt to income ratio std: Numeric input, standardized debt-to-income ratio for mortgage applicants.

- debt to income ratio missing: Binary numeric input, missing marker (1) for debt to income ratio std.

- income std: Numeric input, standardized income for mortgage applicants.

- loan amount std: Numeric input, standardized amount of the mortgage for applicants.

- intro rate period std: Numeric input, standardized introductory rate period for mortgage applicants.

- loan to value ratio std: Numeric input, ratio of the mortgage size to the value of the property for mortgage applicants.

- no intro rate period std: Binary numeric input, whether or not a mortgage does not include an introductory rate period.

- property value std: Numeric input, value of the mortgaged property.

- term 360: Binary numeric input, whether the mortgage is a standard 360 month mortgage (1) or a different
type of mortgage (0).



## Evaluation Data

**Source of evaluation data:** https://github.com/jphall663/GWU_rml/tree/master/assignments/data

**General view:** There are 19831 rows and 22 columns in evaluation data.

**Difference:** Evaluation data contains column ‘high_priced’ which is the binary target variable in the training data.


## Model Details

- This model was developed by master’s students at George Washington University to aid lenders in validating lending decisions, from the perspectives of both fairness and default risk.

- The model date is in June 2021 

- Explainable boosting machine.


## Quantitative Analysis

**metrics used:** We used AUC to evaluate our model and the best AUC is 0.8048 after we run through the stress testing, residual analysis, and remove the outlier.

- Assignment 1
<img width="726" alt="Screen Shot 2021-06-26 at 10 48 18" src="https://user-images.githubusercontent.com/31415735/123516944-af40be80-d66c-11eb-8c9a-40e2217268c5.png">

- Assignment 2
<img width="327" alt="Screen Shot 2021-06-26 at 10 54 42" src="https://user-images.githubusercontent.com/31415735/123517148-6b9a8480-d66d-11eb-8937-1aa3eb5f0d68.png">

- Assignment 3


## Ethical Considerations

- x

- x

- x
