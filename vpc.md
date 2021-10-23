# Virtual Private Cloud (VPC)

* Think as a box containing all apps, configs, particular to that space
* Contains subnets: configure the traffic to this VPC
* Choose a region and range of IP Addresses
* Internet Gateway: Routes traffic from outside to the subnet
	* Route Table: Configure addresses
	* It's possible to create private subnets
* Subnets can be placed on all AZ within a Region
* Two instances in two different VPC can have the same IP address

## CIDR (Classless Inter-Domain Routing)

When you create a VPC you must specify a range of IP addresses in the form of a CIDR block. After you can add one or more subnets in each AZ, the subnets CIDR block is a a subset of the VPC CIDR block.

## Virtual Private Gateway (VGW)

Private access to your VPC

## Elastic IP Address

* IP address that is allocated to your AWS account, and it's yours until you release it
* Can be associated with instances or network interfaces
