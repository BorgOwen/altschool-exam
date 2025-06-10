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
- **Let’s Encrypt SSL** for secure HTTPS access
- A **dynamic HTML landing page** with personalized content

---

## 👤 Author Info

**Name:** Toluwabori Ogunwenmo 
**Track:** Cloud Engineering
**AltSchool ID:** ALT/SOE/024/6033

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
- ✅ UFW firewall configured (if applicable)
- ✅ SSL secured with Let’s Encrypt
- ✅ Reverse proxy optional configuration for Node.js apps

---

## 🧰 Deployment Instructions

1. **Provision EC2 Instance**
   ```bash
   # Ubuntu 22.04 on AWS EC2
   ssh -i your-key.pem ubuntu@your-ec2-public-ip

2. **Update and Install Nginx**
   ```bash
   sudo apt update
   sudo apt upgrade -y
   sudo apt install nginx -y

