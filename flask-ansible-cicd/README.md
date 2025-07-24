# Flask App CI/CD with Jenkins + Ansible + Docker

## 🚀 Project Overview

This project demonstrates a full CI/CD pipeline:
- Flask App in Docker
- Jenkins to automate the pipeline
- Ansible to deploy on remote EC2

## 🧱 Stack

- Python (Flask)
- Docker
- Ansible
- Jenkins
- GitHub
- AWS EC2

## 📁 Folder Structure

flask-ansible-cicd/
├── flask-app/
├── ansible/
├── Jenkinsfile
└── README.md

markdown
Copy
Edit

## ✅ Steps

1. Code is pushed to GitHub
2. Jenkins pulls code
3. Jenkins triggers Ansible
4. Ansible installs Docker and deploys Flask app on EC2

## 🌐 Output

Visit: `http://<target-ec2-ip>:5000`

