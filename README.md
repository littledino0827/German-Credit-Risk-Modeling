German Credit Risk Modeling
===========================

PD Estimation & Cost-Sensitive Credit Decisions
-----------------------------------------------

Overview
--------

This project builds a credit risk classification model using the German Credit (Statlog) dataset to estimate Probability of Default (PD) and translate model outputs into practical credit approval decisions.

The focus is not only predictive performance, but also decision threshold selection under business cost trade-offs, reflecting real-world credit policy constraints.

Data
----

- 1,000 loan applicants with mixed numerical and categorical features  
- Target: Good vs. Bad credit outcome (bad rate ≈ 30%)  
- Data source: UCI German Credit dataset  

Approach
--------

- Logistic Regression with probability outputs (PD)  
- One-Hot Encoding for categorical variables  
- Model evaluation using Accuracy and ROC-AUC  
- Threshold analysis incorporating:
  - Approval rate  
  - Bad capture vs. false decline trade-offs  
  - Cost-sensitive decision rules  

Key Insight
-----------

Optimal credit decisions depend heavily on cost assumptions and approval-rate constraints.  
Accuracy-optimal thresholds differ meaningfully from business-optimal thresholds, even with the same model.

Tools
-----

Python · pandas · scikit-learn · Logistic Regression
