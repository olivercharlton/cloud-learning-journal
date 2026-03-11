## Directing Traffic with Elastic Load Balancing

### Overview

This section explains how AWS handles the problem of uneven traffic distribution across multiple EC2 instances.

Even if a business has enough EC2 instances running, requests still need to be distributed properly. That is where **Elastic Load Balancing (ELB)** comes in.

ELB helps improve application scalability and efficiency by routing incoming traffic across multiple instances.

### Why load balancing matters

The lesson uses a coffee shop analogy.

If customers choose lines unevenly:
- one cashier can become overloaded
- other cashiers can sit idle

This is inefficient and slows down service.

The same problem can happen in AWS:
- some EC2 instances may receive too much traffic
- others may receive very little traffic

A load balancer helps solve this by directing requests more evenly.

### What a load balancer does

A **load balancer** receives incoming requests and routes them to available instances.

Its main goal is to:
- distribute workloads efficiently
- prevent some instances from being overloaded
- avoid leaving other instances idle
- improve application performance and scalability

### Elastic Load Balancing (ELB)

AWS provides a managed load balancing service called **Elastic Load Balancing (ELB)**.

With ELB:
- AWS handles the underlying management
- AWS handles patching and maintenance
- AWS handles upgrades and failover support

This is different from using a self-managed load balancer, where the customer would need to maintain it themselves.

### Why it is called “elastic”

The word **elastic** refers to ELB’s ability to adjust to changing traffic levels.

ELB can scale up or down with traffic demand automatically, helping applications handle variable workloads efficiently.

### Internal and external traffic

The lesson explains that ELB can manage:
- **external traffic** coming into AWS
- **internal traffic** between application tiers inside AWS

This makes it useful both for public-facing applications and for communication between internal components of an architecture.

### Decoupling application tiers

One of the most important ideas in this lesson is that ELB helps **decouple** parts of an application.

Example:
- a frontend tier sends requests to a backend tier
- without a load balancer, every frontend instance would need to know about every backend instance
- if a new backend instance is added, the frontend layer would need to be updated

This becomes difficult as the system grows.

With ELB:
- the frontend uses a single load balancer endpoint
- ELB handles sending traffic to the right backend instances
- backend instances can be added or removed without the frontend needing to track each one directly

This makes the architecture simpler and more scalable.

### Regional nature of ELB

The lesson explains that ELB is **Regional**.

This means it provides a single endpoint within a Region that can distribute traffic to instances behind it.

That makes it easier for one application tier to communicate with another without needing to know the details of every target instance.

### How ELB works with scaling

ELB works especially well with **Amazon EC2 Auto Scaling**.

When new backend instances are launched:
- they can register with the load balancer once ready
- ELB can then begin routing traffic to them automatically

This means the application can scale without requiring manual reconfiguration of all other components.

### Routing behavior

The lesson describes ELB directing traffic to the backend instance with the **least outstanding requests**.

This helps spread work efficiently and improves overall performance.

### Why this matters

Elastic Load Balancing is important because scaling is not just about having more instances. It is also about making sure traffic reaches those instances efficiently.

ELB helps businesses:
- distribute traffic evenly
- improve performance
- reduce overload on individual instances
- simplify multi-tier application design
- work smoothly with Auto Scaling

### Important terms

**Load balancer**  
A service or device that receives requests and routes them across multiple resources.

**Elastic Load Balancing (ELB)**  
AWS’s managed service for distributing traffic across multiple targets such as EC2 instances.

**Decoupling**  
Designing parts of an application so they are less dependent on each other.

**Frontend tier**  
The part of an application that interacts more directly with users or incoming requests.

**Backend tier**  
The part of an application that performs processing, logic, or data handling behind the scenes.

### Real-world examples

- A website sends incoming user traffic through ELB so requests are spread across several EC2 web servers.
- A frontend application tier sends requests to a backend tier through ELB instead of tracking every backend instance directly.
- A growing application launches new EC2 instances through Auto Scaling, and ELB automatically begins routing traffic to them once they are ready.

### Exam reminders

- ELB distributes incoming traffic across multiple EC2 instances.
- ELB improves scalability by routing traffic automatically.
- ELB can handle both internal and external traffic.
- ELB is a managed AWS service, so AWS handles patching, upgrades, and maintenance.
- ELB works well with EC2 Auto Scaling.
- ELB helps decouple application tiers by providing a single endpoint for traffic routing.
- One routing strategy mentioned in the lesson is sending traffic to the instance with the least outstanding requests.

### Test your skills takeaway

- Elastic Load Balancing improves scalability by automatically routing traffic to instances using routing methods designed to balance workload efficiently.
- One of ELB’s main tasks is to distribute a workload across multiple Amazon EC2 instances.

### My takeaway

This section made it clear that adding more EC2 instances is only part of the solution. Traffic also needs to be directed properly, otherwise some instances can become overloaded while others sit idle.

The main value of ELB is that it distributes traffic automatically and simplifies architecture by acting as a central point between users or application tiers and the EC2 instances behind it.
