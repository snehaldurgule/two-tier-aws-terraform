# Two-Tier AWS Architecture using Terraform

## Project Description 
This project aims to create highily available web application infrastructure using a two-tier architecture on Amazon Web Services (AWS). The architecture comprises a web tier that handles user requests and a database tier for data storage. I leveraged Terraform for Infrastructure as Code (IaC) to provision and manage AWS resources efficiently.

## Architecture
- VPC with 2 Public & 2 Private Subnets
- Internet Gateway + Public Route Table
- Application Load Balancer in Public Subnets
- EC2 Instances in Private Subnets
- RDS MySQL in Private Subnets
- Security Groups

## Key Features
Infrastructure as Code (IaC): Leveraging Terraform for defining and provisioning the entire infrastructure, ensuring consistency and repeatability.
High Availability: Utilized multiple Availability Zones (AZs), the application is designed for high availability, minimizing downtime in case of failures.
Security: Implementing security best practices, such as network ACLs, security groups, and encryption, to protect data and resources.
Database Management: A managed database service Amazon RDS is used to store and manage application data, providing reliability and data durability.
Load Balancing: Employing Elastic Load Balancers (ELBs) to distribute incoming traffic across multiple web servers, optimizing resource utilization.

## Tech Stack
AWS, Terraform, EC2, RDS, ALB

## Deploy
terraform init
terraform plan
terraform apply

## Destroy (to save cost)
terraform destroy





