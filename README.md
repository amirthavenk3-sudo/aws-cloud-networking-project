AWS VPC Peering Project

1. Project Overview

This project demonstrates how to create and configure two Virtual Private Clouds (VPCs) in Amazon Web Services (AWS) and establish communication between them using VPC Peering.

The project includes creating VPCs, configuring subnets and route tables, launching EC2 instances, configuring security groups, and testing connectivity between the VPCs.

2. Project Objectives

- Create and configure two AWS VPCs.
- Configure public and private networking components.
- Launch and configure EC2 instances.
- Configure security groups and route tables.
- Establish a VPC Peering connection.
- Test network connectivity using the ping command.

3. AWS Services and Technologies Used

- Amazon VPC
- Amazon EC2
- VPC Peering
- Internet Gateway
- Route Tables
- Security Groups
- Amazon Linux 2023
- SSH
- ICMP Ping
- GitHub

4. Project Architecture

The project consists of two VPCs:

VPC A

- VPC Name: ewb-vpc-a
- CIDR Block: 10.10.0.0/16
- Internet Gateway: ewb-igw-a
- EC2 Instance: Bastion Host and App-A

VPC B

- CIDR Block: 10.20.0.0/16
- EC2 Instance: App-B

VPC Peering is configured to enable communication between the two VPCs through appropriate routing and security group rules.

5. Implementation Steps

Step 1: Create VPCs

Created two separate VPCs with different CIDR blocks to provide isolated network environments.

Step 2: Configure Networking

Created subnets, Internet Gateway, and route tables according to the project requirements.

Step 3: Launch EC2 Instances

Launched EC2 instances to act as the bastion host and application servers.

Step 4: Configure Security Groups

Configured security group rules to control SSH access and allow the required ICMP traffic for connectivity testing.

Step 5: Establish VPC Peering

Created a VPC Peering connection between VPC A and VPC B to enable private communication between the networks.

Step 6: Update Route Tables

Configured the necessary routes in both VPCs to direct traffic through the VPC Peering connection.

Step 7: Test Connectivity

Used the ping command to test communication between the EC2 instances in the two VPCs before and after establishing VPC Peering.

6. Testing and Results

Before VPC Peering:
Communication between the two VPCs failed, resulting in packet loss.

After VPC Peering:
Connectivity was successfully established after configuring the peering connection, route tables, and security group rules.

The ping test showed successful communication between the instances.

7. What I Learned

Through this project, I gained practical experience in:

- Creating and configuring AWS VPCs.
- Understanding CIDR blocks and IP addressing.
- Configuring subnets, Internet Gateways, and route tables.
- Launching and connecting to EC2 instances.
- Understanding bastion host connectivity.
- Configuring security groups and network access rules.
- Establishing VPC Peering between two VPCs.
- Troubleshooting network connectivity using ping.
- Understanding how AWS networking components work together.

8. Conclusion

This project helped me understand the fundamentals of AWS networking and how VPC Peering enables communication between two separate VPCs.

It also provided hands-on experience with EC2 instances, network routing, security groups, SSH connectivity, and troubleshooting.

9. Project Files

This repository contains the project documentation, configuration-related files, and supporting resources used during the AWS project implementation.
