# Elastic Beanstalk

* Rapid application development; User manages code dev, AWS manages capacity provisioning, load balancing, scaling, health monitoring
* Support various languages including Docker
* Possible to activate AWS managed updates to the platform

## Blue/Green Deployments

When AWS performs updates on your apps, it can become unavailable. You can avoid this performing a blue/green deployment, where you deploy the new version to a separate environment, and instantly redirect traffic to the new version.