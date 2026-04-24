# Fraud Detection Analytics

## Overview
This project analyzes large-scale transactional data to identify fraudulent behavior using data analysis, feature engineering, and machine learning techniques.

---

## Problem Statement
Digital payment systems are vulnerable to fraud, leading to financial loss and operational risk.  
The objective of this project is to detect fraudulent transactions and understand underlying fraud patterns.

---

## Dataset
- Source: PaySim Fraud Detection Dataset  
- ~6.3 million transaction records  
- Due to size constraints, a sample dataset is included in this repository  

---

## Approach

### 1. Data Understanding & Cleaning
- Analyzed dataset structure, data types, and distributions  
- Validated data consistency and checked for anomalies  

### 2. Exploratory Data Analysis (EDA)
- Identified fraud distribution and class imbalance (~0.13%)  
- Discovered fraud concentration in **TRANSFER** and **CASH_OUT** transactions  
- Analyzed transaction amount and balance behavior  

### 3. Hypothesis Testing
- Conducted statistical testing to validate differences between fraud and non-fraud transactions  

### 4. Feature Engineering
- Created features based on:
  - Balance inconsistencies  
  - Transaction amount ratios  
  - High-value transaction indicators  

### 5. Model Building
- Built a **Random Forest Classifier**  
- Handled class imbalance using appropriate techniques  
- Evaluated using **precision and recall**

### 6. Threshold Optimization
- Analyzed prediction thresholds to balance:
  - Fraud detection (recall)  
  - False positives (precision)  

---

## Key Insights
- Fraud is concentrated in **TRANSFER** and **CASH_OUT** transactions  
- Fraudulent transactions involve **significantly higher amounts**  
- Fraud patterns show:
  - **Sharp decrease in sender balance**  
  - **Sudden increase in receiver balance**  
- Transaction amount and balance behavior are strong fraud indicators  

---

## Model Performance
- Achieved strong precision and recall for fraud detection  
- Threshold tuning demonstrated trade-offs between detection rate and false positives  

---

## Limitations
- Dataset is synthetic, leading to highly separable fraud patterns  
- Real-world fraud detection is more complex and requires advanced techniques  

---

## Future Improvements
- Build interactive dashboard for visualization  
- Deploy model using Streamlit  
- Incorporate real-time fraud detection pipeline  

---

## Repository Structure

```
fraud-detection-analytics/
│
├── fraud_detection.ipynb  
├── sample_data.csv  
└── README.md  
```

---

## Tools & Technologies
- Python (Pandas, NumPy, Scikit-learn)  
- Data Visualization (Matplotlib, Seaborn)  
- Machine Learning (Random Forest)  

---

## Author
Sutapa Banerjee
