📌 Project Overview

Designed and implemented an end-to-end CI/CD pipeline to automate build, test, and deployment of a Django + React Notes Application.

This project demonstrates real-world DevOps practices using Jenkins, Docker, and Amazon Web Services (EC2).

🏗️ Architecture

<img width="2533" height="1472" alt="Screenshot 2026-03-04 161958" src="https://github.com/user-attachments/assets/a2ed1f3c-b443-4279-898b-78fe4f67b689" />

<img width="2552" height="1521" alt="Screenshot 2026-03-02 223059" src="https://github.com/user-attachments/assets/59f9a846-41f1-4eb3-8646-e64996d0eb99" />


⚙️ Tech Stack
Frontend: React
Backend: Django
CI/CD: Jenkins
Containerization: Docker
Cloud: Amazon Web Services (EC2)
Web Server: Nginx
Version Control: GitHub
🔥 Key Features
Automated build, test, and deployment pipeline
Dockerized application for consistency
Jenkins pipeline triggered via GitHub Webhooks
Secure authentication using GitHub PAT & Jenkins credentials
Docker images pushed to Docker Hub
Deployment using Docker Compose on EC2
Nginx reverse proxy setup
Reduced manual deployment effort
📂 Project Setup
1️⃣ Clone Repository
git clone https://github.com/LondheShubham153/django-notes-app.git
cd django-notes-app
2️⃣ Build Docker Image
docker build -t notes-app .
3️⃣ Run Container
docker run -d -p 8000:8000 notes-app:latest
4️⃣ Install Nginx
sudo apt update
sudo apt install nginx
🐳 Docker Workflow

(Docker build → tag → push → pull flow)
👉 docs/docker-workflow.png

🔁 CI/CD Pipeline Flow
Developer pushes code to GitHub
GitHub Webhook triggers Jenkins
Jenkins pulls latest code
Builds Docker image
Pushes image to Docker Hub
Deploys on EC2 using Docker Compose
Nginx serves the application

<img width="2533" height="1472" alt="Screenshot 2026-03-04 161958" src="https://github.com/user-attachments/assets/a8c30d35-9b49-4130-a6c3-f89ffae4a590" />


(Pipeline stages view in Jenkins)

👉 docs/jenkins-dashboard.png
(Jenkins dashboard overview)

🔐 Jenkins Configuration
Added GitHub PAT for authentication
Stored credentials in Jenkins
Configured webhook:
http://<jenkins-url>/github-webhook/

☁️ Deployment on AWS EC2
Launched EC2 instance
Installed Docker, Jenkins, Nginx
Configured security groups
Deployed using Docker Compose

(EC2 instance dashboard)
<img width="2544" height="1466" alt="Screenshot 2026-03-02 222540" src="https://github.com/user-attachments/assets/1bbd4fd5-fa18-4b8b-99f8-2382bd1b326a" />


(Final running Notes App UI)
<img width="2552" height="1521" alt="Screenshot 2026-03-02 223059" src="https://github.com/user-attachments/assets/22904cf8-eb22-4be9-8d57-eea8ebed5a97" />



📈 Impact
🚀 Automated deployments
⏱️ Reduced manual effort
🔁 Faster release cycles
📦 Consistent environments

👨‍💻 Author
Sumant Swain
