# Getting Started

### Reference Documentation

For further reference, please consider the following sections:

* [Official Apache Maven documentation](https://maven.apache.org/guides/index.html)
* [Spring Boot Maven Plugin Reference Guide](https://docs.spring.io/spring-boot/3.4.0/maven-plugin)
* [Create an OCI image](https://docs.spring.io/spring-boot/3.4.0/maven-plugin/build-image.html)
* [Spring for RabbitMQ](https://docs.spring.io/spring-boot/3.4.0/reference/messaging/amqp.html)
* [Spring Configuration Processor](https://docs.spring.io/spring-boot/3.4.0/specification/configuration-metadata/annotation-processor.html)
* [Spring Data JDBC](https://docs.spring.io/spring-boot/3.4.0/reference/data/sql.html#data.sql.jdbc)
* [Spring Data JPA](https://docs.spring.io/spring-boot/3.4.0/reference/data/sql.html#data.sql.jpa-and-spring-data)
* [Rest Repositories](https://docs.spring.io/spring-boot/3.4.0/how-to/data-access.html#howto.data-access.exposing-spring-data-repositories-as-rest)
* [Spring Boot DevTools](https://docs.spring.io/spring-boot/3.4.0/reference/using/devtools.html)
* [Docker Compose Support](https://docs.spring.io/spring-boot/3.4.0/reference/features/dev-services.html#features.dev-services.docker-compose)
* [JDBC API](https://docs.spring.io/spring-boot/3.4.0/reference/data/sql.html)
* [OAuth2 Authorization Server](https://docs.spring.io/spring-boot/3.4.0/reference/web/spring-security.html#web.security.oauth2.authorization-server)
* [Spring Security](https://docs.spring.io/spring-boot/3.4.0/reference/web/spring-security.html)
* [Spring Session](https://docs.spring.io/spring-session/reference/)
* [Spring Web](https://docs.spring.io/spring-boot/3.4.0/reference/web/servlet.html)
* [Spring Web Services](https://docs.spring.io/spring-boot/3.4.0/reference/io/webservices.html)
* [Spring Reactive Web](https://docs.spring.io/spring-boot/3.4.0/reference/web/reactive.html)

### Guides

The following guides illustrate how to use some features concretely:

* [Messaging with RabbitMQ](https://spring.io/guides/gs/messaging-rabbitmq/)
* [Using Spring Data JDBC](https://github.com/spring-projects/spring-data-examples/tree/master/jdbc/basics)
* [Accessing Data with JPA](https://spring.io/guides/gs/accessing-data-jpa/)
* [Accessing JPA Data with REST](https://spring.io/guides/gs/accessing-data-rest/)
* [Accessing Neo4j Data with REST](https://spring.io/guides/gs/accessing-neo4j-data-rest/)
* [Accessing MongoDB Data with REST](https://spring.io/guides/gs/accessing-mongodb-data-rest/)
* [Accessing Relational Data using JDBC with Spring](https://spring.io/guides/gs/relational-data-access/)
* [Managing Transactions](https://spring.io/guides/gs/managing-transactions/)
* [Accessing data with MySQL](https://spring.io/guides/gs/accessing-data-mysql/)
* [Securing a Web Application](https://spring.io/guides/gs/securing-web/)
* [Spring Boot and OAuth2](https://spring.io/guides/tutorials/spring-boot-oauth2/)
* [Authenticating a User with LDAP](https://spring.io/guides/gs/authenticating-ldap/)
* [Building a RESTful Web Service](https://spring.io/guides/gs/rest-service/)
* [Serving Web Content with Spring MVC](https://spring.io/guides/gs/serving-web-content/)
* [Building REST services with Spring](https://spring.io/guides/tutorials/rest/)
* [Producing a SOAP web service](https://spring.io/guides/gs/producing-web-service/)
* [Building a Reactive RESTful Web Service](https://spring.io/guides/gs/reactive-rest-service/)

### Docker Compose support

This project contains a Docker Compose file named `compose.yaml`.
In this file, the following services have been defined:

* mysql: [`mysql:latest`](https://hub.docker.com/_/mysql)
* rabbitmq: [`rabbitmq:latest`](https://hub.docker.com/_/rabbitmq)

Please review the tags of the used images and set them to the same as you're running in production.

### Maven Parent overrides

Due to Maven's design, elements are inherited from the parent POM to the project POM.
While most of the inheritance is fine, it also inherits unwanted elements like `<license>` and `<developers>` from the
parent.
To prevent this, the project POM contains empty overrides for these elements.
If you manually switch to a different parent and actually want the inheritance, you need to remove those overrides.
