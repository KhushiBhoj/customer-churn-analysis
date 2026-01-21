# End-to-End Customer Churn Analysis

This project analyzes customer churn for a telecommunications company using the IBM Telco Customer Churn dataset. The goal is to identify **why customers churn, who is at risk, and what business actions can reduce churn**, combining predictive modeling with clear, decision-oriented insights.

---

## 📊 Dataset

**IBM Telco Customer Churn Dataset**  
Source: Kaggle  
Link: https://www.kaggle.com/datasets/blastchar/telco-customer-churn  

The dataset contains ~7,000 customers with information on:
- Demographics
- Contract details
- Services subscribed
- Billing and payment behavior
- Churn outcome (Yes / No)

---

## 🎯 Business Problem

Customer churn directly impacts revenue and increases customer acquisition costs.  
This project aims to:

- Predict which customers are likely to churn
- Understand the key drivers behind churn
- Segment customers by churn risk
- Translate model outputs into **actionable retention strategies**

---

## 🧠 Project Approach

### 1. Project Framing
- Defined churn as a binary classification problem
- Prioritized **recall on churners** over raw accuracy
- Emphasized **interpretability** for stakeholder trust

---

### 2. Data Audit & Cleaning
- Checked missing values, duplicates, and data types
- Validated churn imbalance
- Converted categorical variables into model-ready formats

---

### 3. Targeted EDA
Focused on **high-signal analysis**, not exhaustive plots:
- Churn by contract type and tenure
- Monthly charges vs churn
- Service adoption patterns
- Revenue exposure from churners

---

### 4. Feature Engineering
Created features aligned with business intuition:
- Early-tenure indicator
- Aggregated service counts
- Contract and payment behavior flags
- Normalized charges (`charges_vs_avg`)

---

### 5. Modeling
Models explored:
- Logistic Regression (baseline, interpretable)
- Decision Tree
- **Random Forest (final model)**

Key evaluation metrics:
- Recall (primary)
- Precision tradeoff
- ROC-AUC

---

### 6. Model Performance (Random Forest)

- **ROC-AUC:** ~0.84  
- Strong recall for churners
- Stable precision–recall tradeoff
- Balanced performance across customer segments

---

### 7. Risk Segmentation
Customers were grouped into:
- **High Risk**
- **Medium Risk**
- **Low Risk**

This enables targeted retention actions instead of blanket campaigns.

---

### 8. Business Recommendations
Insights were converted into concrete actions:
- Retention offers for early-tenure, month-to-month users
- Bundling strategies for service-light customers
- Payment method optimizations for high-risk segments

---

## 📌 Deliverables

- End-to-end Jupyter notebook
- Saved production-ready model
- Stakeholder-friendly written report
- Model summary and feature importance
- Risk segmentation and action plan

All documentation is designed to be **readable by non-technical stakeholders** while remaining technically rigorous.

---

## 🧾 Credits

Dataset provided by **BlastChar** on Kaggle:  
https://www.kaggle.com/datasets/blastchar/telco-customer-churn  

This project is for educational and portfolio purposes.

---

## 🚀 Why This Project Matters

This project demonstrates:
- Business-first problem framing
- Thoughtful metric selection
- Controlled EDA
- Interpretable machine learning
- Clear translation from model output → business decision

---
