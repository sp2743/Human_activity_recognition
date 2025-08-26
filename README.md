Human Activity Recognition Using Smartphone Sensors

# 📌 Overview

This project focuses on developing a Human Activity Recognition (HAR) system using smartphone sensor data (accelerometer and gyroscope). The goal is to classify six daily activities:
🚶 Walking
🧗 Walking Upstairs
🏃 Walking Downstairs
🪑 Sitting
🙆 Standing
🛌 Laying

We use the UCI HAR Dataset and apply classical machine learning models with feature selection and optimization to achieve high accuracy while ensuring computational efficiency for real-time applications.

# 📊 Dataset
Source: UCI HAR Dataset
Participants: 30 volunteers (ages 19–48)
Sensors: Accelerometer & Gyroscope (Samsung Galaxy S II)
Sampling Rate: 50 Hz
Features: 561 extracted features (time & frequency domain)
Classes: 6 activities

Data is pre-processed with filtering, windowing, and feature extraction.

# ⚙️ Methodology
## 1. Data Preprocessing
Cleaning missing/duplicate values
Feature engineering (PCA, RFE, SelectKBest)
Normalization for model input

## 2. Model Selection
We trained and compared the following models:
Logistic Regression
Support Vector Machines (SVM)
Decision Tree
Random Forest
AdaBoost

## 3. Hyperparameter Tuning
GridSearchCV used for SVM and Logistic Regression
Cross-validation for robustness

🏗️ Project Structure
├── Human_activity_recognition.ipynb   # Jupyter Notebook with implementation
├── README.md                          # Project documentation

# 📈 Results
Model	Accuracy	Precision	Recall	F1-Score
Logistic Regression	0.96	0.96	0.96	0.96
SVM (Optimized)	0.97	0.97	0.97	0.97
Random Forest	0.93	0.93	0.93	0.93
Decision Tree	0.86	0.86	0.86	0.86
AdaBoost	0.35	0.15	0.35	0.21

# 🔑 Key Findings:
SVM with RBF kernel and tuned hyperparameters achieved the best performance (97% accuracy).
Feature reduction (PCA, RFE, SelectKBest) helped improve efficiency without major performance loss.

# 🚀 Future Work
Integrate deep learning models (CNN-LSTM, Transformers) for sequential dependencies.
Extend dataset with diverse demographics & activities.
Implement real-time HAR on mobile devices.
