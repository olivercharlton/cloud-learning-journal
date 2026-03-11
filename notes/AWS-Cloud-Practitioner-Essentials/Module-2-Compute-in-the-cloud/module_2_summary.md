## Module 2 Summary

In Module 2, I learned about compute in the cloud and how AWS provides virtual server capacity through Amazon EC2.

Amazon EC2 allows businesses to launch virtual machines, called EC2 instances, on demand instead of buying and maintaining physical servers. EC2 is flexible, cost-effective, and quick to provision compared with on-premises infrastructure. I also learned that EC2 instances are virtual machines that run in a multi-tenant environment, where multiple instances share the same physical host while remaining isolated through the hypervisor.

I learned about EC2 instance families and how different workloads need different resource profiles. General purpose instances provide a balanced mix of compute, memory, and networking. Compute optimized instances are best for CPU-heavy workloads, memory optimized instances are best for workloads that process large datasets in memory, accelerated computing instances use hardware accelerators such as GPUs, and storage optimized instances are designed for workloads that need high-performance local storage.

I also learned how AWS resources are provisioned. In AWS, everything is an API call, and resources can be managed through the AWS Management Console, the AWS CLI, or the AWS SDK. The console is useful for learning and visual management, while the CLI and SDK are more suitable for automation and repeatable deployments.

Another major topic was launching an EC2 instance. To launch one, key choices include the Amazon Machine Image (AMI), instance type, networking, storage, and access method. An AMI provides the operating system and software template used to launch the instance.

Module 2 also covered Amazon EC2 pricing models. On-Demand pricing is flexible and requires no commitment. Savings Plans and Reserved Instances are useful for more predictable usage, Spot Instances provide major savings for interruption-tolerant workloads, and Dedicated Hosts provide isolated physical servers for specialized needs.

Finally, I learned how AWS handles changing demand through scalability and elasticity. Amazon EC2 Auto Scaling can automatically add or remove instances based on metrics, while Elastic Load Balancing distributes traffic across instances. I also learned about messaging and queuing with Amazon SQS and Amazon SNS, and how loosely coupled architectures help improve reliability by reducing direct dependencies between components.

## Key Points to Remember

- Amazon EC2 provides virtual servers in the cloud.
- EC2 instances are virtual machines that can be launched, resized, stopped, and terminated on demand.
- Multi-tenancy means multiple VMs share a physical host while remaining isolated.
- Instance families are designed for different workloads:
  - General purpose = balanced
  - Compute optimized = CPU-heavy
  - Memory optimized = RAM-heavy
  - Accelerated computing = GPUs / hardware accelerators
  - Storage optimized = high-performance local storage
- AWS resources can be managed through the Console, CLI, or SDK.
- An AMI is the template used to launch an EC2 instance.
- On-Demand pricing is best for flexibility and no commitment.
- Spot Instances offer the biggest savings but can be interrupted.
- Auto Scaling adjusts capacity automatically.
- ELB distributes traffic across instances.
- SQS stores messages until they are processed.
- SNS pushes notifications immediately.
- Loosely coupled systems are more resilient than tightly coupled systems.
