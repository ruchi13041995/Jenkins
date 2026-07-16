# 🚀 End-to-End GitOps CI/CD Pipeline using Jenkins, Docker, Kubernetes & ArgoCD

> A production-style DevOps project demonstrating Continuous Integration, Continuous Deployment, and GitOps using Jenkins, SonarQube, Docker, Kubernetes (Minikube), and ArgoCD.

---

# 📌 Project Overview

This project automates the complete software delivery lifecycle of a Spring Boot application.

Starting from a developer's code commit, the pipeline automatically:

- 📥 Pulls source code from GitHub
- 🔨 Builds the application using Maven
- 🔍 Performs code quality analysis using SonarQube
- 🐳 Builds and pushes Docker images to Docker Hub
- 📝 Updates Kubernetes deployment manifests
- 🔄 Commits updated manifests to GitHub
- 🚀 Automatically deploys the latest version to Kubernetes using ArgoCD

---

# 🏗️ Architecture

```
               👨‍💻 Developer
                     │
             Git Push to GitHub
                     │
                     ▼
          ⚙️ Jenkins Pipeline (SCM)
                     │
                     ▼
        🐳 Custom Jenkins Docker Agent
                     │
      ┌──────────────┼──────────────┐
      │              │              │
      ▼              ▼              ▼
 🔨 Maven Build   🔍 SonarQube   🐳 Docker Build
                                     │
                                     ▼
                           📦 Docker Hub
                                     │
                                     ▼
                      📝 Update deployment.yml
                                     │
                                     ▼
                         📤 Push Manifest to GitHub
                                     │
                                     ▼
                           🚀 ArgoCD (GitOps)
                                     │
                                     ▼
                     ☸️ Kubernetes (Minikube)
                                     │
                                     ▼
                      🌐 Spring Boot Application
```

---

# 🛠️ Tech Stack

| Category | Technologies |
|----------|--------------|
| 💻 Source Control | Git, GitHub |
| ⚙️ CI Tool | Jenkins |
| 🔨 Build Tool | Maven |
| 🔍 Code Quality | SonarQube |
| 🐳 Containerization | Docker |
| 📦 Container Registry | Docker Hub |
| ☸️ Orchestration | Kubernetes (Minikube) |
| 🚀 GitOps | ArgoCD |
| ☕ Application | Spring Boot |

---

# 🔄 CI/CD Workflow

### ✅ Continuous Integration

- 📥 Checkout code from GitHub
- 🔨 Compile using Maven
- 🧪 Run Tests
- 🔍 SonarQube Static Analysis
- 🐳 Build Docker Image
- 📦 Push Docker Image to Docker Hub

### ✅ Continuous Deployment (GitOps)

- 📝 Update Kubernetes Deployment Manifest
- 📤 Commit Manifest Changes to GitHub
- 👀 ArgoCD detects Git changes
- ☸️ Kubernetes performs Rolling Update
- 🌐 Latest application becomes available automatically

---

# ⭐ Key Features

- ✅ Declarative Jenkins Pipeline
- ✅ Pipeline from SCM
- ✅ Custom Jenkins Docker Agent
- ✅ Docker-in-Docker Integration
- ✅ SonarQube Code Analysis
- ✅ Docker Hub Integration
- ✅ GitOps Deployment using ArgoCD
- ✅ Kubernetes Deployment & Service
- ✅ Automatic Image Tag Update
- ✅ Rolling Deployment

---

# 📂 Project Structure

```
📦 Jenkins
│
├── 📄 JenkinsFile
├── 📁 jenkins-agent
│   ├── Dockerfile
│   └── ...
│
├── 📁 java-maven-sonar-argocd-helm-k8s
│   ├── 📁 spring-boot-app
│   ├── 📁 spring-boot-app-manifests
│   ├── 📁 Argo CD
│   └── ...
│
└── 📄 README.md
```

---

# 📸 Project Screenshots

- 📌 Jenkins Pipeline Success
- 
  <img width="1028" height="100" alt="image" src="https://github.com/user-attachments/assets/c76c53fe-5546-463c-8761-3e47c5350cab" />

  <img width="1364" height="273" alt="image" src="https://github.com/user-attachments/assets/2e398801-d51e-4bfb-afcb-1bdae8f79353" />


- 📌 SonarQube Dashboard

  <img width="921" height="177" alt="image" src="https://github.com/user-attachments/assets/6139587d-d444-4f9b-a962-e73a502aece3" />

- 📌 Docker Hub Repository

  <img width="1346" height="556" alt="image" src="https://github.com/user-attachments/assets/7c07cac8-821d-4c65-b4f3-4f32ab10546c" />

- 📌 ArgoCD Sync Status

  <img width="1354" height="598" alt="image" src="https://github.com/user-attachments/assets/0829f2f5-634c-4043-a91a-33a4cc8abe64" />

- 📌 Kubernetes Pods

  <img width="623" height="190" alt="image" src="https://github.com/user-attachments/assets/6855132e-6951-4bcf-9ce9-5eb11e867695" />


  - 📌 Running Spring Boot Application

    <img width="1350" height="508" alt="image" src="https://github.com/user-attachments/assets/4d3be28c-d06e-4777-9926-3ef97c47a79e" />


---  

# 🎯 Learning Outcomes

This project helped me gain hands-on experience with:

- 🔹 Jenkins Declarative Pipelines
- 🔹 Docker & Docker Hub
- 🔹 SonarQube Integration
- 🔹 Kubernetes Deployments & Services
- 🔹 GitOps using ArgoCD
- 🔹 CI/CD Pipeline Automation
- 🔹 Infrastructure Troubleshooting
- 🔹 Linux & Container-based Development

---

# 👩‍💻 Author

**Ruchita Gholap**

DevOps Engineer | AWS | Docker | Kubernetes | Jenkins | Terraform | Ansible

⭐ If you found this project useful, feel free to star the repository!
