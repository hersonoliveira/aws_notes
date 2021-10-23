# Simple Notification Service

* Push mobile notifications, email or SMS
* Durability guaranteed; Once the message is sent it's removed

* Filter Policies
    - Default: Subscriber receives all messages from the topic
    - Filter: Subscriber receives only messages that match filter

* Various metrics send to AWS Cloudwatch
* Subscribers can be:
    - HTTP/HTTPS
    - Email
    - AWS SQS
    - AWS Lambda
    - SMS
    - Amazon Kinesis
    - Platform Application Endpoint

- PurgeQueue - Delete the messages but keep the queue
- DeleteQueue - Delete the queue
