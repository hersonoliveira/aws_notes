# AWS EC2 (Elastic Computing Cloud)

- AMI (Amazon Machine Image) - Contains the OS plus applications to be installed on that instance.
- Optimized instances for specific use cases e.g. more memory, more storage.
- Elastic Load Balancer: Able to create an endpoint which will then route the traffic to selected instances.
- Pricing is per *Region*


## EC2 Instance Store

Storage that is physically attached to the host computer or instance.

- Ideal for temporary storage like buffers, cache, scratch data
- Better I/O performance
- Data in the storage is lost if instance is stopped or terminated

## Pricing Options

* On-Demand
    - Hourly
    - No long-term commitment
    - No upfront payments

* Spot Instances
    - Bid on spare compute capacity
    - Up to 90% discount

* Reserved Instances
    - Reserves compute capacity for when needed
    - Up to 75% discount
    - Standard (Cannot modify instance family) or Convertible
    - Zonal (can reserve capacity) or Regional

* Dedicated Hosts
    - Physical EC2 server dedicated for your use
    - Eases compliance

## Elastic Load Balancer

- Cross-zone: Distribue traffic evenly across all nodes on all AZ's
- A Load Balancer can target EC2 instances **only within an AWS Region**
- Access logs: Capture detailed information about requests sent to your Load Balancer

### Classic Load Balance

* Layer 4 (TCP) and Layer 7 (HTTP)

### ALB - Application Load Balance

* Layer 7 (HTTP)
* Docker and AWS ECS support
* Server Name Indication (SNI) allows you to expose multiple HTTPS applications each with its own SSL certificate on the same listener
