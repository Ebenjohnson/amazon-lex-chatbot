# AMAZON LEX CHATBOT

## ðŸŒ Overview
This project demonstrates how to set up [Project Name] using AWS services. The goal is to [brief description of the project's purpose].

## ðŸ—ï¸ Architecture
<img src="Architecture%20Diagram.png" alt="drawing" width="500"/>

## ðŸ¥ª Prerequisites
- AWS Account
- IAM user with sufficient permissions
- [Other tools, e.g., AWS CLI, Terraform, etc.]

## ðŸ§± Setup Instructions

### Step 1: Create an S3 Bucket
1. Log in to your AWS Management Console.
2. Navigate to the S3 service.
3. Click on "Create bucket" and follow the prompts to create a new bucket.

### Step 2: Configure IAM Roles
1. Navigate to the IAM service.
2. Create a new role with the necessary permissions.
3. Attach the role to your EC2 instance.

### Step 3: Launch an EC2 Instance
1. Navigate to the EC2 service.
2. Click on "Launch Instance" and follow the prompts to launch a new EC2 instance.
3. Select the previously created IAM role during the instance setup.

## ðŸ› ï¸ Configuration Details

### S3 Bucket Configuration
- Bucket Name: `example-bucket`
- Public Access: Enabled
- Static Website Hosting: Enabled

### IAM Role Configuration
- Role Name: `example-role`
- Attached Policies: `AmazonS3FullAccess`, `AmazonEC2FullAccess`

## ðŸ½ï¸ Usage Instructions
1. Access the S3 bucket at `http://example-bucket.s3-website-region.amazonaws.com`.
2. SSH into the EC2 instance using the public IP address: `ssh -i "key-pair.pem" ec2-user@ec2-public-ip`.
3. [Other usage instructions]

## ðŸš¨ Troubleshooting

### Common Issues
- **Issue 1:** Unable to access S3 bucket.
  - **Solution:** Check the bucket's public access settings and ensure the bucket policy allows public access.

- **Issue 2:** SSH connection to EC2 instance fails.
  - **Solution:** Verify that the security group attached to the instance allows inbound SSH traffic on port 22.

## ðŸ”— Additional Resources
- [AWS S3 Documentation](https://docs.aws.amazon.com/s3/)
- [AWS IAM Documentation](https://docs.aws.amazon.com/iam/)
- [AWS EC2 Documentation](https://docs.aws.amazon.com/ec2/)
