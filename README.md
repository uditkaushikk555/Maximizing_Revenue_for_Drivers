# Maximizing Revenue for Taxi Cab Drivers through Payment Type Analysis

## Overview
This project uses **data analysis and hypothesis testing** to identify how different payment methods (cash vs. card) impact taxi driver revenue.  
The study explores whether encouraging specific payment types can lead to higher earnings for drivers without hurting customer experience.

---

## Objective
To determine if there is a **significant difference in average fares** between customers who pay with **credit cards** and those who pay with **cash**, using Python-based statistical analysis.

---

## Problem Statement
In the fast-paced taxi industry, understanding revenue patterns is crucial for driver profitability and operational efficiency.  
This analysis aims to answer:  
> “Is there a relationship between total fare amount and payment type — and can drivers increase revenue by promoting certain payment methods?”

---

## Dataset
**Source:** NYC Yellow Taxi Trip Records (January 2020)

**Key Columns Used:**
- `passenger_count`
- `trip_distance`
- `fare_amount`
- `payment_type`
- `duration`

Unnecessary columns were dropped to focus on the relationship between fare amount and payment type.

---

## Technologies Used
- **Python**
- **Pandas** – Data cleaning & manipulation  
- **Matplotlib / Seaborn** – Data visualization  
- **Scipy / Statsmodels** – Statistical hypothesis testing  

---

## Data Cleaning & Preparation
- Removed missing and duplicate records  
- Filtered valid payment types (`1: Card`, `2: Cash`)  
- Excluded invalid values (negative distance, fare, duration)  
- Removed outliers using the **IQR (Interquartile Range)** method  
- Converted categorical codes to readable labels  

---

## Exploratory Data Analysis
- Distribution of fares and trip distances by payment type  
- Passenger count and payment preferences  
- Visualization of cash vs. card usage patterns  
- Boxplots, histograms, and pie charts for insights  

---

## Hypothesis Testing

**Null Hypothesis (H₀):**  
There is **no significant difference** in average fare between card and cash payments.  

**Alternative Hypothesis (H₁):**  
There **is** a significant difference in average fare between card and cash payments.  

- Normality checked via **QQ Plot**  
- Conducted **Independent T-Test** (unequal variances)

**Result:**  
  *P-value < 0.05 → Reject Null Hypothesis*  
There is a statistically significant difference between the two payment types.

---

## Key Insights
- **Card payments** generally result in **higher average fares** than cash payments.  
- Encouraging passengers to use **credit/debit cards** can **increase driver revenue**.  
- Most passengers travel solo or in pairs; larger groups are rare.

---

## Business Implication
Taxi companies and ride-hailing services can implement **incentives or digital nudges** to promote card payments, improving both driver earnings and transaction transparency.

---
## Repository Structure
- README.md  
- taxi_payment_analysis.ipynb   # Colab notebook  
- yellow_tripdata_2020-01.csv   # Dataset (or link to source)  
- visuals/                      # Optional folder for charts
  
---

## Author
**Udit Kaushik**  
uditkaushikk555@gmail.com  
[LinkedIn](https://www.linkedin.com/in/udit-kaushik-883341377)  



