# AWS EC2 Windows VM Lab

## Overview
This lab demonstrates how to create and access a basic Windows virtual machine using Amazon EC2.

## Steps Performed

### 1. Create an EC2 Instance
- **Service:** Amazon EC2  
- **AMI:** Windows Server (default image)  
- **Instance Type:** t2.micro (Free Tier eligible)  
- **Key Pair:** Created or selected existing key pair for RDP access  
- **Network Settings:** Default VPC, Auto-assign public IP enabled  
- **Storage:** Default settings  
- **Security Group:** Allowed RDP (port 3389) inbound from my IP address  

### 2. Launch the Instance
- Clicked **Launch Instance** to deploy the VM.
- Waited for the instance state to show **Running** and verified status checks passed.

### 3. Retrieve Windows Login Credentials
- Selected the instance → Clicked **Connect** → Chose **RDP Client**.
- Clicked **Get Password** and uploaded my private key file to **decrypt the administrator password**.

### 4. Connect via RDP
- Copied the decrypted **Administrator password**.
- Used **Remote Desktop Connection (RDP)** on my local machine.
- Entered the **public IPv4 address** and **Administrator credentials**.
- Successfully logged in to the Windows EC2 instance.

## Verification
- Verified network connectivity and desktop environment.
- Confirmed ability to interact with the instance via RDP.

## Cleanup
- Stopped or terminated the EC2 instance to avoid incurring charges.

## Notes
- Always restrict RDP access to specific IPs for security.
- Store private keys securely; they cannot be recovered from AWS if lost.
