## Scaling Amazon EC2

### Overview

This section introduces two major cloud concepts: **scalability** and **elasticity**.

These ideas explain how AWS can adjust compute capacity based on demand, helping businesses maintain performance for customers while also controlling cost.

The lesson also introduces:
- horizontal scaling
- vertical scaling
- high availability across multiple Availability Zones
- Amazon EC2 Auto Scaling
- Amazon CloudWatch

### Why scaling matters

Demand is not always constant.

A business might have:
- regular average traffic
- seasonal spikes
- short-term demand surges
- unpredictable usage changes

If a company only plans for average demand, customers may have a poor experience during busy periods.

If a company always plans for peak demand, it may end up paying for a lot of unused capacity.

AWS helps solve this by allowing resources to grow and shrink based on real demand.

### Scalability and elasticity

#### Scalability
**Scalability** is the ability to increase or decrease resources to handle changing workload demands.

#### Elasticity
**Elasticity** is the ability to automatically adjust capacity so it closely matches current demand.

Together, these help businesses:
- maintain performance
- avoid over-provisioning
- reduce wasted cost

### Redundancy and high availability

Before scaling for traffic growth, the lesson first explains the importance of redundancy.

If only one EC2 instance is handling a task and that instance fails, the service could go down.

A best practice is to launch redundant EC2 instances so another instance can continue serving traffic if one fails.

To improve resilience further, these instances should be deployed across **multiple Availability Zones (AZs)** in a Region.

This helps provide:
- high availability
- reduced risk of a single point of failure

### Horizontal scaling

**Horizontal scaling**, also called **scaling out**, means adding more instances or resources to the environment.

This allows more work to be handled in parallel.

Example:
- if more customer requests come in
- more EC2 instances can be added to handle the load

This is often useful when adding more separate workers is better than just making one machine more powerful.

### Vertical scaling

**Vertical scaling**, also called **scaling up**, means increasing the power of an existing instance.

This can involve adding more:
- CPU
- memory

Vertical scaling makes an individual machine stronger, but it does not always solve every performance problem.

### Scaling different parts independently

A useful point from the lesson is that not every part of a workload needs to scale the same way.

For example:
- one part of the system may need more front-end instances
- another part may not need additional back-end processing instances yet

This means different layers of an application can be scaled independently based on where the actual bottleneck is.

That helps avoid over-provisioning resources in one area just because another area needs more capacity.

### Amazon EC2 Auto Scaling

**Amazon EC2 Auto Scaling** automatically adds or removes EC2 instances based on demand and scaling metrics.

It works by:
- adding instances when demand rises
- removing instances when demand falls

This helps maintain the desired number of instances at any given time.

Benefits include:
- better performance during traffic increases
- lower cost when demand drops
- less manual intervention
- more efficient capacity management

### Amazon CloudWatch

The lesson explains that automatic scaling depends on monitoring data.

**Amazon CloudWatch** is used to collect and monitor metrics such as:
- instance performance
- latency
- other application metrics

These metrics help determine when scaling actions should happen.

CloudWatch provides the data that Auto Scaling uses to respond automatically to changing demand.

### Why this matters

Scaling is one of the biggest cloud advantages because it allows businesses to match resources to actual usage.

This means:
- customers get better performance
- businesses reduce unnecessary cost
- infrastructure becomes more flexible
- capacity planning becomes easier

### Important terms

**Scalability**  
The ability to increase or decrease resources to meet workload demand.

**Elasticity**  
The ability to automatically adjust resources based on real-time demand.

**Horizontal scaling (scaling out)**  
Adding more instances or resources to handle more work in parallel.

**Vertical scaling (scaling up)**  
Making an individual instance more powerful by increasing its resources.

**High availability**  
Keeping applications accessible with minimal downtime.

**Amazon EC2 Auto Scaling**  
A service that automatically adds or removes EC2 instances based on demand and metrics.

**Amazon CloudWatch**  
A monitoring service that collects and tracks metrics for AWS resources and applications.

### Real-world examples

- A website adds more EC2 instances during a sales event and removes them afterward.
- An application runs instances in multiple Availability Zones so traffic can continue if one AZ has a failure.
- A system increases the size of an instance when a workload needs more CPU and memory.
- A company uses CloudWatch metrics to trigger Auto Scaling when traffic rises.

### Exam reminders

- Scalability and elasticity allow AWS resources to grow and shrink based on demand.
- **Horizontal scaling** means adding more instances.
- **Vertical scaling** means making an instance larger or more powerful.
- Deploying EC2 instances across multiple Availability Zones improves **high availability**.
- **Amazon EC2 Auto Scaling** automatically adjusts the number of EC2 instances based on demand.
- **Amazon CloudWatch** collects the metrics used to inform scaling decisions.
- Scaling different parts of a workload independently helps avoid over-provisioning.

### Test your skills takeaway

- The primary benefit of scalability and elasticity is the ability to grow and shrink resources dynamically based on demand.
- Deploying EC2 instances across multiple Availability Zones helps provide high availability.
- AWS helps meet changing demand without over-provisioning by using automatic scaling based on metrics.

### My takeaway

This section shows why scaling is such a major cloud benefit. Instead of guessing how much infrastructure a business might need, AWS makes it possible to adjust capacity as demand changes.

The main things to remember are the difference between horizontal and vertical scaling, the importance of deploying across multiple Availability Zones, and the role of EC2 Auto Scaling and CloudWatch in making scaling automatic.
