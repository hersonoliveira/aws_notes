# Amazon S3 (Simple Storage  Service)

It's an object-level storage. It can store any type of data on it's original format.

- Objects are stored in buckets, that lives within a Region
- Objects are accessible via HTTP and HTTPS
- Buckets Naming: Globally unique and DNS-compliant
- (bucket, key, version[optional]) example: http://mybucket.s3.amazonaws.com/picture.jpg
- Objects can be up to 5TB in size
- Pricing: Based on the location/region and what you use
- Versioning of objects is possible
- S3 bucket names **cannot** be changed after bucket is created

## Data consistency

* Read-after-write consistency for new objetcs
* Eventually consistent
  * Read after write might return old data
  * List after write might not have new object

## Storage Classes

### General Purpose

* AWS S3 Standard
  * Data stored in 3 AZs
  * High durability
  * Backed by AWS SLA
  * 99.99% availability

### Infrequent Access

* AWS S3 Standard-Infrequent Access
  * Less frequently accessed files
  * 99.9% availability

* AWS S3 OneZone-Infrequent Access
  * Even less frequently accessed files 
  * Data stored in one AZ
  * 99.5% availability

## Cross-Region replication

* Must enable versioning
* Replicate bucket or some objects to another bucket from other region

## Events

* Possible to send events to SNS topics, when an object is put, post, delete, etc.
