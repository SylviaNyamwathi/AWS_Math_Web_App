# 🧮 AWS Math Web Application

This project demonstrates how to build a **fully functional web application on AWS** using five core services: **AWS Amplify**, **AWS Lambda**, **IAM (Identity and Access Management)**, **API Gateway**, and **Amazon DynamoDB**. The result is a responsive, serverless **Math Web App** that can process user input, perform calculations, and store results securely.

---

## 📌 Project Overview

This repository contains the infrastructure and source code for a serverless math web app that allows users to:

- Input two numbers
- Choose a mathematical operation (addition, subtraction, multiplication, division)
- View the result
- Store the result in DynamoDB for future retrieval

---

## 🧰 AWS Services Used

| Service       | Purpose |
|---------------|---------|
| **AWS Amplify** | Hosts the frontend and handles deployment. Simplifies connecting to backend services like API Gateway and Lambda. |
| **AWS Lambda** | Handles backend logic and computations. Serverless functions are triggered via HTTP requests. |
| **API Gateway** | Exposes Lambda functions as RESTful APIs. Acts as a secure entry point for client requests. |
| **IAM** | Manages secure permissions and roles between services (e.g., Lambda → DynamoDB). |
| **Amazon DynamoDB** | Stores user calculation history in a NoSQL table. Scalable and cost-effective storage solution. |

---

## 🚀 How It Works

1. **Frontend via Amplify**: A simple web interface is created and hosted using AWS Amplify. It sends user input to API Gateway.
2. **API Gateway**: Routes HTTP requests to AWS Lambda.
3. **Lambda**: Performs the math operations and optionally stores/retrieves data from DynamoDB.
4. **DynamoDB**: Stores calculation history per user/session.
5. **IAM**: Provides the necessary permissions for services to communicate securely.

---

## 🛠️ Setup Instructions

### Prerequisites

- AWS Account
- AWS CLI configured
- Node.js and npm
- Amplify CLI (`npm install -g @aws-amplify/cli`)
