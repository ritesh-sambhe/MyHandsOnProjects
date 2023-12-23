# Scalable Serverless Web Backend for Cleaning Supplies E-commerce Platform

Actions performed to address Scalable Serverless Web Backend for Cleaning Supplies E-commerce Platform

Led the design and implementation of a serverless web backend on AWS to meet the dynamic needs of a client in the cleaning supplies industry.
Successfully addressed the client's requirement for scalable infrastructure, utilizing AWS Lambda for serverless compute and AWS API Gateway for efficient API management.
Implemented event-driven architecture to ensure decoupling of application components, enhancing flexibility and maintainability.
Achieved optimal scalability and responsiveness, handling demand spikes seamlessly.
Provided comprehensive documentation and training to ensure the client's team could effectively manage and extend the solution.
# Architecture To Be Implemented
![EDA-Question](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/f7a8cc3a-042e-428e-8b1b-14e21b227bb5)

![EDA-Question2](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/71612ff6-e382-451a-98c9-f24b2f85fe35)

![EDA-Result-01](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/f91cb7f6-4c68-4662-8ed9-be29be281a3e)

# Used IAM Policies
#1st Policy- Lambda-Write-DynamoDB
![image](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/6801cbaa-0a67-42ee-8790-61d8f8b063a8)

#2nd Policy- Lambda-SNS-Publish
![image](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/ae3f58a4-2fe4-4e66-8afe-900ddde7b93e)

#3rd Policy- Lambda-DynamoDBStreams-Read
![image](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/bb77d534-deb2-4b34-a3ac-6961454a5f9d)

#4th Policy- Lambda-Read-SQS
![image](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/872f5cb5-9912-4e9a-9b1c-fc7bed4e0a42)

# Creating Roles, in Total 3-Roles We Are Creating Roles as Mentioned Below.

Creating IAM roles and attaching policies to the roles
Because AWS follows the principle of least privilege, we recommend that you provide role-based access to only the AWS resources that are required to perform a task. In this step, you create IAM roles and attach policies to the roles.

In the navigation pane of the IAM dashboard, choose Roles.

Choose Create role and in the Select trusted entity page, configure the following settings:
Trusted entity type: AWS service
Common use cases: Lambda
Choose Next.

On the Add permissions page, select Lambda-Write-DynamoDB and Lambda-Read-SQS.

Choose Next
For Role name, enter Lambda-SQS-DynamoDB(#1st Role)

Choose Create role.

Follow the previous steps to create two more IAM roles:

An IAM role for AWS Lambda: This role grants permissions to obtain records from the DynamoDB streams and send the records to Amazon SNS. Use the following information to create the role.

IAM role name: Lambda-DynamoDBStreams-SNS(2nd Role)

Trusted entity type: AWS service
Common use cases: Lambda
Attach policies: Lambda-SNS-Publish and Lambda-DynamoDBStreams-Read
An IAM role for Amazon API Gateway: This role grants permissions to send data to the SQS queue and push logs to Amazon CloudWatch for troubleshooting. Use the following information to create the role.

IAM role name: APIGateway-SQS(#3rd Role)

Trusted entity type: AWS service
Common use cases: API Gateway
Attach policies: AmazonAPIGatewayPushToCloudWatchLogs.

![EDA-Result-02](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/3036daf8-7910-4254-b5e3-d24036871977)
![EDA-Result-03](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/bb86c171-6135-451f-ade3-af4d36a3a298)
![EDA-Result-04](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/7111fefa-00c5-40be-a0d8-bb19108c6514)
![EDA-Result-5](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/ad28eb19-371a-4ce3-9981-2142f42d848d)
![EDA-Result-6](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/73e79727-66a6-4118-9777-9b9375645aac)
![EDA-Result-7](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/9bd6de4a-e653-4864-ba98-843e59234ea7)
![EDA-Result-8](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/54b05a01-ffbd-4c18-8a10-97208a57ffd2)
![EDA-Result-09](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/bbdc1ee0-35c9-46fb-8baf-100e029fc8ed)
![EDA-Result-10](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/bc50df54-46c2-46a5-8337-2d352e0a4f9b)
![EDA-Result-11](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/e2e81bc1-19af-4551-b46e-08138a8ee071)
![EDA-Result-12](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/de0f113b-3239-45af-90d1-b77c94d3b450)
![EDA-Result-13](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/70ba501c-e1ea-4511-a94c-4af87ada8167)
![EDA-Result-14](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/9e0a1055-9206-4dd7-9bd7-cba5bee04271)
![EDA-Result-15](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/524de598-9698-490f-aee7-ad75df8bf7b5)
![EDA-Result-16](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/ecb6bca9-e05e-4c5f-8a1c-172e54fa607f)
![EDA-Result-17](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/ad20337b-5757-40ac-b3ea-34985df325a2)
![EDA-Result-18](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/225b768a-94c6-49c3-98b7-66bc6fc56074)
![EDA-Result-19](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/c5905d62-9211-43c4-a5cc-b9c29345f84d)
