## Dataset Description

The **Credit Card Customer Dataset** (`CC_GENERAL.csv`) contains the credit card usage behavior of **8,950 customers** over a period of 6 months. Each row represents a single credit card holder, and the dataset includes **18 columns** that describe various behavioral and financial attributes.

The goal of this dataset is to help group similar customers together so that the company can better understand its customer base and design more effective marketing strategies.

### Features

| # | Column Name | Description |
|---|------------|-------------|
| 1 | `CUST_ID` | Unique identifier for each credit card holder |
| 2 | `BALANCE` | Remaining balance left in the customer's account to make purchases |
| 3 | `BALANCE_FREQUENCY` | How frequently the balance is updated (score between 0 and 1) |
| 4 | `PURCHASES` | Total amount of purchases made from the account |
| 5 | `ONEOFF_PURCHASES` | Maximum purchase amount done in one-go |
| 6 | `INSTALLMENTS_PURCHASES` | Total amount of purchases done in installments |
| 7 | `CASH_ADVANCE` | Total cash advance taken by the user |
| 8 | `PURCHASES_FREQUENCY` | How frequently purchases are being made (score between 0 and 1) |
| 9 | `ONEOFF_PURCHASES_FREQUENCY` | How frequently one-off purchases are being made (score between 0 and 1) |
| 10 | `PURCHASES_INSTALLMENTS_FREQUENCY` | How frequently purchases in installments are being made (score between 0 and 1) |
| 11 | `CASH_ADVANCE_FREQUENCY` | How frequently the cash in advance is being paid (score between 0 and 1) |
| 12 | `CASH_ADVANCE_TRX` | Number of transactions made with cash advance |
| 13 | `PURCHASES_TRX` | Number of purchase transactions made |
| 14 | `CREDIT_LIMIT` | Credit card limit for the user |
| 15 | `PAYMENTS` | Total amount of payments done by the user |
| 16 | `MINIMUM_PAYMENTS` | Minimum amount of payments made by the user |
| 17 | `PRC_FULL_PAYMENT` | Percent of full payment paid by the user |
| 18 | `TENURE` | Tenure of credit card service for the user (in months) |

### Dataset Summary

- **Number of rows:** 8,950 customers
- **Number of columns:** 18 features
- **Target variable:** None (this is an unsupervised learning problem)
- **Missing values:** Present in `MINIMUM_PAYMENTS` (313) and `CREDIT_LIMIT` (1)
- **Source:** [Kaggle — Credit Card Dataset for Clustering](https://www.kaggle.com/datasets/arjunbhasin2013/ccdata/data)
