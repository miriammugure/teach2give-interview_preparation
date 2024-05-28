<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->


- [SYSYTEM DESIGN](#sysytem-design)
  - [Definition](#definition)
  - [Need for system design](#need-for-system-design)
  - [Design methods used in system design](#design-methods-used-in-system-design)
  - [Fundamental designs of system design](#fundamental-designs-of-system-design)
    - [Consistency Patterns](#consistency-patterns)
    - [Availability Patterns](#availability-patterns)
  - [Advanced Concepts](#advanced-concepts)
  - [COMPONENTS OF SYSTEM DESIGN](#components-of-system-design)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

# SYSYTEM DESIGN  
## Definition  
---   
It is a step by step procedure of defining a particular software's architecture , modules and components.  
## Need for system design   
--- 
 <li>It is used to prepare architecture of the system.</li>   
<b>Example</b>: Acustomer comes to you as a software developer ,for you to develop a certain software for them. The first step is requirement collection, both functional and non-functional requirements. The non-functional requirements are scalability,security etc. System design comes into picture  when you have to choose which database you will use,SQL or No SQL . You will also need to know how to make the application scalable incase traffic  increases. The Tech Giants like GOOGLE , have servers worldwide and serve resources to users from the nearest server to make their applications more efficient.  

## Design methods used in system design    
---  
Developers have to chose a particular method based on the project's requirements.    
<ol>
<li>ARCHITECTURAL DESIGN</li>  
it is used to design the base of the system, the infratsructure,model,view,components and interactionslike the client-server interaction and micro-services.  
<li>ENTITY RELATIONSHIP DIAGRAM</li>
It is mainly used in designing the application's database.  
here, you can define multiple schemas, add entities in each, add multiple attributes for each entity and connect the entities of two different schemas if a relationship exists between them.  
<li>UNIFIED MODELLING LANGUAGE</li>  
it is used to prepare the modelling software systems contains different diagrams like activity diagrams, class diagrams and sequence diagrams.  
<li>CLASS DIAGRAMS</li>  
They represents classes and contain class's attributes,methods and relationships between multiple classes.They show the system's data and functionalities.  
<li>SEQUENCE DIAGRAMS</li>
They represents interactions between various components of the sytem , model behaviour of the system. They describe how and in what order the objects in a system function.    

## Fundamental designs of system design  
---    
<ol>  
<li>PERFOMANCE AND SCALABILITY</li>    
Perfomance refers to how well a system executes tasks or processes within a given timeframe.  
Some websites take more time to load and others get loaded in a fraction of a second. If it's longer , traffic can decrease as visitors prefer other websites. Who wants that?Caching involves storing frequently accessed data in a temporary storage location for quick retrieval. It is essential in system design because it improves performance by reducing the time required to fetch data, thereby enhancing user experience and scalability.  

Scalability is the ability to scale the application ,enabling the system to handle more and more users by adding what it needs.For example, your application is becoming more popular day by day , your application server is getting more requests. How do you deal with that? Scaling your application by distributing the load across multiple servers or increasing the server's capacity.  
<li> LATENCY AND THROUGHPUT</li>  
 
Latency is the measurement of the time delay to complete a single request or data operation. It is crucial for live streaming for seamless operations.  
It occurs due to geographical distance,transport protocols or network experience. 
Throughput is the number of operations the system can handle in a particular time or number of data passed through a network request in a given time.   
It is measured in Mega Bytes Per Second(MB/S). It is used to check the capability of the systems. If the thriughput is low, architectures can scale the server to make it more efficient.  
<li>CONSISTENCY PATTERNS AND AVAILABILITY PATTERNS</li>
Consistency means that all nodes in the system have read the same data at a particular time.  
Availabilty - The systems availabilty ensures that each request receives a repsonse with frsh or old data. 

### Consistency Patterns  
---  
<ol>  
<li>Strong Consistency</li> - Each request should get most recent data. To achieve this you require synchronized communication which prioritizes consistency over availability.  
<li>Eventual Consistency</li> -Allows temporary inconsistencies to be resolved soon. It prioritizes availability over cnsistency.  
<li>Weak Consistency</li> -The user may get fresh data after writing the data.It focuses on fast access and can be used in live streaming or videa chats.  

### Availability Patterns  
---  
<ol>
<li>Load Balancing</li>- Upcomng requests can be distributed across multiple servers to achieve high availability. As we balance the load here, it is called  load balancing.   
<li>Retry and timeout strategies</li>- You can implement the retry mechanism to process the request after every interval. If the system fails,for example, if there is no reposnse in a website, you can refresh the page to get a response.   

## Advanced Concepts  
<ol>
<li>CDN (CONTENT DELIVERY NETWORK)  
- It is a distibuted server network located at different geolocations.It is used to deliver content from the server eg. images.  
A user requests for resources and if the resources are already cached,it delivers them to the customer. If not, it requests the resources from the original server and then delivers to the customer.  
<li>DNS (DOMAIN NAME SYSTEM)  
- It allows users to access the web and its resources using doamin name unlike in the 20<sup>th</sup> century where the IP address was being used. eg <a href ="">www.example.com</a>.  
It maps the unique domain name with a unique IP address when you make a request of the particular domain name.  
<li>CACHING  
Mechanism used to save resources faster AKA high speed storage.  
It works between the web application and source of data.Cookies are used for caching  
<li>PROXIES(PROXY SERVER)  
When you request to get resources from the internet, the application requests the proxy and the proxy gets resources and send s them back to the application.They are used for caching.  
When you change the VPN , it changes the proxy server ,so you can access the reources that were blocked from your proxy.  

## COMPONENTS OF SYSTEM DESIGN
<ol>
<li>Microservices and Service Discovery  
-Microservices is an architectural and organizational approach to software development where complex applications is broken down into small services such that each service works independently and accomplish specific tasks.  
<ul>  
Service Identification-Every microservice has a uniques id and name for its identification.  
Dynamic Service Discovery- Every microservice can dynamically find other services located in the same system so scaling and balancing becomes easy.  
</ul>
<li>Database Systems:RDBMS & NoSQL  
<ul>
Choosing the right database is important for system design.  
<li>RDBMS(Relational database management systems)  
SQL databases are built on top of RDBMS.  
They are used when you need to store structured data and it makes it easier to access data from the database and connect it with other data as they are stored in the table format. </ul> 
CHARACTERISTICS OF RDBMS  
<ul>
<li>Stores data in table format.
<li>Cannot be scaled horizontally, but can vertically.
<li>SQL is a query language for the RDBMS.
<li>Accessing the data is slow.
</ul>  
<ul>
NoSQL database  
It stores data in key value pairs and stores unstructured data in the database.  
CHARACTERISTICS OF NoSQL  
<ul>
<li>Stores data in key value pairs.
<li>Can be scaled horizontally.
<li>Store unstructurd data in the database.
<li>Each record can contain different key value pairs.
<li>Supports frequent changes in the database.
</ul></UL>  
<li>COMMUNICATION PROTOCOLS  
These are rules to exchange data between two systems.  
<ul>
<li>HTTP & HTTPS  

HTTP-Hypertext protocol  
HTTPS is a secure versio of HTTP.  
<li>TCP-Transmission control protocol It is used to communicate over the internet.
<li>UDP-user datagram protocol. It is used mainly for live streaming where data loss can be tolerable.  
<li>WebSockets- Used for bidirectional duplex communication.It builds connection between two web applications.
</ul>
<!-- ##APPROACHING SYSTEM DESIGN INTERVIEW QUESTIONS  

STEP BY STEP GUIDE  
<ol>
<li>Requirements clarification  

-Before designing a system design for any software,it is important to now thw requirements.  
<ul>
<li>Functional Requirements-These are requirements in the application which the user interacts with eg Authentication  
<li>Non-Functional Requirements-These are requirements that improves the application's capabilities eg Scalability.  
</ul>
<li>Estimation of resources  
-DEciding what kind if resources you should use to build the application ,eg for the server ,keep in mind how many requests it will receive per day or second.  
<li>System Interface Definition  
-Design the system interface like the API endpoints and what to expect from each.  
<li>Defining Data Models  
-Selecting a database for the application.  
<li>High Level Design  
-You cannot desigm the system for a whole application in a single go , so you need to go step by step.  
Decide how you will connect  the components with each other eg connecting the server with a database or server with client.  
<li>Detailed Design  
-Analyze the system to fulfill non-funstional requirements.  

eg <ul><li>How do we scale an application through load balancing.  
<li>How would you handle filure of the application.
</ul>  
<li>Identifying and Resolving Bottlenecks  
Bottlenecks are restrictive elements that limits the system's perfomance.  
eg Do you have nough replicas of the database to handle failures. -->









