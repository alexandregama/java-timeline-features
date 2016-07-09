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



**Enterprise JavaBeans - EJB 3.2 (JSR 345)**

**Java Message Service - JMS 2.0 (JSR 343)**

**Concurrency Utilities 1.0 (JSR 236)**

**Batch Applications 1.0 (JSR 352)**

**Java Persistence API - JPA 2.1 (JSR 338)**

**Java Server Faces - JSF 2.2 (JSR 344)**

**Expression Language 2.0 (JSR 341)**

**Java Transaction APIs - JTA 1.2 (JSR 907)**

**Java API for WebSocket 1.0 (JSR 356)**
