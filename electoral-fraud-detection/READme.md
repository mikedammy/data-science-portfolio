# Election Fraud Detection

Detecting fraudulent electoral activity using machine learning and adversarial election analytics.

---

## Overview

This project explores election fraud detection using a synthetic political analytics dataset containing electoral statistics, cybersecurity indicators, manipulation metrics, voting behavior patterns, and adversarial activity signals.

The objective was to build a classification pipeline capable of distinguishing fraudulent electoral activity from legitimate voting behavior while handling multicollinearity, class imbalance, synthetic noise variables, and potential target leakage.

---

## Model Performance

<p align="center">
  <img src="decision_threshold.png" width="700" alt="Model Performance Chart">
</p>

---

## Key Insight

The project revealed that standard accuracy was a misleading evaluation metric due to class imbalance and model overfitting.

Models that initially appeared to achieve strong predictive performance were largely memorizing noisy structures and majority-class patterns. More reliable evaluation using balanced accuracy, ROC-AUC, recall, and threshold tuning exposed the true generalization capability of the models.

The final optimized XGBoost pipeline prioritized fraud recall over raw accuracy, achieving approximately 80% minority-class recall after threshold adjustment.

---

## Approach

- Data cleaning and preprocessing
- Missing value handling
- Exploratory data analysis
- Multicollinearity reduction
- Feature engineering
- Log transformation of skewed variables
- Class imbalance handling
- Classification modeling and evaluation

---

## Models Used

- Logistic Regression
- Random Forest
- HistGradientBoosting
- XGBoost

---

## Tools & Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost

---

## Future Improvements

- Advanced feature engineering using temporal election behavior
- Sequence-based fraud modeling
- SHAP-based model interpretability
- PyTorch neural network implementation
- Hyperparameter optimization using Bayesian search

---

## Project Notebook

<a href="electoral_fraud_project.html">
    View Full Notebook
</a>
