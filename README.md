# ☁️ Cloud Resume Challenge (Azure)
An end-to-end Azure project that transforms a traditional resume into a production-ready cloud application, following the Cloud Resume Challenge requirements.
This project demonstrates practical skills across cloud fundamentals, infrastructure as code, serverless computing, CI/CD, and secure cloud architecture — all built and deployed on Microsoft Azure.

---

## Technologies
 - Microsoft Azure
 - HTML / CSS / JavaScript
 - Azure Storage (Static Website)
 - Azure CDN (HTTPS)
 - Azure DNS
 - Azure Functions (Python)
 - Azure Cosmos DB (Table API, serverless)
 - ARM Templates (Infrastructure as Code)
 - GitHub Actions (CI/CD)
 - Python (backend logic & tests)
#
## Features
 - Resume hosted as a static website on Azure Storage
 - Styled HTML/CSS resume (no PDFs or Word docs)
 - Secure HTTPS delivery using Azure CDN
 - Custom domain name mapped via DNS
 - Visitor counter implemented with JavaScript
 - Serverless backend API built with Azure Functions
 - Persistent visitor count stored in Cosmos DB
 - Infrastructure fully defined using ARM templates
 - Automated CI/CD pipelines for both frontend and backend
 - Unit tests for backend Python code
#
## 🧠 The Process
This project began as a simple static resume, but evolved into a full cloud application.

Rather than manually configuring services in the Azure Portal, I defined all backend resources using Infrastructure as Code, ensuring deployments were repeatable and auditable.

The visitor counter introduced real-world architectural decisions:
  - JavaScript communicates with an API — not directly with the database
  - Azure Functions handle logic and validation
  - Cosmos DB provides low-cost, serverless persistence
    
CI/CD pipelines were implemented to automatically test and deploy changes, reinforcing best practices around automation, security, and reliability.
#
## Architecture Overview
 - Frontend
  - HTML/CSS/JavaScript resume
  - Hosted on Azure Storage Static Website
  - Delivered securely via Azure CDN + HTTPS
  - Custom domain configured with DNS
 - Backend
  - Azure Function (Python, HTTP trigger)
  - REST API for visitor count
  - Unit tests executed during CI/CD
 - Database
  - Azure Cosmos DB (Table API, serverless)
  - Stores and updates visitor count
 - Automation
  - ARM templates define backend infrastructure
  - GitHub Actions handle build, test, and deployment

## ▶️ Running the Project
### Backend
 1. Clone the backend repository
 2. Update ARM parameters as needed
 3. Push changes to GitHub
 4. GitHub Actions:
    - Runs Python tests
    - Packages and deploys Azure Function + Cosmos DB
### Frontend
 1. Clone the frontend repository
 2. Update HTML/CSS/JavaScript
 3. Push changes to GitHub
 4. GitHub Actions:
    - Uploads files to Azure Storage
    - Purges Azure CDN cache

## 📷 Preview
<img width="1858" height="1119" alt="image" src="https://github.com/user-attachments/assets/3b31d8bf-5ff0-40a4-b5c2-4736ff4de98e" />
<img width="1852" height="1109" alt="image (1)" src="https://github.com/user-attachments/assets/8db25cd0-50cd-4f85-911c-a6202c093953" />


