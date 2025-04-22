# Container Security Tool

Welcome to the **Container Security Tool** repository — a project with three key deliverables focused on container image security, Kubernetes cluster scanning, and GoLang app deployment.

---

## 📋 Project Overview

### 1️⃣ Problem 1: Product Requirements & Wireframes  
- Document detailing requirements for a container image security scanning product.  
- Low-fidelity wireframes for the user interface design.  
- Goal: Help users identify vulnerabilities across thousands of container images and prioritize fixes.

### 2️⃣ Problem 2: Kubernetes Security Scan Findings  
- JSON file containing findings from scanning a Kubernetes cluster using tools like Kubescape.  
- Helps identify security risks in the cluster setup.

### 3️⃣ Problem 3: GoLang Date-Time Web App & Kubernetes Deployment  
- A simple Go web app that displays current date and time.  
- Dockerfile for containerizing the app.  
- Kubernetes manifests to deploy 2 replicas and expose the app via service.  
- Includes screenshots showing deployment commands and app running.

---

## 🗂️ Repository Structure

```plaintext
/
├── Product_Requirements_and_Wireframes.pdf    # Problem 1 deliverable
├── results.json                               # Problem 2 findings JSON
├── go-date-time-app/                          # Problem 3 source and Docker files
│   ├── Dockerfile
│   ├── go.mod
│   └── main.go
├── datetime-app-deployment.yaml               # K8s deployment YAML (Problem 3)
├── datetime-app-service.yaml                   # K8s service YAML (Problem 3)
├── screenshot-command.png                      # Deployment command screenshot
└── screenshot-datetime.png                      # Running app screenshot
## ⚙️ How to Use

### Problem 1  
Review the `Product_Requirements_and_Wireframes.pdf` to understand the product scope and wireframes.
---
### Problem 2  
Check out the `results.json` file to see the Kubernetes security scan results.
---
### Problem 3  

1. **Build the Docker image** using the Dockerfile inside the `go-date-time-app/` directory.  
2. **Deploy the app on Kubernetes** with the following commands:

```bash
docker push Karthikeinmr/go-date-time-app:latest

kubectl apply -f datetime-app-deployment.yaml
kubectl apply -f datetime-app-service.yaml


Contact
For questions or feedback, please reach out to kushikarthikeyenmr@gmail.com
