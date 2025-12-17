# 🚀 GCP CI/CD Pipeline to Deploy App with Cloud Run

This project demonstrates a **complete CI/CD pipeline on Google Cloud Platform (GCP)** using **Cloud Build** and **Cloud Run**. The pipeline automatically builds a Docker image, pushes it to **Artifact Registry**, and deploys the application to **Cloud Run** whenever code is pushed to the `main` branch.
---

## 📌 Project Overview

**Goal:**  
Automate the build and deployment of a containerized application on GCP using native CI/CD services.

**Trigger:**  
- GitHub push to `main` branch

**Outcome:**  
- Application is automatically deployed to Cloud Run with a public URL

---

## 🛠️ Technologies & Services Used

- Google Cloud Run – Serverless container hosting
- Cloud Build – CI/CD pipeline
- Artifact Registry – Docker image storage
- Docker – Containerization
- IAM – Access control and permissions
- GitHub – Source code repository
- Python (Flask) – Sample web application

---

## 🧩 Application Details

The application is a simple **Flask web app**.

**Endpoint:**
- `/` → `Hello from Cloud Run CI/CD!`

---

## 🔄 CI/CD Workflow

1. Developer pushes code to GitHub (`main` branch)
2. Cloud Build trigger starts automatically
3. Docker image is built from the source code
4. Image is pushed to Artifact Registry
5. Cloud Run service is deployed or updated
6. Public URL is generated

---

## ⚙️ Cloud Build Configuration

Key pipeline features:
- Docker image build
- Image push to Artifact Registry
- Automated deployment to Cloud Run
- Logs written to Cloud Logging using a user-managed service account

---

## 🔐 IAM & Security

A **user-managed service account** is used for Cloud Build execution.

**Roles assigned:**
- Cloud Run Admin  
- Artifact Registry Writer  
- Service Account User  
- Logs Writer  

This follows the **principle of least privilege**.

---

## 🚀 Deployment Result

After a successful build:
- Cloud Run service is deployed
- Application is publicly accessible via Cloud Run URL

---

## 🧠 Key Learnings

- Implemented CI/CD using native GCP tools
- Deployed containerized applications to Cloud Run
- Worked with Artifact Registry and IAM
- Debugged real-world Cloud Build permission and logging issues
- Resolved regional and repository configuration errors

---
