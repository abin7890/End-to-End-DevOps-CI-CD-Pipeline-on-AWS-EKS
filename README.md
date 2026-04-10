# 🚀 End-to-End DevOps CI/CD Pipeline on AWS EKS

## 📌 Project Overview
This project demonstrates a complete DevOps pipeline using modern tools to automate build, test, and deployment on AWS EKS.

---

## 🏗️ Architecture Diagram

![Architecture](./images/fullstack-blogging-app.jpeg)

---

## ⚙️ Tech Stack

- GitHub
- Jenkins
- Maven
- SonarQube
- Trivy
- Docker
- Terraform
- Kubernetes (EKS)
- Prometheus
- Grafana
- AWS Elastic Load Balancer

---

## 🔄 Pipeline Workflow

### 🔹 CI Process
1. Developer pushes code to GitHub  
2. Jenkins triggers pipeline  
3. Maven builds the project  
4. SonarQube checks code quality  
5. Trivy scans for vulnerabilities  

### 🔹 Build Process
6. Docker image is built  
7. Trivy scans Docker image  

### 🔹 Deployment Process
8. Terraform provisions infrastructure  
9. App is deployed to Kubernetes (EKS)  
10. Load Balancer exposes the app  

### 🔹 Monitoring
11. Prometheus collects metrics  
12. Grafana visualizes dashboards  

---

## 🌐 Application Access
Application is accessible via AWS Load Balancer URL.

---

## 📂 Project Structure
