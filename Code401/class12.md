## What is a Spring RequestMapping??
A: The annotation is used to map web requests to Spring Controller methods.

## What is the request mapping basics??
It can be done by:
1. RequestMapping — by Path:is an annotation which indicates that a method parameter should be bound to a URI template variable. 
2. RequestMapping — the HTTP Method: The HTTP method parameter has no default.


## What is RequestMapping and HTTP Headers??
The mapping can be narrowed even further by specifying a header for the request

## @RequestMapping Consumes and Produces:
Mapping media types produced by a controller method is worth special attention.


## RequestMapping With Request Parameters:
The @RequestParam annotation is used with @RequestMapping to bind a web request parameter to the parameter of the handler method. It can be used with or without a value. The value specifies the request param that needs to be mapped to the handler method parameter.

## How to access data from JPA??
JPA Stands for Java Persistence API (JPA) JPA is an abbreviation that stands for Java Persistence API. It's a specification which is part of Java EE and defines an API for object-relational mappings and for managing persistent objects.


### @SpringBootApplication: 
it is convenience annotation that use to auto-configuration, component scan and be able to define extra configuration on application class.

### @EnableAutoConfiguration: 
Tells Spring Boot to start adding beans based on classpath settings, other beans, and various property settings.

### @Configuration: 
Allow to register extra beans in the context or import additional configuration classes.

### @ComponentScan:
Enable @Component scan on the package where the application is located.

### CRUD OPERATIONS:
1. save(): save an Iterable of entities. Here, we can pass multiple objects to save them in a batch.
2. findOne(): get a single entity based on passed primary key value.
3. findAll():  get an Iterable of all available entities in database.
4. count(): return the count of total entities in a table.
5. saveAndFlush(): save the entity and flush changes immediately.
6. deleteInBatch(): delete an Iterable of entities. Here, we can pass multiple objects to delete them in a batch.


