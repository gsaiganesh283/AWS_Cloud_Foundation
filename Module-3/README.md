# AWS Global Infrastructure Overview

## AWS Global Infrastructure

  - The AWS global infrasturcture is ddesigned and bulit to deliver a **Flexible, Reliable, Scalable, and Secure** cloud computing environment with high-quality global network performance.

## AWS Regions

  - An AWS Region is a geographical area
    - Data replication across regions is controlled by you.
    - Communication between region uses AWS backbone network infrastructure.
  - Each region provides full redundancy and connectivity to the network.
  - A region typically consists of two or more availability zones.

### Selecting a Region
  Determine the right region for your services, applications, and data based on these factors
  - Data goverance, legal requirements
  - Proximity to customers
  - Services available within the region
  - costs (vary by region)

### Availability Zones
  - Each region has multiple availability zones.
  - Each availability zone is a fully isolated partition of the AWS infrastructure.
    - There a currently 69 availability zones workload.
    - Availability zones consists of discrete data centres
    - They are designed for fault isolation.
    - They are interconnected with other availability zones by using high-speed private networking.
    - You choose your availability zones.
    - AWS recommends replicating data and resources across availability zones for resiliency.
## AWS Data Centers
  - AWS data centers are designed for security.
  - Data centers are where the data resides and data processing occurs.
  - Each data center has redundent power, networking, and connectivity, and is housed in a separate facility.
  - A data center typically has 50,000 to 80,000 physical servers.

##
- AWS provides a global network of 187 points of presence locations.
- Consists of 176 edge locations and 11 regional edge caches.
- Used with Amazon CloudeFront
  - A global content Devlivert network (CDN) that ddelivers content to end users with reduced latency.
- Reginal edges caches used for content with infrequent access.

## AWS Infrastucture Features
- **Elasticity and Scalability**
  - **Elastic infrsturucture:** dynamic adaption of capacity
  - **Scalable infrasturcture:** adapts to accommodate growth
- **Fault-tolerance**
  - Continues operating properly in the presence of a failure.
  - Bulit-in redundancy of components.
- **High availability**
  - High level of operational performance
  - Minimized downtime
  - No human intervention

## AWS Services and service category overview
### Storage service category
- Amazon Simple Storage Service (Amazon S3)
- Amazon Elastic Block Store (Amazon EBS)
- Amazon Elastic File System (Amazon EFS)
- Amazon S3 Glacier
### Compute Servie Category
- Amazon Elastic Cloud Computing (Amazon EC2)
- Amazon EC2 Auto-Scaling
- Amazon Elastic Container Service (Amazon ECS)
- Amazon EC2 Container Registry
- Amazon Elastic Beanstalk
- AWS Lambda
- Amazon Elastic Kubernets Service (Amazon EKS)
- AWS Fargate
### Database Service Caterogry
- Amazon Relational Database service
- Amazon Aurora
- Amazon Redshift
- Amazon DynamoDB
### Networking and Content delivery service category
- Amazon Virtual Private Cloud (Amazon VPC)
- Elatic Load Balancing
- Amazon Cloud Front
- AWS Transit Gateway
- Amazon Route S3
- AWS Direct Connect
- AWS Virtual Private Network (Amazon VPN)
### Security, Identity, and Compliance Service Category
- AWS Identity and Access Management (Amazon IAM)
- AWS Organization
- Amazon Cognito
- AWS Artifact
- AWS Key Management Service
- AWS Shield
### AWS Cost Managemnt Service Category
- AWS Cost and Usage Report
- AWS Budgest
- AWS Cost Explorer
### Management and Governace Service Category
- AWS Management Console
- AWS Config
- Amazon CloudWatch
- AWS Auto-Scaling
- AWS Command Line Interface
- AWS Trusted Advisor
- AWS Well-Architected Tool
- AWS Cloud Trail
