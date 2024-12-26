# 2.12-assignment-lambda
Given a Lambda function that is triggered upon the creation of files in an S3 bucket, answer the following:

1.	What is the purpose of the execution role on the Lambda function?
The execution role on the Lambda function grants the permissions to create log group, create log stream and put log events on the Amazon CloudWatch logs.

2.	What is the purpose of the resource-based policy on the Lambda function?
The resource-based policy on the Lambda function grants S3 Bucket permission to invoke function to Lambda.

3.	If the function is needed to upload a file into an S3 bucket, describe (i.e no need for the actual policies)
a.	What is the needed update on the execution role?
Update the Lambda function's execution role to allow it to upload objects to the S3 bucket.
b.	What is the new resource-based policy that needs to be added? To which resource?
Add a resource-based policy to the S3 bucket to allow the Lambda function’s execution role to upload files to the bucket.
