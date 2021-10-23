# Elastic Beanstalk

* Rapid application development; User manages code dev, AWS manages capacity provisioning, load balancing, scaling, health monitoring
* Support various languages including Docker
* Possible to activate AWS managed updates to the platform

## Blue/Green Deployments

When AWS performs updates on your apps, it can become unavailable. You can avoid this performing a blue/green deployment, where you deploy the new version to a separate environment, and instantly redirect traffic to the new version.

## Deployment Types

- **Rolling**: Deploy the new version in batches. Cost remains the same. Avoids downtime and minimizes reduced availability.

- **Rolling with additional batches**: Avoids any reduced availability, at a cost of an even longer deployment time compared to the Rolling method. Suitable if you must maintain the same bandwidth throughout the deployment. These increase the costs as you're adding extra instances during the deployment.

## Config files

- Place .config files inside the `.ebextensions` folder
