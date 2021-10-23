# AWS Lambda - Serverless Compute

* Scales automatically
* Pay for the time you consume
* Code monitoring and logging
* Language supported: Java, Python, Node.js, Go, C#

* Lambda functions run on containers on Amazon Linux
    - User specify **max memory** and **execution time**

* Functions can be invoked by an API Gateway event
* 1000 Concurrent executions -> can be increased via support ticket
* Security - Integrated with IAM (Policies and roles)
* Lambda functions provide access to a **single VPC**

## Lambda Programming Model

* Handler
    - The function Lambda calls to start execution

* Context Object
    - Passed to the handler as second param

* Logging
    - Log statements on code; Written to Cloudwatch

* Exceptions
    - Function must return result to Lambda

## Pricing

Price is determined by these three factors:

* Memory allocated
* Amount of time spent on a compute, with increments of 100 ms
* Number of times you execute or trigger a function
