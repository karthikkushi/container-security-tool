### 🖥️ Problem 3: GoLang Date-Time Web App & Kubernetes Deployment

This problem involves creating a simple GoLang web application that displays the current date and time. The application is containerized using Docker and deployed on Kubernetes using declarative manifests. This section also includes screenshots showing deployment and output.

---

#### 📁 Project Structure

```
go-date-time-app/
├── Dockerfile                 # Container instructions
├── go.mod                     # Go module file
└── main.go                    # Go source file

datetime-app-deployment.yaml   # Kubernetes Deployment with 2 replicas
datetime-app-service.yaml      # Kubernetes NodePort Service

screenshot-command.png         # Screenshot of deployment command
screenshot-datetime.png        # Screenshot of app showing current date & time
```

---

#### 🚀 Deployment Instructions

**Step 1: Build & Push Docker Image**

```bash
docker build -t karthikeinmr/go-date-time-app:latest go-date-time-app/
docker push karthikeinmr/go-date-time-app:latest
```

**Step 2: Deploy to Kubernetes using declarative YAMLs**

```bash
kubectl apply -f datetime-app-deployment.yaml
kubectl apply -f datetime-app-service.yaml
```

**Step 3: Access the application**

After deployment, run the following command to get the exposed NodePort or external IP:

```bash
kubectl get svc
```

Access the app in your browser using `http://<EXTERNAL-IP>:<PORT>`.

---

#### 📸 Screenshots

- **screenshot-command.png** – Shows Kubernetes deployment command output
- **screenshot-datetime.png** – Displays the running Go web app with current date and time

