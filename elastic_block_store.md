# Elastic Block Store

Amazon Elastic Block Store (EBS) is an easy to use, high performance block storage service designed for use with Amazon Elastic Compute Cloud (EC2) for both throughput and transaction intensive workloads at any scale.

- SSD and HDD storage types
- Independent lifecycle from EC2 instances
- Attaches to one EC2 instance at a time
- Pricing: Based on the amount (volume) and storage type
- Encryption of EBS volumes is optional

## EBS Snapshots

Make a backup (snapshot) of your EBS storage at any point in time.

- Not necessary to detach volume to do snapshot but recommended
- Can copy backups across AZ and Regions

## EBS Volume Types

### SSD

- gp2/gp3: Cost effective storage, low latency
- Provisioned IOPS SSD: Critical business application, apps that need more than 16000 IOPS
- More than 32000 IOPS only with Nitro EC2 instances (64000 IOPS) 

### HDD

- Cannot be a boot volume
- Low cost volumes

## EBS Multi-Attach

Attach a same EBS to multiple EC2 instances in the same AZ. Only available on io1 and io2 family.