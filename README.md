# Gestational Diabetes Prediction Using Machine Learning

This project aims to predict the risk of Gestational Diabetes Mellitus (GDM) early in pregnancy using clinical and demographic data. By leveraging machine learning models and statistical analysis, the system identifies high-risk individuals to enable timely intervention. The study was conducted using R and emphasizes both predictive accuracy and clinical relevance.

---

## Project Objectives

- Develop machine learning models to predict GDM risk
- Address class imbalance using SMOTE
- Evaluate and compare model performance
- Interpret key clinical features contributing to GDM
- Assess model limitations and propose improvements

---

## Technologies Used

- **Language**: R
- **Libraries**: caret, e1071, xgboost, ROCR, ggplot2, DMwR (SMOTE)
- **Models**: Logistic Regression, SVM, XGBoost
- **Techniques**: Feature selection, class imbalance correction, statistical analysis

---

## Key Features

- **SMOTE Balancing**: Addressed class imbalance to enhance prediction of minority class (GDM-positive cases)
- **Model Variety**: Evaluated both interpretable (Logistic Regression) and complex (XGBoost, SVM) models
- **Relevant Clinical Features**: Used biologically meaningful features like Glucose, BMI, and Age
- **Strong Performance**: Achieved AUC scores between 84%–90%, demonstrating good discriminative ability

---

## Model Analysis

### Strengths

- **Model Diversity**: Evaluated a spectrum from interpretable to complex models.
- **Class Imbalance Handling**: SMOTE successfully balanced minority GDM cases.
- **Robust Performance**: Models achieved strong AUCs (~84–90%), indicating high discrimination.
- **Biological Relevance**: Selected features aligned with key findings in published studies.

### Limitations

- **Dataset Scope**: Lacked important clinical features like HbA1c, ethnicity, or family history.
- **Cross-Sectional Data**: Only one time-point per patient limits modeling of progression over pregnancy.
- **Interpretability vs Accuracy**: XGBoost outperformed others but is harder to interpret than logistic models, which is critical for clinical use.
- **Generalizability**: Dataset (PIMA) has limited population diversity, restricting global applicability.

---

## Recommendations for Future Work

- **Richer Feature Set**: Include additional clinical/behavioral features (HbA1c, physical activity, ethnicity).
- **Time-Series Data**: Collect data across pregnancy phases for dynamic risk modeling.
- **Model Interpretability**: Use SHAP or LIME to make complex models clinically explainable.
- **Advanced Preprocessing**: Apply multiple imputation, quantile scaling, or predictive mean matching.
- **External Validation**: Validate on independent and demographically diverse datasets for generalizability.

---

## Conclusion

This project demonstrates that machine learning models, even on limited datasets, can effectively predict GDM risk when properly balanced and validated. The findings also stress the importance of using explainable models in clinical settings and highlight opportunities for improving generalizability through richer data and external validation.

---
