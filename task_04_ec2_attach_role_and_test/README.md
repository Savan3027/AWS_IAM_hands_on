EC2 Attach IAM Role and Test S3 Access

Objective  
To understand how EC2 uses IAM Roles to access AWS services securely without access keys.

What I did  

Created an IAM Role for EC2  
Attached S3 read only permissions to the role  
Attached the role to a running EC2 instance  
Connected to EC2 using Session Manager  
Installed AWS CLI on EC2  
Verified role access using AWS STS  

Verification  

AWS CLI installed successfully  
aws sts get-caller-identity worked  
EC2 assumed the IAM role successfully  
Confirmed S3 access using IAM Role without access keys  

Learning  

IAM Roles are the secure way to grant permissions to EC2  
No need to store access keys on servers  
STS shows which role EC2 is currently using  
This follows AWS best security practices
