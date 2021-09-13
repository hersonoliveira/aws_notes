# Amazon RDS (Relational Database Service)

Amazon Relational Database Service (Amazon RDS) makes it easy to set up, operate, and scale a relational database in the cloud. It provides cost-efficient and resizable capacity while automating time-consuming administration tasks such as hardware provisioning, database setup, patching and backups.

- Currently supports six database engines:
	- Amazon Aurora (MySQL and PostgreSQL compatible RDS)
	- PostgreSQL
	- MySQL
	- MariaDB
	- Oracle
	- Microsoft SQL Server

- You can use the AWS Database Migration Service (AWS DMS) to quickly and securely migrate your databases to AWS
- Allocated storage defined during launch; can be scaled without downtime
- Possible to deploy **Multi-AZ** RDS instances

## Pricing

## Security

There are security access related to the DB instance using security groups

## Scaling

* Vertical
  * Modify Instance class e.g. choose a instance with more CPU/memory

* Horizontal
  * Create read replicas; insert/update/insert is done on the master RDS instance
