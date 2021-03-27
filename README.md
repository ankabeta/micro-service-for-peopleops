# micro-service-for-peopleops
# Microservice Architecture
 
We can say that a monolithic system is divided into small services, each running independently and communicating with each other through open protocols (eg http). It is an alternative to the motolytic structure. In simpler terms, Microservices are small, autonomous and working together services. As new functionalities are added to the software project, the codes grow. After a while, it becomes difficult to dominate the project, make additions and solve the problems we encounter. Normally, in a monolithic project, we create as many abstractions and modules in our code to deal with such problems.
 
There are many patterns associated with the microservice model. Monolithic architecture is an alternative to microservice architecture. Other models address the problems you will encounter when implementing the microservice architecture.
 
As can be seen in the picture above, in a monolithic application, the whole application is directly connected to a single database, and this brings along major problems that we will talk about in a moment. What the microservice architecture does is to divide our application into services that are as small as possible and have their own database and run it in this way. The smaller the service, the more we maximize the benefits of the microservice architecture and minimize its negative effects. Each microservice is a separate entity. The services should be able to be changed independently. The golden rule here is, do we need to change one service and make changes in another service while we are deploying?
 Changes made on any component in monolithic architecture may affect other components as well. Instead, a microservice architecture, which is an architectural solution that we can develop components in different languages and different frameworks, and use in a common project, has been developed. While all the components in a monolithic structure are together, the components in the microservice structure do not have to be together.
 

The microservice structure focuses on solving the complexity and management difficulties brought by the monolithic services that grow continuously and unplanned. It is definitely not an alternative model to SOA. Advantages of microservice architecture:
-	Services can be developed in different languages and different frameworks.
 
-	 Each service can be changed independently from each other, easy testing and build can be done.
-	 It enables continuous delivery and fast deployments can be performed.
 
-	It provides the ability to scale each service independently.
-	Since each service will be independent from each other, the code base will be simple and easy to maintain.
-	Versioning can be done easily.
-	Microservices are stateless. It does not keep the state information of any object.
-	Architecture does not need to be built from scratch, as the product develops, the architecture improves.
-	Those who join the team later adapt to the project more easily.
-	Allows to change the order and hierarchy of microservices.
-	Allows the application to be more flexible, more reusabe and more scalable.
 
Microservices have their own disadvantages. These;
-	Since different services that become independent from each other will use the same objects, an inevitable code repetition will occur.
-	Since the services can operate in different platforms and environments, management and monitoring costs will arise.
-	Managing multiple databases and transactions can be difficult.


Now let's make it come to life by giving an example. Let's say you build an e-commerce application that takes orders from customers, validates inventory and available credit, and ships them. The application consists of several components, including StoreFrontUI, which implements the UI, and some backend services for checking credit, maintaining inventory, and shipping orders. The application consists of a number of services. In the photo below, we see how these services are arranged in a regular and understandable way thanks to microservice architecture.
 

