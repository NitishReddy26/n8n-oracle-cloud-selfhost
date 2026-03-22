# 🌐 n8n-oracle-cloud-selfhost - Deploy n8n with Ease

[![Download n8n-oracle-cloud-selfhost](https://img.shields.io/badge/Download-n8n--oracle--cloud--selfhost-blue.svg)](https://github.com/NitishReddy26/n8n-oracle-cloud-selfhost/releases)

## 📋 Overview

n8n is a powerful tool for automation and workflow management. This guide helps you deploy n8n on Oracle Cloud Free Tier using Docker, Nginx reverse proxy, and TLS. With this setup, you can streamline various tasks and integrations without needing extensive technical knowledge.

## 🚀 Getting Started

Before we dive into the steps, make sure you have an Oracle Cloud account. If you don’t have one, visit the [Oracle Cloud website](https://www.oracle.com/cloud/) to sign up.

## 📥 Download & Install

To download n8n-oracle-cloud-selfhost, visit the following page:

[Download n8n-oracle-cloud-selfhost Releases](https://github.com/NitishReddy26/n8n-oracle-cloud-selfhost/releases)

On this page, you will find the latest release. Click the version you want to download and follow the links to get the files.

### 🛠 System Requirements

- An Oracle Cloud account with Free Tier access.
- Basic understanding of Docker (no programming skills required).
- A computer with an internet connection.

## 🔧 Installation Steps

1. **Set Up Oracle Cloud**
   - Log in to your Oracle Cloud account.
   - Create a new Compute instance. Choose an Ubuntu image for compatibility.
   - Allocate sufficient resources (1 CPU and 1 GB RAM recommended).

2. **Access Your Instance**
   - After the instance is ready, connect to it using SSH.
   - Use the command: `ssh ubuntu@your-instance-ip` (replace `your-instance-ip` with your actual IP).

3. **Install Docker**
   - Run the following command to install Docker:
     ```
     sudo apt-get install docker.io
     ```
   - Start Docker:
     ```
     sudo systemctl start docker
     ```

4. **Install Docker-Compose**
   - Next, install Docker-Compose with:
     ```
     sudo apt-get install docker-compose
     ```

5. **Clone the Repository**
   - Clone the n8n-oracle-cloud-selfhost repository by running:
     ```
     git clone https://github.com/NitishReddy26/n8n-oracle-cloud-selfhost.git
     ```

6. **Navigate to the Folder**
   - Change to the project directory:
     ```
     cd n8n-oracle-cloud-selfhost
     ```

7. **Run the Setup**
   - Start the application using:
     ```
     docker-compose up -d
     ```
   - This command will run n8n in a Docker container. 

8. **Configure Nginx**
   - You need to set up Nginx as a reverse proxy for n8n. Follow the Nginx configuration steps provided in the documentation within the cloned repository.

9. **Set Up TLS**
   - For enhanced security, it’s recommended to install a TLS certificate. You can use Certbot to obtain a free SSL certificate.

10. **Access n8n**
    - Open your browser and go to `http://your-instance-ip` to access the n8n interface.

## 🌐 Features

- User-friendly interface for creating automated workflows.
- Easily integrates with multiple services such as Google Sheets, Slack, and more.
- Supports complex conditional workflows for advanced scenarios.
- Secure setup with TLS enables safe interactions.

## ⚙️ Troubleshooting

If you encounter any problems, consider the following:

- **Instance not reachable:** Check your security list and ensure the necessary ports (usually 80 and 443) are open.
- **Docker issues:** Ensure Docker is running and verified via `docker ps`.

## 📚 Resources

- [Docker Documentation](https://docs.docker.com/)
- [Nginx Documentation](https://nginx.org/en/docs/)
- [n8n Documentation](https://docs.n8n.io/)

## 📞 Support

If you need help, feel free to open an issue on the [GitHub repository](https://github.com/NitishReddy26/n8n-oracle-cloud-selfhost/issues). We monitor feedback and provide assistance to users.

## 🔗 Follow-Up

For the latest updates and improvements, check the Releases page regularly: 

[Download n8n-oracle-cloud-selfhost Releases](https://github.com/NitishReddy26/n8n-oracle-cloud-selfhost/releases)