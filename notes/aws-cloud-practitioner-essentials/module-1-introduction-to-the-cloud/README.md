# Module 1: Introduction to the Cloud

## Overview

This section introduces the basic idea of cloud computing and begins with one of the most important foundational concepts: the **client-server model**. It also introduces a core AWS principle: **you only pay for what you use**.

The lesson uses a coffee shop analogy to explain these ideas in a simple way.

## Key concepts

### What is the cloud?
The cloud refers to computing resources and services that are delivered over the internet instead of being hosted entirely on local, on-premises infrastructure.

AWS provides a wide range of cloud services that businesses can use for things like:
- compute power
- storage
- databases
- content delivery
- generative AI
- specialized application services

AWS is designed to help organizations become more agile, reduce costs, and innovate faster.

### The client-server model
The client-server model is a basic computing concept where:
- the **client** makes a request
- the **server** receives, processes, and responds to that request

In the lesson’s analogy:
- the **customer** is the client
- the **barista** is the server

The customer places an order, and the barista prepares and returns the drink. In computing, this is similar to a user requesting data or a service from a server.

### Request and response
A major part of the client-server model is the idea of a request and response.

The process looks like this:
1. the client sends a request
2. the server checks whether the request is valid
3. the server returns a response

In the coffee shop example:
- the request is the coffee order
- the validation is whether the customer paid and whether the item can be made
- the response is the finished drink

## AWS-specific idea introduced

### Pay only for what you use
One of the first AWS-specific principles introduced in this section is that AWS uses a **pay-as-you-go** model.

This means:
- you do not need to pre-pay for unused capacity
- you can provision resources when needed
- you can remove resources when they are no longer needed
- once resources are deprovisioned, you stop paying for them

The coffee shop analogy explains this through staffing:
- busy periods may require more baristas
- quiet periods require fewer baristas
- paying for extra idle staff all day would be inefficient

This is compared to traditional on-premises infrastructure, where businesses often need to buy enough capacity in advance to handle peak demand, even if much of that capacity sits unused most of the time.

With AWS, resources can be scaled up or down more flexibly.

## Why this matters

These concepts matter because they explain two important cloud fundamentals:

1. **how cloud systems work at a basic level**
   - users request services
   - servers process and return results

2. **why cloud computing is attractive to businesses**
   - more flexibility
   - less wasted capacity
   - better cost efficiency
   - easier scaling

## Real-world examples

- A user opens a website in their browser. The browser acts as the client and sends a request to a server, which returns the webpage.
- A streaming app requests video data from a server, and the server delivers it back to the user.
- A business increases AWS resources during high demand and reduces them later so it only pays for what it actually used.

## Important terms

**Cloud computing**  
The delivery of IT resources over the internet.

**Client**  
The user or system that makes a request.

**Server**  
The system that receives the request, processes it, and sends back a response.

**Provision**  
To create or allocate resources.

**Deprovision**  
To remove resources that are no longer needed.

**Pay-as-you-go**  
A pricing model where you only pay for the resources you actually use.

## Exam reminders

- The **client** makes the request.
- The **server** processes the request and returns a response.
- AWS emphasizes **only paying for what you use**.
- Cloud computing helps reduce the problem of overpaying for unused infrastructure.
- On-premises environments often require capacity planning in advance, while AWS allows more flexible provisioning.

## My takeaway

This section is mainly about understanding the very basics of cloud computing before moving into more detailed AWS topics. The two biggest ideas here are the client-server model and AWS’s pay-as-you-go pricing approach.

The coffee shop analogy makes it easier to understand that cloud computing is not just about technology, but also about operating more efficiently. AWS allows businesses to get resources when needed and stop paying when they are no longer needed.
