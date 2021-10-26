# Monitoring

## CloudWatch

### Metrics

- Metrics for every service on AWS
- CPUUtilization, NetworkIn, etc
- EC2 memory usage is by default **not** pushed, need to create custom metric
- Metrics has namespace, timestamp
- Ec2 instances gets metrics every 5 minutes, detailed monitoring 1 min
- Out of the box metrics for EC2: CPU, disk, network (high level)

### Logs

- Apps can send logs to CloudWatch using SDK
- CloudWatch can collects logs from lots of services: ECS, Elastic Beanstalk, Lambda, CloudWatch log agents
- Can export to: S3, Elastic Search
- To send logs to CloudWatch, make sure IAM permissions are correct!
- Encryption of logs using KMS
- CloudWatch log agent on EC2 (or on-premise server): needed to push logs
- Unified Agent: Collects metrics and logs
- Filters: Look for patterns on logs

### Events

- Intercept events from AWS services (EC2 Instance start, CodeBuild failure)
- Schedule or cron
- Lots of targets

### Alarms

- Trigger notifications for any metric
- States: OK, INSUFFICIENT_DATE, ALARM
- Targets: EC2 (stop, terminate, reboot, etc), ASG, SNS

## X-Ray

- Debug tool; Visual analysis of the apps
- Review requests behaviour
- Troubleshooting performance
- Tracing: E2E way to follow a request
- Every request, or **sample** request

### How to enable

1) Import X-Ray SDK to your code
2) Install X-Ray daemon or enable X-Ray AWS integration
   - AWS services need to have proper permissions to send data to X-Ray!

## CloudTrail
