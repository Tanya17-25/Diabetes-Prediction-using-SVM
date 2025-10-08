# Diabetes-Prediction-using-SVM 🩺

A Python project that uses Support Vector Machine (SVM) to predict whether a person has diabetes based on medical measurements. Built using the PIMA Diabetes Dataset.

## Project Overview

This project implements a supervised learning model to classify if a person is diabetic or not, based on health features such as glucose level, blood pressure, BMI, insulin, age, etc. The core algorithm is a linear Support Vector Machine (SVM).

## Motivation

- Diabetes is a serious health issue worldwide. Early detection and prediction can help in timely intervention.  
- Building this model helps me understand end-to-end ML pipeline: from data preprocessing to model deployment.  
- It is also a good showcase project for machine learning, data science, and health-tech use cases.

## Dataset

- I used the **PIMA Indians Diabetes Dataset**  
- The dataset consists of medical predictor variables and one target variable “Outcome” (0 = non-diabetic, 1 = diabetic).  
- The features include:  
  > Pregnancies, Glucose, BloodPressure, SkinThickness, Insulin, BMI, DiabetesPedigreeFunction, Age  

## Methodology / Workflow

1. **Data Loading & Exploration** – Load dataset, view head, descriptive statistics, class balance  
2. **Data Preprocessing** – Standardize / scale features using `StandardScaler`  
3. **Train – Test Split** – Split data into 80% training and 20% testing (with stratification)  
4. **Model Training** – Train an SVM (kernel = linear) on training set  
5. **Model Evaluation** – Evaluate performance via accuracy on train and test data  
6. **Predictive System** – Accept new input data, preprocess, and output prediction  

## Model

**Support Vector Machine (SVM)**  
- SVM is a supervised learning algorithm used for classification (and regression) tasks.  
- It attempts to find an optimal hyperplane that maximizes the margin between classes.  
- In high-dimensional spaces, SVM is effective and tends to generalize well.  

I used a **linear kernel** for this problem, as the features are standardized and the classes are fairly separable in this setting.

## Results & Evaluation

- **Training Accuracy**: 78% 
- **Test Accuracy**: 72%  

These metrics show how well the model fits the training data and how well it generalizes to unseen data.  
You can further evaluate with metrics like precision, recall, F1-score, ROC-AUC if needed.
