# CloudFormation

* Template-based creation and deletion of resources
* IAM access policies
* Drift detection - Detect if any property or resource was changed from it's expected value

## Concepts

* Templates
    - JSON or YAML file
    - Blueprint for the Stack
    - Save locally or S3

* Stack
    - Collection of resources managed as a single unit
    - Create, update and delete stacks
    - Create stack -> Submit template to AWS CloudFormation

* Change Sets
    - Summary of your proposed changes to update a Stack
    - See how your changes are going to impact your running resources

* Stack Sets
    - Enables creation of Stacks across regions using a single template
    - Regional resource


## Cloud Development Kit (CDK)

- Software development framework for defining cloud infrastructure in code and provisioning it through AWS CloudFormation.
- Support Typescript, Javascript, Python, Java, C#
