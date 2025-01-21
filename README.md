# BNP Paribas Fraud Detection Challenge  

## Description  

This repository contains the code and resources for the BNP Paribas Fraud Detection Challenge hosted by ENS. Our team achieved **1st place on the leaderboard as of 2024**, with a test PR-AUC score of **0.3507**, significantly outperforming the benchmarks. The challenge focuses on building models to predict fraudulent transactions based on detailed shopping basket data, emphasizing the detection of the minority fraud class.  

---

## Context  

**BNP Paribas Personal Finance**, a leader in consumer financing in Europe, actively develops methods to detect fraud, which is increasingly a pressing issue for financial institutions. Fraud detection is particularly challenging due to the low occurrence of fraud (approximately **1.4%** of observations) and the ingenuity of fraudsters who normalize their behaviors to evade detection systems.  

The objective of this challenge was to develop a model to detect fraudulent transactions based on basket data (content and characteristics of purchases). Successful fraud detection minimizes financial loss and improves customer experience while maintaining profitability.  

---

## Data Description  

The dataset consists of **147 features** describing customer purchase data across 115,988 observations.  

### Input Features (`X`):  
- **General Features**:  
  - `ID`: Unique transaction identifier.  
  - `Nb_of_items`: Number of unique items in the basket.  
- **Basket Details (up to 24 items)**:  
  - `item1`–`item24`: Product categories.  
  - `cash_price1`–`cash_price24`: Price of each item.  
  - `make1`–`make24`: Manufacturer of each item.  
  - `model1`–`model24`: Model of each item.  
  - `goods_code1`–`goods_code24`: Item codes.  
  - `Nbr_of_prod_purchas1`–`Nbr_of_prod_purchas24`: Quantity of products per item.  

### Target Variable (`Y`):  
- `fraud_flag`: Binary variable indicating whether a transaction was fraudulent (1) or not (0).  

### Class Distribution:  
- **Fraud (Y=1)**: ~1.4% of data (1,681 observations).  
- **Non-Fraud (Y=0)**: ~98.6% of data (114,307 observations).  

---

## Challenge Objective  

The task was to predict the likelihood of fraud for each transaction, focusing on optimizing the **Precision-Recall Area Under Curve (PR-AUC)** metric.  

This metric is particularly suitable for imbalanced datasets as it prioritizes performance on the minority class.  

---

## Approach  

### See detailled explanation on notebook   

---

## Results  

- **Final PR-AUC Score**: **0.3507** (1st place on the leaderboard).  
- **Benchmarks**:  
  - Benchmark 1 (Random Guessing): **0.017**.  
  - Benchmark 2 (Optimized ML Model): **0.14**.  

Our model significantly outperformed the benchmarks.  

---


