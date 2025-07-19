# 🧮 AWS Math Web Application

This project demonstrates how to build a **fully functional web application on AWS** using five core services: **AWS Amplify**, **AWS Lambda**, **IAM (Identity and Access Management)**, **API Gateway**, and **Amazon DynamoDB**. The result is a responsive, serverless **Math Web App** that can process user input, perform calculations, and store results securely.

---

## 📌 Project Overview

This repository contains the infrastructure and source code for a serverless **Math Web App** that allows users to:

- Enter a base number and an exponent
- Calculate the result of raising the base to the given power (e.g., 2^3 = 8)
- View the result instantly in the browser
- Store each calculation in DynamoDB for future reference

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
4. **DynamoDB**: Stores calculation history per session.
5. **IAM**: Provides the necessary permissions for services to communicate securely.

---

🔗 **Live App**: [Click here to view the deployed app](https://dev.d2ehtjaip89vwa.amplifyapp.com/)

