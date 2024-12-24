# Terraform AWS Setup Project

This project uses Terraform to provision an AWS infrastructure that includes:
- An EC2 instance.
- An S3 bucket to store Terraform state files.
- A DynamoDB table for state locking and consistency.

## Prerequisites

- [Terraform](https://www.terraform.io/downloads) >= 0.12
- AWS credentials configured on your system (e.g., via `aws configure`).
