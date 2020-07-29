# Agile Engineering

## Disclaimer
* This technotes will not cover indepth implementation of any engg practices
* No coding and all strategies. :( *[I am not proud of this..]*

There are 2 terms in this topic - "Agile" and "Engineering". Below is the definition that the document will adhere to and specifically to software engineering side.

## What is Agile?

> **Individuals and interactions** over processes and tools <br>
> **Working software** over comprehensive documentation <br>
> **Customer collaboration** over contract negotiation <br>
> **Responding to change** over following a plan <br>

## What is Engineering?
> the branch of science and technology concerned with the design, building, and use of engines, machines, and structures.



## Software Engineering in Agile
> Simplicity-- is the key.<br>

The Reason for emergence of agile based software development is widely known and has been explored in depth. So we are not going to cover those. While we would be curious to understand and answer the below questions
* Will the old school engg practices fit to new agile scheme?
* What part of old school engg process will stick on?
* What changes in engineering would enable agile with zero impact on quality?

### 1. Scope  - **Responding to change** over following a plan
> Welcome changing requirements, even late in
development. Agile processes harness change for
the customer's competitive advantage. <br>
> The best architectures, requirements, and designs
emerge from self-organizing teams.<br>

#### What does this mean to engineering practices? 
* Arch/Design should be **evolutionary** in nature as compared to static archicture, to support changing requirements.
    *  Adopt **microservices** based architecture to support abstraction, partitioning, technology freedom, cloud enablement
    * Support **Domain Driven design** - Organize around business functionalities.
    * Encourage **experimentation**
        * A simple example would be to use a **feature toggle** for controlling the functionalities that are unstable
    * **Last responsible moment** - When decisions occur is a major distinction between traditional architecture and evolutionary architecture. These decisions could be around the structure of the application, the technology stack, specific tools, or communication patterns. In a traditional architecture, these decisions manifest themselves early, before writing code. In an evolutionary architecture, we wait for the last responsible moment to make decisions.The benefit of delaying a decision is the additional information available to make the decision. The cost is any potential re-work that has to occur once a decision has been made, which can be mitigated through appropriate abstractions—but the cost is still real. 
    * **Bring the pain forward** - When something on a project has the potential to cause pain, force yourself to do it more often and earlier, which in turn encourages you to automate the pain away and identify issues early. 
    * **Fitness function** - Much like in evolutionary computation techniques like genetic algorithms, an architectural fitness function specifies what our target architecture looks like. The up-front thinking about what the fitness function should be for a particular system provides the guidance for decision making and the timing of decisions. Architectural decisions are scored relative to the fitness function so that we can see that the architecture is evolving in the right direction. 
![alt text][logo1]

[logo1]: fitness.png ""

* Deployment architecture should follow **Infra as code** principle to adopt to any changes impacting he infra and runtime.

### 2. Time - **Responding to change** over following a plan
> Our highest priority is to satisfy the customer
through early and continuous delivery
of valuable software.<br>
> Deliver working software frequently, from a
couple of weeks to a couple of months, with a
preference to the shorter timescale.<br>

#### What does this mean to engineering practices? 
Frequent delivery of software is a key differentiator for being agile and the backbone that enables this is devops.

[Devops](https://github.com/gearuprepo/technotes/blob/master/IT/Engg%20Process/devops/devops.md) - At a very basic level, devops means interplay of code and operations targeted to synergize for accelerating the product delivery.

At a very high level, 3 key terms emerge out of devops
* Cont Integration - Integrate early and often.
* Cont Deployment - deploy as the final stages of CI.
* Cont Delivery - software is always deployable.

##### Core Princples
1. Treat infra as a code
2. create a repeatable and reliable process
3. Automate and toolify
4. Version control and branching strategy will be key.
5. if it hurts, do it more frequently.
6. done means released.
7. Integrate quality steps and security steps part of devops pipeline
8. stringent code review is a must. eg, git pull request.
9. DVCS is a magic. eg, git.


### 3. Quality - **Working software** over comprehensive documentation
> Working software is the primary measure of progress.<br>
> Continuous attention to technical excellence
and good design enhances agility.<br>

Ensuring working software will directly impact the quality of the product. All the classical QA process needs to be adhered to, say
* Functional validation
    * Domain validation.
* Non funtional validation
    * Performance
    * Usability
    * reliability
    * scalability


#### What does this mean to engineering practices? 

The silver bullet to sustain quality along with the previously defined scope and time is **depth of automation**

* Automate Testcases
* Encourage TDD
* Create spike solutions to reduce risks and not prototypes
* Implement mutation testing to verify the quality of test cases.
* Techincal debt should be constantly eliminated.
* Encourage innovative developer interaction like  pair programming




### 4. Stakeholder - **Customer collaboration** over contract negotiation and **Individuals and interactions** over processes and tools
> Business people and developers must work
together daily throughout the project.<br>
> Build projects around motivated individuals.
Give them the environment and support they need,
and trust them to get the job done.<br>
> Agile processes promote sustainable development.
The sponsors, developers, and users should be able
to maintain a constant pace indefinitely.<br>







## References
https://sea.ucar.edu/sites/default/files/Agile_Engineering_Practices.pdf <br>
https://www.thoughtworks.com/insights/blog/microservices-evolutionary-architecture<br>