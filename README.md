# 💉 Predicting Flu Vaccine Uptake: Multi-Output Gradient Boosting
**A Predictive Analytics Study for VaxCare to Combat Declining Vaccination Rates**

## 📌 Project Overview
Since 2021, the U.S. has seen a 10% decline in adults opting for flu vaccines, representing a $12.5M revenue risk for pharmaceutical producers like **VaxCare**. This project builds a predictive model to identify the key drivers of vaccine uptake for both H1N1 and Seasonal flu, allowing for targeted public health interventions.

## 🛠️ Tech Stack
* **Language:** Python (Google Colab)
* **Libraries:** `Scikit-Learn`, `XGBoost`, `Pandas`, `NumPy`
* **Models Evaluated:** Logistic Regression (Baseline), Random Forest, Bagging Ensembles, and **Tuned Gradient Boosting**.
* **Architecture:** Multi-Output Classifier Pipeline with RandomizedSearchCV.

## 📊 The Dataset
* **Source:** National 2009 H1N1 Flu Survey (NHFS) via DrivenData.
* **Features:** 35+ variables including physician recommendations, health behaviors, and personal opinions on vaccine effectiveness and risk.
* **Preprocessing:** Standard Scaling for numerical data and One-Hot Encoding for categorical variables, handled within a robust `Scikit-Learn Pipeline`.

## 🧠 Model Evolution & Performance
We moved beyond simple classifiers to ensemble methods to capture complex behavioral interactions:
* **Baseline Logistic Regression:** Mean AUC 0.8242
* **Tuned Random Forest:** Mean AUC 0.8412
* **Tuned Gradient Boosting (Final Model):** **Mean AUC 0.8523** 🏆

## 📈 Strategic Insights
Using **Permutation Importance**, we identified the top predictors for vaccine uptake:
1. **Physician Recommendation:** The strongest driver for both H1N1 and Seasonal vaccines.
2. **Perception of Risk:** Personal belief in the likelihood of getting sick without the vaccine.
3. **Opinion on Effectiveness:** Trust in the vaccine's ability to prevent illness.
