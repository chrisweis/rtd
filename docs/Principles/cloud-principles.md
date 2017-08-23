## Vision 

* First, the principle of disposability. When we work with cloud infrastructure, we’re necessarily building distributed systems. This, in turn, requires a critical shift in both our mindset and our architectural and risk management principles. In internet-connected distributed systems, **we must accept that failures and security breaches are inevitable**.  Thus we change the focus of our work from trying to prevent outages or attacks to **developing the capability to detect them and restore service rapidly**. To prove we can withstand failure, we continually inject it into our systems, proactively attacking our infrastructure — a key principle behind cloud disaster recovery testing exercises and Netflix’s Chaos Monkey, known as chaos engineering.  
 
* Systems built on cloud infrastructure must assume the infrastructure is unreliable. Thus to meet our goal of being able to restore service rapidly in the event of failure, we should treat it as disposable, ensuring we can rebuild it from scratch automatically using only configuration and scripts held in version control.  

## Principles
To build consistent, healthy, production-ready applications, incorporate the following practices into your development workflow from the beginning. 

* Design for operations at the beginning.  Application Teams will be empowered to own more of their footprints; Operate what you build 
* Architect for failure; Optimize for detecting and recovering from failures quickly MTTR 
* Optimize applications for total cost of ownership (TCO) such as: turning off when not needed 
* Minimize work in GUI, instead favoring automation and configuration-as-code through Terraform or ARM templates 
* Everything needed to run and operate the platform that is not a secret will be managed by configuration management 
* All configuration must be stored in centralized version control system (TBD) unless it is a secret 
* All changes should be tested locally and then tested in the staging environment either manually or optimally automatically by our pipeline  
* A Pull Request (PR) is created that addresses a required change.  The change should be reviewed by a peer and merged by reviewer 
* Each application and accompanying platform will include monitoring examples: https://cloud.gov/docs/ops/continuous-monitoring/ 
* Zero downtime deploys using green/blue deploys and other tactics 
* Platform as a service (PAAS) is a plus and a minus.  Columbia may not always get to choose when changes occur.   
* RBAC (Role Based Access Control) to maintain security and minimize unintended changes