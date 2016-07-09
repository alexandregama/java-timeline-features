# Java Timeline Features

This is just an overview about the Java features in the Timeline

### Java EE 7

**Bean Validation 1.1 ([JSR 349](https://jcp.org/en/jsr/detail?id=349))**

http://beanvalidation.org/

- Method-level validation (validation of parameters or return values)

- Dependency injection for the different components of Bean Validation

- Integration with Context and Dependency Injection (CDI)

- Error message interpolation using the EL expressions

**Java API for JSON Processing - JSONP 1.0 ([JSR 353](http://jcp.org/en/jsr/detail?id=353))**


**Java API for RESTful web services - JAX-RS 2.0 ([JSR 339](http://jcp.org/en/jsr/detail?id=339))**

- Defining standardized client APIs to interact with REST WS

- Using interceptors

- Asynchronous request handling

**Java Servlet 3.1 ([JSR 340](http://jcp.org/en/jsr/detail?id=340))**

- Providing security improvement (run as, session fixation, and so on)

- Non-blocking IO in an asynchronous servlet and filter

- Deprecating the SingleThreadModel interface

- Upgrading support to communication protocol

- Providing annotation support (Servlet 3.0)

- Miscellaneous, such as ServletResponse.reset and sendRedirect using relative URL and so on

**CDI 1.1 ([JSR 346](http://jcp.org/en/jsr/detail?id=346))**

In the CDI specifications 1.1, a lot of small changes are included as follows:

- Added global enablement of interceptors

- Added support for the @AroundConstruct lifecycle callback for constructors

- Allowed binding interceptors to constructors

- Moved interceptor binding to interceptors spec, allowing for reuse by other specifications

- Added support decorators on built-in beans

- Added EventMetadata

**Interceptors 1.2 ([JSR 318](http://jcp.org/en/jsr/detail?id=318))**

Interceptors are used in conjunction with Java EE managed classes to allow developers to invoke the interceptor methods on an associated target class in conjunction with method invocations or lifecycle events.

The common uses of interceptors are logging, auditing, and profiling. Interceptors 1.2 have several new enhancements as follows:

- Rules to specify the interceptor order

- The @AroundConstruct interceptors

- The @Priority annotation to determine the interceptor order

**Enterprise JavaBeans - EJB 3.2 ([JSR 345](http://jcp.org/en/jsr/detail?id=345))**

EJB 3.2 (JSR 345) includes a lot of minor improvements as follows:

- This includes support for a local asynchronous session bean invocations

- Non-persistent EJB TimerService has been added for the EJB 3.2 Lite set of features

- Restriction on obtaining the current class loader has been removed

- Access to the Java I/O has been altered, replacing must not with should exercise caution

- The lifecycle callback interceptor methods of the Stateful session bean can now be executed in the transaction context 
determined by the lifecycle callback method's transaction attribute)

- It is now possible to completely disable passivation for a specific Stateful session bean

- The TimerService API has been extended to query all active timers in the same EJB module

**Java Message Service - JMS 2.0 ([JSR 343](http://jcp.org/en/jsr/detail?id=343))**

A new JMS Version 2.0 has been introduced, aiming to simplify the messaging interaction. We can list some of these improvements as follows:

- Simplified API consists of three new interfaces: JMSContext, JMSProducer, JMSConsumer, and some new methods

- A default connection factory, which connects to the application server's built-in JMS provider

- Multiple consumers are allowed on the same topic subscription

- Message delivery delay, after which the message is delivered

- Clients have the ability to send messages asynchronously

- JMSXDeliveryCount is changed into mandatory


**Concurrency Utilities 1.0 ([JSR 236](http://jcp.org/en/jsr/detail?id=236))**

Concurrency Utilities 1.0 (JSR 236) contains the following main components:

- ManagedExecutorService: This component is used to execute submitted tasks asynchronously

- ManagedScheduledExecutorService: This component is used to execute submitted tasks asynchronously at a specific time

- ContextService: This component is used to create dynamic proxy objects that capture the context of a container and enable applications to run within that context at a later time or submit to ManagedExecutorService

- ManagedThreadFactory: This component is used to create managed threads

**Batch Applications 1.0 ([JSR 352](http://jcp.org/en/jsr/detail?id=352))**

Batch Applications 1.0 (JSR 352) is the specification for batch applications and a runtime to schedule and execute jobs.

The batch framework consists of the following components:

- A job specification language based on XML

- A set of batch annotations and interfaces for application business logic

- A batch container that manages the execution of batch jobs

**Java Persistence API - JPA 2.1 ([JSR 338](http://jcp.org/en/jsr/detail?id=338))**

JPA 2.1 includes a lot of changes as follows:

- Support for stored procedures

- Bulk update/delete using the Criteria objects

- Predefined and user-defined functions using FUNCTION

- Using the TREAT and ON keywords

- Using CDI for the Entity listeners

- Support of unsynchronized persistence context


**Java Server Faces - JSF 2.2 ([JSR 344](http://jcp.org/en/jsr/detail?id=344))**

JSF 2.2 includes a lot of new improvement features as follows:

- The Faces Flows feature allows you to create a set of pages for user actions. For example, an online shopping journey. It also has a new defined scope, @FlowScoped.

- The Faces Flows feature gives you HTML 5 support using either the pass-through elements or the pass-through attributes.

- The Faces Flows feature gives you resource library contracts.

**Expression Language 2.0 ([JSR 341](http://jcp.org/en/jsr/detail?id=341))**

Expression language 3.0 (JSR 341) includes some new enhancements as follows:

- The new operator, ; ,to separate statements

- The use of a static field and method

- String concatenation operator using + or cat

- Lambda expression:


**Java Transaction APIs - JTA 1.2 ([JSR 907](http://jcp.org/en/jsr/detail?id=907))**

JTA 1.2 includes a few enhancements as follows:

- A new annotation named ```javax.transaction.Transactional``` and an exception ```javax.transaction.TransactionalException```

- A new annotation named ```javax.transaction.TransactionScoped```

**Java API for WebSocket 1.0 (JSR 356)**

WebSocket API is a new feature in Java EE; it complies with HTML 5 and the WebSocket technology, which is widely adapted by browsers these days

- It supports the annotated and programmatic patterns

- It uses the ws:// protocol for nonsecure communication and wss:// for secure communication (similar to http:// and https://)

- Each client should connect to one endpoint while a server can connect many clients to a single end point

- Each WebSocket server side is called endpoint; the process to create and deploy a WebSocket endpoint is as follows:

Create an endpoint class.

Implement the lifecycle methods of the endpoint (onOpen, onMessage, onError, and onClose).

Add business logic to the endpoint methods.

Deploy the endpoint method inside a web application.

At the most, we can have three methods annotated with @OnMessage in an endpoint method, one for each message of the text, binary, and pong types.
