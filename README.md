# Config Server Microservice

Spring Boot microservice that handles the configuration of other microservices

## Stack
- Java 11
- Spring Boot 2.x
- Spring Cloud Config Server

## Configuration
application.yml
```yaml
spring:
  profiles:
    active: native
  application:
    name: config-server
  cloud:
    config:
      server:
        native:
          search-locations: classpath:/configurations

server:
  port: 8888

```
