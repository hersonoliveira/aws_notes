# AWS EC2 (Elastic Computing Cloud)

- AMI (Amazon Machine Image) - Contains the OS plus applications to be installed on that instance.
- Optimized instances for specific use cases e.g. more memory, more storage.
- Elastic Load Balancer: Able to create an endpoint which will then route the traffic to selected instances.

## EC2 Instance Store

Storage that is physically attached to the host computer or instance.

- Ideal for temporary storage like buffers, cache, scratch data
- Better I/O performance
- Data in the storage is lost if instance is stopped or terminated
