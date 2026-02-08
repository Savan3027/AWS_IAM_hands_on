Task 2 Custom IAM Policy for Specific S3 Bucket

Objective
To understand how to create a custom IAM policy and apply least privilege by allowing access to only one specific S3 bucket.

What I did
1. Created a custom IAM policy using the Visual Editor
2. Selected Amazon S3 as the service
3. Allowed read actions only
   - ListBucket
   - GetObject
4. Restricted access to a single S3 bucket
5. Attached the policy to an IAM user

Verification
- Able to list objects inside the allowed bucket
- Able to read files from the allowed bucket
- Not able to access other S3 buckets
- Not able to upload or delete objects

Learning
- Custom policies provide fine grained access control
- Resource level permissions are more secure than full service access
- Least privilege means giving only what is required
