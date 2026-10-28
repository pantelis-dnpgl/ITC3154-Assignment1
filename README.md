# ITC 3154 – Cognitive Computing | Assignment 1 (Fall 2026)

Exploratory data analysis of the **Loan Approval dataset**: which features drive `loan_status` (Approved / Rejected)?

**Student:** Pantelis Donoupoglou (290785) · **Instructor:** Dr. Dimitris Grigoriadis 

## Contents
| File | Description |
|---|---|
| `ITC3154_Assignment1_Loan_EDA.ipynb` | Executed notebook – all code, outputs and comments (Tasks 1–5) |
| `loan_approval_dataset.csv` | Dataset from Blackboard (semicolon-separated) |
| `figures/` | Plots used in the report |
| `requirements.txt` | Python dependencies |

## How to run
```bash
pip install -r requirements.txt
jupyter notebook ITC3154_Assignment1_Loan_EDA.ipynb
```
Or open the notebook in Google Colab, upload `loan_approval_dataset.csv`, and run all cells.

## Key findings
- `cibil_score` dominates the decision (r = +0.77); a cut-off at 550 alone reproduces 95.4% of the outcomes.
- `loan_term` has a weak negative effect (r = −0.11); 2–4 year loans are approved ~80% of the time.
- Income, loan amount, assets and dependents have no measurable effect, although they are highly inter-correlated.
- `education` and `self_employed` are independent of loan status (Chi-square p = 0.77 and 1.00).
