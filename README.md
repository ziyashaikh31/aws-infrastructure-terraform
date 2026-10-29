# 🏗️ Two-Tier AWS Infrastructure with Terraform  

![Two-Tier Architecture](https://imgur.com/X4dGBg6.gif)



## 📌 Project Overview

This project focuses on provisioning a two-tier AWS infrastructure using **Terraform (Infrastructure as Code)**. It demonstrates automated infrastructure provisioning, cloud networking, load balancing, scalability, and database integration using AWS services.

## 🎯 Problem Statement

Manual AWS infrastructure setup is time-consuming and prone to errors. This project uses Terraform to automate the provisioning of AWS networking, compute resources, load balancing, Auto Scaling, and database services for consistent and scalable infrastructure management.

## ✨ Key Features

- **Infrastructure as Code:** Automates AWS resource provisioning using Terraform.
- **Modular Configuration:** Organizes infrastructure code into reusable modules.
- **Network Isolation:** Uses VPCs and public and private subnets.
- **Load Balancing:** Distributes application traffic through an Application Load Balancer (ALB).
- **Auto Scaling:** Configures EC2 Auto Scaling for application capacity.
- **Database Integration:** Provisions an Aurora MySQL database cluster.
- **Security:** Configures IAM roles, policies, and security groups.

## 🛠️ Technologies Used

- Amazon Web Services (AWS)
- Terraform
- Amazon VPC
- Amazon EC2
- Application Load Balancer (ALB)
- EC2 Auto Scaling
- Amazon Aurora MySQL
- AWS IAM
- Amazon CloudWatch
- Git and GitHub

## 🏗️ Architecture

The infrastructure is designed around two tiers:

- **Application Tier:** EC2 instances distributed across subnets and managed through an Application Load Balancer and Auto Scaling.
- **Database Tier:** An Aurora MySQL database cluster intended to provide managed relational database services.
- **Networking and Security:** VPC networking, subnet configuration, route tables, security groups, and IAM permissions.

*Note: This describes the intended infrastructure design. AWS resources have been destroyed, so the infrastructure is not currently running.*

## 🚀 Getting Started

### Prerequisites

- An AWS account
- Terraform installed (version 1.0 or later)
- AWS CLI installed and configured
- Appropriate AWS IAM permissions

### 1. Clone the Repository

```bash
git clone https://github.com/ziyashaikh31/aws-infrastructure-terraform.git
cd aws-infrastructure-terraform
```

### 2. Configure Variables

Review `variables.tfvars` and update the values according to your AWS environment. Use a secure database password and never commit credentials or secrets to GitHub.

### 3. Initialize Terraform

```bash
terraform init
```

### 4. Review the Execution Plan

```bash
terraform plan -var-file="variables.tfvars"
```

### 5. Deploy the Infrastructure

```bash
terraform apply -var-file="variables.tfvars"
```

Review the plan before approving the deployment. AWS charges may apply.

### 6. Destroy Resources

When finished, remove the resources managed by Terraform to help avoid ongoing costs:

```bash
terraform destroy -var-file="variables.tfvars"
```

Review the destruction plan before confirming. Check separately for any resources left behind.

## 📁 Project Structure

The repository contains Terraform configuration and supporting project files. The exact structure may vary depending on the files present in the repository.

- `main.tf` — Main Terraform configuration and resource or module definitions.
- `variables.tf` — Input variable declarations.
- `variables.tfvars` — Environment-specific variable values.
- `modules/` — Reusable Terraform modules, if included.

## 🌐 Project Links

- **GitHub Repository:** [AWS Infrastructure with Terraform](https://github.com/ziyashaikh31/aws-infrastructure-terraform)
- **Website:** [View Website](https://ziyashaikh31.github.io/aws-infrastructure-terraform/index.html)

*The website link opens the static portfolio template published through GitHub Pages. It does not represent a currently running AWS infrastructure deployment.*

## 👨‍💻 Author

**Shaikh Ziya**

- GitHub: [ziyashaikh31](https://github.com/ziyashaikh31)
- LinkedIn: [Ziya Shaikh](https://www.linkedin.com/in/ziya-shaikh-za9699/)

