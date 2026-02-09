# AWS S3 Hands On for Machine Learning Pipeline

## Project Overview

This project demonstrates practical usage of Amazon S3 as the storage layer for a Machine Learning pipeline.

The goal of this work is to show hands on experience with S3 concepts including buckets objects permissions versioning and ML data organization.

---

## What I Implemented

I used Amazon S3 to store and manage all artifacts of an ML project.

This includes  
datasets  
trained models  
logs  
outputs  

S3 acted as the central storage across all stages of the ML workflow.

---

## S3 Concepts Covered

What S3 is  
Buckets and objects  
Folder structure logic  
Uploading and downloading data  
Bucket permissions basics  
Public vs private buckets  
Versioning concept  
Why S3 is used in ML pipelines  
Storing datasets  
Storing model artifacts  
Storing logs and outputs  

---

## Bucket Structure Design

The following logical structure was created inside the S3 bucket.

dataset  
raw  
processed  
train  
test  

models  
v1  
v2  

logs  
training  
inference  

outputs  
predictions  
reports  

Note  
These folders are logical paths created using object keys.

---

## Dataset Storage

Raw dataset was uploaded to  
dataset raw  

Processed dataset was uploaded to  
dataset processed  

This separation helps maintain data integrity and reproducibility.

---

## Upload and Download

The dataset was downloaded from S3 and re uploaded to verify object level operations.

This confirms practical experience with S3 upload and download functionality.

---

## Versioning

Bucket versioning was enabled.

Uploading the same file multiple times created multiple versions.

This allows rollback and protects against accidental data loss.

---

## Model Artifacts Storage

After training the ML model locally the trained model file was saved as

model.joblib

This model artifact was uploaded to

models v1

This represents model versioning in a real ML system.

---

## Logs Storage

Training logs were manually created and stored in

logs training

Logs help track training status errors and performance.

---

## Outputs Storage

Model evaluation results and reports were stored in

outputs reports

These outputs represent final results of the ML pipeline.

---

## ML Pipeline Explanation

This project represents a manual ML pipeline.

Flow  
Raw data stored in S3  
Processed data stored in S3  
Model trained locally  
Model artifact stored in S3  
Logs stored in S3  
Outputs stored in S3  

Amazon S3 acts as the backbone storage connecting all stages.

---

## Security and Permissions

The S3 bucket was kept private.

Public access was blocked by default.

Only selected files can be shared if required.

---

## Key Learnings

Understood real world usage of S3 in ML projects  
Designed clean data organization strategy  
Applied versioning for safety  
Used S3 as a pipeline storage layer  

---

## Tools Used

Amazon S3  
Python  
Scikit Learn  
Joblib  

---

## Author

Savan Patel
