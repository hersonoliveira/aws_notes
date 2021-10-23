# Dynamo DB

* Managed NoSQL DB
* Fault tolerant design distributed across AZs
* Access through API, no JDBC/ODBC
* **No** security groups with DynamoDB
* Each region is independent and isolated from other regions

* **Local secondary index** - Same partition key, different sort key
* **Global secondary index** - Different partition key and sort key

* DynamoDB Accelerator (DAX) - in-memory cache

* Keeping data together is a basic characteristic of a NoSQL database such as Amazon DynamoDB. Keeping related data in proximity has a major impact on cost and performance. Instead of distributing related data items across multiple tables, keep related items in your NoSQL system as close together as possible

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

When Streams is enabled in a table, it records information about every modification to data items in the table.

## DynamoDB Local

DynamoDB Local is the downloadable version of DynamoDB that enables you to write and test applications without accessing the web service.

## DynamoDB transactions

With Amazon DynamoDB transactions, you can group multiple actions together and submit them as a single all-or-nothing **TransactWriteItems** or **TransactGetItems** operation
