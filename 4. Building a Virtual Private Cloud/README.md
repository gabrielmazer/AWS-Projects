# AWS VPC Project

## Documentation:
You can view the full project documentation, including all visualizations and analysis, in this [PDF](https://gabrielmazer.github.io/AWS-Projects).

## Overview
In this project, I created and configured a Virtual Private Cloud (VPC) in AWS, set up subnets, route tables, internet gateways, and configured security groups and network ACLs to secure and manage my network.

## Part 1: VPC, Subnets, Route Tables, and Security Groups

### 1. Setting up the VPC
I started by creating a custom VPC with a private CIDR block (e.g., `10.0.0.0/16`). This VPC serves as my own isolated network in AWS, where I can define all the necessary networking settings.

### 2. Creating Subnets
Next, I set up two subnets within the VPC:
- One public subnet, associated with an internet gateway for external traffic (e.g., `10.0.1.0/24`).
- One private subnet, isolated from the internet (e.g., `10.0.2.0/24`).

### 3. Configuring Route Tables
I created two route tables:
- The public subnet’s route table had a route pointing to the internet gateway (IGW), allowing outbound traffic to the internet.
- The private subnet’s route table did not have a route to the IGW, keeping it isolated.

### 4. Setting up Security Groups
I configured a security group to control inbound and outbound traffic for my instances:
- I allowed HTTP traffic on port 80 from anywhere.
- By default, outbound traffic was allowed for all destinations.

## Part 2: Network ACLs and Additional Configuration

### 1. Configuring Network ACLs
I created a custom Network ACL for both subnets:
- The public subnet’s ACL allowed inbound traffic on port 80 (HTTP) and outbound traffic to any destination.
- The private subnet’s ACL had more restrictive rules, denying unnecessary inbound and outbound traffic.

### 2. Security Group vs. Network ACL
I ensured a dual layer of security by using both Security Groups and Network ACLs:
- The Security Group was applied at the resource level (instance), while the Network ACL secured the subnet as a whole.

### 3. Final Review
I tested the configuration by launching an instance in the public subnet, confirming access to the internet, and another in the private subnet, verifying its isolation.

## Reflection

### What I Didn’t Expect
One thing I didn’t expect was how detailed and interdependent the settings for route tables and network ACLs would be. Proper configuration required careful attention to make sure everything functioned as expected.
