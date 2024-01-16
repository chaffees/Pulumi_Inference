# Pulumi Inference

## Description
This Pulumi program deploys a Hugging Face Language Model (LLM) on an Amazon SageMaker instance. It includes configurations for instance type, environment variables, and health check timeouts, ensuring a robust and scalable deployment of machine learning models.

## Features
- Deployment of Hugging Face Language Models on Amazon SageMaker.
- Customizable AWS instance types and environment variables.
- Health check timeouts for reliable deployment.
- CloudWatch monitoring setup for the deployed model.

## Prerequisites
- Python 3.x
- Pulumi
- AWS CLI
- AWS account with SageMaker and CloudWatch access

## Setup and Installation
1. **Clone the Repository:**
   `git clone https://github.com/chaffees/Pulumi_Inference.git`
   `cd Pulumi_Inference`
2. **Install Pulumi:**
   Follow the instructions at Pulumi Installation Guide.
3. **Configure AWS Credentials:**
   Set up your AWS credentials to allow Pulumi to interact with your AWS account.
4. **Deploy the Model:**
   `pulumi up`

## Usage
- The deployment will create a SageMaker endpoint for the Hugging Face Language Model.
- You can interact with this endpoint using AWS SDKs or the AWS CLI.
- Monitor the performance and health of your model through AWS CloudWatch.

## Additional Information
- **HuggingFaceLlm Component:** This component handles the deployment of the Hugging Face LLM model on Amazon SageMaker. See `huggingface_llm.py` for implementation details.
- **Main Deployment Script:** The main deployment logic, including configurations and resource creation, is defined in `__main__.py`.
