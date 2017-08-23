# CI/CD Pipeline requirements

## Vision 

* CI/CD pipeline will be the only mechanism that delivers changes to production environments (regardless of where they are hosted, including On-Prem, Azure, AWS, etc).  

* A reasonably familiar person should be able to initiate and debug a pipeline even if they did not create the underlying artifacts or services. 

* More broadly the deployment pipeline's job is to detect any changes that will lead to problems in production. These can include performance, security, or usability issues. A deployment pipeline should enable collaboration between the various groups involved in **delivering** and **operating** solutions and provide everyone visibility about the flow of changes in the system, together with a thorough audit trail.

* The key test is that a business sponsor could request that the current development version of the software can be deployed into production at a moment's notice - and nobody would bat an eyelid, let alone panic.

* The pipeline delivers **EVERYTHING** required to operate a service/application including:
    * test cases
    * monitoring
    * infrastructure
    * containers
    * plaforms
    * permissions
    * configuration
    * API calls
    * runbooks
    * etc. 

## Requirements (MVP) 

* Microsoft Developers can leverage **must have features** of visual studio or visual studio team services (vsts) while interacting with the pipeline
    * PaaS Requirements: Logic Apps, APIs, etc.
    * IaaS Requirements: ?

* Pipeline as code: With “Pipeline as Code”, your code, your automation and your orchestration are now commited to the source code management. The pipeline have the exact same versioned lifecycle, helping you to ensure long term maintainability.

* IT Auditor, Security, Change Review considerations

* The pipeline should respect idempotence principles

* Automated Builds : Generate artifacts from source following directives
    * MS Build
    * Make
    * Rake

* Automated Tests : Get insight of the application behavior and reliability.  We should have any TDD scripts alongside the application & infrastructure configuration
    * Unit Tests - Junit, 
    * Load Tests - Jmeter, Gatlin
    * Acceptance Tests - Cucumber, Selenium, 

* Automated Release : Create and package release to the specified version endpoint
    * Artifact repository - Nexus, Artifactory, etc.
    * Object storage - Azure Blob, S3, On premise

* Automated Deployment : Deploy any specific version (including prior versions) to the target/region
    * Infrastructure provisioning - AWS, Azure, Terraform, VMware
    * Server provisioning - Chef
    * Application Provisioning

* Pipeline Orchestration
    * (Preferred) GitLabCI
    * TravisCI
    * Jenkins
    * Bamboo

## Resources
* [Continuous Delivery](https://martinfowler.com/bliki/ContinuousDelivery.html)
* [Deployment Pipeline](https://martinfowler.com/bliki/DeploymentPipeline.html) 