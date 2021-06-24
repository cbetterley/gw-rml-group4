# Using This Repo

*This section to be deleted before submitting model card!*

To make any changes to this repo:

1. Before you start working, pull the latest code from the `main` branch and create your own branch.

```
cd gw-rml-group4
git checkout main
git pull
git checkout -b new-branch-name
```

2. Commit and push your edits.

```
git status
git add .  # this adds everything.  add individual files instead, if needed
git commit -m "tuned XGB parameters"
git push origin new-branch-name
```

3. Make a pull request. A pull request is how we apply your changes to the main branch.

    - When you `git push`, your terminal will give you a link to create the pull request on GitHub.

    - Make sure the target branch is `main`.

    - Add Chip as a reviewer to the pull request.

    - Hit Create Pull Request.

4. Ask Chip to review & merge.


---

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

- x

- x

- x


## Evaluation Data

- x

- x

- x


## Model Details

- x

- x

- x


## Quantitative Analysis

- x

- x

- x


## Ethical Considerations

- x

- x

- x
