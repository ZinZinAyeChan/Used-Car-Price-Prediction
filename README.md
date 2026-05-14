# 🚗 Used Car Price Prediction — Kaggle Competition

A machine learning regression project completed for **BUSA3020 Applied Machine Learning** at Macquarie University. The project predicts used car sale prices from vehicle characteristics using a full ML pipeline — from data cleaning and feature engineering through to model tuning and Kaggle competition submission.

---

## 🏆 Project Overview

This project was completed as part of a **Kaggle forecasting competition** in a team of 3. The goal was to build the most accurate regression model for predicting used car prices based on features such as mileage, horsepower, engine specs, and fuel economy. Five models were developed and compared, with the best submitted to Kaggle for public and private leaderboard ranking.

- **Team Name:** BUSA3020_Quacks
- **Competition:** Macquarie Analytics Competition S1 2024
- **Dataset:** 3,000 test observations, 38 features (22 numeric, 16 categorical)

---

## 👥 Team

| Member | Task |
|---|---|
| Zin Zin Aye Chan | Task 3 — Model Building, Tuning & Kaggle Submission |
| Anisha Nawar Hoque | Task 1 — Problem Description & Initial Data Analysis |
| Hsu Thanzin Zaw | Task 2 — Data Cleaning, Imputation & Feature Engineering |

---

## ✨ Key Results

| Model | Public Score | Private Score |
|---|---|---|
| Linear Regression | 0.50872 | 0.48956 |
| Elastic Net | 0.29294 | 0.29401 |
| **Random Forest** ✅ | **0.13642** | **0.11984** |

> 📉 Lower scores are better — the metric is RMSLE (Root Mean Squared Log Error).

**Random Forest** was the best performing model, achieving the lowest scores on both leaderboards. Built with 1,000 trees and StandardScaler preprocessing. Lasso and Ridge were also tested but showed no meaningful improvement over Elastic Net, so Random Forest was selected as the final submission.

---

## 🛠️ Built With

- Python 3
- `pandas` · `numpy` — data manipulation
- `scikit-learn` — modelling, imputation, encoding, cross-validation
- `matplotlib` · `seaborn` — EDA and visualisation
- Jupyter Notebook
- Kaggle

---

## 📁 Project Structure

```
/Used_Car_Price_Prediction.ipynb       # Full pipeline — EDA, cleaning, modelling
/linear_regression_prediction.csv      # Kaggle submission — Linear Regression
/lasso_prediction.csv                  # Kaggle submission — Lasso
/ridge_prediction.csv                  # Kaggle submission — Ridge
/elasticnet_prediction.csv             # Kaggle submission — Elastic Net
/randomforest_prediction.csv           # Kaggle submission — Random Forest (final)
/sample_submission.csv                 # Kaggle sample submission format
/data
  └── train.csv                        # Training dataset
  └── test.csv                         # Test dataset
/README.md
```

---

## 🧠 Concepts Demonstrated

- Exploratory Data Analysis (EDA) — summary statistics, histograms, pairplots, heatmaps
- Data cleaning — extracting numerical values from mixed-type columns
- Feature engineering — extracting torque value/RPM, power value/RPM, engine type from raw text
- Missing value imputation — median (numeric), mode (categorical) via `SimpleImputer`
- Categorical encoding — One-Hot Encoding with top-5 frequency bucketing
- Feature selection — correlation-based threshold filtering
- Regression modelling — Linear Regression, Lasso, Ridge, Elastic Net, Random Forest
- Hyperparameter tuning — alpha selection via cross-validation
- Model evaluation — MSE, R², Kaggle leaderboard scoring
- Kaggle competition workflow — submission, public vs private leaderboard

---

## 💡 Suggested Improvements

- Hyperparameter tuning for Random Forest (depth, number of estimators)
- Additional feature engineering or interaction terms
- Ensemble methods — blending or stacking multiple models
- Outlier handling and advanced imputation strategies

---

## 📌 Data Source

- Macquarie Analytics Competition S1 2024 — dataset provided via Kaggle
- Competition link: [kaggle.com/t/ff5fb5beaeb14f7686df98fef9d1c0bc](https://www.kaggle.com/t/ff5fb5beaeb14f7686df98fef9d1c0bc)

> Data used for non-commercial, educational purposes only.

---

## 👤 Author

**Zin Zin Aye Chan** — Student ID: 46866531  
Bachelor of [Your Degree], Macquarie University  
[LinkedIn](https://linkedin.com/in/yourprofile) · [GitHub](https://github.com/yourusername) · [Email](mailto:youremail@example.com)
