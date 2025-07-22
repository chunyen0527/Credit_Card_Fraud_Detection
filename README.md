# Credit Card Fraud Detection using Machine Learning

This project focuses on detecting fraudulent credit card transactions using supervised machine learning techniques, built as part of a graduate-level analytics course.

---

## Dataset

- **Source**: [Kaggle - Credit Card Fraud Prediction](https://www.kaggle.com/datasets/kelvinkelue/credit-card-fraud-prediction) 
- Contains demographic and transaction-level information
- Highly imbalanced data (~0.1% fraud ratio)

---


## Features & Engineering Highlights

- Derived features:
  - `age_years` from `dob`
  - `time_period` from transaction hour
  - `is_weekend` based on transaction date
- Dropped irrelevant or sensitive columns (e.g., `cc_num`, `merchant`, coordinates)
- Encoded categorical variables with LabelEncoder
- Normalized continuous variables with MinMaxScaler
- Saved encoders and scaler using `joblib`

---

## Technologies Used

- Python 3.12
- pandas, NumPy
- scikit-learn
- matplotlib, seaborn
- joblib
- Jupyter Notebook

---

## Model Summary

| Model                | Metrics Used                     | Performance                               |
|---------------------|----------------------------------|-------------------------------------------|
| Logistic Regression | Accuracy, Precision, Recall, F1 | ✅ Used as a baseline                      |
| Random Forest       | Confusion Matrix, AUC           | ✅ Improved performance on fraud class     |

---

## Files Overview

| File                          | Description                                           |
|-------------------------------|-------------------------------------------------------|
| `code/model_and_analysis.ipynb` | Data cleaning, feature engineering, model training    |
| `code/loadmodel.ipynb`         | Reloading models, encoders for evaluation/prediction |
| `docs/final-report.pdf`        | Detailed written report                              |
| `docs/presentation-slides.pdf` | Summary slide deck                                   |

