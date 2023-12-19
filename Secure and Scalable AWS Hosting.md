# Secure and Scalable AWS Hosting
Customer Requirement:
A firm wants to launch their new application. To reduce cost it has been decided
that the entire application will be hosted on AWS. It’s a photo and video storage
application. This application will store movies and videos, and customers can also
upload photos and their custom made videos using this application.
To buy videos, movies and wallpapers stored in the application customers have to
pay some amount using their credit card. Customer will have to provide their
home address and some other personal information as well.
Following are some of the requirements:
1. The most important requirement is that the application should be very
much secure and none of the servers (front-end UI, back-end application,
database) should be available over Internet.
2. Application should handle sudden spike in customer activity without any
problem.
3. Customer information should be kept secure as much as possible.
4. It has been decided that 2 types of NoSQL databases would be used to
store metadata information about videos and photos. 3 Relational
databases would be used for transactional purposes.
5. Performance is vital for the success of the product. Make sure that users
get low latent responses wherever possible.
6. Photos and videos should be stored securely at rest.
7. Access to AWS resources should be authorized as per business need, e.g.
application developers should not have access to database servers. DBAs
should not have any access to application servers.
8. Whenever customer uploads a photo/video he or she should get an email
notification.
9. Photos/videos older than 2 years should be archived to save cost.
10. Application should be highly available. It should not go down in the event
of any data center failure. Disaster Recovery has to be set up to mitigate
regional failures as well.
11. Transactions should be as secure as possible.
12. All the SysOps out there configure and use AWS CLI to provision all
services.

Steps:
Setup VPC for Load Balancer, Application EC2 instance and RDS Database - one public and two private subnets.
• Create Load balancer and Auto Scaling Group.
• Create RDS DB instance and DynamoDB table.
• S3 Bucket
• Get domain name and map it with Load Balancer
• Create instance profile that has to be attached to the EC2 instances being launched. Instance profile should have
permission to access RDS, DynamoDB and S3 bucket.
• Lambda function to get triggered when an object is uploaded to the bucket
• SNS Topic for Lambda and user email id subscription
# Technical Architecture
![Technical-Architecture-Of-Project](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/134cbed2-28c6-4d6e-a904-ab8ebf639c3e)
![AWS Case Study-NEW-Result-01](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/469406c0-a55c-4a7d-8316-4b34c5b6a645)
![AWS Case Study-NEW-Result-02](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/e8f8e946-d97d-43f7-b728-9619cbb43c2b)
![AWS Case Study-NEW-Result-03](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/5067a0c3-cd03-4d14-90e0-6b9fd1918184)



