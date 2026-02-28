# 🚀 CI/CD Pipeline Project – Flask App with Docker & Jenkins on AWS EC2

This project demonstrates a complete end-to-end CI/CD pipeline setup using:

- 🐍 Flask (Python Web App)
- 🐳 Docker
- 🤖 Jenkins
- ☁️ AWS EC2
- 🔗 GitHub Webhooks

---

## 📌 Project Architecture

Developer → GitHub → Webhook → Jenkins → Docker Build → Docker Run → AWS EC2

Whenever code is pushed to GitHub:
1. GitHub triggers Jenkins via webhook
2. Jenkins pulls latest code
3. Jenkins builds Docker image
4. Jenkins deploys container on EC2
5. Updated app becomes live automatically

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| Flask | Backend Web Application |
| Docker | Containerization |
| Jenkins | CI/CD Automation |
| AWS EC2 | Deployment Server |
| GitHub | Source Control & Webhooks |

---

## 📂 Project Structure

```
Devops-Projects/
│
├── 01-CI-CD-Pipeline-Project/
│   ├── app/
│   │   └── app.py
│   ├── Dockerfile
│   ├── requirements.txt
│   └── Jenkinsfile
│
└── README.md
```

---

## ⚙️ How It Works

### 1️⃣ Flask App
A simple Python Flask app running on port 5000.

### 2️⃣ Docker
Dockerfile builds an image using:

- python:3.9-slim
- Installs requirements
- Exposes port 5000

### 3️⃣ Jenkins Pipeline
Pipeline stages:

- Checkout Code
- Build Docker Image
- Run Docker Container

### 4️⃣ GitHub Webhook
Automatically triggers Jenkins on every push to `main` branch.

---

## 🔥 Live Demo

App running at:

```
http://<EC2-Public-IP>:5000
```

---

## 🧠 Key DevOps Concepts Demonstrated

- Infrastructure setup on AWS
- Secure SSH key management
- Docker image creation & deployment
- CI/CD automation with Jenkins
- Webhook integration
- Handling build issues & debugging pipelines

---

## 🚀 Future Improvements

- Add Nginx reverse proxy
- Add HTTPS with Let's Encrypt
- Use Docker Compose
- Implement multi-stage builds
- Add automated tests
- Deploy using Kubernetes
- Implement GitHub Actions version

---

## 👨‍💻 Author

Asim Anand  
Software Engineer
DevOps Enthusiast 🚀

---
