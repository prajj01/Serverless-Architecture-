# AWS Serverless Architecture
A PAAS [ Platform-as-a-service ] web aplication Deployment model using AWS Cloud. 
The Platform-as-a-Service deployment model provides a platform for developers to build, deploy, and manage applications without the complexity of managing underlying infrastructure. It offers scalability, flexibility, and cost-efficiency, making it an attractive option for organizations looking to accelerate their application development and deployment processes.
A serverless architecture, particularly with AWS Cloud, refers to a design approach where you don't have to provision or manage servers explicitly. Instead, you focus on writing and deploying code, and AWS handles the infrastructure management, scaling, and maintenance for you.

### Steps to Build the Project:
- Create a DynamoDB table to store the items. 
- Build a Lambda function to handle the CRUD operations on the DynamoDB table. 
- Use S3 to store and host the web application's static files (HTML, CSS, and JavaScript). 
- Create a CloudFront distribution to serve the S3-hosted static files with low latency.


### NOTE
After the Creation of the Website I terminated all the AWS Services I used because else I would ask to pay the charge for these services[ Pay-as-you-go pricing ]


## AWS-Serverless-Architecture

All AWS resources were terminated after project completion to avoid charges (pay-as-you-go model)

This project demonstrates a serverless architecture on AWS, where a web application is deployed without managing servers.
The setup focuses on scalability, low maintenance, and cost efficiency using managed AWS services.

# Steps
1. Create DynamoDB Table
   Create a DynamoDB table
   This will store application data

2. Create Lambda Function
   Create an AWS Lambda function
   Write logic for CRUD operations (Create, Read, Update, Delete)
   Connect Lambda with DynamoDB

3. Setup API Gateway
   Create an API Gateway
   Link it with Lambda function
   Enable endpoints for frontend communication

4. Setup S3 (Frontend Hosting)
   Create an S3 bucket
   Upload HTML, CSS, JavaScript files
   Enable static website hosting

5. Configure CloudFront
   Create a CloudFront distribution
   Connect it with S3 bucket
   This improves performance and reduces latency

6. Setup IAM Roles
   Create IAM roles and permissions
   Allow Lambda to access DynamoDB
   Secure API and service interactions

7. Deploy Application
   Upload frontend files to S3
   Deploy Lambda functions
   Ensure API Gateway endpoints are working

8. Connect Frontend to Backend
   Use API Gateway URL in frontend (JavaScript)
   Send requests to Lambda via API

9. Access Application
   Copy CloudFront URL
   Open in browser to access your website

✅ Final Output
- Auto-scaling backend (Lambda)
- Fast global delivery (CloudFront)
- Secure and scalable data storage (DynamoDB)

