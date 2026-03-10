## What is cloud computing?

### Overview

This section explains how AWS began, gives a working definition of cloud computing, and introduces the idea of cloud deployment models such as hybrid deployment.

A key message from this section is that cloud computing is not just about technology, but about giving organizations easier access to IT resources without needing to own and manage all the underlying infrastructure themselves.

### How AWS started

AWS began as a solution to Amazon’s own internal technology challenges.

In the early 2000s, Amazon.com was growing quickly as an ecommerce platform. As more customers used the site, Amazon’s IT teams had to keep expanding their infrastructure by adding more servers, storage, and compute capacity.

To manage this growth more efficiently, Amazon developed standardized tools and systems that made its infrastructure more scalable and easier to operate. Eventually, the company realized these tools and methods could also help other businesses facing similar problems.

This led to the idea of offering computing resources as an on-demand service.

### Early AWS services

AWS launched its first public infrastructure service in **November 2004**:
- **Amazon Simple Queue Service (Amazon SQS)**

Later, AWS launched:
- **Amazon Simple Storage Service (Amazon S3)** for storage
- **Amazon Elastic Compute Cloud (Amazon EC2)** for scalable compute

At first, AWS was mainly used by start-ups and developers, but over time it expanded to serve:
- large enterprises
- government agencies
- businesses of all sizes

AWS continued to grow by adding services for:
- databases
- networking
- analytics
- and many other cloud functions

### Definition of cloud computing

Cloud computing is:

**the on-demand delivery of IT resources over the internet with pay-as-you-go pricing**

This definition can be broken into three main parts.

### 1. On-demand delivery

On-demand means you can access resources whenever you need them.

You do not need to buy hardware in advance or wait for long procurement and setup processes. Instead, you can create resources when needed and remove them when they are no longer required.

Example:
- if a business needs a large amount of storage, it can use Amazon S3
- if those files are no longer needed, they can be deleted
- once deleted, the business stops paying for that storage

### 2. Over the internet

Cloud resources are accessed remotely over the internet.

This means users can manage infrastructure from almost anywhere, as long as they have:
- an internet connection
- access to their AWS account

Instead of needing to be physically present in a company-owned data center, users can manage resources through a web browser or other tools.

### 3. Pay-as-you-go pricing

Pay-as-you-go means you only pay for the resources you actually use.

This allows organizations to avoid spending money on unused infrastructure. If a resource is no longer needed, it can be deprovisioned and the cost stops.

Important idea:
- provision resources when needed
- deprovision them when no longer needed
- avoid paying for idle capacity

### Data centers and traditional infrastructure

Before cloud computing became widely available, businesses usually had two main options:
- run applications in their own data centers
- colocate infrastructure in a shared facility

A **data center** is a building, or group of buildings, that houses servers and related infrastructure. Data centers are designed with:
- power redundancy
- cooling systems
- security measures

Traditionally, companies had to manage much more of this infrastructure themselves. With AWS, businesses can run applications in AWS data centers instead of owning and operating all the infrastructure directly.

This reduces operational burden and allows teams to focus more on building and improving their applications.

### Why AWS became important

AWS changed the way businesses use IT resources because it removed a lot of the barriers of traditional infrastructure.

Instead of:
- buying hardware upfront
- maintaining physical servers
- planning for maximum capacity in advance

businesses could:
- access resources on demand
- scale more easily
- manage infrastructure remotely
- pay only for what they use

This helps organizations move faster and focus more on innovation.

### Hybrid deployment

The skill check introduces the idea of **hybrid deployment**.

A hybrid deployment combines:
- on-premises resources
- cloud-based resources

This can be useful when:
- certain data must remain on-premises for compliance or legal reasons
- cloud resources are still needed for flexibility or scaling

Example:
A charity keeps sensitive data within its own country for compliance, but uses cloud resources to handle seasonal spikes in demand. That is a **hybrid deployment**.

### Important terms

**Cloud computing**  
The on-demand delivery of IT resources over the internet with pay-as-you-go pricing.

**Data center**  
A facility that contains servers and supporting infrastructure such as power, cooling, and security.

**Provision**  
To create or allocate resources.

**Deprovision**  
To remove resources that are no longer needed.

**Hybrid deployment**  
A deployment model that combines on-premises infrastructure with cloud-based resources.

### Real-world examples

- A company stores files in Amazon S3 instead of buying and managing physical storage hardware.
- A business launches compute resources in AWS when traffic increases and removes them when demand drops.
- An organization keeps regulated data on-premises but uses the cloud for extra capacity during busy periods.

### Exam reminders

- Cloud computing means **on-demand delivery of IT resources over the internet with pay-as-you-go pricing**.
- AWS started from Amazon’s internal need to build scalable infrastructure.
- Amazon SQS was AWS’s first public infrastructure service.
- Amazon S3 provides storage.
- Amazon EC2 provides scalable compute.
- Hybrid deployment means using both on-premises and cloud resources together.
- A major benefit of AWS is avoiding large upfront investment in hardware.

### My takeaway

AWS began by solving Amazon’s own infrastructure problems and then turned that solution into a service other organizations could use. The key cloud definition here is really important: on-demand, over the internet, and pay-as-you-go.

This section also helped show why cloud computing became so valuable. Instead of owning and managing everything yourself, you can use AWS resources when needed, access them remotely, and scale more easily. Hybrid deployment is also useful to remember because it shows that businesses do not always move everything fully into the cloud.
