# Simple Queue Service

* Managed distributed queue service
* Temporary repository for messages that are awaiting process

## Queue types

* Standard
    - Available in all regions
    - Unlimited throughput
    - **At-Least-Once delivery** - Messages are copied to multiple serves, it can be returned more than one time (apps should handle this)
    - Messages may be delivered out of order
    - Visibility timeout - Started when message is retrieved from the queue, if message not deleted before timer expiration it can be retrieved again
    - Possible to set delivery delays

* FIFO
    - Ohio, Oregon, Ireland regions
    - High throughput - but not unlimited
    - **Exactly-Once processing**
    - The order messages are sent and received is preserved

## Lambda triggers

Message triggers certain Lambda functions
