# 01-secure-aws-vpc
Terraform project to deploy a secure AWS VPC with EC2, public/private subnets, and a Bastion host.
# Secure AWS VPC Deployment (Terraform)

This project provisions a secure Virtual Private Cloud (VPC) on AWS using Terraform.

## 🛠️ Tech Stack
- **Cloud Provider:** AWS
- **Infrastructure as Code:** Terraform (v1.5.7)
- **Region:** us-east-1
- **VPC CIDR:** 10.0.0.0/16

## 🔐 Security Focus
- Infrastructure is defined and deployed as code
- No use of default VPC (custom VPC only)
- Project set up for secure subnets, routing, and tagging
- Deployed using Terraform from a Git-tracked repo (CI-ready)

## 📦 Resources Created
- 1x Custom AWS VPC with name tag: `MainVPC`
- Prepped for future additions:
  - Public + private subnets
  - Internet Gateway / NAT Gateway
  - Bastion Host

## 🚀 How to Deploy
1. Clone this repo:
   ```bash
   git clone https://github.com/Cloudby-MB/01-secure-aws-vpc.git
   cd 01-secure-aws-vpc