Kubernetes CI/CD on AWS (EKS)

📌 Overview

    This project demonstrates a complete end-to-end CI/CD pipeline for deploying a containerized application on Kubernetes (AWS EKS) using GitHub Actions.
    Every code change pushed to the repository automatically triggers a pipeline that builds, pushes, and deploys the application.
    

🏗️ Architecture

<img width="1536" height="1024" alt="CI_CD pipeline flow on AWS EKS" src="https://github.com/user-attachments/assets/7f125b6f-2c97-4d5a-8228-7ea32e9f3e54" />


🧰 Tech Stack

    Cloud: AWS (EKS, ECR, IAM)
    Containerization: Docker
    Orchestration: Kubernetes (EKS)
    CI/CD: GitHub Actions
    Version Control: Git & GitHub
    Application: Node.js

🔧 Features

    Fully automated CI/CD pipeline
    Dockerized application
    Kubernetes deployment on AWS EKS
    Private container registry using Amazon ECR
    Auto deployment on every Git push
    Exposed via AWS LoadBalancer
    Scalable and production-style architecture

🔄 CI/CD Workflow

    Developer pushes code to GitHub
    GitHub Actions pipeline is triggered
    Docker image is built
    Image is pushed to Amazon ECR
    Kubernetes deployment is updated on EKS
    Application is exposed via LoadBalancer

🚀 How to Run

    1. Clone the repository
       git clone https://github.com/anam-rehan/k8s-project.git
       cd k8s-project
       
    2. Configure AWS CLI
       aws configure
      
    3. Create EKS cluster
       eksctl create cluster --name my-eks-cluster --region ap-south-1
      
    4. Deploy application
       kubectl apply -f deployment.yaml
      
    5. Expose service
       kubectl expose deployment k8s-project --type=LoadBalancer --port=80 --target-port=3000
      
🌐 Access Application

      kubectl get svc

Open the EXTERNAL-IP in browser.


📂 Repository Structure

    .
    ├── app.js
    ├── Dockerfile
    ├── deployment.yaml
    ├── .github/
    │   └── workflows/
    │       └── deploy.yml
    └── architecture.png
    

🎯 Key Learning Outcomes

    This project enhanced my practical experience with Kubernetes, AWS infrastructure, containerization, and implementing end-to-end CI/CD workflows in a real-world environment.


![k8s-project-pipeline](https://github.com/user-attachments/assets/7e69c586-e386-442a-8c3c-aec63a3cf356)



![k8s-project1](https://github.com/user-attachments/assets/80cc451e-beb8-46d8-8e2b-089631ea4d7b)


