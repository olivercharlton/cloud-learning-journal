## Introduction to AWS Global Infrastructure

### Overview

This section introduces the AWS Global Infrastructure and explains how it supports **high availability** and **fault tolerance**.

The main idea is that AWS does not rely on a single data center in one place. Instead, AWS uses infrastructure spread across different geographic locations so applications can stay available even when problems occur.

### Why global infrastructure matters

AWS builds and maintains data centers around the world. This global reach is useful not only for serving users in different countries, but also for improving reliability.

If all resources were stored in one data center, a single outage or disaster could bring everything down. By spreading infrastructure across multiple locations, AWS helps reduce that risk.

### Coffee shop analogy

The lesson compares AWS infrastructure to a chain of coffee shops.

If one coffee shop location has a problem, such as a power outage or damaged equipment, the business can still continue operating because customers can go to another nearby location.

This is similar to AWS:
- if one part of the infrastructure has a problem
- another location can continue supporting the service

This helps keep applications available for customers.

### High availability

**High availability** means making sure applications remain accessible with minimal downtime.

If one component fails, another can continue operating so the service stays available.

The goal of high availability is to reduce interruptions and keep systems running as smoothly as possible.

### Fault tolerance

**Fault tolerance** goes further than high availability.

Fault tolerance means designing a system so it can continue operating even if multiple components fail.

This is about building resilience into the system so that no single failure causes the entire application to stop working.

### AWS Regions

AWS organizes its global infrastructure into **Regions**.

A **Region** is a geographic area that contains AWS infrastructure.

Examples mentioned in the lesson include:
- Paris
- Tokyo
- São Paulo
- Dublin
- Ohio

Regions are designed to be located near customers around the world, which helps with both availability and performance.

### Availability Zones

Within each Region are **Availability Zones (AZs)**.

An Availability Zone is one or more discrete data centers with:
- redundant power
- redundant networking
- redundant connectivity

Each Region has **three or more Availability Zones** for redundancy.

AWS does not place Availability Zones right next to each other. This separation helps protect against local events such as:
- power problems
- connectivity issues
- natural disasters

This design helps improve resilience within a Region.

### Data centers

Inside an Availability Zone, AWS uses one or more physical data centers.

These data centers are built with redundancy so that infrastructure remains reliable even if some components fail.

### Multiple Regions

Running resources in one Region improves resilience, but if a business wants stronger disaster recovery, it may also operate across **multiple Regions**.

This means:
- if one Region has an outage
- operations can fail over to another Region

This helps businesses build even greater resilience, though the lesson notes this will be covered more deeply later.

### Why this matters

AWS Global Infrastructure helps businesses design systems that are:
- more reliable
- more resilient
- more available to customers

Instead of depending on one location, businesses can use AWS infrastructure across different Availability Zones and even different Regions to reduce downtime and improve continuity.

### Real-world examples

- A website runs in multiple Availability Zones so it stays online even if one data center has a failure.
- A company uses multiple Regions so it can recover from a large regional outage.
- An online service serves customers globally while also improving resilience by distributing infrastructure.

### Important terms

**High availability**  
The ability of an application to remain accessible with minimal downtime.

**Fault tolerance**  
The ability of a system to continue operating even when multiple components fail.

**Region**  
A geographic area that contains AWS infrastructure.

**Availability Zone (AZ)**  
One or more discrete data centers within a Region, designed with redundant power, networking, and connectivity.

**Redundancy**  
Having extra components or locations available so a failure in one place does not stop the system completely.

### Exam reminders

- AWS Global Infrastructure is designed to support **high availability**.
- A **Region** is a geographic area containing AWS infrastructure.
- Each Region contains **three or more Availability Zones**.
- Availability Zones are separated physically to reduce the impact of local failures.
- High availability means keeping applications accessible with minimal downtime.
- Fault tolerance means a system can continue operating even if multiple components fail.
- Businesses can also use **multiple Regions** for stronger resilience and disaster recovery.

### Test your skills takeaway

The best description of the AWS Global Infrastructure benefit of high availability is:

**AWS provides multiple data centers across different geographic regions so your website can remain operational even if one location faces issues.**

That reflects the core idea that AWS reduces the risk of a single point of failure.

### My takeaway

This section helped me understand that AWS Global Infrastructure is not just about having data centers around the world for convenience. It is also about reliability and resilience.

The most important idea here is that AWS uses Regions and Availability Zones to reduce downtime and help applications stay available, even when failures happen.
