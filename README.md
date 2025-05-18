# Heart Disease Prediction
---


<img src="https://github.com/nileshsharma-dp/heart_disease_prediction/blob/main/Assets/heart.jpeg" alt="Heart Disease" width="1200"/>

---

This project predicts the likelihood of heart disease using machine learning algorithms (Logistic Regression and Random Forest) based on various health indicators such as age, cholesterol, and blood pressure.

---

## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Features](#features)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Cleaning & Preprocessing](#data-cleaning--preprocessing)
- [Modeling](#modeling)
- [Results](#results)
- [How to Run](#how-to-run)
- [Requirements](#requirements)
- [References](#references)

---

## Overview
The goal of this project is to predict whether a patient has heart disease based on clinical and laboratory features. The project covers data cleaning, exploratory data analysis (EDA), feature engineering, and model building.

---

## Dataset
- **Source:** UCI Heart Disease Dataset
- **Total Samples:** 303 (after cleaning: 296)
- **Target Variable:** `target` (1 = heart disease, 0 = no heart disease)

Each row represents a patient's medical record.

---

## Features

| Feature | Description |
|--------|-------------|
| `age` | Age in years |
| `sex` | Male/Female |
| `chest_pain_type` | Type of chest pain (typical angina, atypical angina, non-anginal pain, asymptomatic) |
| `resting_blood_pressure` | Resting blood pressure (mm Hg) |
| `cholesterol` | Serum cholesterol in mg/dl |
| `fasting_blood_sugar` | Fasting blood sugar > 120 mg/dl (True/False) |
| `resting_electrocardiogram` | ECG results (normal, ST-T wave abnormality, left ventricular hypertrophy) |
| `max_heart_rate_achieved` | Maximum heart rate achieved |
| `exercise_induced_angina` | Exercise-induced angina (Yes/No) |
| `st_depression` | ST depression induced by exercise relative to rest |
| `st_slope` | Slope of the peak exercise ST segment (upsloping, flat, downsloping) |
| `num_major_vessels` | Number of major vessels colored by fluoroscopy (0-3) |
| `thalassemia` | Type of thalassemia (fixed defect, normal, reversible defect) |
| `target` | 1 = heart disease, 0 = no heart disease |

---

## Exploratory Data Analysis
- Identified and dropped missing or faulty values (`ca`, `thal`).
- Visualized feature distributions and their relation with the target using **Seaborn** and **Matplotlib**.

---

## Data Cleaning & Preprocessing
- Renamed columns for clarity.
- Mapped categorical numerical values to readable labels.
- Dropped rows with invalid or missing values based on documentation.

---

## Modeling
- Split features into **numerical** and **categorical** types.
- Split data into **training** and **testing** sets.
- Applied **StandardScaler** for numerical feature scaling.
- Machine learning models used:
  - Logistic Regression
  - Random Forest Classifier

---

## Results
- Evaluated model performance using:
  - Accuracy Score
  - Confusion Matrix
  - Classification Report
- Visualized class distributions and feature importance.

---

---

## How to Run

To run this project locally, follow these steps:


1. Clone the repository
```bash
git clone https://github.com/nileshsharma-dp/heart_disease_prediction.git
cd heart_disease_prediction
```

2. Install dependencies
```bash
pip install -r requirements.txt
```

3. Launch the Jupyter Notebook
```bash
jupyter notebook ml_heart\ disease_prediction.ipynb
```


Run the cells in the notebook to perform data preprocessing, modeling, and view the results.

---

## Requirements

The following libraries are required to run this project:

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- jupyter

To install the dependencies individually, run:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

---

## References

- [UCI Machine Learning Repository: Heart Disease Dataset](https://archive.ics.uci.edu/ml/datasets/heart+Disease)
- Dataset documentation and preprocessing discussion threads available on various data science forums

---
