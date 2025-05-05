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
| Resource     | Details                                |
|--------------|----------------------------------------|
| `aws_vpc`    | Custom VPC with Name tag `MainVPC`     |
| `aws_subnet` | Public & Private subnets               |
| `aws_nat_gateway` | For outbound traffic from private |
| `aws_internet_gateway` | Public subnet access        |
| `aws_route_table` | Routing for both subnet types     |
| `aws_instance` | Bastion Host in public subnet        |
| `aws_key_pair` | Secure SSH key generation            |
| `aws_security_group` | Bastion Host security group    |

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
	•	✅ Built a production-ready, secure AWS VPC using Terraform
	•	✅ Learned proper use of Terraform provider, resource, and state management
	•	✅ Automated infrastructure provisioning without clicking through AWS Console
	•	✅ Validated resources directly in AWS Console (VPC, Subnets, NAT, Bastion Host)
	•	✅ Used Git for version control and VSCode for IaC development
	•	✅ Managed SSH key pairs and IAM security best practices
	•	✅ Followed Infrastructure as Code (IaC) and DevSecOps principles

---

## 🛠️ What's Next
	•	🔧 Deploy public and private EC2 instances into their respective subnets
	•	🛡️ Lock down access using IAM roles and fine-tuned Security Groups
	•	📡 Configure NAT Gateway for secure outbound access
	•	🚪 Use Bastion Host for SSH into private resources
	•	🔍 Integrate security tools like tfsec, Snyk, and Bandit
	•	📘 Reference NIST, OWASP, and MITRE for cloud security standards
	•	🧪 Add compliance tags (SOC2, HIPAA-ready examples)

---

## 🖥️ Architecture Diagram

> Full infrastructure overview:

![VPC Architecture](https://raw.githubusercontent.com/Cloudby-MB/01-secure-aws-vpc/main/Cloud_VPC_Architecture_Diagram.png)

---

## 📸 Deployment Proof

Here is proof of the successful VPC deployment:

![Deployment Proof](deployment-proof-vpc.png)

## 📸 Subnets Deployment Proof

Here is proof of the deployed **Public** and **Private** subnets, as seen in the AWS Management Console:

![Subnets Proof](subnets-proof.png)


Here is proof of the successful Bastion Host deployment:

![Bastion Host Proof](Bastion_Host_Deployment_Proof.png)

---


## 🧑‍💻 Author

**Cloudby-MB**  
_Building secure cloud environments with automation-first principles.

<!-- update check -->