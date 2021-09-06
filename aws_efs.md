# Elastic File System (AWS EFS)

Provides a simple, scalable, fully managed elastic NFS file system for use with AWS Cloud services and on-premises resources.

Amazon EFS is a regional service storing data within and across multiple Availability Zones (AZs) for high availability and durability. Amazon EC2 instances can access your file system across AZs, regions, and VPCs, while on-premises servers can access using AWS Direct Connect or AWS VPN.

* Can connect to multiple EC2 instances
* Only compatible with Linux based AMI

* Performance mode:
    * General purpose (default) - latency-sensitive use cases
    * Max I/O - higher latency

* Throughput mode:
    * Bursting
    * Provisioned - set throughput regardless of storage size

* Storage Tiers
    * Standard - for frequently accessed files
    * Infrequent Access (EFS-IA) - lower price to store files but costs to retrieve them

## Difference between EFS and EBS

* EBS - Locked to one AZ; Can be attached to multiple instances (Multi-Attach); 

* EFS - Multi AZ; Can be mounted to multiple instances; Linux only instances
