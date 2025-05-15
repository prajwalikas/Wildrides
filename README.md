#  WildRides – AWS Cloud Deployment

WildRides is a sample web application deployed using various AWS cloud services to demonstrate modern, scalable, and secure web architecture. This deployment showcases integration of serverless backend, authentication, and infrastructure management using AWS tools and services.

## 🌐 Overview

The primary goal of this project was to deploy a production-ready web application using a fully managed, serverless AWS stack. Although the application code was pre-built, the focus of the project was on **infrastructure, deployment, and secure access configuration** using the following AWS services:

## 🛠️ Services & Architecture

###  AWS IAM (Identity and Access Management)
- Configured **IAM roles and policies** to securely manage access to AWS services.
- Assigned fine-grained permissions for users and services such as Lambda, Amplify, and DynamoDB.
- Ensured only authorized resources could read/write to DynamoDB or trigger Lambda functions.

###  Amazon DynamoDB
- Used as the **NoSQL database** to store user interaction and ride-related data.
- Configured read/write capacity modes for scalability.
- Ensured fast, low-latency data storage without server management.

###  AWS Amplify
- Used for **front-end hosting** and continuous deployment via GitHub integration.
- Handled environment-based builds, enabling preview URLs and live updates after each push.
- Automatically deployed API endpoints and linked backend services.

###  Amazon Cognito
- Integrated for **user authentication and identity management**.
- Handled sign-up, sign-in, and secure token-based access to backend resources.
- Simplified the addition of user pools and federation with IAM roles for secure API calls.

###  AWS Lambda (Optional)
- Serverless compute used for backend logic (if applicable).
- Configured to respond to API Gateway triggers or DynamoDB stream events.
- Ensured no server provisioning with automatic scaling.

##  Project Structure

```
/wildrides-aws/
├── amplify/
├── backend/
├── iam-policies/
├── cognito-config/
├── dynamodb-schema/
├── README.md
```

##  How to Deploy (High-Level)

1. **Fork or Clone** the WildRides frontend repo (if needed).
2. **Connect GitHub to AWS Amplify** for automatic deployment.
3. **Configure IAM roles** for backend access (DynamoDB, Lambda, etc.).
4. **Set up Cognito user pools** and authentication settings.
5. **Deploy DynamoDB tables** and link to backend logic if needed.
6. **Monitor deployment** via AWS Amplify console.

##  Outcome

- Successfully deployed and hosted a dynamic web app on AWS.
- Secured backend access using IAM and Cognito.
- Leveraged Amplify’s CI/CD capabilities for version-controlled updates.
- Managed a scalable backend with serverless services and DynamoDB.

##  Tools & Technologies

- **AWS Amplify** – Front-end hosting and deployment  
- **AWS IAM** – Role-based access and security  
- **Amazon Cognito** – User authentication and identity control  
- **Amazon DynamoDB** – NoSQL database for ride/user data  
- **AWS Lambda** – Serverless backend compute  
- **GitHub** – Version control and CI/CD integration  


##  Source Code

🔗 [GitHub Repository](https://github.com/machadop1407/pedrotech-portfolio)
