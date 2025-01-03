# Terraform AWS Setup Project

This project uses Terraform to provision AWS infrastructure, including:

- An EC2 instance.
- An S3 bucket to store Terraform state files.
- A DynamoDB table for state locking and consistency.

The project demonstrates how to use Terraform for infrastructure automation while ensuring state management and preventing conflicts when running Terraform in a team environment.

## Prerequisites

Before running the project, make sure you have:

- [Terraform](https://www.terraform.io/downloads) >= 0.12
- AWS credentials configured on your system (e.g., via `aws configure`).

## Project Overview

- **EC2 Instance**: Provision a basic EC2 instance.
- **S3 Bucket**: Store Terraform state files remotely for safe and shared access.
- **DynamoDB Table**: Prevent concurrent state modifications by using DynamoDB for state locking.

## How to Set Up

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/your-repository/terraform-aws-setup.git
    cd terraform-aws-setup
    ```

2. **Configure AWS Credentials**: Run the following if you haven't already configured AWS CLI:
    ```bash
    aws configure
    ```

3. **Initialize Terraform**:
    ```bash
    terraform init
    ```

4. **Apply Terraform Plan**:
    ```bash
    terraform apply
    ```

   Confirm with `yes` when prompted to create resources on AWS.

5. **Teardown Infrastructure**: To delete the resources, run:
    ```bash
    terraform destroy
    ```
  
## Benefits

- **Infrastructure as Code**: Easily manage infrastructure with code.
- **State Management**: Use S3 and DynamoDB to safely store state and prevent conflicts.
- **Automation**: Quickly provision, modify, and destroy AWS resources.

## License

- MIT License

- Copyright (c) 2024 Ayush Trivedi
