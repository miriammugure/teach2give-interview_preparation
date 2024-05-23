<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->


- [SYSYTEM DESIGN](#sysytem-design)
  - [Definition](#definition)
  - [Need for system design](#need-for-system-design)
  - [Design methods used in system design](#design-methods-used-in-system-design)
  - [Fundamental designs of system design](#fundamental-designs-of-system-design)
    - [Consistency Patterns](#consistency-patterns)
    - [Availability Patterns](#availability-patterns)

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




