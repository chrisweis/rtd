# ODP Frameworks
## Automation Framework for Azure and Development
The Automation Framework for Azure and Development is designed to rapidly onboard developers and ensure they are adhering to Columbia’s development standards. This framework also includes code quality checks, automated testing, vulnerability testing and a delivery pipeline. The pipeline runs automatically with code check-in. Included in this pipeline are Azure templates that automatically deploy the assets into the appropriate region in Microsoft Azure. This is to ensure compliance and cost management.

## Data Management Framework with ADW and ADLS
The Data Management Framework with Azure Data Warehouse and Azure Data Lake Store is designed to ensure all data external to Columbia with our third-party vendors or other partners, is retrieved and made available to any authenticated consumer. The Azure Data Warehouse contains conformed data and is intended for heavy workloads whereas the Azure Data Lake Store is intended to be the location where all data is stored first then made available for cloud to cloud integrations or cloud to on-premises interfaces.

## API Service Fabric and Gateway
The API Service Fabric and Gateway is the new Columbia Sportswear Marketplace. This marketplace is intended to be used by developers, whether internal or external, application designers who want to use our data, or third-party integrators who will consume and publish data to the marketplace. The marketplace is also where business partners are able to purchase data from Columbia. This data may be in the form of APIs, applications or mashups.

## Code Quality and Security Framework
The Code Quality and Security framework is built into the development environment and is required for any new development work. This framework utilizes SonarQube and Veracode. SonarQube is an open source solution that is tied into the build process. When a developer builds and publishes their code to the repository, the code quality checks run and return results not only to the developer but also display them in a dashboard. As a start, only critical and high issues are to be resolved. As Columbia matures medium issues may be resolved as well.

## Migration Delivery Framework
Critical to the work with Microsoft, the Migration Delivery Framework is designed to make repeatable pipelines and data factories that prepare and move data into the primary staging database for Microsoft Dynamics 365. The reason it needs to be repeatable and automated is because as we manage datasets and start our migration steps we will do several “dry runs” to move data from the legacy environments into the Dynamics environment. If these tasks are automated it reduces the likelihood of errors and mishaps during critical phases of the move to production.

## Service Bus Framework and Implementation
The Service Bus Framework and implementation strategy is designed to create topics necessary to store transactional data in a persisted state. This pub/sub model allows the consumers to determine when to remove data from the topic and when to archive it. The Service Bus Framework is a global, “build once, use many" framework and solution.

## Functional Service Implementation
The Functional Service implementation consists of rapid prototyping and iteration. Each iteration provides more functionality and meets the requirements of the business users. This implementation strategy allows Columbia developers to work quickly and deliver quality, production ready services within 2-3 weeks.

----

![Enterprise Product Servicev1.png](../assets/images/digitalservicefabric-96.png)
![Enterprise Product Servicev1.png](../assets/images/opendataplatform-96.png)