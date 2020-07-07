# Enterprise Integration Patterns
## Basics
Below are core subject matter that is explored in EIP.<br>
> * Integrations through the eyes of aysnc messaging
> * Components and interactions of such a typical system involving - message channels, producers, consumers, message, routing, translation/conversion, reliability, scalability, monitoring, etc.

Any enterprise application deals with integration with each others and with itself in some cases. These integrations needs to cross various challenges to be successful.
> * Reliability of network
> * System availability
> * Network speed
> * Diverse application interfaces
> * Changes to the application.

Industry has evolved very high level strategies to address this need and some of them are below
> * File Transfer
> * Shared DB
> * RPCs
> * Messaging

## What is messaging?
excepts from EIP classsic "**Messaging is a technology that enables high speed, async , program-program communication with reliable delivery.**"

## Why would you choose messaging over other strategies?
The quick answer is <br>
- is **more immediate** than File transfer
- is **provides better encapsulation** than Shared DB
- is **more reliable** than RPCs

## Pros of such a system
- Remote Communication
- Platform/Language integration
- Async comm
- Variable Timing
- Throttling
- Reliability
- Mediation

## Cons?
- Complex programming model
- Sequencing issues
- Difficult to handle sync issues
- Performance
- Vendor lock-in

## What does it to take to implement such a system?
Lets see the below abstract representation of such a system 

*https://www.enterpriseintegrationpatterns.com/patterns/messaging/*
![alt text][logo]
[logo]: https://github.com/gearuprepo/technotes/raw/master/IT/Architecture/eai/eaiflow.png "Logo Title Text 2"
