# AWS-Web-Application
# Serverless Power Calculator

This repository contains the code for a serverless web application that calculates the result of raising a base number to an exponent. The application showcases the use of AWS services to build and deploy a full-stack application.

## Project Overview

The Serverless Power Calculator is designed to demonstrate a practical implementation of a serverless architecture on AWS. It provides a simple yet interactive user interface for users to input two numbers and get the result of the first number raised to the power of the second.

### Key Features

- **Serverless Architecture**: Utilizes AWS services including Lambda, API Gateway, DynamoDB, and IAM to create a scalable and cost-efficient application.
- **Full-Stack Development**: Employs HTML, CSS, and JavaScript for the frontend and AWS Lambda for the backend processing.
- **API Integration and Data Persistence**: Implements a RESTful API for the frontend to interact with and stores computational results in DynamoDB.

## Usage

1. Enter the base number and the exponent in the provided fields.
2. Click on the "Calculate" button to get the result.
3. The result will be displayed in an alert box on the webpage.

## Local Setup

1. Clone the repository.
2. Open the `index.html` file in your browser to use the application locally.
3. Use the lambda function and role policy file from my repository.

## Deployment

To deploy this application to AWS, you will need to set up the respective AWS services and configure them accordingly. Replace the placeholder URLs and ARNs in the provided code with your AWS resources.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

