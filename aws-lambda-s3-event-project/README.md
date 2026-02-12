# 🚀 AWS Lambda S3 Event-Driven Serverless Project

## 📌 Project Overview

This project demonstrates an event-driven serverless architecture using AWS Lambda and Amazon S3.

When a file is uploaded to an S3 bucket, the Lambda function is automatically triggered.  
The function processes the event and logs the file details into Amazon CloudWatch.

This project proves understanding of:

- Serverless architecture
- Event-driven execution
- AWS Lambda triggers
- S3 event notifications
- CloudWatch logging
- Lambda limitations concept

---

## 🏗 Architecture

User uploads file  
⬇  
Amazon S3 detects object creation  
⬇  
AWS Lambda is triggered automatically  
⬇  
Execution logs stored in CloudWatch  

---

## 🛠 Technologies Used

- AWS Lambda  
- Amazon S3  
- Amazon CloudWatch  
- Python  

---

## 🪣 Step 1 – Create S3 Bucket

Created an S3 bucket named:

lambda-aws-12

This bucket will generate events when a file is uploaded.

---

## ⚡ Step 2 – Create Lambda Function

Created a Lambda function named:

s3-file-trigger  

Runtime used: Python 3.x  

The function extracts:

- Bucket name  
- Uploaded file name  

And logs the event details.

---

## 🔗 Step 3 – Configure S3 Trigger

Configured the S3 bucket as a trigger for the Lambda function.

Event type selected:

All object create events

This ensures that every new file upload triggers the function.

---

## 📂 Step 4 – Upload File to S3

Uploaded a test file to the S3 bucket to validate the trigger configuration.

---

## 📊 Step 5 – Verify Execution in CloudWatch

Verified successful execution by checking logs in Amazon CloudWatch.

The logs show:

- Event received  
- Bucket name  
- File name  
- Successful execution  

---

## 🧠 Key Concepts Explained

### What is Serverless?

Serverless means developers do not manage infrastructure.  
AWS handles servers, scaling, and availability automatically.

### What is Event-Driven Execution?

The function runs only when an event occurs.  
In this case, the event is an S3 object upload.

### When to Use Lambda?

- File processing automation  
- Backend APIs  
- Scheduled jobs  
- Data transformation  
- Lightweight workloads  

### Lambda Limitations

- Maximum execution time: 15 minutes  
- Limited memory  
- Cold start delay  
- Not suitable for long-running applications  
- Stateless by design  

---

## 🎯 Conclusion

This project demonstrates a real-world serverless event-driven system using AWS services without managing servers.

It showcases practical understanding of cloud-native architecture principles.
