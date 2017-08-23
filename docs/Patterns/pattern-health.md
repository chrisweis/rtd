# GRP Architecture Pattern
## Health Endpoint Monitoring
______
Health Endpoint Monitoring refers to monitoring web applications and services to ensure they are available and storage or applications can reach them. Since it is often more difficult to monitor solutions in the cloud because we don’t have control over the environment, we must work closely with the cloud vendors and ensure that we have tools to meet the availability thresholds.

Health Endpoint Monitoring is implemented by sending periodic requests to an application. This is not the traditional 20x status check but rather an echo test to ensure that the service is up and returning data in a way that meets the needs of a consumer.

There are typically 3 measures in a Health Check
* Is the application or API alive?
* Is the data correct?
* Is the latency within proper parameters?

____
### Model: Health Endpoint Monitoring Pattern
![Image](https://docs.microsoft.com/en-us/azure/architecture/patterns/_images/health-endpoint-monitoring-pattern.png)