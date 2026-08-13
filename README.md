# AWS-VPC-Peering
AWS VPC Peering project demonstrating secure private communication between two VPCs using VPC Peering, Route Tables, Subnet, Internet Gateway and EC2 instances.
# Project Overview
The project demonstrate how to establish secure private communication between two isolated Amazon VPCs using AWS VPC Peering. Two separate VPCs were created with different CIDR ranges, and EC2 instances were deployed in each VPC. A VPC Peering connection was configured along with appropriate route tables and security group rules to allow communication between the EC2 instances using their private IP addresses.
# Objectives
- Create and configure two isolated AWS VPCs.
- Create subnets and launch EC2 instances in each VPC.
- Establish a VPC Peering connection between the VPCs.
- Configure route tables for communication in both directions.
- Configure Security Groups to control network traffic.
- Test private communication between EC2 instances.
- Understand AWS networking and private connectivity.
# AWS Services Used
Amazon VPC, VPC Peering, Amazon EC2, Route Table, Security Groups, Subnets, Internet Gateway
# Project Workflow & Architecture
1. Create VPC-A and VPC-B.
2. Create subnets in both VPCs.
3. Launch EC2 instances in the required subnets.
4. Create a VPC Peering Connection.
5. Accept the peering request.
6. Add routes to the route tables of both VPCs.
7. Update Security Groups to allow communication.
8. Test connectivity between the EC2 instances using private IP addresses.
# Key Configuration
VPC-A
- CIDR: 10.0.0.0/16
- Subnet: 10.0.1.0/24
VPC-B
- CIDR: 10.1.0.0/16
- Subnet: 10.1.1.0/24
Routes were configured so that:
- VPC-A sends traffic destined for 10.1.0.0/16 through the VPC Peering connection.
- VPC-B sends traffic destined for 10.0.0.0/16 through the VPC Peering connection.
Security Group rules were configured to allow the required private traffic between the EC2 instances.
# Expected Result
After successful configuration, the EC2 instance in VPC-A can communicate with the EC2 instance in VPC-B using private IP addresses through the VPC Peering Connection.
# Key Learning 
Through this project, I learned how AWS VPC networking works and how different AWS networking components work together. I gained practical experience with VPC Peering, CIDR blocks, subnets, route tables, Security groups, EC2 networking and private IP communication.
# Future Scope
- Implement VPC Peering across different AWS accounts.
- Configure cross-region VPC Peering.
- Use AWS Transit Gateway for connecting multiple VPCs.
- Implement additional security controls and monitoring.
# Project Type
AWS Cloud & Networking Project
This project was created for hands-on learning and practical understanding of AWS networking concepts.
# Screenshots
1. VPC
<img width="1917" height="660" alt="VPC" src="https://github.com/user-attachments/assets/cc51c5b5-f56f-4582-9d56-4e5b0e24655a" />
