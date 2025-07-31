---

## ☁️ Infrastructure as Code with Terraform (EC2 + EKS)

You can deploy the 3-tier application to AWS using Terraform, either on EC2 instances or using EKS for container orchestration.

---

### 📦 Option 1: Deploy to AWS EC2

#### 📁 Files Used:
- `terraform/ec2/*`

#### 🔧 What It Does:
- Provisions VPC, Subnets, IGW
- Creates EC2 instances for frontend and backend
- Installs required software using user data scripts
- Optionally connects to a remote database

#### ▶️ Steps:

```bash
cd terraform/ec2
terraform init
terraform plan
terraform apply
```
---
### ☸️ Option 2: Deploy to AWS EKS
#### 📁 Files Used:
- `terraform/eks/*`

### 🔧 What It Does:
- Provisions an EKS cluster with node groups
- Sets up IAM roles, security groups, and kubeconfig
- Optionally deploys the app using Helm charts

#### ▶️ Steps:
```bash
cd terraform/eks
terraform init
terraform plan
terraform apply
```
