# Predicting High-Cost Patients in Healthcare Using Predictive Analytics  

## 📌 Overview  
This repository contains my **Master’s Thesis (May 2025)** on predicting **high-cost patients in healthcare** using predictive analytics.  
High-cost patients, though a small fraction of the population, account for a disproportionately high share of healthcare expenditure.  
Accurately identifying such patients can help hospitals, insurers, and policymakers design **targeted interventions**, reduce costs, and improve patient outcomes.  

The study applies **XGBoost regression and classification models** on the **SPARCS (New York State) dataset** and uses **SHAP explainability** to interpret model results.  

---

## 🎯 Research Objectives  
- Build predictive models for identifying high-cost patients using inpatient healthcare data.  
- Apply **XGBoost regression** to predict patient costs.  
- Apply **XGBoost classification** to identify patients likely to fall into high-cost categories.  
- Use **SHAP values** to explain model predictions and highlight cost drivers.  
- Evaluate regression vs. classification approaches for accuracy and interpretability.  

---

## 📂 Dataset  
- **Source**: SPARCS – Statewide Planning and Research Cooperative System (New York)  
- **Size**: ~2.1 million rows, 33 features (~70 million datapoints)  
- **Key Variables**:  
  - Demographics (age, gender, race, ethnicity, zip code)  
  - Admission details (type, severity, risk of mortality, length of stay)  
  - Diagnosis & procedures (CCSR codes, APR-DRG categories)  
  - Hospital characteristics (service area, facility)  
  - Costs & charges (total estimated cost, total charges)  

- **Target Variables**:  
  - **Regression** → Predict total healthcare cost  
  - **Classification** → Categorize patients as *low*, *medium*, or *high-cost*  

---

## ⚙️ Methodology  
1. **Data Preprocessing**  
   - Removal of duplicates and invalid records  
   - Missing value imputation (mode/median)  
   - Outlier treatment with log transformations for skewed cost data  
   - One-hot encoding for categorical features  

2. **Exploratory Data Analysis (EDA)**  
   - Univariate & bivariate analysis of demographics, admissions, and costs  
   - Distribution of costs across hospital service areas, diagnosis categories, and procedures  
   - Correlation between charges, length of stay, and severity of illness  

3. **Modeling**  
   - **XGBoost Regression** for continuous cost prediction  
   - **XGBoost Classification** for cost-tier prediction (low/medium/high)  

4. **Evaluation**  
   - Regression → RMSE, MAE, R²  
   - Classification → Accuracy, Precision, Recall, F1-score, ROC-AUC  
   - Cross-validation to ensure generalizability  
   - **SHAP analysis** for model interpretability (global & class-specific feature importance)  

---

## 📊 Results & Key Insights  
- **XGBoost Classification** achieved high performance in identifying high-cost patients, with strong recall for the high-cost class.  
- **XGBoost Regression** predicted continuous costs but faced challenges due to skewed distributions.  
- **SHAP Interpretability** showed that:  
  - **Length of stay**, **severity of illness**, and **diagnosis categories** were major cost drivers.  
  - Demographic and admission-related features (age, admission type, hospital area) also influenced predictions.  
- Portfolio of models provides a **scalable, interpretable, and pragmatic framework** for healthcare cost prediction.  

---

## 🚀 Tools & Libraries  
- Python  
- Pandas, NumPy  
- Scikit-learn  
- XGBoost  
- SHAP (for explainability)  
- Matplotlib, Seaborn  
- Jupyter Notebook  

---

## 📑 Contributions  
- Developed an **interpretable ML framework** for high-cost patient prediction.  
- Compared regression vs. classification approaches on the same dataset.  
- Used **multi-class classification** (low, medium, high) to better reflect healthcare practice.  
- Applied **SHAP explainability** to enhance transparency and clinical usability.  
- Highlighted **policy and practical implications** for hospitals, insurers, and policymakers.  

---

## 👤 Author  
**Sambhav Jain**  

