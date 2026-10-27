# OpenClaw-AI-Agent-Amazon-Bedrock-models-for-AWS-Infrastructure-Management

## Overview

This project demonstrates how to integrate OpenClaw with Amazon Web Services (AWS) to manage cloud infrastructure using natural-language instructions.

I configured OpenClaw on an Amazon EC2 server and used an attached IAM role to interact with AWS resources. I also explored AI model selection, EC2 instance management, and verification of infrastructure changes through the AWS Management Console.

## Technologies Used

- **OpenClaw** — AI agent for natural-language infrastructure management
- **Amazon EC2** — Cloud server infrastructure
- **AWS IAM** — Role-based authentication and permissions
- **Amazon Bedrock** — Access to supported AI foundation models
- **AWS CLI** — AWS service interaction
- **Linux** — Server operating environment

## Project Features

### 1. OpenClaw Integration

Configured OpenClaw on an EC2 instance to accept natural-language requests and perform supported AWS infrastructure operations.

### 2. AI Model Selection

Explored available AI models through OpenClaw, including supported Amazon Bedrock models, and selected a model for the agent.

<img width="1230" height="672" alt="image" src="https://github.com/user-attachments/assets/1e2a5624-6d03-4240-859f-824124580b80" />


### 3. EC2 Instance Discovery

Used OpenClaw to list EC2 instances in the `us-west-2` Region through the IAM role attached to the server.

The agent identified three running EC2 instances and displayed their instance IDs, instance types, private IP addresses, and names.

<img width="1447" height="587" alt="image" src="https://github.com/user-attachments/assets/e4f7d078-cedc-4ed5-a68c-22536141c56b" />


### 4. EC2 Instance Renaming

Used natural-language instructions through OpenClaw to rename two EC2 instances by updating their Name tags:

- `Open` → `OpenServer1`
- `Open` → `OpenServer2`

<img width="1402" height="572" alt="image" src="https://github.com/user-attachments/assets/8839271a-e9dd-46fd-9a62-a58ac39b8043" />


### 5. AWS Console Verification

Opened the AWS Management Console and verified that the updated instance names appeared on the EC2 Instances page.

This demonstrated that the changes initiated through OpenClaw were reflected in AWS.

<img width="1107" height="747" alt="image" src="https://github.com/user-attachments/assets/40b0c18f-0b47-4114-99af-ee539ce33a5c" />


## Security Considerations

- Used an attached IAM role instead of embedding long-lived AWS access keys in the workflow.
- Relied on IAM policies to control which AWS operations were permitted.
- Verified infrastructure changes through the AWS Management Console.
- Considered AWS compute costs when stopping instances that were no longer needed.

## Key Learnings

- Integrating AI agents with AWS infrastructure
- Using IAM roles for secure, temporary AWS credentials
- Managing EC2 instances through natural-language instructions
- Updating EC2 Name tags through an AI-assisted workflow
- Exploring AI models available through Amazon Bedrock
- Verifying cloud infrastructure changes independently
- Managing EC2 lifecycle and compute costs
---

**Author:** Rauf Bairamov

**Project:** OpenClaw AI-Assisted AWS Infrastructure Management
