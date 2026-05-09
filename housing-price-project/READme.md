# Ames Housing Price Prediction

## Overview

This project builds an end-to-end supervised machine learning pipeline to predict house prices using the Ames Housing dataset. The dataset contains a high-dimensional mix of numerical, ordinal, and categorical variables describing residential properties.

The goal is to build a robust regression system capable of generalizing across heterogeneous housing structures while handling multicollinearity, skewed distributions, and nonlinear feature interactions.

---

## Key Insight

House prices are primarily driven by structural quality, living area, and neighborhood effects, but the relationship is not purely linear, especially in the upper price range.

Regularized linear models perform well on the central distribution of the dataset but show increasing error in high-value properties, indicating that luxury housing behaves as a distinct regime with stronger nonlinear dependencies.

---

## Approach

- Data cleaning and missing value handling  
- Ordinal encoding for hierarchical categorical variables  
- One-hot encoding for nominal features  
- Feature engineering (age-based variables, binary indicators, and aggregated features)  
- Log and square-root transformations for skewed numerical variables  
- Multicollinearity reduction through feature pruning and derivation  
- Model training (Linear Regression, Ridge, Lasso, ElasticNet, Random Forest, Gradient Boosting)  
- Residual diagnostics and error segmentation  

---

## Model Results

- Linear Regression: Baseline model with moderate bias and limited flexibility  
- Ridge Regression: Improved stability but similar predictive performance  
- Lasso Regression: Feature sparsity introduced without major performance gains  
- ElasticNet: Best-performing linear model with balanced regularization  
- Random Forest: Strong training performance but significant overfitting  
- Gradient Boosting: High variance and unstable generalization  

ElasticNet was selected as the final model due to its best balance between stability and generalization.

---

## Key Findings from Residual Analysis

Residual diagnostics revealed:

- Errors are centered around zero for most predictions  
- Strong right-skew in residual distribution due to under-prediction of high-value homes  
- Increasing error variance with price (heteroscedasticity)  
- Isolated extreme residuals rather than systematic structural drift  

This indicates that model limitations are concentrated in the upper tail of the price distribution rather than uniformly across all observations.

---

## Tools

- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  
- Seaborn  

---

## Future Improvements

- Apply log transformation to target variable to stabilize variance  
- Introduce interaction features (e.g., quality × area effects)  
- Explore stronger gradient boosting regularization strategies  
- Investigate quantile regression for tail performance  
- Deploy model as an interactive prediction interface
