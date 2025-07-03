# Serverless Contact Us Form with AWS Lambda & DynamoDB

This project demonstrates a fully serverless "Contact Us" form built using AWS Lambda, API Gateway, and DynamoDB. When a user submits the contact form, the data is securely sent to an AWS Lambda function, which then stores the information in a DynamoDB table. This architecture ensures high scalability, no server management, and minimal operational overhead.

## Features

- **Serverless Architecture:** No servers to manage or maintain.
- **AWS Lambda:** Handles form submissions and processes data.
- **API Gateway:** Provides a RESTful endpoint for the frontend to trigger the Lambda function.
- **DynamoDB:** Stores all contact form submissions reliably and scalably.
- **Secure:** Data is transmitted securely and stored on AWS infrastructure.

## Project Structure 
    USER---->API GATEWAY----->LAMBDA FUNCTION----->DYNAMODB


## How It Works

1. **User fills the contact form** on the frontend (e.g., `index.html`).
2. **Form submission triggers an HTTP POST request** to the API Gateway endpoint.
3. **API Gateway** forwards the request to the **AWS Lambda** function.
4. **Lambda function** parses the form data and stores it in the **DynamoDB** table.
5. **Data is persisted** and can be accessed or analyzed as needed.
