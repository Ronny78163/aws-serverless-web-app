# aws-serverless-web-app
AWS serverless web application using Amplify, Lambda, API Gateway, DynamoDB and IAM

## Architecture Diagram
![aws_serverless_architecture/aws_serverless_architecture.png](https://github.com/Ronny78163/aws-serverless-web-app/blob/26c2ff1f63ca872a83e7b909278a0e9d3858008b/aws_serverless_architecture/aws_serverless_architecture.png)

## Project Overview
This project demonstrates the deployment of a serverless web application using Amazon Web Services (AWS).
The application allows users to enter a base number and an exponent to perform a mathematical calculation.
The project was completed as a hands-on learning excercise

## AWS Services Used
| AWS Service | Purpose |
| :--- | :--- |
| **AWS Amplify** | Hosts the web application frontend |
| **Amazon API Gateway** | Provides an API endpoint for frontend requests |
| **AWS Lambda** | Executes Python code to process calculations |
| **Amazon Dynamo DB** | Stores calculation results |
| **AWS IAM** | Manages permissions for AWS service integration |

## Application Workflow
1. The user accesses the web application hosted on AWS Amplify
2. The user enters two numbers and submits a calculation
3. The forntend sends a request to Amazon API Gateway
4. API Gateway invokes the AWS Lambda function
5. Lambda processes the calculation and writes the result to DynamoDB
6. The calculated result is returned to the frontend and displayed to the user

## Project Implementation
The following components were configured during the tutorial:
- IAM: Configured permissions allowing Lambda to interact with DynamoDB
- Lambda: Deployed a Python function to process mathematical calculations
- API Gateway: Created an API endpoint integrated with Lambda
- DynamoDB: Created a table to store calculation results
- Amplify: Hosted the frontend and connected it to the backend API

## Learning Outcomes
- Deploying AWS serverless application components
- Connecting frontend and backend services through an API
- Configuring AWS IAM permissions
- Integrating Lambda with DynamoDB
- Understanding how multiple AWS services work together

