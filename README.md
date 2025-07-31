# 🛠️ 3-Tier App Deployment Using Multiple DevOps Tools

This repository contains a reusable **3-tier application** (frontend, backend, database) that can be deployed and practiced using multiple DevOps tools and cloud provisioning methods. It is designed to be used as a base setup for learning and showcasing DevOps tools like:

- Docker & Docker Compose
- Terraform on AWS (EC2 + EKS)
- Kubernetes (YAML)
- Jenkins Pipeline (CI/CD)

> Whether you're practicing containerization, infrastructure as code, or CI/CD pipelines — this repo has you covered!
---

## ⚙️ How This Repository Works

This repo provides a full-stack 3-tier application (React frontend + Node.js backend + MySQL database) and allows you to practice deploying it using multiple DevOps tools and techniques.

Each folder inside the repo maps to a specific tool or platform:

| Folder | Purpose |
|--------|---------|
| `app/client/` | React frontend application |
| `app/backend/` | Node.js + Express backend API |
| `database/mysql/` | MySQL database Docker setup |
| `docker/` | Dockerfile, docker-compose, and container scripts |
| `jenkins/` | Jenkins pipeline (CI/CD) to deploy frontend & backend |
| `terraform/ec2/` | Deploy frontend/backend using Terraform on AWS EC2 |
| `terraform/eks/` | Deploy on AWS EKS cluster via Terraform |
| `kubernetes/` | Raw Kubernetes manifests for manual kubectl deployment |
| `assets/` | Architecture diagrams, screenshots, or GIFs |

You can pick any toolset you want to practice and use this repo to:
- Run locally with Docker
- Deploy to AWS via Terraform
- Use Jenkins CI/CD pipelines
- Practice raw K8s deployments

The app code stays the same. Only the **DevOps tooling** changes.
---

## 🐳 Run Locally with Docker

You can run the entire 3-tier app locally using Docker and Docker Compose.

### ▶️ Prerequisites:
- Docker installed
- Docker Compose installed

### 📁 File Used:
- `docker/docker-compose.yaml`
- `docker/Dockerfile` (if applicable)
- `app/`, `database/`

### 🚀 Steps:

```bash
cd docker
docker-compose up --build
```

This will:

- ✅ Build and run frontend (app/client)

- ✅ Build and run backend (app/backend)

- ✅ Set up MySQL container (database/mysql)

- ✅ Connect all services using Docker networking

- ➡️ Access the frontend at: http://localhost:3000
