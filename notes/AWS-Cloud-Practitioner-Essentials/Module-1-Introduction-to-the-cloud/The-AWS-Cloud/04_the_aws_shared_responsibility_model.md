## The AWS Shared Responsibility Model

### Overview

This section explains how security works on AWS through the **AWS Shared Responsibility Model**.

The key idea is that security on AWS is shared between:
- **AWS**
- **the customer**

AWS and the customer are both responsible for security, but they are responsible for different parts of the environment.

### Core principle

The simplest way to remember this model is:

**AWS is responsible for security of the cloud**  
**The customer is responsible for security in the cloud**

This is one of the most important foundational ideas in AWS.

### House analogy

The lesson compares AWS security to owning a house.

- The builder is responsible for building strong walls and solid doors.
- The homeowner is responsible for locking the doors and controlling who can enter.

In the same way:
- AWS secures the infrastructure it provides
- the customer secures what they run and store on top of that infrastructure

### AWS responsibilities: security of the cloud

AWS is responsible for securing the underlying infrastructure that runs AWS services.

This includes:
- the **physical layer**
- the **network layer**
- the **hypervisor layer**

#### Physical layer
This includes the physical hardware and facilities used to run AWS services.

Examples:
- securing buildings
- controlling physical access
- protecting servers and infrastructure hardware

#### Network layer
AWS is responsible for protecting the networking systems that support the cloud environment.

#### Hypervisor layer
The hypervisor is the virtualization layer that allows multiple workloads to run in isolated environments.

AWS secures this layer to help maintain separation and protection between customer workloads.

### Customer responsibilities: security in the cloud

The customer is responsible for what they run inside AWS.

This includes:
- the **operating system**
- **applications**
- **data**

#### Operating system
If you are running an operating system in the cloud, you are responsible for managing and securing it.

This includes:
- patching the OS
- managing user accounts
- controlling access
- applying security updates

AWS does not log into your operating system and apply patches for you.

#### Applications
You are also responsible for the applications you deploy.

This means you must:
- manage application security
- configure them properly
- keep them updated
- protect them from vulnerabilities

#### Data
Your data is also your responsibility.

You control:
- who can access it
- whether it is public or private
- how it is protected
- whether it is encrypted

AWS gives customers tools and controls for managing access and encryption, but the customer decides how those controls are used.

### Encryption

The lesson also highlights that customers can encrypt their data.

Encryption helps protect data by making it unreadable without the proper key.

This is useful because even if access is misconfigured, encrypted data adds another layer of protection.

### Responsibility can vary by service

The shared responsibility model stays true across AWS, but the exact details can vary depending on which AWS service is being used.

In general:
- AWS always secures the underlying cloud infrastructure
- the customer is responsible for the things they configure, manage, and store

Later services may shift some responsibilities depending on how managed the service is.

### Why this matters

This model is important because customers should not assume AWS handles all security automatically.

Using AWS does not remove the customer’s responsibility. Instead, AWS and the customer each handle their own part of securing the environment.

Understanding this helps prevent security mistakes and makes it clearer who is responsible for what.

### Real-world examples

- AWS secures the physical data center, but the customer is responsible for patching the operating system on a virtual server.
- AWS protects the infrastructure, but the customer controls whether their application is properly configured.
- AWS provides encryption tools, but the customer decides whether to enable encryption and who can access the data.

### Important terms

**Shared Responsibility Model**  
A security model in which AWS and the customer each have different security responsibilities.

**Security of the cloud**  
AWS’s responsibility to protect the infrastructure that runs AWS services.

**Security in the cloud**  
The customer’s responsibility to secure their operating systems, applications, and data.

**Hypervisor**  
The virtualization layer that allows multiple workloads to run in isolated environments.

**Encryption**  
The process of protecting data by converting it into unreadable form unless the correct key is used.

### Exam reminders

- Security on AWS is a **shared responsibility**.
- AWS is responsible for **security of the cloud**.
- The customer is responsible for **security in the cloud**.
- AWS secures the physical infrastructure, networking, and hypervisor.
- The customer is responsible for the operating system, applications, and data.
- Applying security patches to the operating system is the **customer’s responsibility**.

### Test your skills takeaway

If an operating system in the cloud needs a security patch, the correct answer is:

**The customer is responsible for applying security patches to the operating system.**

This is because the operating system is part of the customer’s responsibility in the shared responsibility model.

### My takeaway

This section makes it clear that AWS does not handle every part of security automatically. AWS secures the cloud infrastructure, but customers still need to secure what they run inside AWS.

The most important phrase to remember is: **security of the cloud vs security in the cloud**. That seems like one of the biggest foundational ideas for understanding AWS security.
