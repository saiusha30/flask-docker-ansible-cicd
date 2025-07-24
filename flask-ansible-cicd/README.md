# 🚀 Flask Docker CI/CD with Jenkins and Ansible on AWS

This project demonstrates a **Complete CI/CD Pipeline** for deploying a Python Flask application using **Jenkins**, **Ansible**, **Docker**, and **AWS EC2**.

## 📦 Tech Stack

- 💻 Jenkins – CI/CD Server
- 🤖 Ansible – Configuration Management & App Deployment
- 🐳 Docker – Containerization
- 🐍 Flask – Lightweight Web Framework
- ☁️ AWS EC2 – Target Server
- 📂 GitHub – Source Code Repository

---

## 🔧 Project Workflow

```plaintext
GitHub ➝ Jenkins ➝ Ansible ➝ EC2 ➝ Docker ➝ Flask App
1.Developer pushes code to GitHub

2.Jenkins is triggered (poll SCM or webhook)

3.Jenkins runs Ansible playbook

4.Ansible connects to EC2 and:

.Installs Docker

.Pulls code

.Builds Docker image

.Runs Flask app in a container

5.Flask app becomes accessible via EC2 public IP

🗂️ Folder Structure

flask-docker-ansible-cicd/
├── ansible/
│   ├── inventory
│   └── playbook.yml
├── flask-app/
│   ├── app.py
│   └── requirements.txt
├── Dockerfile
├── Jenkinsfile
├── README.md
└── .gitignore

 Screenshots 
## 📸 Screenshots

### ✅ Jenkins Build Output 1
![Jenkins Build 1](screenshots/jenkinsbuildoutput1.png)

### ✅ Jenkins Build Output 2
![Jenkins Build 2](screenshots/jenkinsbuildoutput2.PNG)

### ✅ Jenkins Job Output
![Jenkins Job Output](screenshots/jenkinjoboutput3.PNG)

### 🐳 Docker Image and Container
![Docker Image](screenshots/dockerimage,container.png)

### 🌐 Accessing the Application
![Access App](screenshots/accessapp.png)

📝 How to Run This Project
1. Setup Jenkins:
Install required plugins: Git, Ansible, Docker Pipeline

Configure credentials and GitHub repo

Create a pipeline job and use Jenkinsfile

2. Configure Ansible:
Inventory file with EC2 IP

SSH key placed in Jenkins user’s .ssh/ directory

Run ansible-playbook from Jenkins

3. App Access:
Get EC2 public IP

Visit: http://<your-ec2-ip>:5000

📌 Pre-requisites
EC2 instances (Jenkins + Target node)

SSH key pair

Ansible installed on Jenkins node

Docker setup via playbook



🙋‍♀️ Author
Usha Rani Parvathina
👩‍💻 DevOps Learner | Passionate about CI/CD and Automation
🔗 GitHub: saiusha30
