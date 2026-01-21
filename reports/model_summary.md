# Customer Churn Prediction: Model Summary

**Model Type:** Random Forest Classifier  
**Purpose:** Predict at-risk customers and guide retention actions.

---

## Hyperparameters
| Parameter | Value |
|-----------|-------|
| n_estimators | 500 |
| max_depth | 20 |
| min_samples_split | 20 |
| min_samples_leaf | 10 |
| max_features | 1.0 |
| class_weight | balanced |
| random_state | 42 |

---

## Performance (Test Set, Threshold=0.5)
| Metric | Churn=0 | Churn=1 | Weighted / Avg |
|--------|---------|---------|----------------|
| Precision | 0.89 | 0.54 | 0.79 |
| Recall    | 0.77 | 0.73 | 0.76 |
| F1-score  | 0.83 | 0.62 | 0.77 |
| Accuracy  | —     | —     | 0.76 |
| ROC-AUC   | —     | —     | 0.837 |

---

## Top 10 Features (Importance)
| Feature | Importance |
|---------|-----------|
| month_to_month | 0.4129 |
| charges_vs_avg | 0.2071 |
| tenure | 0.1345 |
| MonthlyCharges | 0.1021 |
| total_services | 0.0206 |
| paperless_billing | 0.0175 |
| FiberOptic | 0.0153 |
| OnlineSecurity | 0.0150 |
| two_year | 0.0117 |
| TechSupport | 0.0109 |

**Insights:**  
- Month-to-month contract, higher charges, and early tenure are the strongest predictors of churn.  
- Service adoption (total_services, TechSupport, OnlineSecurity) reduces churn risk.  
- Paperless billing and fiber optic internet have moderate influence.

---

## Notes
- Balanced class weights handle churn imbalance  
- Model identifies high-risk customers for targeted retention  
- Can be updated/retrained as new customer data arrives
