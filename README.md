# Predictive Modeling of Bank Term Deposits — A Kaggle Competition Project
![Python](https://img.shields.io/badge/Python-3.9-blue)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.1.3-orange)
![Kaggle](https://img.shields.io/badge/Kaggle-Competition-blue)
![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)

---

## 📌 Overview

This project is part of the [Kaggle Playground Series S5E8 (2025)](https://kaggle.com/competitions/playground-series-s5e8) 

The challenge is to predict whether a client will subscribe to a bank term deposit based on tabular features.

The competition provides an approachable, real-world inspired dataset for practicing supervised machine learning workflows.
  
## 🎯 Goal

-  **Objective**: Predict the probability that a client subscribes to a term deposit (y).

-  **Problem Type**: Binary Classification

-  **Evaluation Metric**: Area Under the Receiver Operating Characteristic Curve (ROC-AUC)

## ✨ Key Highlights

-  Conducted comprehensive Exploratory Data Analysis (EDA) with visualizations.

-  Implemented data preprocessing: missing values imputation, categorical encoding, and feature scaling.

-  Developed and compared multiple machine learning models:

    -  Logistic Regression (baseline model)

    -  LightGBM Classifier

    -  XGBoost Classifier

-  Evaluated models using ROC-AUC, confusion matrices, and classification reports.

-  Produced a submission file with probability predictions for Kaggle evaluation.

## 🛠️ Tools & Libraries

-  Language: Python

-  Core Libraries:

    -  numpy, pandas → Data manipulation

    -  matplotlib, seaborn → Data visualization

    -  scikit-learn → Preprocessing, Logistic Regression, model evaluation

    -  lightgbm → LightGBM Classifier

    -  xgboost → XGBoost Classifier


## 📂 Dataset

The dataset is synthetically generated from the original Bank Marketing Dataset.

  -  train.csv → Training dataset (with target y)

  -  test.csv → Test dataset (no labels, predictions required)

  -  sample_submission.csv → Correct submission format

**Target variable**:

  -  y = 1 → Client subscribes

  -  y = 0 → Client does not subscribe

## 📊 Results

Validation ROC-AUC performance across models:

|   Rank  |          Model          | ROC-AUC Score |
|---------|-------------------------|---------------|
|    1    |         LightGBM        |     0.9680    |
|    2    |          XGBoost	      |     0.9672    |
|    3    |   Logistic Regression   |     0.9346    |

- **LightGBM** achieved the highest validation performance, closely followed by **XGBoost**.

- Logistic Regression, while less accurate, served as a strong and interpretable baseline.

## 📁 Repository Structure
```
├── notebooks/
│   ├── Binary_Classification_Bank_Dataset.ipynb   # Full project workflow
├── data/
│   ├── train.csv
│   ├── test.csv
│   ├── sample_submission.csv
├── results/
│   ├── submission.csv
├── requirements.txt
└── README.md
```
## 📚 Citation  
Walter Reade and Elizabeth Park.  
**Binary Classification with a Bank Dataset**.  
[Kaggle Playground Series S5E8 (2025)](https://kaggle.com/competitions/playground-series-s5e8)  

---

## 🚀 Next Steps  
- Perform hyperparameter tuning with GridSearchCV / Optuna  
- Explore advanced feature engineering for categorical variables  
- Compare additional models (CatBoost, Random Forest, Neural Networks)  
- Deploy the best-performing model using Streamlit or Flask  
- Build a Power BI / Tableau dashboard for interactive insights  

---

## 📄 License  
This project is licensed under the **MIT License** - you are free to use, modify, and distribute this project with proper attribution. 

