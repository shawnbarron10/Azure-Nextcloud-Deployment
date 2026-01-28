# Azure Virtual Machine + Web Server Deployment

## Overview
This project demonstrates deploying an Ubuntu Virtual Machine in Microsoft Azure and hosting a web server using Apache.

## Technologies Used
- Microsoft Azure
- Ubuntu Linux
- Apache Web Server
- SSH
- Networking & Security Groups

## Steps Performed
1. Created an Ubuntu VM in Azure
2. Configured Network Security Group to allow HTTP (port 80)
3. Connected to VM via SSH
4. Installed Apache web server
5. Deployed a custom HTML webpage
6. Verified deployment via public IP

## Key Commands Used
```bash
sudo apt update
sudo apt install apache2 -y
sudo systemctl start apache2
sudo systemctl enable apache2
