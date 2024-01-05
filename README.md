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

1. **Clone the Repository**
   - Clone the repository to your local machine using `git clone [repository-url]`.

2. **Frontend Setup**
   - Navigate to the cloned directory.
   - Open the `index.html` file in your browser to interact with the frontend of the application.

3. **Backend Setup**
   - To simulate the backend on your local machine, you'll need to install [AWS SAM CLI](https://aws.amazon.com/serverless/sam/).
   - Set up AWS credentials on your local machine using AWS CLI. You can follow the [official AWS guide](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-files.html).
   - Use the `lambda_function.py` file for the Lambda function's code, which is included in the repository.
   - Replace the `"YOUR API GATEWAY ENDPOINT"` placeholder in the `index.html` file's script with your local or AWS endpoint.

4. **Execution Role Policy**
   - The `role-policy.json` file contains the necessary permissions for the Lambda function to interact with other AWS services.
   - If you are running the setup locally with SAM CLI, update the `template.yaml` file to include the execution role policy.
   - Make sure to replace the `"YOUR-TABLE-ARN"` placeholder in the `role-policy.json` file with your actual DynamoDB table ARN.

5. **Starting the Application Locally**
   - Use the SAM CLI to build and test the Lambda function locally.
   - Run `sam build` and `sam local start-api` to start the local API Gateway simulation.

6. **Interacting with the Application**
   - Once the setup is complete, you can use the frontend to send requests to your local backend.
   - Any changes to the frontend or backend code can be immediately tested by refreshing the browser or restarting the SAM local API.

For comprehensive instructions on deploying to AWS, refer to the 'Deployment' section.

## Deployment

To deploy this application to AWS, you will need to set up the respective AWS services and configure them accordingly. Replace the placeholder URLs and ARNs in the provided code with your AWS resources.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

