
# Hospital Readmission Prediction – Diabetes Medication Focus

This project explores hospital readmission risk among diabetic patients, focusing on whether **changes in diabetes medication (e.g., insulin initiation or adjustment)** are predictive of readmission within 30 days.

---

## 📌 Objective

To test the hypothesis:

> **Patients whose diabetes medications were adjusted (especially insulin) during hospitalization are more likely to be readmitted within 30 days.**

---

## 🧠 Dataset

- **Source:** UCI Machine Learning Repository  
- **Title:** [Diabetes 130-US hospitals for years 1999–2008](https://archive.ics.uci.edu/ml/datasets/diabetes+130-us+hospitals+for+years+1999-2008)
- **Size:** ~100,000 patient encounters  
- **Format:** Structured tabular data (CSV)

---

## 🧪 Features of Interest

| Feature         | Description                                                   |
|----------------|---------------------------------------------------------------|
| `insulin`       | Insulin prescription pattern: `No`, `Up`, `Down`, `Steady`   |
| `change`        | Whether any diabetes medication was changed during visit      |
| `diabetesMed`   | Whether diabetes medication was prescribed                    |
| `readmitted`    | Readmission status: `<30`, `>30`, or `NO`                     |

A binary column (`readmitted_30`) was created to flag `<30` readmissions.

---

## 🔍 Analysis Steps

1. **Data Cleaning & Preprocessing**
   - Handle missing values, drop irrelevant columns
   - Encode categorical variables
   - Create `readmitted_30` target column

2. **Exploratory Data Analysis (EDA)**
   - Visualize readmission rates by `insulin`, `change`, and `diabetesMed`
   - Use bar plots and crosstabs

3. **Statistical Testing**
   - Chi-squared tests to assess significance of relationships

4. **Modeling**
   - Logistic Regression and Random Forest for baseline prediction
   - SHAP for feature importance (optional)

5. **Evaluation**
   - Accuracy, Precision, Recall, Confusion Matrix

---

## 📊 Key Findings

- Readmission was more common among patients who had medication changes.
- Insulin adjustments (especially `Up`) were associated with higher readmission risk.
- These features were moderately predictive in logistic models.

---

## 🚀 Future Work

- Include comorbidities and lab results as additional predictors
- Use more advanced models (XGBoost, LightGBM)
- Analyze temporal trends in readmission behavior

---

## 📁 Folder Structure

```
Project_3_Readmission_Prediction/
│
├── notebook/
│   └── analysis.ipynb
├── data/
│   └── diabetes.csv (cleaned)
├── README.md
```

---

## 📚 References

- [UCI Dataset Info](https://archive.ics.uci.edu/ml/datasets/diabetes+130-us+hospitals+for+years+1999-2008)
- Strack et al., *Medical Data Mining*, 2014.
