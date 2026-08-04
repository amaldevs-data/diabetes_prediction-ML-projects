# Diabetes Prediction System 🩺

## Overview

The **Diabetes Prediction System** is a Machine Learning-based healthcare application designed to predict whether a patient is diabetic or non-diabetic using clinical and demographic health information.

The project follows an end-to-end machine learning workflow including data preprocessing, exploratory data analysis, handling class imbalance, model comparison, hyperparameter optimization, and deployment using Streamlit.

The best-performing model, **XGBoost Classifier**, achieved an accuracy of **97%** after hyperparameter tuning using GridSearchCV.

---

# Project Objectives

- Build a machine learning model for early diabetes risk prediction.
- Compare multiple classification algorithms.
- Improve model performance using data preprocessing and optimization techniques.
- Handle imbalanced healthcare data effectively.
- Deploy the trained model as an interactive web application.

---

# Dataset

The dataset contains patient health records with clinical and lifestyle-related attributes.

## Features Used

| Feature | Description |
|---|---|
| Gender | Patient gender |
| Age | Patient age |
| Hypertension | History of hypertension |
| Heart Disease | Presence of heart disease |
| Smoking History | Patient smoking status |
| BMI | Body Mass Index |
| HbA1c Level | Average blood glucose level indicator |
| Blood Glucose Level | Blood glucose measurement |

## Target Variable

**Diabetes**

- 0 → Non-Diabetic
- 1 → Diabetic

---

# Machine Learning Workflow

```
Dataset
   |
   ↓
Data Cleaning & Preprocessing
   |
   ↓
Exploratory Data Analysis (EDA)
   |
   ↓
Feature Encoding
   |
   ↓
Feature Scaling
   |
   ↓
Class Balancing using SMOTE
   |
   ↓
Train-Test Split
   |
   ↓
Model Training
   |
   ↓
Hyperparameter Tuning (GridSearchCV)
   |
   ↓
Model Evaluation
   |
   ↓
Deployment using Streamlit
```

---

# Data Preprocessing

The following preprocessing techniques were applied:

- Missing value handling
- Exploratory Data Analysis
- Label encoding for categorical features
- Feature scaling using StandardScaler
- Train-test splitting
- Handling class imbalance using SMOTE

---

# Handling Class Imbalance

Healthcare datasets often contain unequal distribution between diabetic and non-diabetic cases.

To improve model performance and reduce bias:

**SMOTE (Synthetic Minority Oversampling Technique)** was applied.

SMOTE creates synthetic samples for the minority class, helping machine learning models learn better patterns from both classes.

---

# Models Implemented

Multiple classification algorithms were trained and evaluated:

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)
- Naive Bayes
- AdaBoost Classifier
- Gradient Boosting Classifier
- XGBoost Classifier

---

# Hyperparameter Optimization

To improve model performance:

- Hyperparameter tuning was performed using **GridSearchCV**.
- Different parameter combinations were tested using cross-validation.
- The best parameters were selected based on model performance.

The optimized **XGBoost Classifier** achieved the highest performance.

---

# Model Performance

## Best Model: XGBoost Classifier ⭐

| Metric | Score |
|---|---|
| Accuracy | 97% |
| Precision | High |
| Recall | High |
| F1 Score | High |
| ROC-AUC | High |

The XGBoost model provided the best classification performance after hyperparameter optimization.

---


<img width="1920" height="1020" alt="Screenshot 2026-08-05 005133" src="https://github.com/user-attachments/assets/894d3b20-6a5b-4f5c-a89c-540c92ce1c35" />

# Streamlit Deployment

The final trained model was deployed using **Streamlit** to create an interactive prediction application.

## Application Features

- User-friendly interface
- Patient health information input
- Real-time diabetes prediction
- Instant classification result

---

# Technologies Used

## Programming Language

- Python

## Machine Learning Libraries

- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Imbalanced-learn
- Joblib

## Data Visualization

- Matplotlib
- Seaborn

## Deployment

- Streamlit

## Development Tools

- Jupyter Notebook
- VS Code
- Git & GitHub

---

# Project Structure

```
Diabetes-Prediction-System/

│
├── dataset/
│   └── diabetes.csv
│
├── models/
│   ├── xgboost_model.pkl
│   ├── scaler.pkl
│
├── notebooks/
│   └── diabetes_prediction.ipynb
│
├── app.py
├── requirements.txt
└── README.md
```

---

# Installation and Usage

## Clone Repository

```bash
git clone https://github.com/yourusername/Diabetes-Prediction-System.git
```

## Install Dependencies

```bash
pip install -r requirements.txt
```

## Run Streamlit Application

```bash
streamlit run app.py
```

---

# Future Improvements

- Add Explainable AI techniques like SHAP for prediction explanation.
- Deploy the application on cloud platforms.
- Integrate with healthcare management systems.
- Improve model interpretability for medical decision support.

---

# Author

**Amal Dev S**

Data Science | Machine Learning | Artificial Intelligence
