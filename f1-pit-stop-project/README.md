# F1 Pit Stop Prediction  

<p align="center">
Predicting next-lap pit stop decisions in Formula 1 using machine learning.
</p>

<p align="center">
<a href="f1_claasification.html"> View Notebook</a> • 
<a href="#key-insight"> Key Insight</a> • 
<a href="#approach"> Approach</a>
</p>

---

## Overview

This project uses machine learning to predict whether a driver will make a pit stop on the next lap in Formula 1 race data.

The model learns from race telemetry such as tyre wear, lap performance, and race context to identify patterns behind strategic pit decisions.

---

## Feature Importance

<p align="center">
  <img src="feature_importance.png" width="750">
</p>

---

## Key Insight

Pit stop decisions are primarily driven by **performance degradation over time**, particularly changes in lap time and tyre wear progression.

Rather than relying on static features like tyre compound, the model captures how race performance evolves—reflecting real-world strategy dynamics.

---

## Approach

- Data cleaning and preprocessing  
- Exploratory data analysis  
- Feature engineering  
- Classification modeling  

---

##  Tools

`Python` • `Pandas` • `Seaborn` • `Scikit-learn`

---

## Future Improvements

- SHAP for feature interpretability  
- Hyperparameter tuning  
- Time-aware sequential modeling  

---
