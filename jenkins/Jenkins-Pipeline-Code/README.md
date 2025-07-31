---

## ⚙️ CI/CD with Jenkins (Frontend + Backend)

This repo includes Jenkins pipeline scripts for deploying both frontend and backend apps.

### 📁 Files Used:
- `jenkins/frontend-pipeline.groovy`
- `jenkins/backend-pipeline.groovy`
- `app/`, `docker/`

### ⚙️ Jenkins Pipeline Features:
- Clone app code from GitHub
- Build Docker images for frontend/backend
- Push images to Docker Hub (or any registry)
- Deploy containers on Docker or K8s

### 🚀 Setup Steps:

1. Install Jenkins and required plugins:
   - Docker Pipeline
   - GitHub Integration
   - Blue Ocean (optional)

2. Create a new pipeline job → Use `Pipeline Script from SCM`

3. Point to:
   - Frontend: `jenkins/frontend-pipeline.groovy`
   - Backend: `jenkins/backend-pipeline.groovy`

4. Configure Docker Hub credentials in Jenkins UI

5. Run the pipeline!

You can also customize the pipeline to deploy to ECS, EKS, or other services.
