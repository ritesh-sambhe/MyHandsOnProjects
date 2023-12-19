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
![image](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/8e0a3a2a-7356-4829-92fc-89c9fd0c4c33)
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
![AWS Case Study-NEW-Result-04](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/24532f14-1196-4cce-ad18-960bf14195e0)
![AWS Case Study-NEW-Result-05](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/01f8a2a1-49a8-4827-866a-bb88d0d4576f)
![AWS Case Study-NEW-Result-06](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/49fb6d12-49d2-47f1-a5d4-8300f0bc6cc8)
![AWS Case Study-NEW-Result-07](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/899a8549-485c-404b-b7ca-3d1384ccc510)
![AWS Case Study-NEW-Result-08](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/fb10ff39-0a17-472b-8d11-89af6f06a3bc)
![AWS Case Study-NEW-Result-09](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/cdd495d1-a1e6-47cf-9d72-52d3ccc7b355)
![AWS Case Study-NEW-Result-10](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/2cfc54f9-2650-4b66-b7a2-2b9203243f24)
![AWS Case Study-NEW-Result-11](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/71f15a41-2594-4fa3-b787-d5090b227071)
![AWS Case Study-NEW-Result-12](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/379af235-ba7d-4988-8c15-2baa9dd4bb47)
![AWS Case Study-NEW-Result-13](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/a4cec039-26ee-45c6-997f-fb79b4363953)
![AWS Case Study-NEW-Result-14](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/e0877b1b-1c3b-427c-aeed-7433e37fd07f)
![AWS Case Study-NEW-Result-15](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/68f9452f-1700-4723-a8eb-8be6936af87c)
![AWS Case Study-NEW-Result-16](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/ec9bcc47-27ab-4798-b557-5d9263effc0a)
![AWS Case Study-NEW-Result-17](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/7a61902b-c673-4472-8929-801c9f33b8df)
![AWS Case Study-NEW-Result-18](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/c545093d-694d-47c3-b9a0-f6a5153055ab)
![AWS Case Study-NEW-Result-19](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/b3619cee-d8d6-4c5f-a9e6-75c9031e1b62)
![AWS Case Study-NEW-Result-20](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/2c4dc2ba-b0ad-455f-a667-3257c5224bcf)
![AWS Case Study-NEW-Result-21](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/ebf75332-a762-463c-ab79-df556ba26125)
![AWS Case Study-NEW-Result-22](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/cfb89d9a-76e4-4e01-a51c-513ba55a7cbc)
![AWS Case Study-NEW-Result-23](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/6fac2603-0c03-4fbc-a2ca-494cd770b5ad)
![AWS Case Study-NEW-Result-24](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/671cea58-ff4d-4034-97b2-76d238071032)
![AWS Case Study-NEW-Result-25](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/a227734a-a8c5-4997-9a7b-da5f753b273c)
![AWS Case Study-NEW-Result-26](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/61784e64-a72c-45bc-a527-14dbf936192e)
![AWS Case Study-NEW-Result-27](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/54c2e4ed-c3de-41d8-aa9b-428073a6ab45)
![AWS Case Study-NEW-Result-28](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/96b62be0-3f42-4f66-b6bd-4ab8565d31b3)
![AWS Case Study-NEW-Result-29](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/9477d962-6e4e-4ad9-8f94-ade9d1c4c2b5)
![AWS Case Study-NEW-Result-30](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/fa289685-0de6-4a25-b418-21ce22aa91f6)
![AWS Case Study-NEW-Result-31](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/beb55dda-1563-45dd-846f-11c7aaade2d7)
![AWS Case Study-NEW-Result-32](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/5a60cee5-888e-4dd7-a74b-9a8ceb5ffc3f)
![AWS Case Study-NEW-Result-33](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/613a9e26-f062-4ce5-b70d-ddcdeabd7aa7)
