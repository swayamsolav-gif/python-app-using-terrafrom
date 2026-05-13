# 🚀 Containerized Python Application using Terraform & Ansible

This project demonstrates complete automation of deploying a Python Streamlit application on AWS using Terraform, Ansible, and Docker.

Terraform provisions the AWS EC2 infrastructure, while Ansible installs Docker and deploys a containerized Python application that runs a live Streamlit dashboard.

---

# 📌 Project Overview

This project automates the complete deployment workflow:

1. Terraform launches AWS EC2 instance
2. Ansible connects to the EC2 server
3. Docker is installed automatically
4. Python container is deployed
5. Streamlit application becomes publicly accessible

---

# 🏗️ Architecture Diagram

```text
                    ┌────────────────────┐
                    │     Terraform      │
                    │────────────────────│
                    │ Launch AWS EC2     │
                    └─────────┬──────────┘
                              │
                              ▼
                 ┌────────────────────────┐
                 │        Ansible         │
                 │────────────────────────│
                 │ Install Docker         │
                 │ Configure Server       │
                 │ Deploy Python App      │
                 └─────────┬──────────────┘
                           │
                           ▼
                 ┌────────────────────────┐
                 │         Docker         │
                 │────────────────────────│
                 │ Run Python Container   │
                 └─────────┬──────────────┘
                           │
                           ▼
                 ┌────────────────────────┐
                 │   Streamlit Dashboard  │
                 │────────────────────────│
                 │ Runs on Port 8501      │
                 │ Student Data Analysis  │
                 └────────────────────────┘
```

---

# ⚙️ Technologies Used

| Technology | Purpose |
|------------|----------|
| Terraform | Infrastructure Provisioning |
| AWS EC2 | Cloud Hosting |
| Ansible | Configuration Management |
| Docker | Containerization |
| Python | Data Science Application |
| Streamlit | Dashboard UI |
| Linux | Server Environment |

---

# ☁️ Infrastructure Deployment

## Configure Terraform Variables

Update the `terraform.tfvars` file with your AWS credentials.

```bash
% cat terraform.tfvars

AWS_ACCESS_KEY=""
AWS_SECRET_KEY=""
AWS_REGION="us-east-1"
```

---

# 🚀 Terraform Commands

## Initialize Terraform

```bash
% terraform init
```

## Launch Infrastructure

```bash
% terraform apply --auto-approve
```

## Destroy Infrastructure

```bash
% terraform destroy --auto-approve
```

---
