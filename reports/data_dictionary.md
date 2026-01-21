# Customer Churn Dataset — Data Dictionary

| Column Name           | Data Type    | Description |
|-----------------------|-------------|-------------|
| customerID            | object      | Unique customer identifier |
| gender                | object      | Customer gender (Male/Female) |
| SeniorCitizen         | int64       | 1 if senior citizen, 0 otherwise |
| Partner               | object      | Yes/No — if customer has a partner |
| Dependents            | object      | Yes/No — if customer has dependents |
| tenure                | int64       | Number of months the customer has stayed with the company |
| PhoneService          | object      | Yes/No — if customer has phone service |
| MultipleLines         | object      | Yes/No/No phone — if customer has multiple lines |
| InternetService       | object      | DSL/Fiber optic/No — type of internet service |
| OnlineSecurity        | float64     | 1 if customer has online security, 0 if not, NaN if unknown |
| OnlineBackup          | float64     | 1 if customer has online backup, 0 if not, NaN if unknown |
| DeviceProtection      | float64     | 1 if customer has device protection, 0 if not, NaN if unknown |
| TechSupport           | float64     | 1 if customer has tech support, 0 if not, NaN if unknown |
| StreamingTV           | float64     | 1 if customer has streaming TV, 0 if not, NaN if unknown |
| StreamingMovies       | float64     | 1 if customer has streaming movies, 0 if not, NaN if unknown |
| PaperlessBilling      | int64       | 1 if customer has paperless billing, 0 otherwise |
| MonthlyCharges        | float64     | Monthly charges (USD) |
| TotalCharges          | float64     | Total charges to date (USD) |
| Churn                 | int64       | 1 if customer churned, 0 otherwise |
| tenure_bucket         | category    | Tenure binned into ranges (0–6, 6–12, 12–24, 24–48, 48+) |
| early_tenure          | int64       | 1 if tenure < 12 months, 0 otherwise |
| month_to_month        | bool        | True if contract is month-to-month |
| one_year              | bool        | True if contract is 1-year |
| two_year              | bool        | True if contract is 2-year |
| total_services        | float64     | Total number of add-on services subscribed |
| charges_vs_avg        | float64     | Ratio of MonthlyCharges to dataset average |
| FiberOptic            | int64       | 1 if customer has fiber optic internet, 0 otherwise |
| DSL                   | int64       | 1 if customer has DSL internet, 0 otherwise |
| NoInternet            | int64       | 1 if customer has no internet service, 0 otherwise |
| PaymentMethod_Credit card (automatic) | bool | Payment via automatic credit card |
| PaymentMethod_Electronic check | bool | Payment via electronic check |
| PaymentMethod_Mailed check | bool | Payment via mailed check |
