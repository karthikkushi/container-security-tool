# Container Security Tool

Welcome to the **Container Security Tool** repository — a project with three key deliverables focused on container image security, Kubernetes cluster scanning, and GoLang app deployment.

---

## 📋 Project Overview

1️⃣ **Problem 1: Product Requirements & Wireframes**  
- Document detailing requirements for a container image security scanning product.  
- Low-fidelity wireframes for the user interface design.  
- **Goal:** Help users identify vulnerabilities across thousands of container images and prioritize fixes.

2️⃣ **Problem 2: Kubernetes Security Scan Findings**  
- JSON file containing findings from scanning a Kubernetes cluster using tools like Kubescape.  
- Helps identify security risks in the cluster setup.

3️⃣ **Problem 3: GoLang Date-Time Web App & Kubernetes Deployment**  
- A simple Go web app that displays current date and time.  
- Dockerfile for containerizing the app.  
- Kubernetes manifests to deploy 2 replicas and expose the app via service.  
- Includes screenshots showing deployment commands and app running.
---

## 🗂️ Repository Structure

/ ├── Product_Requirements_and_Wireframes.pdf # Problem 1 deliverable ├── results.json # Problem 2 findings JSON ├── go-date-time-app/ # Problem 3 source and Docker files │ ├── Dockerfile │ ├── go.mod │ └── main.go ├── datetime-app-deployment.yaml # K8s deployment YAML (Problem 3) ├── datetime-app-service.yaml # K8s service YAML (Problem 3) ├── screenshot-command.png # Deployment command screenshot └── screenshot-datetime.png # Running app screenshot


---

## ⚙️ How to Use

### 🧩 Problem 1  
Review the `Product_Requirements_and_Wireframes.pdf` to understand the product scope and wireframes.  
You can also visit the Notion documentation for more details:  
- 🔗 [Assignment Overview](https://www.notion.so/AccuKnox-Product-Management-Assignment-1da908eb890b80a6878ec1d0df68acae?pvs=4)  
- 🔗 [Low-Fidelity Wireframes](https://www.notion.so/Low-Fidelity-Wireframes-1da908eb890b8027b9acd690b83f98c5?pvs=4)  
- 🔗 [Vulnerability Details for nginx:latest](https://www.notion.so/Vulnerability-Details-nginx-latest-1da908eb890b8038a105cfbc363a6c13?pvs=4)  
- 🔗 [Bulk Action Dashboard](https://www.notion.so/Bulk-Action-Dashboard-1da908eb890b802bb838e89add11f3a8?pvs=4)
---

### 🔍 Problem 2  
The `results.json` file contains Kubernetes security scan findings generated using tools like **Kubescape**.  
It identifies vulnerabilities and misconfigurations in your K8s cluster setup.

---

### 🖥️ Problem 3  

This is a simple GoLang web application that displays the **current date and time**.

Steps to run:

1. **Build & Push the Docker image**  
   Inside the `go-date-time-app/` directory, build and push the image:

   ```bash
   docker build -t karthikeinmr/go-date-time-app:latest .
   docker push karthikeinmr/go-date-time-app:latest
Deploy to Kubernetes using declarative YAMLs
kubectl apply -f datetime-app-deployment.yaml
kubectl apply -f datetime-app-service.yaml


Contact
For questions or feedback, feel free to reach out:
📧 kushikarthikeyenmr@gmail.com
