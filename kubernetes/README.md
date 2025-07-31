---

## ☸️ Kubernetes Deployment (Raw YAMLs)

This project includes Kubernetes manifests to manually deploy the 3-tier app on any K8s cluster.

### 📁 Files Used:
- `kubernetes/*`

### ⚙️ What It Includes:
- Deployment and Service YAMLs for:
  - Frontend (React)
  - Backend (Node.js)
  - MySQL (Stateful or Deployment)
- ConfigMaps and Persistent Volumes (if required)

### ▶️ Steps:

1. Ensure your kubeconfig is configured:
   ```bash
   kubectl config get-contexts
    ```
2. Apply all manifests:
    ```bash
   kubectl apply -f kubernetes/
    ```
4. Verify resources:
    ```bash
    kubectl get all
    ```
5. Access the frontend service via NodePort, LoadBalancer, or Ingress (based on your manifest configuration).
