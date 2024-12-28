# Software Architecture Overview Guide
Six popular software architectural patterns include:
  
* Controller-Worker Pattern
  + Processing and control logic become separated.
    - Controllers handle ingress/incoming requests, data flow, and handing off tasks to 'worker' components for processing.
    - Useful for highly scalable environments (multiple workers can operate at once)/asynchronous task handling.
* Event-Driven Architecture
  + As the parts of the app in this architecture are independent/decoupled, flexibility in design and high scalability can result.
    - This is especially useful for apps that work in real-time and therefore must be highly responsive.
  + As the name implies, parts/components of the app integrate based on the occurrence of events.
    - When a specified event (whether from a user or the system) occurs, code/logic is called to handle it. 
* Layered Architecture
  + Responsibilities are mapped to unique layers of the app, such as data access, business logic, and data presentation.
    - Separation of duties between layers assists with app configuration and maintenance.
    - A potential down side is that the layers must be well-defined and set up to communicate properly, or errors and bottlenecks may occur.
* Microservices Architecture
  + This involves breaking down apps into smaller services that rely upon APIs.
    - Services perform independently, including development, deployment, and scaling.
    - Apps become more flexible, in terms of technologies that can be integrated into a stack for each service. 
  + Each service can be mapped to a specific business function/feature.
    - A potential down side to this is that apps and their services (both internally and in communications with other services) can become more difficult to configure/manage.
* Model View Controller (MVC)
  + This design is especially popular in web app development/deployment.
  + This divides an app into three parts/components: the Model, the View, and the Controller.
    - Models handle business logic and data.
    - Views are associated with interfacing/data display for users.
    - Controllers interface with Models and handle input from users.
  + MVC helps with organizing apps into self-documented classes and methods, simplifying scaling and configuration/management. 
* Monolithic Architecture
  + Every app component is integrated into one codebase, simplifying deployment and management.
    - This is especially useful for smaller apps, but can be a challenge for larger apps due to scalability needs and redeploying systems due to changes.
