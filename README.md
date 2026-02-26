# E-commerce Purchase Intention Prediction (ML Project)

End-to-End Machine Learning Project | Pipeline | Model Selection | ROC-AUC Optimization

---

##  Project Overview
This project predicts whether an online shopping session will result in a purchase (Revenue) using Machine Learning models.  
The model is built using an end-to-end ML pipeline including preprocessing, feature engineering, and model selection.

Dataset Used: Online Shoppers Intention Dataset (E-commerce user behavior data)

---

## Objective
- Predict customer purchase intention (Revenue: 0 or 1)
- Build a reusable ML Pipeline
- Perform model selection using Cross Validation (ROC-AUC)
- Evaluate model using multiple metrics

---

## Dataset Features
The dataset contains:
- Administrative & Informational Pages
- Product Related Pages
- Bounce Rates & Exit Rates
- Page Values
- Visitor Type
- Month
- Weekend Activity
- Revenue (Target Variable)

---

## Feature Engineering
- Converted Weekend (True/False) → (0/1)
- Converted Revenue (True/False) → (0/1)
- Created Returning_Visitor feature
- Dropped VisitorType column
- Encoded Month column

---

## ML Pipeline Architecture
Pipeline Components:
- SimpleImputer (Missing Values)
- MinMaxScaler (Scaling)
- OneHotEncoder (Categorical Encoding)
- ColumnTransformer (Preprocessing)
- Model Integration

This prevents data leakage and ensures clean workflow.

---

##  Models Used
- Random Forest Classifier
- Decision Tree Classifier
- K-Nearest Neighbors (KNN)
- Bernoulli Naive Bayes
- Support Vector Classifier (SVC)

Model selection done using:
--> 10-Fold Cross Validation with ROC-AUC scoring

---

## 📊 Evaluation Metrics
- ROC AUC Score
- Accuracy Score
- F1 Score
- Classification Report

---

## How to Run This Project
```bash
pip install -r requirements.txt