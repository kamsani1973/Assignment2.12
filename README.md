# Assignment2.12
What is the purpose of the execution role on the Lambda function?
        - Allow logs : Create log Group
        - Allow logs : Create log Stream
        - Allow logs : Put log Events

2. What is the purpose of the resource-based policy on the Lambda function?
        - S3 to allow Lambda Invoke Functions

3. If the function is needed to upload a file onto an S3bucket, describe (i.e no need for the actual policies)
   
Simplified Flow:
Lambda Code -> AWS SDK (authentication) -> IAM(authorization check) -> S3 Service (data transfer & storage) -> 
S3 Response -> Lambda Code (handle result) -> Lambda Exits .
This sequence ensures that data is securely and reliably transferred from your Lambda function to the durable storage of Amazon S3.

    What is the needed update on the execution role?
    Need to Put Object to allow upload Object/files 
     
    What is the new resource-based policy that needs to be added (if any)?
    Specify the ARN of the S3 bucket and its Objects for resource –based policy.


Create a public github repository that has a README.md file, containing the above answers.
Submission is the url to your public github repository.

https://github.com/kamsani1973/Assignment2.12.git




