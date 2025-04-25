<h1 align="center">🔐 Secure AWS VPC Deployment (Terraform)</h1>

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

## 📸 Deployment Screenshot (Optional)
> _You can upload a screenshot of your VPC here to show proof of work!_

---

## 🧑‍💻 Author
**Cloudby-MB**  
_Building secure cloud environments with automation-first principles._