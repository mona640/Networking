
# AWS EC2 and DNS Project

## Project Overview

In this project, I deployed an Nginx web server on an AWS EC2 instance and connected it to a custom domain using Cloudflare DNS.

The aim was to understand how cloud servers, public IP addresses and DNS records work together to make a website accessible through a domain name.

## Steps Taken

### 1. Created an AWS EC2 Instance

I launched an EC2 instance on AWS using the `t3.micro` instance type.

I configured the instance to allow HTTP traffic on port 80 so that the web server could be accessed through a browser.



### 2. Installed Nginx

I installed Nginx on the EC2 instance to serve a webpage.

Nginx is a web server that handles HTTP requests and delivers web content to users.

### 3. Purchased a Domain Name

I purchased the domain `monaaziz.co.uk` so I could access my web server using a domain name instead of entering its public IP address.

### 4. Configured Cloudflare DNS

I configured an A record in Cloudflare to point my domain name to the public IPv4 address of my EC2 instance.

An A record maps a domain name to an IPv4 address, allowing devices to locate the server associated with that domain.



### 5. Tested the Web Server

After configuring the DNS record, I entered my domain name into Safari.

The Nginx welcome page appeared successfully, confirming that my domain was able to reach the web server.



## How It Works

1. A user requests my domain name.
2. DNS resolves the domain to Cloudflare's proxy IP address.
3. Cloudflare forwards the HTTP request to my EC2 instance.
4. Nginx receives the request and serves the webpage.
5. The response is returned to the user's browser.

## What I Learnt

This project helped me understand how to deploy a web server using AWS EC2 and connect it to a custom domain.

I learnt how A records work, why public IP addresses are needed to reach internet-facing servers, and how DNS allows users to access websites without remembering IP addresses.

It also helped me understand how Nginx handles web requests and how different networking components work together.

## Result

Successfully deployed an Nginx web server on AWS EC2 and connected it to my custom domain using Cloudflare DNS.
