<div align="center">
  <h1>📊 Assessing the Long-term Treatment Outcomes in HIV Patients</h1>
</div>

## 📁 Project Overview

- This project explores long-term HIV treatment outcomes by analyzing key clinical and demographic factors. We focus on understanding how adherence to antiretroviral therapy (ART), the presence of opportunistic infections, and changes in CD4 count and viral load are influenced by treatment regimens, patient demographics, and clinical stage.

- Using machine learning models and regression techniques, we predict treatment outcomes and clinical metrics, with an emphasis on improving accuracy through ensemble stacking. Our approach not only offers predictive insights but also contributes to optimizing HIV treatment strategies and patient care.

## 📌 Objectives

- 💊 What drives ART adherence and its impact on treatment outcomes?
- 🦠 What predicts the occurrence of opportunistic infections at the final clinical visit?
- 📉 What factors influence clinical markers like CD4 count and viral load?
- 🤖 How do different machine learning models compare in predicting HIV treatment outcomes?
- 🔧 How can ensemble techniques like stacking enhance predictive performance?

## 🧪 Dataset

- **Source:** [Kaggle - HIV Dataset](https://www.kaggle.com/datasets/iogbonna/quality-of-care-dataset-for-hiv-clients)
- **Size**: 27,289 rows × 46 columns
- **Variables include:** Demographics, ART regimens, adherence levels, opportunistic infections, CD4 count, viral load, clinical staging, and other relevant indicators.
- **Target Variables:**
  - **Classification:** `ArvAdherenceLatestLevel`, `OpportunisticInfectionLastVisit`
  - **Regression:** `MostRecentCD4`, `ViralLoad`

## 🛠️ Methods & Tools

- **Programming Language:** Python
- **Libraries:** `scikit-learn`, `pandas`, `numpy`, `matplotlib`, `seaborn`
- **Validation:** 10-Fold Cross Validation for model robustness
- **Train-Test Split:** 80/20 split for all models

## 🤖 Machine Learning Models Used

### 🔍 Classification Models:
- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier ✅ **Best performer for classification**
- Gradient Boosting Classifier

### 📈 Regression Models:
- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor ✅ **Strong performance**
- Stacking Regressor ✅ **Best overall results for regression**

## 🧠 Evaluation Metrics

### Classification Metrics:
- Accuracy
- Precision, Recall, F1 Score (Classification Report)
- Confusion Matrix
- AUC-ROC Curve
- Feature Importance

### Regression Metrics:
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- Mean Absolute Percentage Error (MAPE)
- R² Score

## ✅ Key Findings

- **Statistical Conclusion:** We rejected the null hypothesis, confirming a significant association between patient demographics, ART regimen types, clinical staging, and the progression of HIV (measured via viral load, CD4 suppression, and infection presence).
- **Best Classification Model:** **Random Forest Classifier** — Highest accuracy and AUC-ROC in predicting adherence and infection status.
- **Best Regression Models:** **Gradient Boosting and Linear Regression** — Best R² and lowest MAPE for CD4 and viral load prediction.
- **Stacking Regressor:** Outperformed individual models, providing the most accurate results for continuous outcomes.

## 🚀 Future Work & Improvements

- **Feature Engineering:** Investigate additional features like medication adherence history, lifestyle factors, or co-morbid conditions that could improve model accuracy and provide more comprehensive insights.

- **Temporal Data Analysis:** Incorporate longitudinal data to analyze how changes over time in clinical markers (e.g., CD4 count, viral load) influence treatment outcomes, providing a more dynamic prediction of patient health.

