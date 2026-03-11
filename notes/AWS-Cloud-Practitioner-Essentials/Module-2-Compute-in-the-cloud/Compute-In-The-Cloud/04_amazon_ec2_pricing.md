## Amazon EC2 Pricing

### Overview

This section explains that Amazon EC2 has multiple pricing options, allowing customers to choose a model that best fits their workload, budget, and level of flexibility needed.

The main idea is that AWS offers different ways to pay for EC2 depending on whether the workload is:
- short-term or unpredictable
- steady and predictable
- interruption-tolerant
- security or compliance sensitive

### Why pricing options matter

Not every workload behaves the same way.

Some workloads:
- are temporary
- change frequently
- need maximum flexibility

Others:
- run consistently over time
- benefit from long-term commitments
- need dedicated hardware for compliance or licensing reasons

AWS provides several pricing models so customers can match cost to usage pattern.

### 1. On-Demand

**On-Demand** pricing means you pay only for the time your EC2 instance runs.

This may be billed:
- per hour
- or per second

depending on the instance type and operating system.

Key characteristics:
- no upfront payment
- no long-term commitment
- flexible and self-service

This is often the best starting point for customers who are:
- testing workloads
- experimenting
- learning EC2
- unsure of long-term usage patterns

It helps customers understand their baseline usage before committing to other pricing models.

### 2. Savings Plans

**Savings Plans** provide lower prices in exchange for a commitment to a consistent amount of usage.

This commitment is measured in:
- dollars per hour

for either:
- 1 year
- 3 years

The lesson states that Savings Plans can provide savings of up to **72%**.

A key benefit is that they can apply broadly across:
- instance family
- instance size
- operating system
- tenancy
- AWS Region

The lesson also notes that Savings Plans can apply to:
- AWS Fargate
- AWS Lambda

This makes them flexible for organizations with consistent compute use across different AWS services.

### 3. Reserved Instances

**Reserved Instances** are designed for workloads with steady or predictable usage.

They can provide up to **75%** discount compared to On-Demand pricing when the customer commits to:
- 1 year
- 3 years

Payment options include:
- **All upfront**
- **Partial upfront**
- **No upfront**

Reserved Instances are useful when a workload is stable enough that long-term planning makes sense.

### 4. Spot Instances

**Spot Instances** let customers use spare AWS compute capacity at a very large discount.

The lesson states that Spot Instances can provide up to **90%** off On-Demand pricing.

The tradeoff is that AWS can reclaim the instance at any time.

Important detail:
- AWS provides a **two-minute warning** before interruption

Spot Instances are a strong choice for workloads that:
- can tolerate interruptions
- can save progress and resume later
- do not require continuous guaranteed runtime

### 5. Dedicated Hosts

**Dedicated Hosts** are physical servers reserved for one customer’s exclusive use.

This means:
- no other customer shares the server
- the customer has control over instance placement
- the customer has more control over resource allocation

This is useful for:
- security-sensitive workloads
- licensing-specific workloads
- regulatory or compliance requirements

Examples mentioned include:
- Windows
- SQL Server

Dedicated Hosts are often chosen when physical isolation matters.

### Choosing the right pricing model

The best pricing model depends on the workload.

General guidance:
- **On-Demand** = best for getting started and for unpredictable usage
- **Savings Plans** = good for consistent ongoing usage with flexibility
- **Reserved Instances** = good for steady predictable workloads
- **Spot Instances** = best for interruption-tolerant workloads
- **Dedicated Hosts** = best for workloads needing physical isolation and control

### Important terms

**On-Demand**  
A pricing model where you pay only for the time the instance runs, with no long-term commitment.

**Savings Plans**  
A pricing model offering reduced rates in exchange for a commitment to a certain amount of usage over time.

**Reserved Instances**  
A pricing option for predictable workloads that offers discounts for 1-year or 3-year commitments.

**Spot Instances**  
A pricing option that uses spare AWS capacity at a large discount, but can be interrupted by AWS.

**Dedicated Hosts**  
Physical servers reserved for one customer only.

**Tenancy**  
Whether hardware is shared or dedicated for use by one customer.

### Real-world examples

- A new customer testing an application starts with **On-Demand** pricing.
- A company with stable long-term usage chooses **Reserved Instances** or **Savings Plans** for lower costs.
- A startup running batch jobs that can pause and resume uses **Spot Instances** to save money.
- A financial services company with strict compliance needs uses **Dedicated Hosts** for isolated physical servers.

### Exam reminders

- **On-Demand** pricing is flexible and requires no upfront commitment.
- **Savings Plans** offer lower prices for consistent usage commitments.
- **Reserved Instances** are best for predictable, steady-state workloads.
- **Spot Instances** offer the biggest savings but can be interrupted.
- **Dedicated Hosts** provide exclusive use of physical hardware.
- Spot Instances can be reclaimed by AWS with a **two-minute warning**.
- Dedicated Hosts are useful for compliance, security, and licensing needs.

### Test your skills takeaway

- A company needing full control over the physical server should choose **Dedicated Hosts**.
- A workload that can tolerate interruptions and wants maximum savings should use **Spot Instances**.
- A customer just getting started with uncertain usage should begin with **On-Demand** pricing.

### My takeaway

This section shows that EC2 pricing is not one-size-fits-all. AWS gives customers multiple pricing options so they can choose the best fit based on flexibility, predictability, and workload requirements.

The easiest way to remember this is:
- start with **On-Demand**
- save more with **Savings Plans** or **Reserved Instances** if usage becomes predictable
- use **Spot** for interruption-tolerant workloads
- use **Dedicated Hosts** when physical isolation matters
