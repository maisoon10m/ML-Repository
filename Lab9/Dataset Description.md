# Lending Club Loan Dataset – Overview

## Description
This dataset contains historical loan data from Lending Club (2007–2010). The goal is to analyze borrower characteristics and build a model to predict whether a loan will be fully paid or not.

## Objective
Predict whether a borrower will **fully repay a loan** (`not.fully.paid`).

---

## Dataset Information
- **Entries:** 9,578  
- **Features:** 14 columns  
- **Type:** Mixed (numerical + categorical)  
- **Target Variable:** `not.fully.paid`

---

## Features Description

| Column | Description |
|--------|------------|
| `credit.policy` | 1 if borrower meets LendingClub credit policy, 0 otherwise |
| `purpose` | Purpose of the loan (categorical) |
| `int.rate` | Interest rate of the loan |
| `installment` | Monthly payment owed |
| `log.annual.inc` | Log of annual income |
| `dti` | Debt-to-income ratio |
| `fico` | FICO credit score |
| `days.with.cr.line` | Days with a credit line |
| `revol.bal` | Revolving balance |
| `revol.util` | Credit utilization rate |
| `inq.last.6mths` | Credit inquiries in last 6 months |
| `delinq.2yrs` | Past due payments (2 years) |
| `pub.rec` | Public derogatory records |
| `not.fully.paid` | Target (1 = not fully paid, 0 = fully paid) |

---

## Categorical Features
- `purpose`

Converted using:
```python
pd.get_dummies()
