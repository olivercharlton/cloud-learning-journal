## How to Provision AWS Resources

### Overview

This section explains how users actually interact with AWS services.

The main idea is that in AWS, **everything is an API call**. AWS provides APIs that customers use to create, configure, and manage resources. These API calls can be made in three main ways:
- AWS Management Console
- AWS Command Line Interface (CLI)
- AWS Software Development Kit (SDK)

### APIs in AWS

An **API** is an **application programming interface**.

In AWS, APIs define the ways customers interact with AWS services. When you create, configure, or manage an AWS resource, you are making an API call.

This means that actions such as:
- launching an EC2 instance
- listing Availability Zones
- checking resources
- updating configurations

are all done through AWS APIs.

### Three main ways to call AWS APIs

### 1. AWS Management Console

The **AWS Management Console** is the browser-based interface for AWS.

It allows users to manage resources visually through a point-and-click interface.

The console is especially useful for:
- getting started with AWS
- learning services visually
- setting up test environments
- viewing AWS bills
- monitoring resources
- handling non-technical management tasks

For beginners, the console is often the easiest place to start.

#### Limitation of the console
The console is less ideal for repeated manual work in production environments.

For example, if you launch an EC2 instance manually through the console, you have to:
- go through several screens
- select configurations
- repeat those steps again for future instances

This manual process increases the chance of human error, such as:
- missing a checkbox
- entering the wrong value
- inconsistent configuration

### 2. AWS Command Line Interface (CLI)

The **AWS CLI** allows users to call AWS APIs from a terminal using text commands.

Instead of clicking through screens, users type commands to interact with AWS resources.

Examples from the lesson:
- `aws ec2 run-instances`
- `aws ec2 describe-availability-zones`

A major benefit of the CLI is that it supports:
- automation
- scripting
- repeatable processes

This makes it much more useful for managing resources efficiently over time.

#### AWS CloudShell
The lesson also mentions **AWS CloudShell**, which is a cloud-based terminal environment with the AWS CLI already installed.

This makes it easier to run AWS CLI commands without setting up the CLI locally.

### 3. AWS Software Development Kit (SDK)

The **AWS SDK** allows users to interact with AWS services through programming languages.

For example, developers can use the SDK in languages such as:
- Python

The SDK is useful when building applications or automation that needs to work directly with AWS resources through code.

In the lesson, a Python script is used to list EC2 instances in the current Region.

### Why automation matters

A major theme in this section is that automation is important in cloud environments.

Automation helps make deployments:
- more consistent
- more predictable
- less dependent on manual steps
- less prone to human error

This is why the CLI and SDK are especially valuable in production-type environments.

### Key idea to remember

No matter which method you use:
- Management Console
- AWS CLI
- AWS SDK

AWS APIs are still being called behind the scenes.

The difference is mainly **how** you interact with them:
- visually
- through terminal commands
- through code

### Shared responsibility reminder for EC2

The skill check also reinforces the AWS Shared Responsibility Model for compute services like Amazon EC2.

For EC2:
- AWS manages the underlying hardware and infrastructure
- the customer is responsible for configuring and managing the operating system, networking, and applications on the EC2 instance

### Important terms

**API (Application Programming Interface)**  
A predefined way to interact with AWS services.

**AWS Management Console**  
The browser-based visual interface for managing AWS resources.

**AWS CLI**  
A command-line tool for interacting with AWS services through text commands.

**AWS SDK**  
A set of tools that allows developers to interact with AWS services through programming languages.

**AWS CloudShell**  
A cloud-based terminal environment that includes the AWS CLI.

**Automation**  
Using scripts or code to perform tasks consistently and with less manual effort.

### Real-world examples

- A beginner launches an EC2 instance through the AWS Management Console while learning the service.
- A system administrator uses the AWS CLI in a script to create and configure resources automatically.
- A developer uses the AWS SDK in Python to list EC2 instances or manage AWS resources from an application.
- A company uses automation to reduce manual provisioning mistakes in production.

### Exam reminders

- In AWS, everything is an **API call**.
- There are three main ways to interact with AWS APIs:
  - AWS Management Console
  - AWS CLI
  - AWS SDK
- The console is useful for learning, visual management, and simple tasks.
- The AWS CLI is useful for automation and scripting.
- The AWS SDK is used to interact with AWS through programming languages.
- AWS CloudShell includes the AWS CLI in a managed cloud-based terminal.
- Manual provisioning increases the risk of human error.
- In Amazon EC2, the customer is responsible for the operating system, networking, and applications.

### Test your skills takeaway

- A primary advantage of the **AWS CLI** over the console is that it supports **automation and scripting**, which reduces manual steps and human error.
- For **Amazon EC2**, the customer is responsible for configuring, securing, and managing the operating system, networking, and applications running on the instance.

### My takeaway

This section made it clearer how AWS resources are actually created and managed. The biggest point is that everything in AWS happens through APIs, whether I use the visual console, the command line, or code.

It also shows why automation matters in the cloud. The console is useful for learning, but the CLI and SDK are much better for repeatable, scalable, and less error-prone ways of managing infrastructure.
