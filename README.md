# Static Website Hosting on AWS EC2 using Nginx

## Project Overview

This project demonstrates how to deploy a static portfolio website on an Amazon EC2 instance running Ubuntu Server. The website was developed using HTML and CSS and hosted using the Nginx web server. Secure Shell (SSH) was used for remote server management, and Secure Copy Protocol (SCP) was used to transfer website files from the local computer to the EC2 instance.

---

## Technologies Used

- Amazon Web Services (AWS)
- Amazon EC2
- Ubuntu Server
- Nginx
- HTML5
- CSS3
- SSH
- SCP
- Visual Studio Code

---

## Project Structure

```
Website Hosting on AWS EC2
│
├── Website Files
│   ├── index.html
│   ├── style.css
│   └── images
│
├── Report
│
├── Screenshots
│
├── README.md
│
└── Commands_Used.txt
```

---

## Features

- Static portfolio website
- Hosted on AWS EC2
- Ubuntu Linux server
- Nginx web server
- Secure SSH access
- Secure file transfer using SCP
- Accessible through the EC2 Public IPv4 address

---

## Steps Performed

1. Created an AWS EC2 Ubuntu instance.
2. Configured Security Groups for SSH and HTTP.
3. Connected to the server using SSH.
4. Installed and configured Nginx.
5. Developed the portfolio website using HTML and CSS.
6. Transferred website files using SCP.
7. Copied website files to `/var/www/html`.
8. Verified successful deployment using a web browser.

---

## Linux Commands Used

```bash
sudo apt update

sudo apt install nginx -y

sudo systemctl status nginx

ssh -i MY_EC2_KEY2.pem ubuntu@<Public-IP>

scp -i MY_EC2_KEY2.pem -r "Website Files" ubuntu@<Public-IP>:/home/ubuntu

sudo cp index.html /var/www/html/

sudo cp style.css /var/www/html/

ls -l /var/www/html
```

---

## Learning Outcomes

- Understanding Amazon EC2
- Linux server administration
- SSH remote access
- Nginx configuration
- Static website deployment
- Secure file transfer using SCP
- Cloud-based web hosting

---

## Future Improvements

- Add HTTPS using SSL/TLS certificates.
- Connect a custom domain name.
- Improve website responsiveness.
- Automate deployment using CI/CD.
- Deploy using Amazon S3 and CloudFront.

---

## Author

**D. Prince Joyal Dhas**

Computer Science and Engineering

Rohini College of Engineering and Technology
