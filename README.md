# 🚀 Docker Beginner Project

Welcome to **Docker-Beginner**, a simple project to help you understand how to create and push your first Docker image.

This guide walks you through the process of setting up Docker on an AWS EC2 instance, building a Docker image, and pushing it to Docker Hub.

---

## 📦 Project Overview

This project contains a basic Python-based Docker app. It’s intended for beginners who are getting started with containerization using Docker.

---

## 🧑‍💻 Prerequisites

- AWS account
- Docker Hub account
- Basic Linux terminal knowledge

---

## 🛠️ Steps to Build & Push Your First Docker Image

### 🔹 Step 1: Set up an EC2 Instance

1. Launch a new **Ubuntu EC2 instance** from your AWS console.
2. Connect to the instance via SSH:
   ```bash
   ssh -i your-key.pem ubuntu@<your-ec2-public-ip>
🔹 Step 2: Install Docker
bash
Copy
Edit
sudo apt update
sudo apt install docker.io -y
sudo usermod -aG docker ubuntu
After this, logout and re-login for the group change to take effect.

🔹 Step 3: Test Docker Installation
bash
Copy
Edit
docker run hello-world
🔹 Step 4: Clone the Repository
bash
Copy
Edit
git clone https://github.com/kiranjk/Docker-beginner.git
cd Docker-beginner/example/my\ first\ docker\ image
🔹 Step 5: Login to Docker Hub
bash
Copy
Edit
docker login -u kirannvn
# Enter your Docker Hub password when prompted
🔹 Step 6: Build the Docker Image
bash
Copy
Edit
docker build -t kirannvn/myfirst-docker-image:latest .
🔹 Step 7: Run the Docker Container
bash
Copy
Edit
docker run -it kirannvn/myfirst-docker-image:latest
🔹 Step 8: Push the Image to Docker Hub
bash
Copy
Edit
docker push kirannvn/myfirst-docker-image:latest
📌 Notes
If you face permission issues, try prefixing commands with sudo or ensure your user is part of the docker group.

Ensure your Dockerfile is correctly configured before building the image.

