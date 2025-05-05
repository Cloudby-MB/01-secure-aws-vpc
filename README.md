<h1 align="center">🔐 Secure AWS VPC Deployment (Terraform)</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Cloud-AWS-orange?style=for-the-badge&logo=amazonaws" />
  <img src="https://img.shields.io/badge/IaC-Terraform-7B42BC?style=for-the-badge&logo=terraform" />
  <img src="https://img.shields.io/badge/Security-Enabled-brightgreen?style=for-the-badge&logo=datadog" />
  <img src="https://img.shields.io/badge/Status-Deployed-success?style=for-the-badge&logo=github" />
</p>

---

## 📑 Table of Contents
- [Tech Stack](#️-tech-stack)
- [Security Highlights](#-security-highlights)
- [Infrastructure Deployed](#️-infrastructure-deployed)
- [Deploy It Yourself](#-deploy-it-yourself)
- [What I Practiced / Learned](#️-what-i-practiced--learned)
- [What's Next](#️-whats-next)
- [Architecture Diagram](#️-architecture-diagram)
- [Deployment Proof](#️-deployment-proof)
- [Author](#️-author)

---

## ⚙️ Tech Stack
- **☁️ Cloud Provider**: AWS
- **🛠️ IaC Tool**: Terraform (v1.5.7)
- **📍 Region**: us-east-1
- **📦 CIDR**: `10.0.0.0/16`

---

## 🔐 Security Highlights
- Custom VPC only (no default VPC)
- Designed for **least privilege** and **network segmentation**
- Deployable via Git + Terraform CLI (CI/CD friendly)
- Future-ready for compliance tagging (SOC2, GDPR)

---

## 🧱 Infrastructure Deployed
| Resource     | Details          |
|--------------|------------------|
| `aws_vpc`    | Custom VPC with Name tag `MainVPC` |
| CIDR Block   | `10.0.0.0/16`    |
| Region       | us-east-1        |

---

## 🚀 Deploy It Yourself

Clone the repo:

```bash
git clone https://github.com/Cloudby-MB/01-secure-aws-vpc.git
cd 01-secure-aws-vpc
terraform init
terraform plan
terraform apply
```

---

## 💡 What I Practiced / Learned
- Structured Terraform provider/resource blocks properly
- Built a secure, custom VPC
- Used Git + Terraform CLI instead of clicking through AWS Console
- Validated infrastructure through AWS Management Console
- Followed Infrastructure as Code (IaC) best practices

---

## 🛠️ What's Next
- Add public and private subnets
- Deploy a Bastion Host for secure access
- Create route tables and connect to Internet Gateway and NAT Gateway
- Lock down access with IAM roles and Security Groups
- Integrate tfsec, Bandit, and Snyk for security scanning

---

## 🖥️ Architecture Diagram

> Full infrastructure overview:

![VPC Architecture](https://raw.githubusercontent.com/Cloudby-MB/01-secure-aws-vpc/main/Cloud_VPC_Architecture_Diagram.png)

---

## 📸 Deployment Proof

Here is proof of the successful VPC deployment:

![Deployment Proof](deployment-proof-vpc.png)
![Bastion Host Proof](Bastion_Host_Deployment_Proof.png)

---

## 📸 Subnets Deployment Proof

Here is proof of the deployed **Public** and **Private** subnets, as seen in the AWS Management Console:

![Subnets Proof](subnets-proof.png)

---

## 🧑‍💻 Author

**Cloudby-MB**  
_Building secure cloud environments with automation-first principles._