# altschool-exam 2025

This is my repository for a cloud-hosted project showcasing a secure, personalized landing page powered by Nginx and hosted on AWS EC2.

## 🌐 Live Demo

> [http://toluwabori.chickenkiller.com](http://toluwabori.chickenkiller.com)  
> or  
> [https://3.89.217.243](https://3.89.217.243)

## 📦 Project Overview

This project demonstrates a modern and production-ready deployment workflow using:

- **AWS EC2** for cloud infrastructure
- **Ubuntu (20.04/22.04)** as the operating system
- **Nginx** as the primary web server
- **Freedns** for subdomains
- **Let’s Encrypt SSL** for secure HTTPS access
- A **dynamic HTML landing page** with personalized content

---

## 👤 Author Info

- **Name:** Toluwabori Ogunwenmo 
- **Track:** Cloud Engineering
- **AltSchool ID:** ALT/SOE/024/6033

## ⚙️ Tech Stack

| Component     | Technology        |
|---------------|-------------------|
| Cloud Provider | AWS EC2           |
| OS            | Ubuntu 22.04 LTS   |
| Web Server    | Nginx              |
| SSL           | Certbot (Let's Encrypt) |
| Frontend      | HTML + CSS         |

---

## 🔐 Networking & Security

- ✅ Port 80 (HTTP) and Port 443 (HTTPS) enabled
- ✅ SSL secured with Let’s Encrypt
- ✅ Reverse proxy optional configuration for Node.js apps

---

## 🧰 Deployment Instructions

1. **Provision EC2 Instance**
   ```bash
   # Ubuntu 22.04 on AWS EC2 with http and HTTPs enabled in setup
   ssh -i your-key.pem ubuntu@your-ec2-public-ip

2. **Update EC2 instance**
   ```bash
   sudo apt update
   sudo apt upgrade -y

3. **Install Nginx**
   ```bash
   sudo apt install nginx -y
   systemctl status nginx

4. **Install Unzip**
   ```bash
   sudo apt install unzip 

5. **Get zip file from Git Repo**
   ```bash
   wget https://github.com/BorgOwen/altschool-exam/archive/refs/heads/main.zip

6. **Unzip file and find location**
   ```bash
   unzip main.zip
   ls

7. **Copy contents of file to /var/www/html**
   ```bash
   sudo cp altschool-exam-main/* /var/www/html
   sudo systemctl reload nginx

8. **Reload nginx, check ec2 IP and subdomain**
   ```bash
   # Create an account on freedns.afraid.com and add your ec2 public address to the specified subdomain destination
   sudo systemctl reload nginx

9. **install Certbot**
   ```bash
   sudo apt install certbot python3-certbot-nginx -y

10.  **Run Certnot with nginx to enable SSL**
   ```bash
    # Follow the prompts to add SSL to your specified domain
   sudo certbot --nginx


## 📸 Screenshot of Deployed page

![domain](assets/01.png)

![Public IP](assets/02.png)
