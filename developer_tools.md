# AWS CodeCommit

* Fully managed source control solution
* Store any file type; no repo size limits

# AWS CodeBuild

* Fully managed build service that compiles source code, runs tests and produces packages that are ready to deploy
* Specify on an YAML file on the repo the steps to be executed on the build process (default: **buildspec.yml**)
* Choose where to place generated artifacts

# AWS CodeDeploy

* Automates deployments to a variety of compute services including AWS EC2, AWS Lambda, and instances running on-premises
* Allows Blue/Green deployments with full control of options
* Appspec file - YAML file to manage the deployment

# AWS CodePipeline

* Build, test and deploys code after every change
* Ties AWS CodeCommit, CodeBuild and CodeDeploy

* If a revision does not pass a manual approval (either by expiring or being rejected), it is treated as a **failed** revision

# AWS Codestar

* Unified interface to develop, build and deploy applications
* AWS Cloud9 - cloud based IDE

# AWS X-Ray

* Analyze the behaviour of distributed apps, provides request tracing, exception collection and profiling capabilities
* AWS X-Ray SDK -> X-Ray daemon -> X-Ray API -> Clients like console, AWS cli
* Can collect data across accounts
