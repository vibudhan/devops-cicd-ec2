# 🚀 DevOps CI/CD Pipeline Deployment on AWS EC2 (Docker + GitHub Actions)

This repository contains a complete **DevOps CI/CD project** where a Dockerized web application is automatically deployed to an **AWS EC2 instance** using **GitHub Actions**.

✅ Every push to the `main` branch triggers an automated deployment pipeline.

---

## 📌 Project Overview

This project demonstrates a real-world DevOps workflow:

1. Developer pushes code to GitHub  
2. GitHub Actions pipeline triggers automatically  
3. Pipeline connects to AWS EC2 via SSH  
4. Latest code is pulled on the server  
5. Docker Compose builds and deploys the application  
6. Application is served live using **Nginx (inside Docker)**

---

## 🧰 Tech Stack

- **GitHub Actions** – CI/CD pipeline
- **Docker** – Containerization
- **Docker Compose** – Service deployment & container lifecycle management
- **AWS EC2 (Ubuntu)** – Cloud server hosting
- **Nginx** – Web server used inside container
- **SSH + GitHub Secrets** – Secure remote deployment

---

## ✅ Features Implemented

✅ Automated deployment on every push (`main` branch)  
✅ Dockerized web application deployment  
✅ Secure deployment using SSH keys stored in GitHub Secrets  
✅ Docker Compose used for easy production-like deployment  
✅ Restart policy enabled for reliability  
✅ Container health check added for monitoring

---

## ⚙️ CI/CD Workflow (How It Works)

### Trigger:
- GitHub Actions runs automatically on:
  - `push` to `main`

### Pipeline steps:
- Checkout repository code
- Connect to AWS EC2 via SSH
- Install required packages (Docker + Docker Compose)
- Clone latest repository code on EC2
- Run deployment using Docker Compose

---

## 📂 Project Structure

```bash
devops-cicd-ec2/
│
├── index.html
├── Dockerfile
├── docker-compose.yml
│
└── .github/
    └── workflows/
        └── deploy.yml

