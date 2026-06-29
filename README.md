# 🩺 Early Breast Cancer Diagnostic Support Using Machine Learning

## Overview

This project develops and evaluates multiple machine learning models capable of classifying breast tumors as **benign** or **malignant** using diagnostic tumor measurements. The goal is to demonstrate an end-to-end healthcare machine learning workflow, from exploratory data analysis and feature engineering to model evaluation and explainable AI.

Rather than relying solely on predictive performance, this project emphasizes **model interpretability** through SHAP (SHapley Additive exPlanations), providing insight into the tumor characteristics that most strongly influence predictions.

> **Disclaimer:** This project is intended for educational and portfolio purposes only. It is not clinically validated and should not be used for medical diagnosis or treatment decisions.

---

## Project Objectives

- Explore diagnostic breast cancer data
- Identify relationships among tumor characteristics
- Prevent data leakage through appropriate feature selection
- Develop multiple classification models
- Compare model performance using healthcare-relevant metrics
- Explain model predictions using SHAP
- Demonstrate a complete machine learning workflow suitable for healthcare analytics

---

## Dataset

**Source**

Enhanced Breast Cancer Diagnostic Dataset (Kaggle)

The dataset contains numerical measurements describing tumor morphology and a binary diagnosis:

- **Benign (B)**
- **Malignant (M)**

Examples of predictor variables include:

- Radius
- Texture
- Perimeter
- Area
- Smoothness
- Compactness
- Concavity
- Concave Points
- Shape Irregularity
- Border Complexity

Several engineered interaction features are also included.

---

## Data Preparation

Prior to model development:

- Removed missing values (none detected)
- Encoded diagnosis labels
- Removed non-informative ID column
- Removed leakage variables:
  - `tumor_aggressiveness`
  - `malignancy_risk_score`
- Performed exploratory data analysis
- Examined feature correlations
- Created an 80/20 stratified train-test split

---

## Machine Learning Models

The following models were trained and compared:

- Dummy Classifier (Baseline)
- Logistic Regression
- Random Forest Classifier
- XGBoost Classifier

---

## Model Evaluation

Models were evaluated using:

- Accuracy
- Precision
- Recall (Sensitivity)
- F1 Score
- ROC-AUC
- Confusion Matrix
- ROC Curve

Because this project focuses on cancer detection, **Recall** and **ROC-AUC** were considered the most important evaluation metrics to minimize false negatives.

---

## Explainable AI

Model interpretability was investigated using **SHAP (SHapley Additive exPlanations)**.

SHAP analysis provides:

- Global feature importance
- Individual prediction explanations
- Feature contribution visualizations
- Improved transparency for healthcare decision support

---

## Visualizations

This project includes visualizations such as:

- Diagnosis distribution
- Correlation heatmap
- Confusion matrices
- ROC curves
- Random Forest feature importance
- XGBoost feature importance
- SHAP summary plot
- SHAP feature importance plot

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- XGBoost
- SHAP
- Jupyter Notebook

---

## Repository Structure

```
breast-cancer-diagnostic-ml/
│
├── notebooks/
│   └── BreastCancerDetectionModel.ipynb
│
├── figures/
│   ├── class_distribution.png
│   ├── correlation_heatmap.png
│   ├── logistic_confusion_matrix.png
│   ├── logistic_roc_curve.png
│   ├── random_forest_confusion_matrix.png
│   ├── random_forest_feature_importance.png
│   ├── xgboost_confusion_matrix.png
│   ├── xgboost_feature_importance.png
│   ├── shap_summary_plot.png
│   └── shap_feature_importance.png
│
├── data/
│   └── README.md
│
├── requirements.txt
│
└── README.md
```

---

## Key Skills Demonstrated

- Healthcare Data Science
- Exploratory Data Analysis
- Data Cleaning
- Feature Engineering
- Binary Classification
- Ensemble Learning
- Gradient Boosting
- Model Evaluation
- Explainable AI
- Scientific Visualization

---

## Future Improvements

Potential extensions include:

- Hyperparameter optimization
- Cross-validation tuning
- Flask web application for interactive predictions
- Streamlit deployment
- Model monitoring
- External dataset validation
- Integration with clinical decision-support workflows

---

## Author

**Alyssa Seal**

MS Data Science

GitHub: https://github.com/alseal17

LinkedIn: www.linkedin.com/in/alyssa-seal-1a855298
