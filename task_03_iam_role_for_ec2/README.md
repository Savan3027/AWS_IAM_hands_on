Task 3 IAM Role for EC2

Objective
To understand IAM roles and how EC2 can access AWS services using a role.

What I did
1. Created an IAM role for EC2 service
2. Selected AWS service as trusted entity
3. Attached AmazonS3ReadOnlyAccess policy
4. Created the role with name ec2-s3-read-role

Verification
The IAM role was successfully created
The role is visible in IAM roles list

Learning
IAM role is used by AWS services
EC2 can assume a role without username or password
Roles follow the least privilege principle
