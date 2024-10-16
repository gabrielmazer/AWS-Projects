# AWS Projects

This repository is a collection of various AWS-related projects that I’ve completed as part of my cloud computing learning journey. Each project explores different AWS services, with the goal of becoming proficient in cloud architecture and infrastructure management.

## Repository Structure

Each project is organized into subfolders for easy navigation and understanding. Every project folder contains:

- **docs/**: Documentation files related to the project.
- **Images/**: Visualizations or screenshots of the project outputs.
- **Project Files/**: The source code, configuration files, or any other files required for the project.
- **README.md**: Detailed explanation of the project, its goals, services used, and insights gained.

## Purpose

The main focus of this repository is to deepen my knowledge of **cloud computing**, particularly using AWS services such as QuickSight, S3, EC2, Lambda, and more. As I progress through my learning journey, I will be adding new projects to this repository, expanding my understanding of AWS and cloud infrastructure.

## Completed Projects

### 1. [Netflix Data Analysis Using AWS QuickSight](https://github.com/gabrielmazer/aws-projects/tree/main/1.%20Visualize%20data%20with%20Quicksight)
This project uses Amazon QuickSight to analyze and visualize Netflix data stored in an S3 bucket. The analysis focuses on content distribution (movies and TV shows) by release year and genre, providing insights into Netflix’s content trends.

#### Key Insights:
- Significant increase in movie releases post-2015 compared to TV shows.
- Trends in certain genres show consistent growth over the years.

**Preview of Visualizations**:
![Netflix Data Visualization](https://github.com/gabrielmazer/AWS-Projects/blob/main/1.%20Visualize%20data%20with%20Quicksight/Images/full_data.jpg)

### 2. [Banking Chatbot Using Amazon Lex, Lambda, and CloudFormation](https://github.com/gabrielmazer/AWS-Projects/tree/main/2.%20Chatbot%20with%20Amazon%20Lex)
This project involves creating a banking chatbot using Amazon Lex for natural language processing, AWS Lambda to handle backend logic, and CloudFormation to automate deployment. The chatbot helps users check their account balances, transfer funds between accounts, and confirm actions through conversational prompts. It also uses context tags for session management and leverages Lambda for dynamic balance responses.

#### Key Insights:
- Integrated Amazon Lex for chatbot interaction, AWS Lambda for backend logic, and CloudFormation for automation.
- Implemented dynamic slot values and context tags for session management, improving conversational flow.
- IAdded confirmation prompts for secure fund transfers between accounts.
- Utilized CloudFormation for quick bot re-deployment.
- Fixed permissions issue between Amazon Lex and Lambda, enhancing the bot's functionality after troubleshooting.

**Preview of Visualizations**:
![Chatbot conversation test](https://github.com/gabrielmazer/AWS-Projects/blob/main/2.%20Chatbot%20with%20Amazon%20Lex/images/images%20-%20part%205/test_2.jpg)

### 3. [AWS IAM and Cloud Security Project](https://github.com/gabrielmazer/AWS-Projects/tree/main/3.%20Cloud%20Security%20with%20AWS%20IAM)
This project focused on using AWS IAM to secure EC2 instances by creating custom policies and managing user permissions. I configured IAM policies, users, and groups to control access based on environment-specific tags (production vs. development).

#### Key Insights:
- Created custom JSON IAM policies to control actions on EC2 instances based on tags.
- Managed user groups to simplify permissions across multiple users.
- Tested permissions by performing real actions and validating policies using the IAM Policy Simulator.
- Successfully restricted access to production instances while allowing full control of development resources.

**Preview of Visualizations**:
![Policy Editor](https://github.com/gabrielmazer/AWS-Projects/blob/main/3.%20Cloud%20Security%20with%20AWS%20IAM/images/POLICY_EDITOR_2.jpg)

### 4. [Building a Virtual Private Cloud](https://github.com/gabrielmazer/AWS-Projects/tree/main/4.%20Building%20a%20Virtual%20Private%20Cloud)
In this project, I configured a Virtual Private Cloud (VPC) in AWS, where I set up subnets, route tables, internet gateways, and security layers using both Security Groups and Network ACLs. By the end of the project, I had successfully created a secure and functional VPC environment, with both public and private subnets and proper routing for internet-bound traffic. I also implemented network security best practices, ensuring that my resources are protected both at the instance and subnet levels.

#### Key Insights:
- VPC Isolation and Control: Setting up a custom VPC provided full control over the network, enabling me to define subnets, routing, and security policies that fit specific needs.
- Subnet Configuration: Public and private subnets serve distinct purposes, where public subnets handle internet-facing resources, and private subnets ensure internal resources remain isolated.
- Dual-layer Security: Using both Security Groups and Network ACLs added an extra layer of protection, securing individual instances and subnets against unauthorized traffic.
- Routing Traffic: Configuring route tables was crucial to ensure proper traffic flow—especially when making the public subnet accessible through an internet gateway, while keeping the private subnet isolated from external access.

**Preview of Visualizations**:
![Policy Editor](https://github.com/gabrielmazer/AWS-Projects/blob/main/4.%20Building%20a%20Virtual%20Private%20Cloud/images/create_VPC_1.jpg)

## Learning Goals

My ultimate goal is to gain expertise in cloud computing, with a focus on:
- Designing scalable, secure, and cost-effective cloud solutions.
- Automating deployments and infrastructure management using AWS services.
- Improving data analytics and visualization using tools like QuickSight.

Stay tuned for more updates as I continue to explore AWS and build more projects!

---

_Last Updated: October 2024_
