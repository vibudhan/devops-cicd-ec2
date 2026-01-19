# 🚀 DevOps CI/CD Pipeline Deployment on AWS EC2 (Docker + GitHub Actions)

This project demonstrates a complete **DevOps CI/CD pipeline** where a static portfolio website is automatically deployed to an **AWS EC2 instance** using **GitHub Actions** and runs inside an **Nginx Docker container**.

✅ Every push to the `main` branch triggers automated deployment.

---

## 🌐 Live Demo
✅ **Live URL:** http://13.239.136.115

---

## 🖼️ Screenshots

### ✅ Website Output (Live on EC2)
![Uploading image.png…]()


### ✅ GitHub Actions Deployment Success
![GitHub Actions Success](screenshots/github-actions-success.png)

---

## 📌 Project Overview

### What happens in this project?
1. Code is pushed to GitHub (`main` branch)
2. GitHub Actions pipeline triggers automatically
3. GitHub Actions connects to AWS EC2 via SSH
4. EC2 pulls the latest repository code
5. Nginx Docker container is deployed on port **80**
6. Website becomes live using EC2 Public IP

---

## 🧰 Tech Stack

- **GitHub Actions** (CI/CD Automation)
- **AWS EC2** (Cloud Server)
- **Amazon Linux 2023** (Server OS)
- **Docker** (Container Runtime)
- **Nginx (Docker Image)** (Web Server)
- **SSH + GitHub Secrets** (Secure Authentication)

---

## ✅ Features Implemented

✅ CI/CD pipeline triggered on every push to `main`  
✅ Secure deployment using GitHub Secrets (`EC2_HOST`, `EC2_USER`, `EC2_KEY`)  
✅ Website hosted inside an Nginx container  
✅ Public deployment via EC2 Public IP and port 80  
✅ Resume-ready DevOps project with real deployment automation  

---

## 📂 Project Structure

```bash
devops-cicd-ec2/
│
├── index.html
├── docker-compose.yml
├── README.md
│
└── .github/
    └── workflows/
        └── deploy.yml
