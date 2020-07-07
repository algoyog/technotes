# Microservices Architecture
 Microservice architecture is sweeping across web development replacing the classic monoliths. This is due to recent  explosion in cloud, devops, languages, nosql's and other technologies.

## What is a microservice?

    Micro -> Not macro and not nano. This is a domain based balance that needs to be applied to the software architecture.
    Service-> the implementation of a business problem limited to a specific domain.

In short, Microservice based architecture can be defined as "loosely coupled domain based bounded services"

Below diagram is a visual representation of world vs nano world vs microservice world.

![alt text][logo]

[logo]: TORSA-1.png ""

**Ok, cool, but what is a domain and how to define loose coupling?**

**Domain** is a cohesive unit that addresses a specific business problem. In figure 1, D1 and D2 represents different domains of business and F1, F2 are functionalities in the corresponding domains.

    * Domain Driven design is a theoretical foundation to understand bounded context and design domain based systems.
    * https://en.wikipedia.org/wiki/Domain-driven_design

**Loose coupling** is de-coupling the service implementation w.r.t design, static code, runtime to achieve high reliability, scalability.


    * 12 factor apps is very good starting place to understand how to achieve loose coupling.
    * https://12factor.net/


**Hmm, What more?**

With the above introduction to "what is what". Below is intro into framework that helps in designing production grade MSA.

![alt text][logo1]

[logo1]: TORSA-2.png ""


- **T**ools
    - This block represents the technologies, tools to be used across various layers in the architecture.
- **O**rchestration
    - This block represents the underlying container and container orchestration technologies to be used.
- **R**untime core
    - This is the core microservice implementation to achieve various business requirements.
- **S**ervice Mesh
    - The interservice and external service facade, communication, telemetry.
- **A**utomation
    - The automation across various layers in the architecture to minimise human intervention enabling high productivity and quality.


**Nice, How would TORSA architectural view look?**

![alt text][logo2]

[logo2]: TORSA-3.png ""

- **T**ools
    - Language - The implementation language used that could range from Java, .NET, python, nodejs, etc.
    - Framework - This would include microservices supported/enabling frameworks like springboot,etc
    - Datastore - This is the core datastore to store domain data. eg, SQL(MySql), NoSQL (Mongo) ..etc
    - Container Engine - The container engine that helps wrap the microservice. eg, Docker, runc
    - Orchestration Engine - Container orchestration engine. Kubernetes, docker swarm, etc
    - Softwares - Other key softwares used in MSA - LDAP, Apache MQ, Kafka, etc
    - APIs - Apache camel, etc
    - Cloud - AWS, GCP, Azure

- **O**rchestration
    - Container 
    - Orchestration
- **R**untime Core
    - Microservice
    - Data
- **S**ervice Mesh
    - Communication - The communication between microservices. This can be sync or async.
    - Registry/Discovery - The microservice discovery and registry services.
    - Telemetry - This includes, metrics, monitoring, logging, tracing.
    - Load balancing - Load balancing across multiple instance of the same service
    - Security - App, N/W and Data security for microservices.
    - Routing - Routing and circuit breaker 
    - API Management and Ingress - Expose services to outside world
    - Documentation - Microservice documentation.
- **A**utomation
    - Devops - CI, CD
    - Test Automation - Automate unit, integration, performance testing
    - Code Quality - Static, dynamic and secure code analysis
    - Code generation - Generate code and scaffolding of code.

**This  is a introduction to the TORSA framework. There will be seperate blogs to dive deep into each area of the framework**