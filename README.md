# AWS VPC Peering Project | EWB Courses Internship

## 📌 Overview

This repository contains the project completed during my 1-Month Internship at EWB Courses as part of the AWS Architect Associate learning track.

The project focuses on designing and implementing secure communication between two isolated AWS Virtual Private Clouds (VPCs) using VPC Peering while maintaining private networking principles.

The objective was to demonstrate end-to-end connectivity between workloads hosted in separate VPCs using private IP addresses without exposing application servers to the internet.

---

## 🏢 Internship Details

**Organization:** EWB Courses  
**Duration:** 1 Month  
**Domain:** AWS Cloud & Networking  
**Project Title:** AWS VPC Peering Architecture Implementation

---

## 🎯 Project Objectives

- Design a secure AWS network architecture
- Create and configure multiple VPCs
- Implement VPC Peering connectivity
- Configure custom Route Tables
- Configure Security Groups
- Deploy EC2 Instances in Public and Private Subnets
- Implement Bastion Host based administration
- Validate private communication between VPCs
- Troubleshoot network connectivity issues

---

## 🛠 Technologies Used

- Amazon Web Services (AWS)
- Amazon VPC
- VPC Peering
- EC2 Instances
- Security Groups
- Route Tables
- Internet Gateway
- Amazon Linux 2023
- SSH & ProxyJump

---

## 🏗 Architecture

The project consists of:

### VPC A
- CIDR: 10.10.0.0/16
- Public Subnet: 10.10.1.0/24
- Private Subnet: 10.10.2.0/24

### VPC B
- CIDR: 10.20.0.0/16
- Private Subnet: 10.20.1.0/24

### EC2 Instances

| Instance | Role | Private IP |
|-----------|-----------|-----------|
| Bastion Host | Administration Server | 10.10.1.10 |
| App-A | Private Application Server | 10.10.2.10 |
| App-B | Private Application Server | 10.20.1.10 |

The Bastion Host provides secure SSH access to private servers, while App-A and App-B communicate over private IPs through a VPC Peering Connection.

---

## 🔑 Key Tasks Performed

### Network Setup
- Created two custom VPCs
- Configured public and private subnets
- Attached Internet Gateway to VPC A
- Created custom Route Tables
- Configured subnet associations

### Security Implementation
- Created dedicated Security Groups
- Restricted SSH access using least-privilege rules
- Allowed ICMP traffic for connectivity testing
- Secured application servers from public internet access

### Compute Deployment
- Launched Amazon Linux EC2 instances
- Assigned custom private IP addresses
- Configured Bastion Host access
- Managed SSH key pairs securely

### Connectivity Configuration
- Created VPC Peering Connection
- Accepted and activated peering requests
- Updated routing tables
- Configured bidirectional traffic flow

### Validation & Troubleshooting
- Verified private connectivity using Ping tests
- Tested SSH access through Bastion Host
- Demonstrated successful and failed connectivity scenarios
- Troubleshot route table and security group issues

---

## ✅ Project Outcomes

- Successfully established private communication between two AWS VPCs.
- Enabled App-A and App-B to communicate using private IP addresses.
- Implemented secure administration through a Bastion Host.
- Demonstrated AWS networking fundamentals and troubleshooting skills.
- Gained practical experience in cloud infrastructure design and security best practices.

---

## 📚 Skills Gained

- AWS Networking
- VPC Design
- VPC Peering
- Route Table Management
- Security Group Management
- EC2 Administration
- Linux Server Management
- SSH Configuration
- Network Troubleshooting
- Cloud Security Fundamentals

---

## 🚀 Internship Learning Outcomes

During this internship, I gained hands-on experience with AWS cloud networking and infrastructure management. I learned how to design secure network architectures, implement VPC Peering, configure routing and security controls, and troubleshoot connectivity issues in a real-world cloud environment.

---

## 👨‍💻 Author

**Samar Raghav**

- GitHub: https
