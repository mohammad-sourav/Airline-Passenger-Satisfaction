# What Drives Airline Passenger Satisfaction? A Data-Driven Analysis of Service Quality and Customer Experience

---

## Executive Summary

This project investigates the primary determinants of airline passenger satisfaction through a rigorous, data-driven machine learning framework. Utilizing a comprehensive dataset of flight operations and service attributes, multiple classification algorithms including Logistic Regression, Random Forest, and XGBoost were trained, evaluated, and compared. The XGBoost classifier emerged as the optimal champion model, achieving an exceptional prediction accuracy of 95.7 percent and a receiver operating characteristic area under the curve score of 0.993. Key feature importance analyses reveal that experiential factors, specifically in-flight entertainment and seat comfort, exert a substantially higher psychological weight on consumer sentiment than traditional operational metrics such as flight delays. Ultimately, these empirical insights indicate that airline management must strategically pivot from basic operational punctuality toward targeted, experience-driven resource allocation to optimize customer satisfaction and long-term retention.

---

## Project Structure

```text
Airline-Passenger-Satisfaction/
│
├── data/
│   ├── raw/
│   │   └── Dataset.csv
│   └── processed/
│       ├── cleaned_dataset.csv
│       └── processed_satisfaction_data.csv
│
├── notebooks/
│   ├── 01_data_cleaning_eda.ipynb
│   ├── 02_hypothesis_testing_feature_engineering.ipynb
│   └── 03_model_training_evaluation.ipynb
│
├── models/
│   ├── best_airline_satisfaction_model.pkl
│   └── scaler.pkl
│
├── visualizations/
│   ├── age_distribution.png
│   ├── arrival_delay_vs_satisfaction_impact.png
│   ├── flight_distance_distribution.png
│   ├── passenger_satisfaction_by_class.png
│   ├── satisfaction_by_class.png
│   ├── satisfaction_distribution.png
│   └── top_10_feature_importance_xgboost.png
│
├── .gitignore
├── requirements.txt
└── README.md
```

---

## Key Methodologies & Model Performance

- **Data Preprocessing & Feature Engineering:** Comprehensive missing value imputation, categorical encoding, hypothesis testing, and standard scaling (`StandardScaler`) implemented via rigorous data pipelines.
- **Algorithm Comparison:** Evaluated Logistic Regression (baseline linear model), Random Forest (non-linear ensemble), and XGBoost (gradient boosting champion).

### Champion Model Metrics (XGBoost)

| Evaluation Metric | Performance |
|:---|:---:|
| Accuracy | 95.7% |
| Precision | 97.0% |
| Recall | 95.0% |
| F1-Score | 0.96 |
| ROC-AUC Score | 0.993 |

---

## Key Findings & Empirical Insights

1. **Experiential Dominance:** In-flight entertainment commands approximately 39.8% of predictive importance, establishing it as the single most critical driver of passenger sentiment.
2. **Physical Ergonomics:** Seat comfort serves as the secondary core pillar governing positive customer reviews.
3. **Operational vs. Experiential Weight:** Experiential service attributes significantly outweigh basic flight delay and scheduling metrics in determining overall passenger satisfaction.

---

## Installation & Setup

To run this project locally, clone the repository and install the required dependencies:

```bash
git clone https://github.com/mohammad-sourav/Airline-Passenger-Satisfaction.git

cd Airline-Passenger-Satisfaction

pip install -r requirements.txt
```

---

## 👤 Author

**Mohammad Sourav**

*Interdisciplinary Researcher | Consumer Psychology, Artificial Intelligence & Data Science*
