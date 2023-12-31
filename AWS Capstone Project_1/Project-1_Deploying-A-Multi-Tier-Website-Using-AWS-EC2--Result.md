# Deploying-A-Multi-Tier-Website-Using-AWS-EC2

Description:
Amazon Elastic Compute Cloud (Amazon EC2) provides scalable computing
capacity in the Amazon Web Services (AWS) cloud. Using Amazon EC2
eliminates your need to invest in hardware up front so you can develop and
deploy applications faster. You can use Amazon EC2 to launch as many or as
few virtual servers as you need, configure security and networking, and manage
storage. Amazon EC2 enables you to scale up or down to handle changes in
requirements or spikes in popularity, reducing your need to forecast traffic.

Requirements:
Company ABC wants to move their product to AWS. They have the following
things set up right now:
1. MySQL DB
2. Website (PHP)
The company wants high availability on this product, therefore wants Auto
Scaling to be enabled on this website.
Steps To Solve:
1. Launch an EC2 Instance
2. Enable Auto Scaling on these instances (minimum 2)
3. Create an RDS Instance
4. Create Database & Table in RDS instance:
a. Database name: intel
b. Table name: data
c. Database password: intel123
5. Change hostname in website
6. Allow traffic from EC2 to RDS instance
7. Allow all-traffic to EC2 instance

# Implementation
![Project-1-result-1](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/f5ba45e7-665b-43f8-bc5e-a532845ba21d)
![Project-1-result-02](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/de3a268f-bbff-4d46-a82b-4c0780358d01)
![Project-1-result-2](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/1b1882ba-5eb6-4404-a1a4-db8d379ea61a)
![Project-1-result-2a](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/2b0fa061-20b0-411b-910e-5e40b8598db4)
![Project-1-result-2aa](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/b716e128-7d9d-42eb-a30d-89b6b3dd942c)
![Project-1-result-2b](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/15be843e-2a92-4351-a01b-870912fe6bd0)
![Project-1-result-2c](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/15ab8297-c4a1-455f-b18b-4af396c0f4d6)
![Project-1-result-2d](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/ee95877b-6b84-42b8-bed0-abc94eec453b)
![Project-1-result-3](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/9145a80d-a645-411b-b869-4c517f9b97ec)
![Project-1-result-4](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/d352eb23-41aa-4e57-b118-bac9a441b5b8)
![Project-1-result-5](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/e217f7d2-be6a-4a62-af9f-0fef74a1834a)
![Project-1-result-6](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/def4529f-d90b-4b7b-acfc-db0f45ac6101)
![Project-1-result-7](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/e5b84819-c8a2-484f-b26d-ed290e3d7f47)
![Project-1-result-8](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/c89cfdc2-fac4-4bbf-86fd-9c6b7d8c329e)
![Project-1-result-9](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/60521873-0047-43f9-8cdb-64b46d16bcc3)
![Project-1-result-10](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/b667a705-3d30-42c3-b618-88760b217baf)
![Project-1-result-11](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/061e1b71-0e3b-4463-96fa-535b34a1ec06)
![Project-1-result-12](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/75cc10f6-5103-4bda-a752-bc53a26d6212)
![Project-1-result-12a](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/79652abd-4105-4270-90c4-25aeda96d9cc)
![Project-1-result-13](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/07e55589-7b1f-45ae-a557-5a2e479c2dc7)
![Project-1-result-14](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/0f06aa6c-a261-454f-9118-59b0bc52335f)

