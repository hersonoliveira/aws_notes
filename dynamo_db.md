# Dynamo DB

* Managed NoSQL DB
* Fault tolerant design distributed across AZs
* Access through API, no JDBC/ODBC
* **No** security groups with DynamoDB
* Each region is independent and isolated from other regions

## Read consistency

* Eventually Consistent Reads (default)
    - Response might include old data

* Strongly Consistent Reads
    - Returns the most up-to-date data

## Read/Write capacity mode

* On-Demand
    - Pay only for what you use

* Provisioned(default, free-tier)
    - Specify reads/writes per second required for the application 

## Replication

Replicate a table to be available on another region

## Streams and AWS Lambda triggers

Amazon DynamoDB is integrated with AWS Lambda so that you can create triggers—pieces of code that automatically respond to events in DynamoDB Streams. With triggers, you can build applications that react to data modifications in DynamoDB tables
