**Terraform Project: AWS 3-Tier Architecture (IaC)**

This repository showcases a **production-grade 3-Tier Architecture** deployed on AWS using **Terraform**. The solution demonstrates deep understanding of **Infrastructure as Code (IaC)** principles, modular Terraform development, and secure cloud architecture patterns.

---

## 1. Project Scope & Objectives

- Design and deploy a **resilient, secure, and scalable 3-tier infrastructure** on AWS  
- Leverage **Terraform** for full automation using reusable and version-controlled code  
- Follow **real-world best practices** in cloud architecture and IaC development  
- Demonstrate expertise in building cloud-native infrastructure with modular design  

---

## 🧱 2. Components & Services Used

| Layer        | AWS Services Used                            |
|--------------|----------------------------------------------|
| **Network**  | VPC, Subnets (public/private), Route Tables, NAT Gateway, IGW |
| **Compute**  | EC2 Instances, Auto Scaling Group, Launch Templates |
| **Database** | RDS (MySQL) in a Multi-AZ Private Subnet     |
| **Security** | Security Groups, Key Pairs, IAM Roles        |
| **Load Balancing** | Application Load Balancer (ALB)         |
| **IaC Tools**| Terraform (v1.x), AWS CLI, Visual Studio Code|

All resources are **parameterized** using Terraform `variables.tf`, and outputs are defined in `outputs.tf`.

---

## 🏗️ 3. Architecture Diagram

![AWS 3-Tier Architecture](architecture.png)

**Tier Breakdown:**

- **Web Tier** → EC2 in Public Subnets + ALB  
- **App Tier** → EC2 in Private Subnets via NAT Gateway  
- **DB Tier** → RDS in Private Subnet with no direct internet access  
- **Multi-AZ** Deployment for High Availability and Fault Tolerance  

---

## 🛠️ 4. Terraform Structure
terraform-aws-3tier-architecture/
│
├── modules/ # Modularized Terraform code
│ ├── vpc/
│ ├── ec2/
│ ├── rds/
│ ├── alb/
│ └── security-groups/
│
├── main.tf # Root Terraform configuration
├── variables.tf # Input variables
├── outputs.tf # Output variables
├── provider.tf # AWS provider & region config
└── README.md # Project documentation


Each module is designed for **clean separation of responsibilities**, making the code reusable and easier to scale.

---

## ✅ 5. Summary: What This Project Demonstrates

> 🧠 This project shows practical knowledge in designing, automating, and securing cloud environments.  
> ⚙️ It reflects real-world workflows, modular Terraform best practices, and AWS architectural depth.  
> 💼 Suitable for Cloud Engineering, DevOps, and Infrastructure-focused roles.

---



