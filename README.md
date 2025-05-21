# CyberSecurity-Home-Lab
Web Application Firewall Home Lab Using SafeLine WAF

1. Lab Architecture and Overview

In this lab, we will build a cybersecurity home lab using VirtualBox, Kali Linux,
Ubuntu, and SafeLine WAF.

![image alt](https://github.com/Teddy-hub-oss/CyberSecurity-Home-Lab/blob/fbbc94de816f74d861977db5ebb81222d62e7fc6/img.png)

The goal is to:

1 Set up a vulnerable web application on Ubuntu, the web will be Damn Vulnerable Web Application(DVWA)

2 Demonstrate how to perform a basic SQL injection attack from Kali Linux.

3 to Show how SafeLine WAF protects against such attacks.

4 HTTP flood defense, custom deny rules, etc


2 Lab Environment Setup 

 Download and Install VirtualBox
 Download Kali Linux and Create the Kali Linux Virtual Machine
 Download Ubuntu Server and Create the Ubuntu Server Virtual Machine 


3 Enable Bridged Networking for Ubuntu and Kali Linux 
To have VMs appear on the same network as your host and each other 
 Install Guest Additions can help with screen resizing shared clipboard and shared folders


4 Ubuntu Server Configuration 
4.1 Update the Package List and Upgrade:
sudo apt-get update && sudo apt-get upgrade -y

Install Net-Tools for for ifconfig and other network utilities:
sudo apt-get install -y net-tools 

Install OpenSSL:
suod apt-get install -y openssl

4.2 Install and Configuring LAMP Stack
Install Apache2, PHP, and MYSQL:
sudo apt-get install -y apache2 php php-mysql mysql server

Secure the MySql Installation optional but recommended 
sudo mysql_secure_installation

4.3 
