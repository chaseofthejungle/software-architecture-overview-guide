# Software Architecture Overview Guide
This is an introductory guide to nine popular software architectural patterns/architectures.
  
#### Table of Contents
  
1. [Controller-Worker Pattern](#cwp)
2. [Event-Driven Architecture](#eda)
3. [Layered Architecture](#layered)
4. [Microservices Architecture](#microservices)
5. [Model View Controller (MVC)](#mvc)
6. [Monolithic Architecture](#monolithic)
7. [Peer-to-Peer Architecture](#p2p)
8. [Pipe-Filter Architecture](#pipe-filter)
9. [Primary-Replica/Primary-Secondary Architecture](#replica)
10. [Supplemental Resources](#supplemental)
  
<hr />
  
## 1. <a name="cwp">Controller-Worker Pattern</a>
  + **Processing and control logic become separated.**
    - Controllers handle ingress/incoming requests, data flow, and handing off tasks to 'worker' components for processing.
    - Useful for highly scalable environments (multiple workers can operate at once)/asynchronous task handling.
  
<hr />
  
## 2. <a name="eda">Event-Driven Architecture</a>
  + **As the parts of the app in this architecture are independent/decoupled, flexibility in design and high scalability can result.**
    - This is especially useful for apps that work in real-time and therefore must be highly responsive.
  + **As the name implies, parts/components of the app react based on the occurrence of events that they detect.**
    - When a specified event (whether from a user or the system) occurs, code/logic is called to handle it.
  + **Events can be handled asynchronously, improving responsiveness.**
  
<hr />
  
## 3. <a name="layered">Layered Architecture</a>
  + **Responsibilities are mapped to unique layers of the app, such as data access, business logic, and data presentation.**
    - Separation of duties between layers assists with app configuration and maintenance, as adjustments in one layer do not directly impact other layers.
    - A potential down side is that the layers must be well-defined and set up to communicate properly, or errors and bottlenecks may occur.
  
<hr />
  
## 4. <a name="microservices">Microservices Architecture</a>   
  + **This involves breaking down apps into smaller, only loosely-coupled services that rely upon APIs.**
    - Services are self-contained, performing independently (such as with development, deployment, scaling).
    - Apps become more flexible, in terms of technologies that can be integrated into a stack for each service. 
  + **Each service can be mapped to a specific business function/feature.**
    - A potential down side to this is that apps and their services (both internally and in communications with other services) can become more difficult to configure/manage.
  
<hr />
  
## 5. <a name="mvc">Model View Controller (MVC)</a>   
  + **This design is especially popular in web app development/deployment.**
  + **This divides an app into three parts/components: the Model, the View, and the Controller.**
    - Models handle business logic and data.
    - Views are associated with interfacing/data display for users.
    - Controllers interface with Models and handle input from users.
  + **MVC helps with organizing apps into self-documented classes and methods, simplifying scaling and configuration/management.** 
  
<hr />
  
## 6. <a name="monolithic">Monolithic Architecture</a>   
  + **Every app component is unified into one interconnected structure, simplifying deployment and management.**
    - This is especially useful for smaller apps, but can be a challenge for larger apps due to scalability needs and redeploying systems due to changes.
  + **A potential drawback is minimal support for unique configurations for specific components/parts.**
  
<hr />
  
## 7. <a name="p2p">Peer-to-Peer Architecture</a>
  + **Every user has server and client capabilities (instead of operating within a dedicated client-server model).**
  + **Popular for decentralized apps and file/resource sharing networks/services with high scalability needs.**
  
<hr />
  
## 8. <a name="pipe-filter">Pipe-Filter Architecture</a>
  + **‘Filters’ are connected by a linear piping/redirection system, which also performs data transformation.**
  + **Useful for apps with heavy data stream and processing (e.g., batch) needs.**
  
<hr />
  
## 9. <a name="replica">Primary-Replica/Primary-Secondary Architecture</a>    
  + **Useful for database systems in which write operations and read replications are distinctively handled by primary and secondary nodes, respectively.**
  + **Helpful for preventing single point of failure while accounting for scalability (highly available to read data).**
  
<hr />

## 10. <a name="supplemental">Supplemental Resources</a>
* *[Amazon Documentation on Monolithic and Microservices Architecture Differences](https://aws.amazon.com/compare/the-difference-between-monolithic-and-microservices-architecture/)*
* *[Microsoft Documentation on Events in Visual Basic](https://learn.microsoft.com/en-us/dotnet/visual-basic/programming-guide/language-features/events/)*
* *[spring.io Documentation on Microservices](https://spring.io/microservices)*
  
<hr />
  
**TODO:** Add diagrams for each software architecture pattern.  
