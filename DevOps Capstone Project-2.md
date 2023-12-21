# DevOps Implementation for Scalable Docker Container Deployment

# Requirement
You are hired as a DevOps engineer for Analytics Pvt Ltd. This company is a product based organization which uses Docker for their containerization needs within 
the company. The final product received a lot of traction in the first few weeks of launch. Now with the increasing demand, the organization needs to have a 
platform for automating deployment, scaling, and operations of application containers across clusters of hosts, As a DevOps engineer, you need implement a DevOps 
life cycle, such that all the requirements are implemented without any change in the Docker containers in the testing environment.
Up until now, this organization used to follow a monolithic architecture with just 2 developers. The product is present on
https://github.com/hshar/website.git
Following are the specifications of life-cycle:
1. Git workflow should be implemented. Since the company follows monolithic architecture of Development you need to take care of version control. The release should happen only on 25th of every month.
2. Code build should be triggered once the commits are made in the master Branch.
3. The code should be containerized with the help of the Docker file, The Dockerfile should be built every time if there is a push to Git-Hub. Create a custom Docker image using a Dockerfile.
4. As per the requirement in the production server, you need to use the Kubernetes cluster and the containerized code from Docker hub should be deployed with 2 replicas. Create a NodePort service and configure the same for port 30008.
5. Create a Jenkins pipeline script to accomplish the above task.
6. For configuration management of the infrastructure, you need to deploy the configuration on the servers to install necessary software and configurations.
7. Using Terraform accomplish the task of infrastructure creation in the AWS cloud provider.

#Architectural Advice

Software’s to be installed on the respective machines using configuration management.
Worker1: Jenkins, Java.
Worker2: Docker, Kubernetes.
Worker3: Java, Docker, Kubernetes
Worker4: Docker, Kubernetes.

![image](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/9a6c4527-0ac4-4395-8f4a-a8161eca8c3f)

![image](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/2eba458e-5520-4106-ad4f-0f13baf2a3b6)
