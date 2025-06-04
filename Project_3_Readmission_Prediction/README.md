# 🏥 Hospital Readmission Prediction

This project predicts whether a patient will be readmitted to the hospital within 30 days using structured clinical data. Early identification of high-risk patients can help healthcare providers take proactive steps to improve outcomes and reduce costs.

## 📁 Project Structure

Project_3_Readmission_Prediction/
│
├── notebook/
│ └── analysis.ipynb # Main analysis notebook
├── data/ # Data files (optional)
├── models/ # Saved models (optional)
├── README.md


## 🧠 Objective

To build a machine learning model that can predict 30-day hospital readmissions using clinical and demographic data from the UCI Diabetes Readmission dataset.

## 📊 Dataset

- **Name**: Diabetes 130-US hospitals for years 1999–2008
- **Source**: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/diabetes+130-us+hospitals+for+years+1999-2008)
- **Size**: 100,000+ records, 50 features
- **Target**: `readmitted` (within 30 days, after 30 days, or never)

## 🔧 Key Techniques

- Data Cleaning & Preprocessing
- Feature Engineering
- Class Imbalance Handling (e.g., SMOTE)
- Model Training (Logistic Regression, Random Forest, XGBoost)
- Model Evaluation (ROC-AUC, Confusion Matrix, Precision/Recall)
- Explainability with SHAP

## 📈 Results

- **Best Model**: Random Forest (or your best-performing model)
- **Accuracy**: XX%
- **AUC-ROC**: XX%
- **Precision/Recall**: XX%

## 🖼️ Visualizations

- Correlation heatmaps
- Feature importance plots
- ROC and Precision-Recall curves
- SHAP summary plots for interpretability

## 🚀 How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/YOUR_USERNAME/healthcare-data-portfolio.git
   cd healthcare-data-portfolio/Project_3_Readmission_Prediction
