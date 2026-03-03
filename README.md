# 🚀 2048 Game – DevSecOps CI/CD Deployment Project

This project demonstrates a complete **DevSecOps CI/CD pipeline** by deploying the classic 2048 Game (built using React and TypeScript) to AWS EKS using modern DevOps tools and security best practices.

Instead of only building the game, this project focuses on:

- Containerization
- Automated CI/CD
- Security Scanning
- Cloud Deployment
- Infrastructure as Code

---

## 🛠 Tech Stack

### 👨‍💻 Application
- React
- TypeScript
- Yarn / npm

### ⚙️ DevOps & Cloud Tools
- Jenkins
- SonarQube
- Trivy
- Docker
- AWS ECR
- AWS EKS
- Terraform
- Kubernetes

---

## 🔁 CI/CD Pipeline Flow

GitHub → Jenkins → SonarQube → Trivy → Docker Build → Push to ECR → Deploy to EKS

---

## 📌 Pipeline Stages

1. Source Code Checkout  
2. Install Dependencies  
3. SonarQube Code Analysis  
4. Quality Gate Validation  
5. Trivy File System Scan  
6. Docker Image Build  
7. Trivy Image Scan  
8. Push Docker Image to AWS ECR  
9. Deploy Application to AWS EKS  

---

## ☁️ Infrastructure Setup

- EKS cluster provisioned using Terraform
- Kubernetes Deployment & Service YAML files
- IAM Roles configured for Jenkins & EKS
- Secure container registry using AWS ECR

---

## 🧪 Run Application Locally

Inside the project directory:

```bash
npm install
npm start
```

Open in browser:

```
http://localhost:3000
```

---

## 🐳 Build Docker Image Manually

```bash
docker build -t 2048-game .
docker run -p 3000:3000 2048-game
```

---

## ☸ Deploy to Kubernetes

```bash
kubectl apply -f deployment.yaml
kubectl get pods
kubectl get svc
```

---

## 🔐 Security Implementation

- Static Code Analysis using SonarQube  
- File System Vulnerability Scanning using Trivy  
- Docker Image Vulnerability Scanning  
- Quality Gate Enforcement in CI/CD  

---

## 🎯 Project Objective

This project demonstrates how a frontend application can be:

- Containerized using Docker  
- Integrated into Jenkins CI/CD pipeline  
- Secured using DevSecOps practices  
- Deployed to AWS EKS using Infrastructure as Code  

---

## 📈 Future Improvements

- Add Helm Charts
- Add Monitoring (Prometheus & Grafana)
- Implement GitHub Webhooks
- Implement GitOps using ArgoCD

---

## 👨‍💻 Author

Shubham Mohare  
DevOps & Cloud Enthusiast
