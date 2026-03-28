📌 Project Overview

Designed and implemented an end-to-end CI/CD pipeline to automate build, test, and deployment of a Django + React Notes Application.

This project demonstrates real-world DevOps practices using Jenkins, Docker, and Amazon Web Services (EC2).

🏗️ Architecture

<img width="2533" height="1472" alt="Screenshot 2026-03-04 161958" src="https://github.com/user-attachments/assets/31633e49-0844-4d52-b24c-0b90fb8e5906" />
<img width="2552" height="1521" alt="Screenshot 2026-03-02 223059" src="https://github.com/user-attachments/assets/03bee0e5-3b5c-4043-a299-0796f90d951d" />

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

<img width="2533" height="1472" alt="Screenshot 2026-03-04 161958" src="https://github.com/user-attachments/assets/4d2dc797-373c-4e53-8b80-51311f562e02" />

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
<img width="2544" height="1466" alt="Screenshot 2026-03-02 222540" src="https://github.com/user-attachments/assets/5d169077-bacc-4e55-a10c-3be3f5a66dc5" />

(Final running Notes App UI)
<img width="2552" height="1521" alt="Screenshot 2026-03-02 223059" src="https://github.com/user-attachments/assets/063e1a81-bbce-4961-ad48-bba8e449d32d" />


📈 Impact
🚀 Automated deployments
⏱️ Reduced manual effort
🔁 Faster release cycles
📦 Consistent environments

👨‍💻 Author
Sumant Swain
