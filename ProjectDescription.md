# Mobile Computing Project Description 2023/24

The Mobile Computing module consists of a project. 
The project is introduced in this document.

In case of questions or problems, a corresponding E-Mail 
including a detailed problem description that can be sent to 
[mobilecomputing@e-technik.org](mobilecomputing@e-technik.org)
In case of major difficulties, a meeting may be scheduled 
to explain the problem further. 
But please always try to solve the issues and research answers on your own first.

The project deals with implementing a 5G core, including Radio Access Networks (RANs), 
User Equipment (UEs), Data Networks (DNs), and Network Slicing. 
This will involve applying previously learned practices from other modules, 
such as Software Engineering, Cloud Computing, and Digital Switching and Routing. 
The general scope of the project is presented in more detail below, including the definition 
of the requirements and recommendations, as well as the submission and evaluation guidelines.

## Scope of the Project

A fundamental 5G design principle is the Service Based Architecture (SBA). It provides the basis for 
comprehensive modularization, which in turn is the prerequisite for being able to compile and combine 
network functions flexibly as required according to the use cases to be supported. 
In practical implementation, this requires using the design principle of network softwarization, i.e., 
the application of NFV (Network Functions Virtualisation) and SDN (Software-defined Networking) for 
the realization of Network Function instances and their interaction. 
If besides, the design principle of multi-tenant capability is to be implemented, network slicing will be useful. 
Here, two or more logical networks, parallel running network slices, are formed. 
They enable several tenants, e.g., a mobile network operator, a fixed network operator and 
an MVNO (Mobile Virtual Network Operator) for eMBB, a Smart Grid Provider and a service provider for 
autonomous vehicles for URLLC, in order to operate several, here 5, logical communication networks with different 
characteristics in parallel on one physical network platform [1].


[1]: Trick, U., 2021. 5G - An Introduction to the 5th Generation Mobile Networks. De Gruyter STEM Hrsg. Berlin/München/Boston: De Gruyter Oldenbourg.

## UML diagrams

You can render UML diagrams using [Mermaid](https://mermaidjs.github.io/). For example, this will produce a sequence diagram:

```mermaid
sequenceDiagram
Alice ->> Bob: Hello Bob, how are you?
Bob-->>John: How about you John?
Bob--x Alice: I am good thanks!
Bob-x John: I am good thanks!
Note right of John: Bob thinks a long<br/>long time, so long<br/>that the text does<br/>not fit on a row.

Bob-->Alice: Checking with John...
Alice->John: Yes... John, how are you?
