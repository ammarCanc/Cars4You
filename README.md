# 🚗 Car Price Prediction — Machine Learning Project

This repository contains a **single Jupyter notebook** that implements an end-to-end machine learning workflow for predicting car prices. The notebook covers data preprocessing, feature engineering, model optimization, evaluation using multiple metrics, and inference for both batch and single-entry predictions.

The focus of the project is not only on achieving good predictive performance but also on understanding model behavior, generalization, and the impact of different modeling decisions.

---

## 📌 Project Overview

- **Problem Type:** Supervised regression  
- **Target Variable:** Car price  
- **Implementation:** Single Jupyter Notebook  
- **Evaluation Strategy:** Holdout train–test split  
- **Deployment Ready:** Yes (supports batch and single-entry prediction)

---

## 📓 Notebook Contents

The notebook is organized into the following main sections:

1. **Data Loading and Exploration**  
   Initial inspection of the dataset, data types, and basic statistics.

2. **Data Preprocessing**  
   - Numerical data cleaning and imputation  
   - Categorical text normalization and rare category handling  
   - Target encoding for categorical variables  
   - Feature scaling and selection  

3. **Feature Engineering**  
   Creation of additional features and removal of highly correlated variables to improve model stability.

4. **Model Training and Optimization**  
   - Training multiple regression models  
   - Hyperparameter tuning using RandomizedSearch  
   - Fair comparison across different model families  

5. **Model Evaluation**  
   Evaluation using multiple metrics including MAE, RMSE, R², Median Absolute Error, MAPE, and a composite generalization score.

6. **Final Model Selection**  
   Selection of the best model based on balanced performance and generalization.

7. **Inference and Deployment Readiness**  
   - Batch prediction from CSV files  
   - Single-entry prediction using saved artifacts  

---

## 🧠 Models Evaluated

- LinearRegression (baseline)
- DecisionTreeRegressor
- RandomForestRegressor
- ExtraTreesRegressor
- BaggingRegressor
- HistGradientBoostingRegressor
- KNeighborsRegressor

Hyperparameters were optimized to ensure each model was evaluated at its best performance.

---

## 📊 Evaluation Metrics

Models were evaluated using the following metrics:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score
- Median Absolute Error
- Mean Absolute Percentage Error (MAPE)
- Composite Score (generalization-aware metric)

---

## 🏆 Final Model

**HistGradientBoostingRegressor** was selected as the final model due to its superior accuracy, stability, and generalization across all evaluation metrics.

Outlier handling was intentionally removed after experimental evaluation showed that it reduced generalization performance.

---
