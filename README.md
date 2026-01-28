# Azure: Create a Virtual Machine and Deploy a Web Server
**Project completed via Coursera Guided Projects**
**Developed by: shawnbarron10**

This project demonstrates the successful completion of the Coursera curriculum focused on Azure infrastructure. It documents the end-to-end process of provisioning a Linux environment, configuring cloud networking, and deploying a functional Nextcloud web server.

## 🛠 Tech Stack
* **Cloud Provider:** Microsoft Azure
* **Operating System:** Ubuntu 22.04 LTS
* **Application:** Nextcloud (Snap distribution)
* **Security:** Azure Network Security Groups (NSG), SSL/TLS
* **Version Control:** Git & GitHub

## 🎓 Skills Demonstrated
* **Azure Resource Management:** Deploying and managing Virtual Machines (VM) within the Azure portal.
* **Network Security Configuration:** Defining Inbound Security Rules for Port 80 (HTTP) and Port 443 (HTTPS) to ensure external accessibility.
* **Cloud Troubleshooting:** Managing NSG rule priorities to resolve connectivity bottlenecks.
* **Web Server Administration:** Installing, configuring, and securing a web application in a headless Linux environment.

## 📋 Prerequisites
* **Active Azure Subscription:** Required for resource provisioning.
* **SSH/Bastion Access:** To interact with the VM terminal.
* **Linux CLI Proficiency:** Knowledge of `sudo`, `mkdir`, `cp`, and `chown` for system management.

## 🚀 Deployment Steps

### 1. Infrastructure Provisioning (Azure VM)
* Deployed an Ubuntu Server VM instance.
* Associated a Public IP (`172.174.155.220`) for web traffic.
* Configured the Network Security Group (NSG) to open firewall ports.

### 2. Web Server Deployment (Nextcloud)
* Installed Nextcloud via Snap for automated dependency handling.
* Applied a self-signed SSL certificate to enable HTTPS.
* Whitelisted the Public IP in the Nextcloud `trusted_domains` configuration to allow remote browser access.

### 3. Version Control & Documentation
* Initialized a Git repository on the VM to track configuration changes.
* Documented the deployment process to create a repeatable cloud infrastructure template.

## 📂 Repository Contents
* `config.php`: Sanitized Nextcloud configuration file.
* `README.md`: Detailed project summary and deployment guide.
