## Launching an Amazon EC2 Instance

### Overview

This section walks through the basic process of launching an Amazon EC2 instance through the **AWS Management Console**.

The example used is a simple **web server**, and the lesson highlights the main configuration choices needed during launch.

### Goal of the example

The purpose of this walkthrough is to show how to create an EC2 instance that can host a basic web server.

The process uses the AWS Management Console and introduces some of the most important launch settings:
- instance name
- Amazon Machine Image (AMI)
- instance type
- key pair
- network settings
- storage
- user data

### Steps to launch an EC2 instance

### 1. Open the EC2 console
The process starts in the **EC2 console** within the AWS Management Console.

From there, the user selects **Launch instance**.

### 2. Choose an instance name
The instance is given a name so it can be identified more easily later.

This is mainly for organization and management.

### 3. Choose an Amazon Machine Image (AMI)
An **Amazon Machine Image (AMI)** is a template used to launch an EC2 instance.

It includes:
- the operating system
- built-in software or applications
- preconfigured settings in some cases

In this example, the chosen AMI is:
- **Amazon Linux AMI**

This AMI is described as a good default choice for a general-use web server.

### 4. Choose the instance type
The **instance type** determines the hardware characteristics of the EC2 instance.

This affects:
- compute power
- memory
- performance characteristics

In the example, the instance type chosen is:
- **t2.micro**

The lesson notes that this option includes:
- 1 virtual CPU
- 1 GiB of memory
- Free Tier eligibility

### 5. Choose a key pair
A **key pair** is used for securely logging in to the EC2 instance.

A key pair includes:
- a **public key**, which is placed on the EC2 instance
- a **private key**, which the user keeps

This is an important part of secure access to the instance.

### 6. Configure network settings
The network settings determine how the instance can be reached.

In the web server example, the key setting is:
- allow **HTTP traffic** from the internet

This is necessary because the EC2 instance is meant to serve web content publicly.

### 7. Configure storage
The instance also needs storage.

In the example, the configuration uses:
- **8 GiB**
- **gp3 EBS volume**

This provides disk space for the instance and its web server files.

### 8. Add user data
The example then uses **User Data** in the **Advanced Details** section.

User data allows a script to run automatically when the instance launches.

In this case, the script installs and starts the **Nginx web server** so that the instance can serve content immediately after launch.

This is a useful automation feature because it helps configure the instance automatically at startup.

### 9. Launch the instance
After choosing the settings, the instance is launched.

Once it is running, the user can view its details in the EC2 console.

### 10. Access the web server
After launch, the lesson copies the instance’s **public IP address** and opens it in a browser.

Because the instance was configured as a web server and allowed HTTP traffic, the browser is able to reach it successfully.

### Important configurations to remember

The skill check highlights three required configurations for launching a basic EC2 web server:
- **Amazon Machine Image (AMI)**
- **Instance type**
- **Storage**

These are core launch choices.

Other options, like load balancing, are useful in some architectures, but are not required for launching a basic single EC2 web server.

### What an AMI does

An **AMI** is especially important because it defines the starting template for the EC2 instance.

It is used to:
- choose the operating system
- include software if needed
- help launch instances quickly with a predefined setup

### Important terms

**Amazon Machine Image (AMI)**  
A template used to launch an EC2 instance, including the operating system and optional software.

**Instance type**  
The selected hardware profile for an EC2 instance, defining CPU, memory, and related resources.

**Key pair**  
A public/private key combination used for securely connecting to an EC2 instance.

**EBS (Elastic Block Store)**  
Block storage that can be attached to an EC2 instance.

**gp3**  
A type of EBS volume used for general-purpose SSD storage.

**User data**  
A startup script that runs automatically when an EC2 instance launches.

**Public IP address**  
An IP address that allows the EC2 instance to be reached over the internet, depending on network configuration.

### Real-world examples

- A developer launches an EC2 instance using an Amazon Linux AMI and installs a web server using user data.
- A team chooses a small instance type such as t2.micro for a lightweight test web server.
- A business uses EBS storage to give an EC2 instance persistent disk space.
- An administrator allows HTTP traffic so users can access a hosted website from a browser.

### Exam reminders

- Launching an EC2 instance requires selecting an **AMI**, **instance type**, and **storage**.
- An **AMI** defines the operating system and possible preinstalled software.
- A **key pair** is used to help securely access the EC2 instance.
- **User data** can automate software installation and configuration at launch.
- A web server must allow **HTTP traffic** if it is meant to be reachable from the internet.
- EBS provides storage for EC2 instances.

### Test your skills takeaway

- The required configurations highlighted for launching a basic EC2 web server are:
  - **Amazon Machine Image (AMI)**
  - **Instance type**
  - **Storage**
- An **AMI** is used to preconfigure the operating system and software for an EC2 instance.

### My takeaway

This section made the EC2 launch process feel much more concrete. Instead of just thinking of EC2 as a virtual server, I now see the key choices involved in creating one, such as the AMI, instance type, networking, and storage.

The most important idea here is that launching an instance is really about choosing the right starting template, hardware profile, access method, and network/storage settings for the workload.
