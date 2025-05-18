
# Model Performance Report: Heart Disease Prediction

## Dataset Summary

- **Number of Samples:** 296 (after data cleaning)  
- **Features Used:** Age, cholesterol, resting blood pressure, max heart rate achieved, ST depression, number of major vessels, and several categorical health indicators.  
- **Target Variable:** Presence of heart disease (binary classification: 0 = no disease, 1 = disease).  

---

## Key Feature Statistics

### Age
- **Average:** 54.5 years  
- **Range:** 29 to 77 years  

### Cholesterol
- **Average:** 247.15 mg/dl  
- **Range:** 126 to 564 mg/dl  
- **Note:** Healthy cholesterol is usually <200 mg/dl.  

### Resting Blood Pressure
- **Average:** 131 mm Hg  
- **Range:** 94 to 200 mm Hg  

### Max Heart Rate Achieved
- **Average:** 149.5 bpm  
- **Range:** 71 to 202 bpm  

### ST Depression
- **Average:** 1.06  
- **Range:** 0 to 6.2  

### Number of Major Blood Vessels
- **Average:** 0.68  
- **Range:** 0 to 3  

---

## Model Evaluation

### 1. Logistic Regression

- **Accuracy:** 0.82  

**Classification Report:**  
```
              precision    recall  f1-score   support
         0       0.81      0.79      0.80        28
         1       0.82      0.84      0.83        32
  accuracy                           0.82        60
 macro avg       0.82      0.81      0.82        60
weighted avg     0.82      0.82      0.82        60
```

**Confusion Matrix:**  
```
[[22  6]
 [ 5 27]]
```

**Interpretation:**  
Logistic Regression achieved balanced precision and recall for both classes, with slightly better recall for predicting heart disease (class 1).

---

### 2. Random Forest

- **Accuracy:** 0.80  

**Classification Report:**  
```
              precision    recall  f1-score   support
         0       0.79      0.79      0.79        28
         1       0.81      0.81      0.81        32
  accuracy                           0.80        60
 macro avg       0.80      0.80      0.80        60
weighted avg     0.80      0.80      0.80        60
```

**Confusion Matrix:**  
```
[[22  6]
 [ 6 26]]
```

**Interpretation:**  
Random Forest performed similarly, with very close precision, recall, and F1-scores for both classes. Slightly more false negatives compared to Logistic Regression.

---

## Model Selection

- **Preferred Model:** Logistic Regression demonstrates slightly better precision and recall, making it the preferred choice for this dataset and configuration.  
- **Random Forest Note:** The Random Forest model is close in performance and may surpass Logistic Regression with further hyperparameter tuning or more data.

---

## Recommendations

1. **Model Improvement:**  
   - Consider cross-validation and hyperparameter optimization, especially for Random Forest.  
   - Explore feature engineering or additional data collection for further improvement.  

2. **Interpretability:**  
   - Logistic Regression can be favored for its interpretability in a medical context.  

3. **Future Work:**  
   - Further evaluate models with ROC curves and AUC.  
   - Assess calibration for predicted probabilities.  

---
