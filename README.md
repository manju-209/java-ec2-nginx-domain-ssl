# Java Application Deployment on AWS EC2 🚀

## Project Overview
This project demonstrates how I deployed a Java web application on AWS EC2, 
connected it with a custom domain using Nginx, and secured it with HTTPS using Let’s Encrypt.

## Tech Stack
- AWS EC2 (Amazon Linux)
- Java (Spring Boot JAR)
- Nginx (Reverse Proxy)
- Domain & DNS (Hostinger)
- SSL (Let’s Encrypt + Certbot)

## Architecture
User → Domain → Nginx (80/443) → Java App (8080)

## What I Did
- Deployed Java app on EC2
- Ran application on port 8080
- Configured Nginx as reverse proxy
- Mapped custom domain (lithu.cfd)
- Enabled HTTPS with SSL
- Closed backend ports for security

## Live Output
🔒 https://lithu.cfd

## Key Learnings
- EC2 server setup
- Nginx reverse proxy
- DNS configuration
- SSL certificate setup
- Real-world troubleshooting

## Author
Manjukrishna
