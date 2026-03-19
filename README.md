### NAME: SURYA P <br>
### REG NO: 212224230280 <br> 
### Date: 18/03/2026

## EX. No. 6 : Scale & Load balance your Architecture

---

## Objective

The objective of this lab is to understand how to design a scalable and highly available architecture on AWS using Auto Scaling and Elastic Load Balancing. This experiment focuses on distributing incoming traffic across multiple EC2 instances, automatically scaling resources based on demand, and validating fault tolerance.

---

## Prerequisites

* Basic knowledge of Amazon EC2 and VPC
* Completion of previous labs (IAM, EC2, EBS, Database Server)
* AWS Academy Lab access
* Stable internet connection

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Elastic Load Balancer (ELB / ALB)
* Auto Scaling Groups (ASG)
* Amazon CloudWatch

---

## Tasks Performed

### Task 1: Review Existing Architecture

Students review the existing EC2-based application architecture created in previous experiments.

### Task 2: Create a Launch Template

Students create a launch template that defines the EC2 instance configuration including AMI, instance type, security group, and user data.

### Task 3: Create an Auto Scaling Group

Students create an Auto Scaling Group using the launch template and configure minimum, maximum, and desired instance capacity.

### Task 4: Configure an Application Load Balancer

Students create an Application Load Balancer and configure target groups for routing traffic to EC2 instances.

### Task 5: Register Auto Scaling Group with Load Balancer

Students attach the Auto Scaling Group to the target group of the load balancer.

### Task 6: Configure Scaling Policies

Students configure scaling policies based on CPU utilization using Amazon CloudWatch alarms.

### Task 7: Test Load Balancing and Scaling

Students test the setup by generating traffic and observing automatic scaling and load distribution.

---

## Workflow (To be filled by Student)

1. Open the AWS Management Console and navigate to the EC2 dashboard.

2. In the left panel, select Instances and verify that Web Server 1 is in a running state (2/2 status checks passed).

3. Select Web Server 1, then go to Actions → Image and templates → Create image.

4. Enter the required details:

    Image Name: WebServerAMI
    Description: Lab AMI for Web Server

5. Click Create image to generate the AMI, which will be used later for Auto Scaling.

---

## Output Screenshots 

Creation of AMI from EC2 Instance (Web Server 1)

<img width="1255" height="559" alt="image" src="https://github.com/user-attachments/assets/b0c7e301-e9c3-4664-8fc5-bcdb1c4e2ba3" />

Application Load Balancer and Target Group Configuration

<img width="1191" height="548" alt="image" src="https://github.com/user-attachments/assets/fc6b4f06-c421-4a60-95dd-cebcb6e5489e" />

Auto Scaling Group with Dynamic Instance Scaling

<img width="1188" height="350" alt="image" src="https://github.com/user-attachments/assets/b86a82e8-7eca-428d-8f89-4b393544f579" />


<img width="1175" height="421" alt="image" src="https://github.com/user-attachments/assets/ee2bb251-7ba8-4d85-be1f-4be3f370cb61" />


<img width="1204" height="401" alt="image" src="https://github.com/user-attachments/assets/0676c9e5-4266-4e3a-bd99-519cc2121b9b" />

Instance Termination

<img width="1254" height="594" alt="image" src="https://github.com/user-attachments/assets/276e8005-52dc-4c05-a521-9c6a6d342d78" />

---


## Result

This experiment demonstrated how to build a scalable and fault-tolerant cloud architecture using Auto Scaling Groups and Elastic Load Balancing. The system automatically adjusted resources based on workload and ensured continuous service availability by distributing traffic across multiple instances.
