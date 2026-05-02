🚀 AWS Resource Automation Script

This project is a Bash-based automation tool that uses the AWS CLI to list and manage AWS resources across multiple services.

📌 Overview

Managing AWS resources manually can be time-consuming. This script simplifies the process by allowing users to:

📋 List resources from multiple AWS services
❌ Delete specific resources safely
⚡ Automate repetitive cloud tasks
🛠️ Tech Stack
🐧 Bash Scripting
☁️ Amazon Web Services (AWS)
🔧 AWS CLI
💻 Linux (Ubuntu)
✨ Features
✅ Supports multiple AWS services
✅ Input validation (region, service, action)
✅ Checks AWS CLI installation & configuration
✅ Uses structured queries for clean output
✅ Safe delete with confirmation prompt
✅ Easy to extend and reusable
📦 Supported Services
EC2
S3
RDS
VPC
IAM
Lambda
DynamoDB
EBS
CloudFormation
CloudWatch
SNS
SQS
Route53
📂 Project Structure
aws-resource-automation/
│── shell.sh        # Main Bash Script
│── README.md       # Documentation
⚙️ Prerequisites

Before running the script, ensure:

AWS CLI is installed
AWS CLI is configured
Install AWS CLI
sudo apt update
sudo apt install awscli -y
Configure AWS CLI
aws configure

Provide:

Access Key
Secret Key
Region
Output format
🚀 Usage
./shell.sh <aws_region> <aws_service> <action>
📌 Example
./shell.sh ap-south-2 ec2 list
./shell.sh ap-south-2 ec2 delete
📊 Sample Output
+----------+----------------------+-----------+-------------+----------------+----------------+---------------+
| Name     | InstanceId          | Type      | State       | Public IP      | Private IP     | AZ            |
+----------+----------------------+-----------+-------------+----------------+----------------+---------------+
| ap-01    | i-027a911cce671d570 | t3.micro  | running     | 16.112.191.73  | 172.31.3.243   | ap-south-2a   |
