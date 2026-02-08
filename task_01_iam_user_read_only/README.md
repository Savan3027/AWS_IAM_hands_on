## Task 1 IAM User with S3 Read Only Access

### Objective
To understand IAM users, managed policies, and the principle of least privilege by granting read only access to Amazon S3.

---

### What I did
1. Created a new IAM user for practice
2. Attached the AWS managed policy AmazonS3ReadOnlyAccess
3. Logged in to AWS using the IAM user credentials
4. Accessed the Amazon S3 service

---

### Verification
1. Able to list S3 buckets
2. Able to open a specific S3 bucket
3. Able to view folders and files
4. Upload operation was denied
5. Delete operation was denied

This confirms that the IAM user has read only permissions.

---

### Learning
1. IAM user represents a human identity in AWS
2. By default, all permissions are denied
3. Permissions must be explicitly granted using policies
4. Read only access follows the least privilege principle
5. AWS managed policies are useful for standard access control

---

### Screenshots
All verification screenshots for this task are available in the screenshots folder.
