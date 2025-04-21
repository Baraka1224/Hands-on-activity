# Heart Disease Prediction Using Machine Learning

This project focuses on building and evaluating machine learning models to predict the likelihood of heart disease based on key patient health indicators such as age, cholesterol, blood pressure, and more. The goal is to compare model performance and identify the best approach for classification.

##  Dataset

- Source: Simulated Heart Disease dataset (based on UCI Heart Disease dataset structure)
- Features include: age, sex, chest pain type, resting blood pressure, cholesterol, fasting blood sugar, ECG results, max heart rate, exercise-induced angina, oldpeak, slope, number of vessels, thalassemia, and diagnosis (`target`)

## Models Implemented

- **Support Vector Machine (SVM)**
- **Random Forest Classifier**
- **Gradient Boosting Classifier**

##  Methods

- GridSearchCV used for hyperparameter tuning
- 80/20 train-test split
- Evaluated on:
  - Accuracy
  - Precision
  - Recall
  - F1-Score
  - AUC-ROC

## Results Summary

| Model             | Accuracy | Precision | Recall | F1-score | AUC-ROC |
|------------------|----------|-----------|--------|----------|---------|
| SVM              | 0.475    | 0.452     | 0.483  | 0.467    | 0.476   |
| Gradient Boosting| **0.590**| **0.567** | **0.586**| **0.576**| **0.606**|
| Random Forest     | 0.525    | 0.500     | 0.448  | 0.473    | 0.502   |

> **Gradient Boosting** achieved the best overall performance across all metrics.

## ROC Curve Comparison

A visual comparison of all three models using ROC curves confirms that Gradient Boosting separates classes better than SVM and Random Forest.

## Reflection

Model performance varied across algorithms, with Gradient Boosting showing more consistent and higher predictive power after tuning. Hyperparameter optimization significantly improved results. ROC-AUC further highlighted the strengths and weaknesses of each model in distinguishing positive cases.

---

##  Technologies Used

- Python 3
- scikit-learn
- pandas, numpy
- matplotlib (for ROC curves)
- Jupyter Notebook

---

##  Author

Baraka Sila  
Master's in Business Analytics
