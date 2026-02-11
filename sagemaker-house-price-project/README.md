# 🏠 House Price Prediction using Amazon SageMaker

## 📌 Overview

This project demonstrates a complete end-to-end Machine Learning workflow using Amazon SageMaker to predict house prices.

The objective was to understand how SageMaker fits into the ML lifecycle, including data storage, model training, deployment, evaluation, and AWS cost management.

---

## 🧠 Problem Statement

Build a regression model to predict house prices using structured tabular data.

**Target Variable:**  
Price  

**Input Features:**  
Numeric housing features such as LotArea, OverallQual, SquareFootage, Basement features, and others.

---

## 🏗️ Architecture Workflow

1. Dataset stored in Amazon S3  
2. Development performed in SageMaker Studio  
3. Data preprocessing and train–test split  
4. Model training using SageMaker built-in Linear Learner  
5. Model deployed as real-time endpoint  
6. Predictions generated via endpoint  
7. Model evaluated using RMSE  
8. Endpoint deleted to control AWS cost  

---

## ⚙️ Machine Learning Pipeline

### 1️⃣ Data Storage
- Dataset uploaded to Amazon S3  
- SageMaker training jobs accessed data directly from S3  

### 2️⃣ Train–Test Split
- 80% training data  
- 20% testing data  
- Ensures evaluation on unseen data  

### 3️⃣ Model Training
- Algorithm: Linear Learner (Regression)  
- Instance Type: ml.m5.large  
- Managed training infrastructure  
- Model artifacts stored automatically in S3  

### 4️⃣ Real-Time Deployment
- Model deployed as an inference endpoint  
- Predictions generated using CSV formatted feature input  

### 5️⃣ Evaluation
- Metric Used: Root Mean Squared Error (RMSE)  
- Final RMSE: 40,897  

RMSE represents the average prediction error in dollar value.

---

## 📊 Key Concepts Demonstrated

- End-to-end ML lifecycle on AWS  
- Training vs Inference  
- Real-time endpoint deployment  
- Model evaluation with RMSE  
- IAM-based secure S3 access  
- AWS cost management best practices  

---

## ☁️ AWS Services Used

- Amazon SageMaker  
- Amazon S3  
- IAM (Execution Role)  

---

## 🛠️ Tech Stack

- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- SageMaker Python SDK  

---

## 📷 Screenshots

Screenshots of:
- S3 dataset upload  
- Training job logs  
- Endpoint deployment  
- RMSE evaluation  

Available inside the `screenshots/` folder.

---

## 🎯 What This Project Demonstrates

- Ability to build and deploy ML models in the cloud  
- Understanding of SageMaker architecture  
- Knowledge of proper model evaluation  
- Awareness of AWS resource and cost management  

---

## 👤 Author

Savan Patel
