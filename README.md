
---

```markdown
# 🚀 DevOps Project #1 – Static Website Deployment on AWS EC2 with Nginx

This is my first hands-on DevOps project where I deployed a static website using **AWS EC2** and **Nginx**.

## 📌 Project Overview

This project demonstrates how to:

- Launch an AWS EC2 instance
- Install and configure **Nginx** as a web server
- Upload a simple static website (HTML + CSS)
- Start and enable the Nginx service
- Access the deployed site via Public IP

---

## 📁 Project Structure

```
DevOps1/
│
├── index.html     # Home page with welcome message
├── style.css      # Styling for the page
```

---

## 🔧 Tech Stack Used

- AWS EC2 (Amazon Linux 2)
- Nginx Web Server
- HTML + CSS
- SSH + Linux CLI

---

## 🚀 Steps to Reproduce

1. **Launch EC2 Instance**  
   Choose Amazon Linux 2 with security group allowing **port 80 (HTTP)**.

2. **Install Nginx**
   ```bash
   sudo yum update -y
   sudo amazon-linux-extras install nginx1 -y
   sudo systemctl start nginx
   sudo systemctl enable nginx
   ```

3. **Upload Files**
   ```bash
   # Copy your project files to the server (via SCP or Git clone)
   sudo cp ~/DevOps1/* /usr/share/nginx/html/
   ```

4. **Access the Website**  
   Open the **Public IPv4 address** in your browser.

---

## 🌐 Live Demo

> _Deployed on AWS EC2_  
> 🔗 http://<Your-EC2-Public-IP>

---

## 📸 Screenshots

![Website Screenshot](./screenshot.png) <!-- optional -->

---

## 🧠 What I Learned

- Basics of launching and managing an EC2 instance
- Installing and serving static content using Nginx
- Handling file permissions with `sudo`
- Starting, restarting, and enabling services using `systemctl`
- Setting up Security Groups for public access

---

## 📍What's Next?

✔️ Add CI/CD using GitHub + AWS CodeDeploy  
✔️ Automate deployment with shell scripts  
✔️ Explore Docker and containerized deployment  

---

## 📬 Connect With Me

Feel free to connect if you're also learning DevOps!  
🔗 [LinkedIn](https://linkedin.com/in/zaheer-mulani)  
📁 [GitHub](https://github.com/RBZAHEER)

---
