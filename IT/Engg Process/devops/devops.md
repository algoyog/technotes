# Devops
At a very basic level, devops means interplay of code and operations targeted to synergize for accelerating the product delivery.

## But, why do you do that?
A small story....<br>
Long long ago, so long ago, in olden times......developers and ops are 2 silos taking care of developing and deploying apps. devs completed the code and threw the binary to the ops team and went to sleep. while the ops team struggled with deployment and maintenance of the code. ops team pushed back the developers with rigorous standards and huge documentations for accepting the changes to be deployed. developers also was bombarded with checklists and approvals making the whole process of developement slower.<br>
To add to the misery, management of projects has evolved into a new paradigm called "agile" which required incremental change to be made to the software across multiple teams/domains. 

## Hmm, What is the benefits
> - Speed
>     - Move at high velocity so you can innovate for customers faster, adapt to changing markets better, and grow more efficient at driving business results. The DevOps model enables your developers and operations teams to achieve these results. For example, microservices and continuous delivery let teams take ownership of services and then release updates to them quicker.
> - Rapid Delivery
>     - Increase the frequency and pace of releases so you can innovate and improve your product faster. The quicker you can release new features and fix bugs, the faster you can respond to your customers’ needs and build competitive advantage. Continuous integration and continuous delivery are practices that automate the software release process, from build to deploy.

> - Reliability
>     - Ensure the quality of application updates and infrastructure changes so you can reliably deliver at a more rapid pace while maintaining a positive experience for end users. Use practices like continuous integration and continuous delivery to test that each change is functional and safe. Monitoring and logging practices help you stay informed of performance in real-time.
> - Scale
>     - Operate and manage your infrastructure and development processes at scale. Automation and consistency help you manage complex or changing systems efficiently and with reduced risk. For example, infrastructure as code helps you manage your development, testing, and production environments in a repeatable and more efficient manner.
> - Improved Collaboration
>     - Build more effective teams under a DevOps cultural model, which emphasizes values such as ownership and accountability. Developers and operations teams collaborate closely, share many responsibilities, and combine their workflows. This reduces inefficiencies and saves time (e.g. reduced handover periods between developers and operations, writing code that takes into account the environment in which it is run).
> - Security
>     - Move quickly while retaining control and preserving compliance. You can adopt a DevOps model without sacrificing security by using automated compliance policies, fine-grained controls, and configuration management techniques. For example, using infrastructure as code and policy as code, you can define and then track compliance at scale.

> - Quality First
>     - Automated quality controls to ensure potential improvement in quality controls in fast moving pipeline of code.

## Ok. How do you do that?


Under a DevOps model, development and operations teams are no longer “siloed.” Sometimes, these two teams are merged into a single team where the engineers work across the entire application lifecycle, from development and test to deployment to operations, and develop a range of skills not limited to a single function.

In some DevOps models, quality assurance and security teams may also become more tightly integrated with development and operations and throughout the application lifecycle. When security is the focus of everyone on a DevOps team, this is sometimes referred to as DevSecOps.

These teams use practices to automate processes that historically have been manual and slow. They use a technology stack and tooling which help them operate and evolve applications quickly and reliably. These tools also help engineers independently accomplish tasks (for example, deploying code or provisioning infrastructure) that normally would have required help from other teams, and this further increases a team’s velocity.

### Attributes that Devops target

Below diagram gives a view of what are the key areas that will devops address.

![alt text][logo1]

[logo1]: devops-11.png ""

> - Lead time for changes
>     - For the primary application or service you work on, what is your lead time for changes (i.e., how long does it take to go from code committed to code successfully running in production)?
> - Deployment Frequency
>     - For the primary application or service you work on, how often does your organization deploy code to production or release it to end users?
> - Change failure rate
>     - For the primary application or service you work on, what percentage of changes to production or released to users result in degraded service (e.g., lead to service impairment or service outage) and subsequently require remediation (e.g., require a hotfix, rollback, fix forward, patch)?
> - Time to restore service
>     - For the primary application or service you work on, how long does it generally take to restore service when a service incident or a defect that impacts users occurs (e.g., unplanned outage or service impairment)?
> - Availability
>     - Availability reflects how well teams define their availability targets, track their current availability, and learn from any outages, making sure their feedback loops are complete. The items used to measure availability form a valid and reliable measurement construct
>     - At a high level, availability represents an  ability for technology teams and organizations to keep promises and assertions about the software they are operating. Notably, availability is about ensuring a product or service is available to and can be accessed  by your end users.
**speed and stability/quality are outcomes that enable each other.** 

![alt text][fig2]

[fig2]: devops-10.png ""

![alt text][fig3]

[fig3]: devops-12.png ""

### How to achieve the targets

At large there are 2 areas to focus and target. 
> - SDO and Organizational Performance
>     - Change Mgmt
>     - Cloud Adoption
>     - Technical practices 
>     - DR strategies
> - Productivity
>     - Tools
>     - Internal Search/Docs
>     - External Search
>     - Technical Debt
> - Culture

![alt text][fig4]

[fig4]: devops-13.png ""

#### Culture
Key to success of devops impmentation is enabling the right culture. 
> A culture that values psychological safety, trust, and respect contributes to productivity by letting employees focus on solving problems and getting their work done rather than politics and fighting with enable the right culture and collaboration in the org.

#### SDO and Org Perf

![alt text][fig5]

[fig5]: devops-14.png ""

##### Special Notes on Technical Practices

![alt text][fig8]

[fig8]: devops-17.png ""



#### Productivity

![alt text][fig6]

[fig6]: devops-15.png ""

##### Special Notes on CI/CD

Below are the key areas that needs to mature to have a clear and elite CI/CD automation

> * Repo and Branching Strategy
> * Automated Build
> * Automated UT
> * Automated Acceptance Test
> * Automated Perf Test
> * Automated Security Test
> * Automated Provisioning
> * Automated Deployment to Test
> * Automated Deployment to Prod
> * Integration with Chatbots and other tools (eg, JIRA)
> * Monitoring, Observability and related integration

Below is a typical view of CI/CD with available tools as of 2020.

![alt text][fig9]

[fig9]: devops-3.png ""


## References
https://aws.amazon.com/devops/what-is-devops/ <br>
http://info.thoughtworks.com/rs/thoughtworks2/images/continuous_delivery_a_maturity_assessment_modelfinal.pdf <br>
https://martinfowler.com/bliki/DevOpsCulture.html<br>
https://martinfowler.com/bliki/StateOfDevOpsReport.html<br>
https://cloud.google.com/devops
