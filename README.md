<h1 align="center">🔐 Secure AWS VPC Deployment (Terraform)</h1>
<p align="center">
  <img src="https://img.shields.io/badge/Cloud-AWS-orange?style=for-the-badge&logo=amazonaws" />
  <img src="https://img.shields.io/badge/IaC-Terraform-7B42BC?style=for-the-badge&logo=terraform" />
  <img src="https://img.shields.io/badge/Security-Enabled-brightgreen?style=for-the-badge&logo=datadog" />
  <img src="https://img.shields.io/badge/Status-Deployed-success?style=for-the-badge&logo=github" />
</p>

<p align="center">
  Deploy a production-grade VPC with Terraform, built for real-world AWS environments and cloud security portfolios.
</p>

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
---

## 💡 What I Practiced / Learned
- Structured Terraform provider/resource blocks
- Created a secure, custom AWS VPC
- Managed infrastructure using Git and Terraform CLI
- Deployed AWS infrastructure without clicking in Console
- Validated deployed VPC through AWS Management Console

---

## 🛠️ What’s Next
- Add public + private subnets
- Deploy a Bastion Host
- Add route tables + IGW/NAT Gateway
- Secure networking with IAM roles and Security Groups
- Integrate tfsec, Bandit, and Snyk for security scanning

---

## 🖥️ Architecture Diagram

> Full infrastructure overview:

![VPC Architecture](https://raw.githubusercontent.com/Cloudby-MB/01-secure-aws-vpc/main/Cloud_VPC_Architecture_Diagram.png)

---

## 🧑‍💻 Author
**Cloudby-MB**  
_Building secure cloud environments with automation-first principles._
