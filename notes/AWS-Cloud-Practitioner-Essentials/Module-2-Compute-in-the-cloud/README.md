# Module 2: Compute in the Cloud

## Introduction to Amazon EC2

### Overview

This section introduces **Amazon Elastic Compute Cloud (Amazon EC2)**, which is AWS’s core compute service for running virtual servers in the cloud.

Amazon EC2 gives businesses access to raw compute capacity without needing to buy and manage physical servers on premises. It is designed to be flexible, scalable, and cost-effective.

### What Amazon EC2 is

Amazon EC2 is a service that provides **virtual machines**, called **EC2 instances**, in the AWS Cloud.

These instances can be used to run:
- business applications
- web applications
- databases
- internal tools
- third-party software

EC2 is essentially AWS’s way of giving customers server capacity on demand.

### Why EC2 matters

Businesses need compute power to host applications and respond to user requests.

Instead of:
- buying physical servers
- installing them in a data center
- maintaining them over time

AWS allows customers to launch EC2 instances in minutes and use only the compute capacity they need.

Compared with running servers on premises, EC2 is:
- more flexible
- more cost-effective
- quicker to get started with

### Pay only for what you use

One important benefit of EC2 is its pricing model.

With EC2:
- you pay for **running instances**
- you do **not** pay for instances that are stopped or terminated

This means businesses can launch instances when needed and stop using them when demand drops, helping reduce wasted cost.

### EC2 instances are virtual machines

EC2 instances are **virtual machines (VMs)**.

A virtual machine is not a separate physical computer. Instead, multiple VMs can run on the same physical host machine.

This setup is called **multi-tenancy**.

### Multi-tenancy

In a multi-tenant environment:
- multiple virtual machines share the same underlying physical hardware
- each VM is kept isolated from the others

This allows AWS to use hardware efficiently while still keeping customer workloads separate and secure.

### Hypervisor

The software that manages this sharing and isolation is called a **hypervisor**.

The hypervisor:
- allows multiple VMs to run on one physical host
- isolates instances from each other
- manages shared access to the host’s resources

For Amazon EC2:
- AWS manages the physical host
- AWS manages the hypervisor
- AWS manages the isolation between instances

Customers do not manage that lower-level infrastructure directly, but it is useful to understand the concept.

### Operating systems and software choices

When launching an EC2 instance, customers choose the operating system.

The transcript mentions choosing between:
- **Windows**
- **Linux**

Customers also decide what software to run on the instance, such as:
- internal applications
- web applications
- databases
- enterprise software packages

This means EC2 gives customers a high level of control over the server environment.

### Resizing EC2 instances

EC2 instances are **resizable**.

If an application needs more resources, the instance can be changed to provide more:
- CPU
- memory

Making an instance bigger or smaller like this is called **vertical scaling**.

This helps businesses adjust compute resources based on workload needs.

### Networking control

Customers also control the networking setup for their EC2 instances.

This includes deciding:
- what traffic can reach the instance
- whether the instance is publicly accessible
- whether it is privately accessible

This gives customers control over how their compute resources are exposed and protected.

### Compute as a Service

Virtual machines are not a new concept, but AWS makes them easier to access through a **Compute as a Service** model.

Instead of building and maintaining the physical server infrastructure yourself, AWS provides server capacity on demand through EC2.

### Important terms

**Amazon EC2**  
A cloud service that provides virtual servers, called instances, on demand.

**EC2 instance**  
A virtual machine running in AWS.

**Virtual machine (VM)**  
A software-based computer that runs on a physical host machine.

**Multi-tenancy**  
A model where multiple virtual machines share a physical host while remaining isolated from each other.

**Hypervisor**  
Software that creates and manages virtual machines on a host machine.

**Vertical scaling**  
Increasing or decreasing the size of an instance by changing its CPU or memory resources.

### Real-world examples

- A company launches EC2 instances to host its website instead of buying physical web servers.
- A business runs internal applications on Linux EC2 instances.
- An application outgrows a small instance, so the team increases memory and CPU by resizing it.
- A company launches extra EC2 instances during busy periods and stops them later to reduce cost.

### Exam reminders

- Amazon EC2 provides **virtual servers in the cloud**.
- EC2 is more flexible, more cost-effective, and quicker to get started with than on-premises servers.
- EC2 instances are **virtual machines**.
- Multi-tenancy means multiple VMs share one physical host while remaining isolated.
- AWS manages the physical host and the hypervisor.
- Customers choose the operating system and software for EC2 instances.
- You pay for **running** instances, not stopped or terminated ones.
- Resizing an instance up or down is called **vertical scaling**.

### Test your skills takeaway

Key points reinforced by the questions:
- Amazon EC2 is more flexible, cost-effective, and faster to start with than on-premises servers.
- Multi-tenancy means virtual machines share host resources while remaining isolated.
- You only pay for running instances.
- Before launching an EC2 instance, you need to choose the **instance type** and the **operating system**.

### My takeaway

Amazon EC2 seems like one of the most important AWS services because it gives businesses direct access to compute power in the form of virtual servers. It offers much of the flexibility of traditional servers, but without needing to own the underlying hardware.

The biggest ideas here are that EC2 instances are virtual machines, AWS manages the lower-level infrastructure, and customers can quickly launch, stop, resize, and configure servers based on their needs.
