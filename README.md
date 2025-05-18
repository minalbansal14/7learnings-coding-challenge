# 7Learnings Snow Forecasting Challenge

This repository contains my solution to the data science coding challenge provided by **7Learnings**.  
The goal was to build a predictive model that can forecast whether it will snow tomorrow, using global historical weather data accessed via **Google BigQuery**.

---

## Contents

- `Coding_Challenge.ipynb`: Main solution notebook with all steps, analysis, and explanations
- `requirements.txt`: Python libraries needed to run the notebook
- `README.md`: Project summary and instructions

---

## Project Highlights

- **Data Extraction** Queried and filtered large-scale weather data directly using **BigQuery**
- **Data Preprocessing** Cleaned, engineered, and transformed features  
- **Imbalance Handling** Handled class imbalance with **RandomOverSampler** from `imblearn`
- **Model Training** Trained and evaluated a **Logistic Regression** model using a **time-based split**
- **Prediction at Target date** Predicted snowfall for a future date and validated predictions against actual labels
- Achieved strong generalization with an F1-score of ~0.53 and accuracy ~78% on the test set

---

## How to Run

1. Install dependencies:
```bash
pip install -r requirements.txt
```

2. Open the notebook:
```bash
jupyter notebook Coding_Challenge.ipynb
```

Google BigQuery credentials may be required for data access.

---

## Notes on BigQuery Access

If you wish to re-run the BigQuery queries:
- You may need a **Google Cloud account** (or use the [BigQuery Sandbox](https://cloud.google.com/bigquery/docs/sandbox))
- Make sure to authenticate using:

```python
%load_ext bigquery_magics
```
---

## Author

**Minal Bansal**  
Submitted for 7Learnings Data Science Coding Challenge

---
